# Comparing `tmp/braincube-aws-core-alpha-0.0.18.tar.gz` & `tmp/braincube-aws-core-alpha-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braincube-aws-core-alpha-0.0.18.tar", last modified: Fri May  5 18:54:15 2023, max compression
+gzip compressed data, was "braincube-aws-core-alpha-0.0.19.tar", last modified: Mon May  8 06:57:23 2023, max compression
```

## Comparing `braincube-aws-core-alpha-0.0.18.tar` & `braincube-aws-core-alpha-0.0.19.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-05 18:54:15.885243 braincube-aws-core-alpha-0.0.18/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 13:41:49.000000 braincube-aws-core-alpha-0.0.18/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9298 2023-05-05 18:54:15.885493 braincube-aws-core-alpha-0.0.18/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8348 2023-05-03 19:09:10.000000 braincube-aws-core-alpha-0.0.18/README.md
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-02 13:42:37.000000 braincube-aws-core-alpha-0.0.18/pyproject.toml
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1086 2023-05-05 18:54:15.886584 braincube-aws-core-alpha-0.0.18/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 13:44:20.000000 braincube-aws-core-alpha-0.0.18/setup.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-05 18:54:15.871083 braincube-aws-core-alpha-0.0.18/src/
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-05 18:54:15.874885 braincube-aws-core-alpha-0.0.18/src/braincube_aws_core_alpha.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9298 2023-05-05 18:54:15.000000 braincube-aws-core-alpha-0.0.18/src/braincube_aws_core_alpha.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-05 18:54:15.000000 braincube-aws-core-alpha-0.0.18/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-05 18:54:15.000000 braincube-aws-core-alpha-0.0.18/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-05 18:54:15.000000 braincube-aws-core-alpha-0.0.18/src/braincube_aws_core_alpha.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-05 18:54:15.000000 braincube-aws-core-alpha-0.0.18/src/braincube_aws_core_alpha.egg-info/top_level.txt
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-05 18:54:15.875278 braincube-aws-core-alpha-0.0.18/src/core/
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.18/src/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-05 18:54:15.877891 braincube-aws-core-alpha-0.0.18/src/core/dal/
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.18/src/core/dal/__init__.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     1289 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.18/src/core/dal/data.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)      281 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.18/src/core/dal/database_errors.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     2257 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.18/src/core/dal/postgres_connection.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)    27337 2023-05-05 18:52:57.000000 braincube-aws-core-alpha-0.0.18/src/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-05 18:54:15.880009 braincube-aws-core-alpha-0.0.18/src/core/di/
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.18/src/core/di/__init__.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)      623 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.18/src/core/di/data.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     3796 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.18/src/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-05 18:54:15.882611 braincube-aws-core-alpha-0.0.18/src/core/rest/
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.18/src/core/rest/__init__.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     2883 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.18/src/core/rest/app_controller.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     3741 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.18/src/core/rest/app_module.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.18/src/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-05 18:54:15.884606 braincube-aws-core-alpha-0.0.18/src/core/utils/
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.18/src/core/utils/__init__.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)      580 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.18/src/core/utils/convert.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     1437 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.18/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 06:57:23.891639 braincube-aws-core-alpha-0.0.19/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 13:41:49.000000 braincube-aws-core-alpha-0.0.19/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-08 06:57:23.891885 braincube-aws-core-alpha-0.0.19/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8348 2023-05-03 19:09:10.000000 braincube-aws-core-alpha-0.0.19/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-02 13:42:37.000000 braincube-aws-core-alpha-0.0.19/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      933 2023-05-08 06:57:23.892998 braincube-aws-core-alpha-0.0.19/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 13:44:20.000000 braincube-aws-core-alpha-0.0.19/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 06:57:23.878317 braincube-aws-core-alpha-0.0.19/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 06:57:23.883482 braincube-aws-core-alpha-0.0.19/src/braincube_aws_core_alpha.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-08 06:57:23.000000 braincube-aws-core-alpha-0.0.19/src/braincube_aws_core_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-08 06:57:23.000000 braincube-aws-core-alpha-0.0.19/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-08 06:57:23.000000 braincube-aws-core-alpha-0.0.19/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-08 06:57:23.000000 braincube-aws-core-alpha-0.0.19/src/braincube_aws_core_alpha.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-08 06:57:23.000000 braincube-aws-core-alpha-0.0.19/src/braincube_aws_core_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 06:57:23.883983 braincube-aws-core-alpha-0.0.19/src/core/
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 06:57:23.886187 braincube-aws-core-alpha-0.0.19/src/core/dal/
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/dal/__init__.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     1289 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/dal/data.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)      281 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/dal/database_errors.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     2257 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/dal/postgres_connection.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)    29861 2023-05-08 06:54:18.000000 braincube-aws-core-alpha-0.0.19/src/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 06:57:23.887803 braincube-aws-core-alpha-0.0.19/src/core/di/
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/di/__init__.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)      623 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/di/data.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     3796 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 06:57:23.889804 braincube-aws-core-alpha-0.0.19/src/core/rest/
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/rest/__init__.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     2883 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/rest/app_controller.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     3741 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/rest/app_module.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/rest/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 06:57:23.891269 braincube-aws-core-alpha-0.0.19/src/core/utils/
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/utils/__init__.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)      580 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/utils/convert.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     1437 2023-05-04 09:08:49.000000 braincube-aws-core-alpha-0.0.19/src/core/utils/data.py
```

### Comparing `braincube-aws-core-alpha-0.0.18/LICENSE` & `braincube-aws-core-alpha-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.18/PKG-INFO` & `braincube-aws-core-alpha-0.0.19/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.18
+Version: 0.0.19
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: <4,>=3.7
+Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # braincube-aws-core
 
 Microframework for Python AWS lambdas.
