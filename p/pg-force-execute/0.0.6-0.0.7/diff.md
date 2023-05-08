# Comparing `tmp/pg_force_execute-0.0.6.tar.gz` & `tmp/pg_force_execute-0.0.7.tar.gz`

## Comparing `pg_force_execute-0.0.6.tar` & `pg_force_execute-0.0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 pg_force_execute-0.0.6/pg_force_execute.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pg_force_execute-0.0.6/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_force_execute-0.0.6/LICENSE
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 pg_force_execute-0.0.6/README.md
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pg_force_execute-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 pg_force_execute-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 pg_force_execute-0.0.7/pg_force_execute.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pg_force_execute-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_force_execute-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 pg_force_execute-0.0.7/README.md
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pg_force_execute-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 pg_force_execute-0.0.7/PKG-INFO
```

### Comparing `pg_force_execute-0.0.6/pg_force_execute.py` & `pg_force_execute-0.0.7/pg_force_execute.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 from threading import Event, Thread
 
 import sqlalchemy as sa
 
 
 @contextlib.contextmanager
-def pg_force_execute(conn, engine,
+def pg_force_execute(conn,
                      delay=datetime.timedelta(minutes=5),
                      check_interval=datetime.timedelta(seconds=1),
                      termination_thread_timeout=datetime.timedelta(seconds=10),
                      logger=logging.getLogger("pg_force_execute"),
 ):
     cancel_exception = None
 
@@ -22,20 +22,20 @@
             exit.wait(timeout=(delay - check_interval).total_seconds())
 
             # Repeatedly check for other backends that block conn, and terminates them if they are
             # The loop addreses the case that as the client context progresses, it might run queries
             # that get blocked by clients not caught in the initial pg_blocking_pids call
             while not exit.wait(timeout=check_interval.total_seconds()):
                 logger.info('Cancelling queries blocking PID %s', pid)
-                with engine.begin() as conn:
+                with conn.engine.begin() as _conn:
                     # pg_cancel_backend isn't strong enough - the blocking PIDs might not be
                     # actually running a query, so there is nothing to cancel. They might
                     # just be holding locks. To force release of the locks, we have to call
                     # pg_terminate_backend
-                    cancelled_queries = conn.execute(
+                    cancelled_queries = _conn.execute(
                         sa.text("""
                             SELECT
                                 activity.usename AS usename,
                                 activity.query AS query,
                                 age(clock_timestamp(), activity.query_start) AS age,
                                 pg_terminate_backend(pids.pid)
                             FROM
```

### Comparing `pg_force_execute-0.0.6/.gitignore` & `pg_force_execute-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_force_execute-0.0.6/LICENSE` & `pg_force_execute-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_force_execute-0.0.6/README.md` & `pg_force_execute-0.0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -18,40 +18,37 @@
 import datetime
 import sqlalchemy as sa
 from pg_force_execute import pg_force_execute
 
 # Run postgresql locally should allow the below to run
 # docker run --rm -it -e POSTGRES_HOST_AUTH_METHOD=trust -p 5432:5432 postgres
 
-engine = sa.create_engine('postgresql://postgres@127.0.0.1:5432/')
+engine = sa.create_engine('postgresql+psycopg://postgres@127.0.0.1:5432/')
 query = 'SELECT 1'  # A more realistic example would be something that needs an exclusive lock on a table
 
 with \
         engine.begin() as conn, \
         pg_force_execute(
             conn,           # SQLAlchemy connection to run the query
-            engine,         # SQLAlchemy engine that will create new connections to cancel blocking queries
             delay=datetime.timedelta(minutes=5),  # Amount of time to wait before cancelling queries
         ):
 
-    results = conn.execute(query)
+    results = conn.execute(sa.text(query))
     print(results.fetchall())
 ```
 
 
 ## API
 
 The API a single context manager `pg_force_execute`.
 
 `pg_force_execute`(conn, engine, delay=datetime.timedelta(minutes=5), check_interval=datetime.timedelta(seconds=1), termination_thread_timeout=datetime.timedelta(seconds=10), logger=logging.getLogger("pg_force_execute"))
 
 - `conn` - A [SQLAlchemy connection](https://docs.sqlalchemy.org/en/20/core/connections.html#sqlalchemy.engine.Connection) that will be unblocked
 
-- `engine` - A [SQLAlchemy engine](https://docs.sqlalchemy.org/en/20/core/connections.html#sqlalchemy.engine.Engine) to create a new connection that will be used to terminate backends blocking `conn`
-
 - `delay` (optional) - How long to wait before attempting to terminate backends blocking `conn`
 
 - `check_interval` (optional) - The interval between repeated attempted to terminate backends blocking `conn`
 
 - `termination_thread_timeout` (optional) - How long to wait for the termination to complete
 
 - `logger` (optional) The Python logger instance through which to log
```

### Comparing `pg_force_execute-0.0.6/pyproject.toml` & `pg_force_execute-0.0.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-force-execute"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Department for International Trade", email="sre@digital.trade.gov.uk" },
 ]
 description = "Context manager to run PostgreSQL queries with SQLAlchemy, terminating any other clients that block them"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -18,15 +18,15 @@
 ]
 dependencies = [
     "sqlalchemy>=1.4.40",
 ]
 
 [project.optional-dependencies]
 dev = [
-    "psycopg2-binary>=2.8.6",
+    "psycopg[binary]>=3.1.9",
     "pytest>=7.2.1",
 ]
 
 [project.urls]
 "Source" = "https://github.com/uktrade/pg-force-execute"
 
 [tool.hatch.build]
```

### Comparing `pg_force_execute-0.0.6/PKG-INFO` & `pg_force_execute-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pg-force-execute
-Version: 0.0.6
+Version: 0.0.7
 Summary: Context manager to run PostgreSQL queries with SQLAlchemy, terminating any other clients that block them
 Project-URL: Source, https://github.com/uktrade/pg-force-execute
 Author-email: Department for International Trade <sre@digital.trade.gov.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: sqlalchemy>=1.4.40
 Provides-Extra: dev
-Requires-Dist: psycopg2-binary>=2.8.6; extra == 'dev'
+Requires-Dist: psycopg[binary]>=3.1.9; extra == 'dev'
 Requires-Dist: pytest>=7.2.1; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # pg-force-execute
 
 Context manager to run PostgreSQL queries with SQLAlchemy, terminating any other clients that continue to block it after a configurable delay.
 
@@ -35,40 +35,37 @@
 import datetime
 import sqlalchemy as sa
 from pg_force_execute import pg_force_execute
 
 # Run postgresql locally should allow the below to run
 # docker run --rm -it -e POSTGRES_HOST_AUTH_METHOD=trust -p 5432:5432 postgres
 
-engine = sa.create_engine('postgresql://postgres@127.0.0.1:5432/')
+engine = sa.create_engine('postgresql+psycopg://postgres@127.0.0.1:5432/')
 query = 'SELECT 1'  # A more realistic example would be something that needs an exclusive lock on a table
 
 with \
         engine.begin() as conn, \
         pg_force_execute(
             conn,           # SQLAlchemy connection to run the query
-            engine,         # SQLAlchemy engine that will create new connections to cancel blocking queries
             delay=datetime.timedelta(minutes=5),  # Amount of time to wait before cancelling queries
         ):
 
-    results = conn.execute(query)
+    results = conn.execute(sa.text(query))
     print(results.fetchall())
 ```
 
 
 ## API
 
 The API a single context manager `pg_force_execute`.
 
 `pg_force_execute`(conn, engine, delay=datetime.timedelta(minutes=5), check_interval=datetime.timedelta(seconds=1), termination_thread_timeout=datetime.timedelta(seconds=10), logger=logging.getLogger("pg_force_execute"))
 
 - `conn` - A [SQLAlchemy connection](https://docs.sqlalchemy.org/en/20/core/connections.html#sqlalchemy.engine.Connection) that will be unblocked
 
-- `engine` - A [SQLAlchemy engine](https://docs.sqlalchemy.org/en/20/core/connections.html#sqlalchemy.engine.Engine) to create a new connection that will be used to terminate backends blocking `conn`
-
 - `delay` (optional) - How long to wait before attempting to terminate backends blocking `conn`
 
 - `check_interval` (optional) - The interval between repeated attempted to terminate backends blocking `conn`
 
 - `termination_thread_timeout` (optional) - How long to wait for the termination to complete
 
 - `logger` (optional) The Python logger instance through which to log
```

