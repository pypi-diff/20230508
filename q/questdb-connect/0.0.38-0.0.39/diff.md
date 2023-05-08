# Comparing `tmp/questdb-connect-0.0.38.tar.gz` & `tmp/questdb-connect-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.38.tar", last modified: Sun May  7 15:13:41 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.39.tar", last modified: Mon May  8 09:36:23 2023, max compression
```

## Comparing `questdb-connect-0.0.38.tar` & `questdb-connect-0.0.39.tar`

### file list

```diff
@@ -1,24 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-07 15:13:41.094624 questdb-connect-0.0.38/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.38/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3375 2023-05-07 15:13:41.094456 questdb-connect-0.0.38/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2668 2023-05-07 15:11:39.000000 questdb-connect-0.0.38/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2514 2023-05-07 15:13:04.000000 questdb-connect-0.0.38/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-07 15:13:41.094663 questdb-connect-0.0.38/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-07 15:13:41.087209 questdb-connect-0.0.38/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-07 15:13:41.089887 questdb-connect-0.0.38/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1938 2023-05-07 15:01:28.000000 questdb-connect-0.0.38/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11459 2023-05-07 15:04:17.000000 questdb-connect-0.0.38/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.38/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    10535 2023-05-04 07:43:58.000000 questdb-connect-0.0.38/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.38/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-07 15:13:41.092515 questdb-connect-0.0.38/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3375 2023-05-07 15:13:41.000000 questdb-connect-0.0.38/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      526 2023-05-07 15:13:41.000000 questdb-connect-0.0.38/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-07 15:13:41.000000 questdb-connect-0.0.38/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-07 15:13:41.000000 questdb-connect-0.0.38/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-07 15:13:41.000000 questdb-connect-0.0.38/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       16 2023-05-07 15:13:41.000000 questdb-connect-0.0.38/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-07 15:13:41.093905 questdb-connect-0.0.38/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.38/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.38/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.38/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 09:36:23.054581 questdb-connect-0.0.39/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.39/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3510 2023-05-08 09:36:23.054443 questdb-connect-0.0.39/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2803 2023-05-08 09:34:56.000000 questdb-connect-0.0.39/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2521 2023-05-08 09:34:56.000000 questdb-connect-0.0.39/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-08 09:36:23.054618 questdb-connect-0.0.39/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 09:36:23.047924 questdb-connect-0.0.39/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 09:36:23.050420 questdb-connect-0.0.39/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.39/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.39/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2433 2023-05-08 09:10:08.000000 questdb-connect-0.0.39/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.39/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.39/src/examples/sqlalchemy_raw.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2668 2023-05-08 09:30:05.000000 questdb-connect-0.0.39/src/examples/trigonometry.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 09:36:23.052031 questdb-connect-0.0.39/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1938 2023-05-07 15:01:28.000000 questdb-connect-0.0.39/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11459 2023-05-07 15:04:17.000000 questdb-connect-0.0.39/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.39/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    10535 2023-05-04 07:43:58.000000 questdb-connect-0.0.39/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.39/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 09:36:23.053139 questdb-connect-0.0.39/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3510 2023-05-08 09:36:23.000000 questdb-connect-0.0.39/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      703 2023-05-08 09:36:23.000000 questdb-connect-0.0.39/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-08 09:36:23.000000 questdb-connect-0.0.39/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-08 09:36:23.000000 questdb-connect-0.0.39/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-08 09:36:23.000000 questdb-connect-0.0.39/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-08 09:36:23.000000 questdb-connect-0.0.39/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 09:36:23.053962 questdb-connect-0.0.39/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.39/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.39/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.39/tests/test_types.py
```

### Comparing `questdb-connect-0.0.38/LICENSE` & `questdb-connect-0.0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.38/PKG-INFO` & `questdb-connect-0.0.39/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.38
+Version: 0.0.39
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -14,88 +14,79 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 ## QuestDB Connect
 