```

### Comparing `braincube-aws-core-alpha-0.0.18/README.md` & `braincube-aws-core-alpha-0.0.19/README.md`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.18/src/braincube_aws_core_alpha.egg-info/PKG-INFO` & `braincube-aws-core-alpha-0.0.19/src/braincube_aws_core_alpha.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.18
+Version: 0.0.19
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: <4,>=3.7
+Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # braincube-aws-core
 
 Microframework for Python AWS lambdas.
```

### Comparing `braincube-aws-core-alpha-0.0.18/src/braincube_aws_core_alpha.egg-info/SOURCES.txt` & `braincube-aws-core-alpha-0.0.19/src/braincube_aws_core_alpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.18/src/core/dal/data.py` & `braincube-aws-core-alpha-0.0.19/src/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.18/src/core/dal/postgres_connection.py` & `braincube-aws-core-alpha-0.0.19/src/core/dal/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.18/src/core/dal/postgres_repository.py` & `braincube-aws-core-alpha-0.0.19/src/core/dal/postgres_repository.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import time
 import math
 import itertools
-from typing import Optional, List, Dict, Union, Tuple
+from typing import TypeVar
 
 from pydantic import BaseModel
 from pypika.queries import QueryBuilder
 from pypika import PostgreSQLQuery, Table, Field, Criterion, EmptyCriterion, CustomFunction, functions as fn
 
 from ..utils.data import Order, OrderType, Condition, ConditionType, Page, Pageable, Paging, Top, Metadata
 from .data import Key, Schema, Relation, SaveType, Column, StatementField
 from .database_errors import DatabaseError, DeleteError, SaveError
 from .postgres_connection import Pool, Connection
 
+T = TypeVar("T", bound=BaseModel)
+
 
 class PostgresRepository:
     """SQL based repository implementation.
     :param pool: Database connection pool.
     :param schema: Representation of master and related tables including columns, sub-queries and storage restrictions.
     :param relation_separator: Character that will be used in order to separate related tables from each column.
     """
@@ -24,52 +26,58 @@
         self._pool = pool
         self._relation_separator = relation_separator
         self.__construct_schema_data(schema)
 
     def __construct_schema_data(self, schema: Schema):
 
         # master table definition:
-        self._master_table: Tuple[Table, str] = \
+        self._master_table: tuple[Table, str] = \
             Table(schema.table).as_(schema.alias) if schema.alias else Table(schema.table), schema.table
 
