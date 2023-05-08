# Comparing `tmp/questdb-connect-0.0.39.tar.gz` & `tmp/questdb-connect-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.39.tar", last modified: Mon May  8 09:36:23 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.40.tar", last modified: Mon May  8 10:52:16 2023, max compression
```

## Comparing `questdb-connect-0.0.39.tar` & `questdb-connect-0.0.40.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 09:36:23.054581 questdb-connect-0.0.39/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.39/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3510 2023-05-08 09:36:23.054443 questdb-connect-0.0.39/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2803 2023-05-08 09:34:56.000000 questdb-connect-0.0.39/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2521 2023-05-08 09:34:56.000000 questdb-connect-0.0.39/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-08 09:36:23.054618 questdb-connect-0.0.39/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 09:36:23.047924 questdb-connect-0.0.39/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 09:36:23.050420 questdb-connect-0.0.39/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.39/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.39/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2433 2023-05-08 09:10:08.000000 questdb-connect-0.0.39/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.39/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.39/src/examples/sqlalchemy_raw.py
--rw-r--r--   0 marregui   (501) staff       (20)     2668 2023-05-08 09:30:05.000000 questdb-connect-0.0.39/src/examples/trigonometry.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 09:36:23.052031 questdb-connect-0.0.39/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1938 2023-05-07 15:01:28.000000 questdb-connect-0.0.39/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11459 2023-05-07 15:04:17.000000 questdb-connect-0.0.39/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.39/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    10535 2023-05-04 07:43:58.000000 questdb-connect-0.0.39/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.39/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 09:36:23.053139 questdb-connect-0.0.39/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3510 2023-05-08 09:36:23.000000 questdb-connect-0.0.39/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      703 2023-05-08 09:36:23.000000 questdb-connect-0.0.39/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-08 09:36:23.000000 questdb-connect-0.0.39/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-08 09:36:23.000000 questdb-connect-0.0.39/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-08 09:36:23.000000 questdb-connect-0.0.39/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-08 09:36:23.000000 questdb-connect-0.0.39/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 09:36:23.053962 questdb-connect-0.0.39/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.39/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.39/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.39/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 10:52:16.089220 questdb-connect-0.0.40/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.40/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3377 2023-05-08 10:52:16.088519 questdb-connect-0.0.40/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2670 2023-05-08 10:47:52.000000 questdb-connect-0.0.40/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2520 2023-05-08 10:43:19.000000 questdb-connect-0.0.40/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-08 10:52:16.089396 questdb-connect-0.0.40/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 10:52:16.080563 questdb-connect-0.0.40/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 10:52:16.083524 questdb-connect-0.0.40/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.40/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.40/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2433 2023-05-08 09:10:08.000000 questdb-connect-0.0.40/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.40/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.40/src/examples/sqlalchemy_raw.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2668 2023-05-08 09:30:05.000000 questdb-connect-0.0.40/src/examples/trigonometry.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 10:52:16.085248 questdb-connect-0.0.40/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1938 2023-05-07 15:01:28.000000 questdb-connect-0.0.40/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11459 2023-05-07 15:04:17.000000 questdb-connect-0.0.40/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.40/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    10535 2023-05-04 07:43:58.000000 questdb-connect-0.0.40/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.40/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 10:52:16.086397 questdb-connect-0.0.40/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3377 2023-05-08 10:52:16.000000 questdb-connect-0.0.40/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      703 2023-05-08 10:52:16.000000 questdb-connect-0.0.40/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-08 10:52:16.000000 questdb-connect-0.0.40/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-08 10:52:16.000000 questdb-connect-0.0.40/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-08 10:52:16.000000 questdb-connect-0.0.40/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-08 10:52:16.000000 questdb-connect-0.0.40/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 10:52:16.087710 questdb-connect-0.0.40/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.40/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.40/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.40/tests/test_types.py
```

### Comparing `questdb-connect-0.0.39/LICENSE` & `questdb-connect-0.0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.39/PKG-INFO` & `questdb-connect-0.0.40/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.39
+Version: 0.0.40
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -14,36 +14,35 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 ## QuestDB Connect
 