-This package provides a [SQLAlchemy 1.4](https://docs.sqlalchemy.org/en/14/index.html) dialect for **QuestDB**, 
-as well as an [Apache Superset 2.0](https://github.com/apache/superset) engine specification. 
-
-SQLAlchemy is an open-source SQL toolkit and Object-Relational Mapping (ORM) library for Python. It provides a set 
-of high-level API for communicating with relational databases, including an SQL expression language, schema creation 
-and modification, and database connection management. SQLAlchemy provides a set of core utilities and an ORM layer 
-that abstracts away the details of the database, allowing you to work with Python objects instead of raw SQL statements.
-
-Apache Superset is an open-source business intelligence web application that enables users to explore and visualize 
-data. It offers a rich set of data visualizations, including charts, tables, and maps, that are used for creating  
-custom dashboards and reports.
+This Python 3 module provides a [SQLAlchemy 1.4](https://docs.sqlalchemy.org/en/14/index.html) dialect
+implementation for **QuestDB**, as well as an [Apache Superset 2.0](https://github.com/apache/superset)
+engine specification, using [psycopg2](https://www.psycopg.org/).
+
+Psycopg2 is a Python module that provides a way to connect to and interact with PostgreSQL databases. It
+is a widely used and popular library due to its comprehensive support for the PostgreSQL database system,
+and its high level of reliability and stability.
+
+SQLAlchemy is an open-source SQL toolkit and Object-Relational Mapping (ORM) library for Python. It provides
+a set of high-level API for communicating with relational databases, including an SQL expression language,
+schema creation and modification, and database connection management. SQLAlchemy provides a set of core
+utilities and an ORM layer that abstracts away the details of the database, allowing you to work with Python
+objects instead of raw SQL statements.
+
+Apache Superset is an open-source business intelligence web application that enables users to explore and
+visualize data. It offers a rich set of data visualizations, including charts, tables, and maps, that are
+used for creating custom dashboards and reports.
 
 ## Requirements
 
-* Python from 3.8.x to no higher than 3.10.x
-* SQLAlchemy 1.4.x
-* Apache Superset 2.x
+* Python from 3.8.x to 3.10.x
+* SQLAlchemy 1.4.x to 2.0.x
 
 ## Installation
 
 You can install this package using pip:
 
 ```shell
 pip install questdb-connect
 ```
 
-## Usage
-
-Use the QuestDB dialect by specifying it in your SQLAlchemy connection string. 
-
-```python
-import sqlalchemy as sqla
-
-
-engine = sqla.create_engine('questdb://localhost:8812/main')
-try:
-    with engine.connect() as conn:
-        pass
-finally:
-    if engine:
-        engine.dispose()
-```
-
-Alternatively,
+## Sample Usage
 
+Use the QuestDB dialect by specifying it in your SQLAlchemy connection string, 
+from that point on use SQLAlchemy:
 
 ```python
 import datetime
 import os
 
 os.environ.setdefault('SQLALCHEMY_SILENCE_UBER_WARNING', '1')
 
 import questdb_connect.dialect as qdbc
-from sqlalchemy import Column, MetaData, insert
+from sqlalchemy import Column, MetaData, create_engine, insert
 from sqlalchemy.orm import declarative_base
 
 Base = declarative_base(metadata=MetaData())
 
 
 class Signal(Base):
     __tablename__ = 'signal'
-    __table_args__ = (
-        qdbc.QDBTableEngine('signal', 'ts', qdbc.PartitionBy.HOUR, is_wal=True),
-    )
+    __table_args__ = (qdbc.QDBTableEngine(
+        'signal',
+        'ts',
+        qdbc.PartitionBy.HOUR,
+        is_wal=True),)
     source = Column(qdbc.Symbol)
     value = Column(qdbc.Double)
     ts = Column(qdbc.Timestamp, primary_key=True)
 
 
 def main():
-    engine = qdbc.create_engine('localhost', 8812, 'admin', 'quest')
+    engine = create_engine('questdb://localhost:8812/main')
     try:
         Base.metadata.create_all(engine)
-
         with engine.connect() as conn:
             conn.execute(insert(Signal).values(
                 source='coconut',
                 value=16.88993244,
                 ts=datetime.datetime.utcnow()
             ))
     finally:
@@ -104,9 +95,10 @@
 
 
 if __name__ == '__main__':
     main()
 ```
 
 ## Contributing
-This package is open-source, contributions are welcome. If you find a bug or would like to request a feature, 
+
+This package is open-source, contributions are welcome. If you find a bug or would like to request a feature,
 please open an issue on the GitHub repository.
```

### Comparing `questdb-connect-0.0.38/README.md` & `questdb-connect-0.0.39/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,74 @@
 ## QuestDB Connect
 
-This package provides a [SQLAlchemy 1.4](https://docs.sqlalchemy.org/en/14/index.html) dialect for **QuestDB**, 
-as well as an [Apache Superset 2.0](https://github.com/apache/superset) engine specification. 
-
-SQLAlchemy is an open-source SQL toolkit and Object-Relational Mapping (ORM) library for Python. It provides a set 
-of high-level API for communicating with relational databases, including an SQL expression language, schema creation 
-and modification, and database connection management. SQLAlchemy provides a set of core utilities and an ORM layer 
-that abstracts away the details of the database, allowing you to work with Python objects instead of raw SQL statements.
-
-Apache Superset is an open-source business intelligence web application that enables users to explore and visualize 
-data. It offers a rich set of data visualizations, including charts, tables, and maps, that are used for creating  
-custom dashboards and reports.
+This Python 3 module provides a [SQLAlchemy 1.4](https://docs.sqlalchemy.org/en/14/index.html) dialect
+implementation for **QuestDB**, as well as an [Apache Superset 2.0](https://github.com/apache/superset)
+engine specification, using [psycopg2](https://www.psycopg.org/).
+
+Psycopg2 is a Python module that provides a way to connect to and interact with PostgreSQL databases. It
+is a widely used and popular library due to its comprehensive support for the PostgreSQL database system,
+and its high level of reliability and stability.
+
+SQLAlchemy is an open-source SQL toolkit and Object-Relational Mapping (ORM) library for Python. It provides
+a set of high-level API for communicating with relational databases, including an SQL expression language,
+schema creation and modification, and database connection management. SQLAlchemy provides a set of core
+utilities and an ORM layer that abstracts away the details of the database, allowing you to work with Python
+objects instead of raw SQL statements.
+
+Apache Superset is an open-source business intelligence web application that enables users to explore and
+visualize data. It offers a rich set of data visualizations, including charts, tables, and maps, that are
+used for creating custom dashboards and reports.
 
 ## Requirements
 
-* Python from 3.8.x to no higher than 3.10.x
-* SQLAlchemy 1.4.x
-* Apache Superset 2.x
+* Python from 3.8.x to 3.10.x
+* SQLAlchemy 1.4.x to 2.0.x
 
 ## Installation
 
 You can install this package using pip:
 
 ```shell
 pip install questdb-connect
 ```
 
-## Usage
-
-Use the QuestDB dialect by specifying it in your SQLAlchemy connection string. 
-
-```python
-import sqlalchemy as sqla
-
-
-engine = sqla.create_engine('questdb://localhost:8812/main')
-try:
-    with engine.connect() as conn:
-        pass
-finally:
-    if engine:
-        engine.dispose()
-```
-
-Alternatively,
+## Sample Usage
 
+Use the QuestDB dialect by specifying it in your SQLAlchemy connection string, 
+from that point on use SQLAlchemy:
 
 ```python
 import datetime
 import os
 
 os.environ.setdefault('SQLALCHEMY_SILENCE_UBER_WARNING', '1')
 
 import questdb_connect.dialect as qdbc
-from sqlalchemy import Column, MetaData, insert
+from sqlalchemy import Column, MetaData, create_engine, insert
 from sqlalchemy.orm import declarative_base
 
 Base = declarative_base(metadata=MetaData())
 
 
 class Signal(Base):
     __tablename__ = 'signal'
-    __table_args__ = (
-        qdbc.QDBTableEngine('signal', 'ts', qdbc.PartitionBy.HOUR, is_wal=True),
-    )
+    __table_args__ = (qdbc.QDBTableEngine(
+        'signal',
+        'ts',
+        qdbc.PartitionBy.HOUR,
+        is_wal=True),)
     source = Column(qdbc.Symbol)
     value = Column(qdbc.Double)
     ts = Column(qdbc.Timestamp, primary_key=True)
 
 
 def main():
-    engine = qdbc.create_engine('localhost', 8812, 'admin', 'quest')
+    engine = create_engine('questdb://localhost:8812/main')
     try:
         Base.metadata.create_all(engine)
-
         with engine.connect() as conn:
             conn.execute(insert(Signal).values(
                 source='coconut',
                 value=16.88993244,
                 ts=datetime.datetime.utcnow()
             ))
     finally:
@@ -86,9 +77,10 @@
 
 
 if __name__ == '__main__':
     main()
 ```
 
 ## Contributing
-This package is open-source, contributions are welcome. If you find a bug or would like to request a feature, 
+
+This package is open-source, contributions are welcome. If you find a bug or would like to request a feature,
 please open an issue on the GitHub repository.
```

### Comparing `questdb-connect-0.0.38/pyproject.toml` & `questdb-connect-0.0.39/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.38"
+version = "0.0.39"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
@@ -77,8 +77,8 @@
 max-args = 10
 
 [tool.ruff.per-file-ignores]
 "tests/test_dialect.py" = ["S101"]
 "tests/test_types.py" = ["S101"]
 "tests/test_superset.py" = ["S101"]
 "tests/conftest.py" = ["S608"]
-"examples/sql_alchemy.py" = ["S608"]
+"src/examples/sqlalchemy_raw.py" = ["S608"]
```

### Comparing `questdb-connect-0.0.38/src/questdb_connect/__init__.py` & `questdb-connect-0.0.39/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.38/src/questdb_connect/dialect.py` & `questdb-connect-0.0.39/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.38/src/questdb_connect/function_names.py` & `questdb-connect-0.0.39/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.38/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.39/src/questdb_connect/superset_engine.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.38/src/questdb_connect/types.py` & `questdb-connect-0.0.39/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.38/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.39/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.38
+Version: 0.0.39
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -14,88 +14,79 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 ## QuestDB Connect
 
-This package provides a [SQLAlchemy 1.4](https://docs.sqlalchemy.org/en/14/index.html) dialect for **QuestDB**, 
-as well as an [Apache Superset 2.0](https://github.com/apache/superset) engine specification. 
-
-SQLAlchemy is an open-source SQL toolkit and Object-Relational Mapping (ORM) library for Python. It provides a set 
-of high-level API for communicating with relational databases, including an SQL expression language, schema creation 
-and modification, and database connection management. SQLAlchemy provides a set of core utilities and an ORM layer 
-that abstracts away the details of the database, allowing you to work with Python objects instead of raw SQL statements.
-
-Apache Superset is an open-source business intelligence web application that enables users to explore and visualize 
-data. It offers a rich set of data visualizations, including charts, tables, and maps, that are used for creating  
-custom dashboards and reports.
+This Python 3 module provides a [SQLAlchemy 1.4](https://docs.sqlalchemy.org/en/14/index.html) dialect
+implementation for **QuestDB**, as well as an [Apache Superset 2.0](https://github.com/apache/superset)
+engine specification, using [psycopg2](https://www.psycopg.org/).
+
+Psycopg2 is a Python module that provides a way to connect to and interact with PostgreSQL databases. It
+is a widely used and popular library due to its comprehensive support for the PostgreSQL database system,
+and its high level of reliability and stability.
+
+SQLAlchemy is an open-source SQL toolkit and Object-Relational Mapping (ORM) library for Python. It provides
+a set of high-level API for communicating with relational databases, including an SQL expression language,
+schema creation and modification, and database connection management. SQLAlchemy provides a set of core
+utilities and an ORM layer that abstracts away the details of the database, allowing you to work with Python
+objects instead of raw SQL statements.
+
+Apache Superset is an open-source business intelligence web application that enables users to explore and
+visualize data. It offers a rich set of data visualizations, including charts, tables, and maps, that are
+used for creating custom dashboards and reports.
 
 ## Requirements
 
-* Python from 3.8.x to no higher than 3.10.x
-* SQLAlchemy 1.4.x
-* Apache Superset 2.x
+* Python from 3.8.x to 3.10.x
+* SQLAlchemy 1.4.x to 2.0.x
 
 ## Installation
 
 You can install this package using pip:
 
 ```shell
 pip install questdb-connect
 ```
 
-## Usage
-
-Use the QuestDB dialect by specifying it in your SQLAlchemy connection string. 
-
-```python
-import sqlalchemy as sqla
-
-
-engine = sqla.create_engine('questdb://localhost:8812/main')
-try:
-    with engine.connect() as conn:
-        pass
-finally:
-    if engine:
-        engine.dispose()
-```
-
-Alternatively,
+## Sample Usage
 
+Use the QuestDB dialect by specifying it in your SQLAlchemy connection string, 
+from that point on use SQLAlchemy:
 
 ```python
 import datetime
 import os
 
 os.environ.setdefault('SQLALCHEMY_SILENCE_UBER_WARNING', '1')
 
 import questdb_connect.dialect as qdbc
-from sqlalchemy import Column, MetaData, insert
+from sqlalchemy import Column, MetaData, create_engine, insert
 from sqlalchemy.orm import declarative_base
 
 Base = declarative_base(metadata=MetaData())
 
 
 class Signal(Base):
     __tablename__ = 'signal'
-    __table_args__ = (
-        qdbc.QDBTableEngine('signal', 'ts', qdbc.PartitionBy.HOUR, is_wal=True),
-    )
+    __table_args__ = (qdbc.QDBTableEngine(
+        'signal',
+        'ts',
+        qdbc.PartitionBy.HOUR,
+        is_wal=True),)
     source = Column(qdbc.Symbol)
     value = Column(qdbc.Double)
     ts = Column(qdbc.Timestamp, primary_key=True)
 
 
 def main():
-    engine = qdbc.create_engine('localhost', 8812, 'admin', 'quest')
+    engine = create_engine('questdb://localhost:8812/main')
     try:
         Base.metadata.create_all(engine)
-
         with engine.connect() as conn:
             conn.execute(insert(Signal).values(
                 source='coconut',
                 value=16.88993244,
                 ts=datetime.datetime.utcnow()
             ))
     finally:
@@ -104,9 +95,10 @@
 
 
 if __name__ == '__main__':
     main()
 ```
 
 ## Contributing
-This package is open-source, contributions are welcome. If you find a bug or would like to request a feature, 
+
+This package is open-source, contributions are welcome. If you find a bug or would like to request a feature,
 please open an issue on the GitHub repository.
```

### Comparing `questdb-connect-0.0.38/tests/test_dialect.py` & `questdb-connect-0.0.39/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.38/tests/test_superset.py` & `questdb-connect-0.0.39/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.38/tests/test_types.py` & `questdb-connect-0.0.39/tests/test_types.py`

 * *Files identical despite different names*