-        self._master_columns: Dict[str, Tuple[Field, Column]] = dict(
+        self._master_columns: dict[str, tuple[Field, Column]] = dict(
             map(lambda c: (c.alias if c.alias else c.name, (
                 (self._master_table[0][c.name]).as_(c.alias) if c.alias else self._master_table[0][c.name], c)),
                 schema.columns))
 
-        self._master_statement_fields: Dict[str, Tuple[Field, StatementField]] = dict(
+        self._master_statement_fields: dict[str, tuple[Field, StatementField]] = dict(
             map(lambda f: (f.alias, (self._master_table[0][f.alias], f)), schema.statement_fields))
 
-        self._master_primary_key: Dict[str, Tuple[Field, Column]] = dict(
+        self._master_primary_key: dict[str, tuple[Field, Column]] = dict(
             itertools.islice(self._master_columns.items(), len(schema.primary_key)))
 
         # related tables definition:
-        self._related_tables: Dict[str, Tuple[Table, Relation]] = dict()
-        self._related_columns: Dict[str, Tuple[Field]] = dict()
-        self._related_forced_tables_aliases: List[str] = list()
+        self._related_tables: dict[str, tuple[Table, Relation]] = dict()
+        self._related_columns: dict[str, tuple[Field]] = dict()
+        self._related_forced_tables_aliases: list[str] = list()
 
         for relation in schema.relations:
             table_alias = relation.alias if relation.alias else relation.table
             related_table = Table(relation.table).as_(relation.alias) if relation.alias else Table(relation.table)
             self._related_tables[table_alias] = related_table, relation
             if relation.force_join:
                 self._related_forced_tables_aliases.append(table_alias)
             for column in relation.columns:
                 column_alias = \
                     f"{relation.table}{self._relation_separator}{column.alias if column.alias else column.name}"
                 self._related_columns[column_alias] = (related_table[column.name]).as_(column_alias),
 
-        self._schema_columns: Dict[str, tuple] = {**self._master_columns, **self._related_columns}
-        self._schema_columns_fields: Dict[str, tuple] = {**self._schema_columns, **self._master_statement_fields}
+        self._schema_columns: dict[str, tuple] = {**self._master_columns, **self._related_columns}
+        self._schema_columns_fields: dict[str, tuple] = {**self._schema_columns, **self._master_statement_fields}
 
         # order by definition:
-        self._schema_order: List[Tuple[Field, OrderType]] = [(self._schema_columns_fields[order.alias][0], order.type)
+        self._schema_order: list[tuple[Field, OrderType]] = [(self._schema_columns_fields[order.alias][0], order.type)
                                                              for order in schema.order]
 
-    async def fetch_raw(self, q: str, params: Optional[list] = None, connection: Optional[Connection] = None):
+    @staticmethod
+    def __base_model_aliases(cls: type[T]):
+        return [f.alias for f in cls.__fields__.values()]
+
+    async def fetch(self, q: str,
+                    params: list | None = None,
+                    connection: Connection | None = None):
         """Retrieve records from raw PSQL query.
         :param q: Query.
         :param params: Query parameters.
         :param connection: (asyncpg) Connection that will execute the query.
         :return: Records as dictionary.
         """
 
@@ -79,97 +87,101 @@
                 return [dict(r) for r in (await connection.fetch(q, *params) if params else await connection.fetch(q))]
             async with self._pool.acquire() as connection_:
                 return [dict(r) for r in
                         (await connection_.fetch(q, *params) if params else await connection_.fetch(q))]
         except Exception as e:
             raise DatabaseError(e)
 
-    async def fetch_one_raw(self, q: str,
-                            params: Optional[list] = None,
-                            connection: Optional[Connection] = None) -> Optional[Dict[str, any]]:
+    async def fetch_one(self, q: str,
+                        params: list | None = None,
+                        connection: Connection | None = None) -> dict[str, any] | None:
         """Retrieve record from raw PSQL query.
         :param q: Query.
         :param params: Query parameters.
         :param connection: (asyncpg) Connection that will execute the query.
         :return: Record as dictionary.
         """
 
-        data = await self.fetch_raw(q, params, connection)
+        data = await self.fetch(q, params, connection)
 
         return data[0] if data else None
 
-    async def execute_raw(self, q: str, params: Optional[list] = None, connection: Optional[Connection] = None) -> any:
+    async def execute(self, q: str,
+                      params: list | None = None,
+                      connection: Connection | None = None) -> any:
         """Execute raw PSQL query.
         :param q: Query.
         :param params: Query parameters.
         :param connection: (asyncpg) Connection that will execute the query.
         :return: Execution results as dictionary.
         """
 
-        return await self.fetch_raw(q, params, connection)
+        return await self.fetch(q, params, connection)
 
     async def _fetch(self, q: QueryBuilder,
                      replace_fields=True,
-                     connection: Optional[Connection] = None) -> List[Dict[str, any]]:
+                     connection: Connection | None = None) -> list[dict[str, any]]:
 
         query = self._replace_statement_fields(q) if replace_fields else str(q)
 
-        return await self.fetch_raw(query, connection=connection)
+        return await self.fetch(query, connection=connection)
 
     async def _fetch_one(self, q: QueryBuilder,
                          replace_fields=True,
-                         connection: Optional[Connection] = None) -> Optional[Dict[str, any]]:
+                         connection: Connection | None = None) -> dict[str, any] | None:
 
         data = await self._fetch(q, replace_fields, connection)
 
         return data[0] if data else None
 
     async def _execute(self, q: QueryBuilder,
-                       returning_aliases: Optional[List[str]] = None,
-                       connection: Optional[Connection] = None) -> any:
+                       returning_aliases: list[str] | None = None,
+                       connection: Connection | None = None) -> any:
 
         table = Table(self._master_table[1])
 
         for field, column in self._aliases_to_fields(returning_aliases, select=False):
             q = q.returning(table[field.name].as_(field.alias))
 
         return await self._fetch(q, False, connection)
 
     def _create_primary_key_criterion(self, key: Key) -> Criterion:
 
         return Criterion.all([
             pk[0] == key.values[i] for i, pk in enumerate(self._master_primary_key.values())
         ])
 
-    def _aliases_to_fields(self, aliases: Optional[List[str]] = None, select: bool = True) -> List[tuple]:
+    def _aliases_to_fields(self, aliases: list[str] | None = None,
+                           select: bool = True) -> list[tuple]:
 
         fields = list()
         accepted = self._schema_columns_fields if select else self._master_columns
         if aliases:
             for alias in aliases:
                 field = accepted.get(alias)
                 if not field:
                     continue
                 fields.append(field)
 
         return fields if fields else list(
             self._master_columns.values() if select else self._master_primary_key.values())
 
-    def _order_to_fields(self, order: List[Order]) -> List[Tuple[Field, OrderType]]:
+    def _order_to_fields(self, order: list[Order]) -> list[tuple[Field, OrderType]]:
 
         data = list()
         for order_ in order:
             field = self._schema_columns_fields.get(order_.alias)
             if not field:
                 continue
             data.append((field[0], order_.type))
 
         return data if data else self._schema_order
 
-    def _conditions_to_criterion(self, conditions: Optional[List[Condition]] = None, select: bool = True) -> Criterion:
+    def _conditions_to_criterion(self, conditions: list[Condition] | None = None,
+                                 select: bool = True) -> Criterion:
 
         if not conditions:
             return EmptyCriterion()
 
         criteria = list()
         for con in conditions:
             column = self._schema_columns.get(con.alias)
@@ -196,17 +208,17 @@
 
         for field, schema_field in self._master_statement_fields.values():
             query = query.replace(f"\"{self._master_table[0].alias}\".\"{field.name}\"",
                                   f"{schema_field.statement} \"{field.name}\"")
 
         return query
 
-    def _filter_save_data(self, data: Dict[str, any], type_: SaveType) -> Dict[str, any]:
+    def _filter_save_data(self, data: dict[str, any], type_: SaveType) -> dict[str, any]:
 
-        data_: Dict[str, any] = dict()
+        data_: dict[str, any] = dict()
 
         for k, v in data.items():
             column = self._master_columns.get(k)
             if not column:
                 continue
             if type_ == SaveType.insert and not column[1].insertable:
                 raise SaveError(f"column:'{column[1].name}' is not insertable", column[1].name)
@@ -215,18 +227,18 @@
             data_[column[1].name] = v
 
         if not data_:
             raise SaveError("no columns provided")
 
         return data_
 
-    def __init_select_query(self, fields: List[tuple],
-                            criterion: Optional[Criterion] = None,
-                            order: Optional[List[Tuple[Field, OrderType]]] = None,
-                            count_query: bool = False) -> Tuple[QueryBuilder, Optional[QueryBuilder]]:
+    def __init_select_query(self, fields: list[tuple],
+                            criterion: Criterion | None = None,
+                            order: list[tuple[Field, OrderType]] | None = None,
+                            count_query: bool = False) -> tuple[QueryBuilder, QueryBuilder | None]:
 
         q = PostgreSQLQuery.from_(self._master_table[0])
 
         table_aliases = self._related_forced_tables_aliases.copy()
 
         for field in fields:
             if len(field) == 2 and isinstance(field[1], StatementField):
@@ -254,48 +266,48 @@
 
         if order:
             for field, type_ in order:
                 q = q.orderby(field, order=type_)
 
         return q, cq
 
-    def _init_select_query(self, aliases: Optional[List[str]] = None,
-                           criterion: Optional[Criterion] = None,
-                           order: Optional[List[Order]] = None,
+    def _init_select_query(self, aliases: list[str] | None = None,
+                           criterion: Criterion | None = None,
+                           order: list[Order] | None = None,
                            set_order: bool = True,
-                           count_query: bool = False) -> Tuple[QueryBuilder, Optional[QueryBuilder]]:
+                           count_query: bool = False) -> tuple[QueryBuilder, QueryBuilder | None]:
 
         fields = self._aliases_to_fields(aliases)
         order_ = self._order_to_fields(order) if order else (self._schema_order if set_order else None)
 
         return self.__init_select_query(fields, criterion, order_, count_query)
 
-    async def _find_one(self, aliases: Optional[List[str]] = None,
-                        criterion: Optional[Criterion] = None,
-                        order: Optional[List[Order]] = None,
-                        connection: Optional[Connection] = None) -> Optional[Dict[str, any]]:
+    async def _find_one(self, aliases: list[str] | None = None,
+                        criterion: Criterion | None = None,
+                        order: list[Order] | None = None,
+                        connection: Connection | None = None) -> dict[str, any] | None:
 
         q, _ = self._init_select_query(aliases, criterion, order)
 
         return await self._fetch_one(q.limit(1), connection=connection)
 
-    async def _find_all(self, aliases: Optional[List[str]] = None,
-                        criterion: Optional[Criterion] = None,
-                        order: Optional[List[Order]] = None,
-                        connection: Optional[Connection] = None) -> List[Dict[str, any]]:
+    async def _find_all(self, aliases: list[str] | None = None,
+                        criterion: Criterion | None = None,
+                        order: list[Order] | None = None,
+                        connection: Connection | None = None) -> list[dict[str, any]]:
 
         q, _ = self._init_select_query(aliases, criterion, order)
 
         return await self._fetch(q, connection=connection)
 
     async def _find_all_page(self, connection: Connection,
-                             aliases: Optional[List[str]] = None,
-                             criterion: Optional[Criterion] = None,
+                             aliases: list[str] | None = None,
+                             criterion: Criterion | None = None,
                              page: Pageable = Pageable(),
-                             order: Optional[List[Order]] = None) -> Union[Page, Top]:
+                             order: list[Order] | None = None) -> Page | Top:
 
         start = time.time()
 
         calc_top = page.top_size > 0
         q, cq = self._init_select_query(aliases, criterion, order, count_query=not calc_top)
 
         # top implementation