-This Python 3 module provides a [SQLAlchemy 1.4](https://docs.sqlalchemy.org/en/14/index.html) dialect
-implementation for **QuestDB**, as well as an [Apache Superset 2.0](https://github.com/apache/superset)
-engine specification, using [psycopg2](https://www.psycopg.org/).
-
-Psycopg2 is a Python module that provides a way to connect to and interact with PostgreSQL databases. It
-is a widely used and popular library due to its comprehensive support for the PostgreSQL database system,
-and its high level of reliability and stability.
-
-SQLAlchemy is an open-source SQL toolkit and Object-Relational Mapping (ORM) library for Python. It provides
-a set of high-level API for communicating with relational databases, including an SQL expression language,
-schema creation and modification, and database connection management. SQLAlchemy provides a set of core
-utilities and an ORM layer that abstracts away the details of the database, allowing you to work with Python
-objects instead of raw SQL statements.
-
-Apache Superset is an open-source business intelligence web application that enables users to explore and
-visualize data. It offers a rich set of data visualizations, including charts, tables, and maps, that are
-used for creating custom dashboards and reports.
+This module offers an implementation of QuestDB's dialect for [SQLAlchemy](https://www.sqlalchemy.org/), 
+as well as an engine specification for [Apache Superset](https://github.com/apache/superset/), using 
+[psycopg2](https://www.psycopg.org/) for database connectivity.
+
+Psycopg2 is a widely used and trusted Python module for connecting to and working with PostgreSQL databases. 
+It provides a comprehensive set of features for interacting with the PostgreSQL database system.
+
+SQLAlchemy is an open-source SQL toolkit and ORM library for Python. It provides a high-level API for 
+communicating with relational databases, including schema creation and modification, an SQL expression 
+language, and database connection management. The ORM layer abstracts away the complexities of the 
+database, allowing developers to work with Python objects instead of raw SQL statements.
+
+Apache Superset is a popular open-source business intelligence web application that enables users to 
+visualize and explore data through customizable dashboards and reports. It provides a rich set of data 
+visualizations, including charts, tables, and maps.
 
 ## Requirements
 
 * Python from 3.8.x to 3.10.x
-* SQLAlchemy 1.4.x to 2.0.x
+* Psycopg2
+* SQLAlchemy
 
 ## Installation
 
 You can install this package using pip:
 
 ```shell
 pip install questdb-connect
```

### Comparing `questdb-connect-0.0.39/README.md` & `questdb-connect-0.0.40/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 ## QuestDB Connect
 
-This Python 3 module provides a [SQLAlchemy 1.4](https://docs.sqlalchemy.org/en/14/index.html) dialect
-implementation for **QuestDB**, as well as an [Apache Superset 2.0](https://github.com/apache/superset)
-engine specification, using [psycopg2](https://www.psycopg.org/).
-
-Psycopg2 is a Python module that provides a way to connect to and interact with PostgreSQL databases. It
-is a widely used and popular library due to its comprehensive support for the PostgreSQL database system,
-and its high level of reliability and stability.
-
-SQLAlchemy is an open-source SQL toolkit and Object-Relational Mapping (ORM) library for Python. It provides
-a set of high-level API for communicating with relational databases, including an SQL expression language,
-schema creation and modification, and database connection management. SQLAlchemy provides a set of core
-utilities and an ORM layer that abstracts away the details of the database, allowing you to work with Python
-objects instead of raw SQL statements.
-
-Apache Superset is an open-source business intelligence web application that enables users to explore and
-visualize data. It offers a rich set of data visualizations, including charts, tables, and maps, that are
-used for creating custom dashboards and reports.
+This module offers an implementation of QuestDB's dialect for [SQLAlchemy](https://www.sqlalchemy.org/), 
+as well as an engine specification for [Apache Superset](https://github.com/apache/superset/), using 
+[psycopg2](https://www.psycopg.org/) for database connectivity.
+
+Psycopg2 is a widely used and trusted Python module for connecting to and working with PostgreSQL databases. 
+It provides a comprehensive set of features for interacting with the PostgreSQL database system.
+
+SQLAlchemy is an open-source SQL toolkit and ORM library for Python. It provides a high-level API for 
+communicating with relational databases, including schema creation and modification, an SQL expression 
+language, and database connection management. The ORM layer abstracts away the complexities of the 
+database, allowing developers to work with Python objects instead of raw SQL statements.
+
+Apache Superset is a popular open-source business intelligence web application that enables users to 
+visualize and explore data through customizable dashboards and reports. It provides a rich set of data 
+visualizations, including charts, tables, and maps.
 
 ## Requirements
 
 * Python from 3.8.x to 3.10.x
-* SQLAlchemy 1.4.x to 2.0.x
+* Psycopg2
+* SQLAlchemy
 
 ## Installation
 
 You can install this package using pip:
 
 ```shell
 pip install questdb-connect
```

### Comparing `questdb-connect-0.0.39/pyproject.toml` & `questdb-connect-0.0.40/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,48 +19,47 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.39"
+version = "0.0.40"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11'
 ]
-dependencies = [
-    'psycopg2-binary~=2.9.6',
-    'SQLAlchemy<=1.4.47',
-]
+dependencies = []
 
 [project.urls]
 "Homepage" = "https://github.com/questdb/questdb-connect/"
 "Bug Tracker" = "https://github.com/questdb/questdb-connect/issues/"
 
 [project.entry-points.'sqlalchemy.dialects']
 questdb = 'questdb_connect.dialect:QuestDBDialect'
 
 [project.entry-points.'superset.db_engine_specs']
 questdb = 'questdb_connect.superset:QDBEngineSpec'
 
 [project.optional-dependencies]
 test = [
-    'ruff~=0.0.261',
-    'pytest~=7.3.0',
+    'psycopg2-binary~=2.9.6',
+    'SQLAlchemy<=1.4.47',
     'apache-superset>=2.1.0',
     'sqlparse==0.4.3',
+    'ruff~=0.0.261',
+    'pytest~=7.3.0',
 ]
 
 [tool.ruff]
 # https://github.com/charliermarsh/ruff#configuration
 select = ["PL", "RUF", "TCH", "TID", "PT", "C4", "B", "S", "I"]
 line-length = 120
 exclude = [
```

### Comparing `questdb-connect-0.0.39/src/examples/__init__.py` & `questdb-connect-0.0.40/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.39/src/examples/hello_world.py` & `questdb-connect-0.0.40/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.39/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.40/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.39/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.40/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.39/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.40/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.39/src/examples/trigonometry.py` & `questdb-connect-0.0.40/src/examples/trigonometry.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.39/src/questdb_connect/__init__.py` & `questdb-connect-0.0.40/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.39/src/questdb_connect/dialect.py` & `questdb-connect-0.0.40/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.39/src/questdb_connect/function_names.py` & `questdb-connect-0.0.40/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.39/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.40/src/questdb_connect/superset_engine.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.39/src/questdb_connect/types.py` & `questdb-connect-0.0.40/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.39/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.40/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.39
+Version: 0.0.40
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -14,36 +14,35 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 ## QuestDB Connect
 
-This Python 3 module provides a [SQLAlchemy 1.4](https://docs.sqlalchemy.org/en/14/index.html) dialect
-implementation for **QuestDB**, as well as an [Apache Superset 2.0](https://github.com/apache/superset)
-engine specification, using [psycopg2](https://www.psycopg.org/).
-
-Psycopg2 is a Python module that provides a way to connect to and interact with PostgreSQL databases. It
-is a widely used and popular library due to its comprehensive support for the PostgreSQL database system,
-and its high level of reliability and stability.
-
-SQLAlchemy is an open-source SQL toolkit and Object-Relational Mapping (ORM) library for Python. It provides
-a set of high-level API for communicating with relational databases, including an SQL expression language,
-schema creation and modification, and database connection management. SQLAlchemy provides a set of core
-utilities and an ORM layer that abstracts away the details of the database, allowing you to work with Python
-objects instead of raw SQL statements.
-
-Apache Superset is an open-source business intelligence web application that enables users to explore and
-visualize data. It offers a rich set of data visualizations, including charts, tables, and maps, that are
-used for creating custom dashboards and reports.
+This module offers an implementation of QuestDB's dialect for [SQLAlchemy](https://www.sqlalchemy.org/), 
+as well as an engine specification for [Apache Superset](https://github.com/apache/superset/), using 
+[psycopg2](https://www.psycopg.org/) for database connectivity.
+
+Psycopg2 is a widely used and trusted Python module for connecting to and working with PostgreSQL databases. 
+It provides a comprehensive set of features for interacting with the PostgreSQL database system.
+
+SQLAlchemy is an open-source SQL toolkit and ORM library for Python. It provides a high-level API for 
+communicating with relational databases, including schema creation and modification, an SQL expression 
+language, and database connection management. The ORM layer abstracts away the complexities of the 
+database, allowing developers to work with Python objects instead of raw SQL statements.
+
+Apache Superset is a popular open-source business intelligence web application that enables users to 
+visualize and explore data through customizable dashboards and reports. It provides a rich set of data 
+visualizations, including charts, tables, and maps.
 
 ## Requirements
 
 * Python from 3.8.x to 3.10.x
-* SQLAlchemy 1.4.x to 2.0.x
+* Psycopg2
+* SQLAlchemy
 
 ## Installation
 
 You can install this package using pip:
 
 ```shell
 pip install questdb-connect
```

### Comparing `questdb-connect-0.0.39/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.40/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.39/tests/test_dialect.py` & `questdb-connect-0.0.40/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.39/tests/test_superset.py` & `questdb-connect-0.0.40/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.39/tests/test_types.py` & `questdb-connect-0.0.40/tests/test_types.py`

 * *Files identical despite different names*