@@ -324,18 +336,18 @@
             page_no = total_pages
             records = await self._fetch(q.limit(page.page_size).offset((page_no - 1) * page.page_size),
                                         connection=connection)
 
         return Page(records, Paging(page_no, page.page_size, total_pages, count),
                     Metadata(int((time.time() - start) * 1000)))
 
-    async def _update(self, data: Union[Dict[str, any], BaseModel],
+    async def _update(self, data: BaseModel | dict[str, any],
                       criterion: Criterion,
-                      returning_aliases: Optional[List[str]] = None,
-                      connection: Optional[Connection] = None) -> Optional[List[Dict[str, any]]]:
+                      returning_aliases: list[str] | None = None,
+                      connection: Connection | None = None) -> list[dict[str, any]] | None:
 
         if isinstance(criterion, EmptyCriterion):
             raise SaveError("update without conditions is not allowed")
 
         uq = PostgreSQLQuery.update(self._master_table[1])
 
         data_ = data.dict(by_alias=True, exclude_unset=True) if data is BaseModel else data.copy()
@@ -343,90 +355,90 @@
         for v, k in self._filter_save_data(data_, SaveType.update).items():
             uq = uq.set(v, k)
         uq = uq.where(criterion)
 
         return await self._execute(uq, returning_aliases, connection)
 
     async def _delete(self, criterion: Criterion,
-                      returning_aliases: Optional[List[str]] = None,
-                      connection: Optional[Connection] = None) -> Optional[List[Dict[str, any]]]:
+                      returning_aliases: list[str] | None = None,
+                      connection: Connection | None = None) -> list[dict[str, any]] | None:
 
         if isinstance(criterion, EmptyCriterion):
             raise DeleteError("delete without conditions is not allowed")
 
         dq = PostgreSQLQuery \
             .from_(self._master_table[1]) \
             .delete() \
             .where(criterion)
 
         return await self._execute(dq, returning_aliases, connection)
 
     async def find_by_id(self, key: Key,
-                         aliases: Optional[List[str]] = None,
-                         connection: Optional[Connection] = None) -> Optional[Dict[str, any]]:
+                         aliases: list[str] | None = None,
+                         connection: Connection | None = None) -> dict[str, any] | None:
         """Find the record from passed key.
         :param key: Record identifier.
         :param aliases: List of fields that will be selected by the query.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Record as dictionary.
         """
 
         criterion = self._create_primary_key_criterion(key)
 
         q, _ = self._init_select_query(aliases, criterion, set_order=False)
 
         return await self._fetch_one(q, connection=connection)
 
-    async def exists_by_id(self, key: Key, connection: Optional[Connection] = None) -> bool:
+    async def exists_by_id(self, key: Key, connection: Connection | None = None) -> bool:
         """Find if record exists from passed key.
         :param key: Record identifier.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Record existence.
         """
 
         aliases = [column.alias for field, column in self._master_primary_key.values()]
 
         return await self.find_by_id(key, aliases, connection) is not None
 
-    async def find_one(self, aliases: Optional[List[str]] = None,
-                       conditions: Optional[List[Condition]] = None,
-                       order: Optional[List[Order]] = None,
-                       connection: Optional[Connection] = None) -> Optional[Dict[str, any]]:
+    async def find_one(self, aliases: list[str] | None = None,
+                       conditions: list[Condition] | None = None,
+                       order: list[Order] | None = None,
+                       connection: Connection | None = None) -> dict[str, any] | None:
         """Find one record from passed filters.
         :param aliases: List of fields that will be selected by the query.
         :param conditions: List of filters that will be applied to query.
         :param order: Order that will be applied to query.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Record as dictionary.
         """
 
         criterion = self._conditions_to_criterion(conditions)
 
         return await self._find_one(aliases, criterion, order, connection)
 
-    async def find_all(self, aliases: Optional[List[str]] = None,
-                       conditions: Optional[List[Condition]] = None,
-                       order: Optional[List[Order]] = None,
-                       connection: Optional[Connection] = None) -> List[Dict[str, any]]:
+    async def find_all(self, aliases: list[str] | None = None,
+                       conditions: list[Condition] | None = None,
+                       order: list[Order] | None = None,
+                       connection: Connection | None = None) -> list[dict[str, any]]:
         """Find all records from passed filters.
         :param aliases: List of fields that will be selected by the query.
         :param conditions: List of filters that will be applied to query.
         :param order: Order in which the records will be returned.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Records as dictionary list.
         """
 
         criterion = self._conditions_to_criterion(conditions)
 
         return await self._find_all(aliases, criterion, order, connection)
 
-    async def find_all_by_id(self, keys: List[Key],
-                             aliases: Optional[List[str]] = None,
-                             order: Optional[List[Order]] = None,
-                             connection: Optional[Connection] = None) -> List[Dict[str, any]]:
+    async def find_all_by_id(self, keys: list[Key],
+                             aliases: list[str] | None = None,
+                             order: list[Order] | None = None,
+                             connection: Connection | None = None) -> list[dict[str, any]]:
         """Find all records from passed keys.
         :param keys: Records identifiers.
         :param aliases: List of fields that will be selected by the query.
         :param order: Order in which the records will be returned.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Record as dictionary.
         """
@@ -434,19 +446,19 @@
         if not keys:
             raise DatabaseError("no keys provided")
 
         criterion = Criterion.any([self._create_primary_key_criterion(key) for key in keys])
 
         return await self._find_all(aliases, criterion, order, connection)
 
-    async def find_all_page(self, aliases: Optional[List[str]] = None,
-                            conditions: Optional[List[Condition]] = None,
+    async def find_all_page(self, aliases: list[str] | None = None,
+                            conditions: list[Condition] | None = None,
                             page: Pageable = Pageable(),
-                            order: Optional[List[Order]] = None,
-                            connection: Optional[Connection] = None) -> Union[Page, Top]:
+                            order: list[Order] | None = None,
+                            connection: Connection | None = None) -> Page | Top:
         """Find records from passed filters using paging.
         :param aliases: List of fields that will be selected by the query.
         :param conditions: List of filters that will be applied to query.
         :param page: Limit and offset of the query.
         :param order: Order in which the records will be returned.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Records wrapped by Page or Top dataclass.
@@ -455,17 +467,17 @@
         criterion = self._conditions_to_criterion(conditions)
 
         if connection:
             return await self._find_all_page(connection, aliases, criterion, page, order)
         async with self._pool.acquire() as connection_:
             return await self._find_all_page(connection_, aliases, criterion, page, order)
 
-    async def insert(self, data: Union[Dict[str, any], BaseModel],
-                     returning_aliases: Optional[List[str]] = None,
-                     connection: Optional[Connection] = None) -> Dict[str, any]:
+    async def insert(self, data: BaseModel | dict[str, any],
+                     returning_aliases: list[str] | None = None,
+                     connection: Connection | None = None) -> dict[str, any]:
         """Insert one record from dictionary.
         :param data: Master column aliases with values.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to insert-constraints or no master column is specified.
         :return: Execution results as dictionary.
         """
@@ -480,44 +492,59 @@
             .columns(list(data_.keys())) \
             .insert(list(data_.values()))
 
         records = await self._execute(iq, returning_aliases, connection)
 
         return records[0] if len(records) > 0 else None
 
-    async def insert_returning_master_columns(self, data: Union[Dict[str, any], BaseModel],
-                                              connection: Optional[Connection] = None):
+    async def insert_returning_master(self, data: BaseModel | dict[str, any],
+                                      connection: Connection | None = None):
         """Insert one record from dictionary and return all master columns.
         :param data: Master column aliases with values.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to insert-constraints or no master column is specified.
         :return: Execution results as dictionary.
         """
 
-        return await self.insert(data, [i[0] for i in self._master_columns.items()], connection)
+        return await self.insert(data, list(self._master_columns.keys()), connection)
+
+    async def insert_data(self, data: BaseModel | dict[str, any],
+                          returning: type[T],
+                          connection: Connection | None = None) -> T:
+        """Insert a record using model.
+        :param data: Model which contains master table column properties.
+        :param returning: Result type.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :raise SaveError: When does not adjust to insert-constraints or no master column is specified.
+        :return: Execution results with returning type.
+        """
+
+        result = await self.insert(data, self.__base_model_aliases(returning), connection)
 
-    async def insert_bulk(self, aliases: List[str],
-                          data: List[List[any]],
-                          returning_aliases: Optional[List[str]] = None,
-                          connection: Optional[Connection] = None) -> List[Dict[str, any]]:
+        return returning(**result) if result else None
+
+    async def insert_bulk(self, aliases: list[str],
+                          data: list[list],
+                          returning_aliases: list[str] | None = None,
+                          connection: Connection | None = None) -> list[dict[str, any]]:
         """Insert many records at once from list.
         :param aliases: Master column aliases.
         :param data: Master column values.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to insert-constraints or no master column is specified.
-        :return: Execution results as dictionary list.
+        :return: Execution result as dictionary list.
         """
 
         for d in data:
             if len(d) == len(aliases):
                 continue
             raise SaveError("invalid bulk insert data")
 
-        column_names: Dict[str, int] = dict()
+        column_names: dict[str, int] = dict()
         for i, alias in enumerate(aliases):
             column = self._master_columns.get(alias)
             if not column:
                 continue
             if not column[1].insertable:
                 raise SaveError(f"column:'{column[1].name}' is not insertable", column[1].name)
             column_names[column[1].name] = i
@@ -529,68 +556,102 @@
             .columns(list(column_names.keys()))
 
         for d in data:
             iq = iq.insert([d[i] for i in column_names.values()])
 
         return await self._execute(iq, returning_aliases, connection)
 
-    async def update(self, data: Union[Dict[str, any], BaseModel],
-                     conditions: List[Condition],
-                     returning_aliases: Optional[List[str]] = None,
-                     connection: Optional[Connection] = None) -> Optional[List[Dict[str, any]]]:
+    async def update(self, data: BaseModel | dict[str, any],
+                     conditions: list[Condition],
+                     returning_aliases: list[str] | None = None,
+                     connection: Connection | None = None) -> list[dict[str, any]] | None:
         """Update records with new data according conditions.
         :param data: Master column aliases with values.
         :param conditions: List of filters that will be applied into the query.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to update-constraints or no master column is specified.
         :return: Execution results as dictionary list.
         """
 
         criterion = self._conditions_to_criterion(conditions, select=False)
 
         return await self._update(data, criterion, returning_aliases, connection)
 
     async def update_by_id(self, key: Key,
-                           data: Union[Dict[str, any], BaseModel],
-                           returning_aliases: Optional[List[str]] = None,
-                           connection: Optional[Connection] = None) -> Optional[Dict[str, any]]:
-        """Update records with new data according to passed key.
+                           data: BaseModel | dict[str, any],
+                           returning_aliases: list[str] | None = None,
+                           connection: Connection | None = None) -> dict[str, any] | None:
+        """Update record with new data according to passed key.
         :param key: Record identifier.
         :param data: Master column aliases with values.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to update-constraints or no master column is specified.
-        :return: Execution results as dictionary.
+        :return: Execution result as dictionary.
         """
 
         criterion = self._create_primary_key_criterion(key)
 
         records = await self._update(data, criterion, returning_aliases, connection)
 
         return records[0] if len(records) > 0 else None
 
-    async def delete(self, conditions: List[Condition],
-                     returning_aliases: Optional[List[str]] = None,
-                     connection: Optional[Connection] = None) -> Optional[List[Dict[str, any]]]:
+    async def update_data(self, data: BaseModel | dict[str, any],
+                          conditions: list[Condition],
+                          returning: type[T],
+                          connection: Connection | None = None) -> list[T] | None:
+        """Update records with new data according conditions using model.
+        :param data: Model which contains master table column properties.
+        :param conditions: List of filters that will be applied into the query.
+        :param returning: Result type.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :raise SaveError: When does not adjust to update-constraints or no master column is specified.
+        :return: Execution results with returning type.
+        """
+
+        results = await self.update(data, conditions, self.__base_model_aliases(returning), connection)
+
+        return [returning(**r) for r in results] if results else None
+
+    async def update_data_by_id(self, key: Key,
+                                data: BaseModel | dict[str, any],
+                                returning: type[T],
+                                connection: Connection | None = None) -> T | None:
+        """Update record with new data according to passed key using model.
+        :param key: Record identifier.
+        :param data: Model which contains master table column properties.
+        :param returning: Result type.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :raise SaveError: When does not adjust to update-constraints or no master column is specified.
+        :return: Execution result with returning type.
+        """
+
+        result = await self.update_by_id(key, data, self.__base_model_aliases(returning), connection)
+
+        return returning(**result) if result else None
+
+    async def delete(self, conditions: list[Condition],
+                     returning_aliases: list[str] | None = None,
+                     connection: Connection | None = None) -> list[dict[str, any]] | None:
         """Delete records according conditions.
         :param conditions: List of filters that will be applied into the query.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When conditions are empty.
         :return: Execution results as dictionary list.
         """
 
         criterion = self._conditions_to_criterion(conditions, select=False)
 
         return await self._delete(criterion, returning_aliases, connection)
 
     async def delete_by_id(self, key: Key,
-                           returning_aliases: Optional[List[str]] = None,
-                           connection: Optional[Connection] = None) -> Optional[Dict[str, any]]:
+                           returning_aliases: list[str] | None = None,
+                           connection: Connection | None = None) -> dict[str, any] | None:
         """Delete records according to passed key.
         :param key: Record identifier.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When conditions are empty.
         :return: Execution results as dictionary.
         """
```

### Comparing `braincube-aws-core-alpha-0.0.18/src/core/di/data.py` & `braincube-aws-core-alpha-0.0.19/src/core/di/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.18/src/core/di/injector.py` & `braincube-aws-core-alpha-0.0.19/src/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.18/src/core/rest/app_controller.py` & `braincube-aws-core-alpha-0.0.19/src/core/rest/app_controller.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.18/src/core/rest/app_module.py` & `braincube-aws-core-alpha-0.0.19/src/core/rest/app_module.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.18/src/core/rest/data.py` & `braincube-aws-core-alpha-0.0.19/src/core/rest/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.18/src/core/utils/convert.py` & `braincube-aws-core-alpha-0.0.19/src/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.18/src/core/utils/data.py` & `braincube-aws-core-alpha-0.0.19/src/core/utils/data.py`

 * *Files identical despite different names*

