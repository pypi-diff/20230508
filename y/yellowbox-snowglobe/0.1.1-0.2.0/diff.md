# Comparing `tmp/yellowbox-snowglobe-0.1.1.tar.gz` & `tmp/yellowbox_snowglobe-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowbox-snowglobe-0.1.1.tar", max compression
+gzip compressed data, was "yellowbox_snowglobe-0.2.0.tar", max compression
```

## Comparing `yellowbox-snowglobe-0.1.1.tar` & `yellowbox_snowglobe-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2022-08-23 15:22:52.761086 yellowbox-snowglobe-0.1.1/LICENSE
--rw-r--r--   0        0        0      526 2022-08-23 15:22:52.761086 yellowbox-snowglobe-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      157 2022-08-23 15:22:52.761086 yellowbox-snowglobe-0.1.1/yellowbox_snowglobe/__init__.py
--rw-r--r--   0        0        0       22 2022-08-23 15:22:52.761086 yellowbox-snowglobe-0.1.1/yellowbox_snowglobe/_version.py
--rw-r--r--   0        0        0     7070 2022-08-23 15:22:52.761086 yellowbox-snowglobe-0.1.1/yellowbox_snowglobe/api.py
--rw-r--r--   0        0        0      508 2022-08-23 15:22:52.761086 yellowbox-snowglobe-0.1.1/yellowbox_snowglobe/schema_init.py
--rw-r--r--   0        0        0     1416 2022-08-23 15:22:52.761086 yellowbox-snowglobe-0.1.1/yellowbox_snowglobe/service.py
--rw-r--r--   0        0        0     5927 2022-08-23 15:22:52.761086 yellowbox-snowglobe-0.1.1/yellowbox_snowglobe/session.py
--rw-r--r--   0        0        0     6266 2022-08-23 15:22:52.761086 yellowbox-snowglobe-0.1.1/yellowbox_snowglobe/snow_to_post.py
--rw-r--r--   0        0        0      629 2022-08-23 15:24:25.762366 yellowbox-snowglobe-0.1.1/setup.py
--rw-r--r--   0        0        0      530 2022-08-23 15:24:25.762649 yellowbox-snowglobe-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-08 13:24:31.698884 yellowbox_snowglobe-0.2.0/LICENSE
+-rw-r--r--   0        0        0      523 2023-05-08 13:24:31.698884 yellowbox_snowglobe-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-05-08 13:24:31.698884 yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-08 13:24:31.698884 yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/_version.py
+-rw-r--r--   0        0        0     7427 2023-05-08 13:24:31.698884 yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/api.py
+-rw-r--r--   0        0        0     1426 2023-05-08 13:24:31.698884 yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/case_mode.py
+-rw-r--r--   0        0        0      508 2023-05-08 13:24:31.698884 yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/schema_init.py
+-rw-r--r--   0        0        0     1834 2023-05-08 13:24:31.698884 yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/service.py
+-rw-r--r--   0        0        0     6417 2023-05-08 13:24:31.698884 yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/session.py
+-rw-r--r--   0        0        0     6403 2023-05-08 13:24:31.698884 yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/snow_to_post.py
+-rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 yellowbox_snowglobe-0.2.0/PKG-INFO
```

### Comparing `yellowbox-snowglobe-0.1.1/LICENSE` & `yellowbox_snowglobe-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowbox-snowglobe-0.1.1/pyproject.toml` & `yellowbox_snowglobe-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "yellowbox-snowglobe"
-version = "0.1.1"
+version = "0.2.0"
 description = ""
 authors = ["Biocatch LTD <serverteam@biocatch.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 yellowbox = { version = ">=0.7.0", extras = ["postgresql", "webserver"] }
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-asyncio = "*"
 flake8 = "*"
 pytest-cov = "*"
 isort = "^5.10.1"
-mypy = "^0.960"
+mypy = ">=1"
 snowflake-connector-python = "^2.7.11"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `yellowbox-snowglobe-0.1.1/yellowbox_snowglobe/api.py` & `yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__ import annotations
 
 import gzip
 import json
 from dataclasses import dataclass
 from datetime import datetime
 from traceback import print_exc
-from typing import Any, Callable, Dict, List, Optional
+from typing import Any, Callable, Container, Dict, List, Optional, Sequence
 from uuid import uuid4
 
 from sqlalchemy.engine import Row
 from starlette.exceptions import HTTPException
 from starlette.requests import Request
 from starlette.responses import JSONResponse, Response
 from yellowbox.extras.postgresql import PostgreSQLService
 from yellowbox.extras.webserver import WebServer, class_http_endpoint
 
+from yellowbox_snowglobe.case_mode import CaseMode
 from yellowbox_snowglobe.session import SnowGlobeSession
 from yellowbox_snowglobe.snow_to_post import snow_to_post, split_sql_to_statements
 
 
 async def unpack_request_body(request: Request):
     body = await request.body()
     uz = gzip.decompress(body)
@@ -44,54 +45,55 @@
     bool: SnowType('BOOLEAN', lambda x: str(int(x))),
     datetime: SnowType('DATETIME', str)
 }  # todo there are a lot more
 
 VARIANT = SnowType('VARIANT')  # this will be the default snow type for when we can't handle the result type
 
 
-def sql_alchemy_result_to_snowglobe_result(result: List[Row]) -> Dict[str, Any]:
-    col_names = result[0]._fields
-    columns = [{'name': col_name.upper(), "length": 0, "precision": 0, "scale": 0, "nullable": False}
-               for col_name in col_names]
-    rows = [list(row) for row in result]
-    for i, col in enumerate(columns):
-        t = None
-        for row in rows:
-            if row[i] is None:
-                col['nullable'] = True
-            else:
-                proposed_type = PY_TYPE_TO_SNOW_TYPE.get(type(row[i]))
-                if proposed_type is None:
-                    # unrecognized type, call it a variant and be done with it
-                    t = VARIANT
-                elif t is None:
-                    t = proposed_type
-                elif t != proposed_type:
-                    # type conflict (I don't know if this can even happen), call it a variant
-                    t = VARIANT
-        if t is None:
-            # if no type was found, we default the column type to variant, AFAICT this will only happen for a result
-            # without rows
-            t = VARIANT
-        col['type'] = t.name
-        if t.connector_converter is not None:
-            for row in rows:
-                row[i] = t.connector_converter(row[i])
-    return {'rowtype': columns, 'rowset': rows}
-
-
 class SnowGlobeAPI(WebServer):
-    def __init__(self, *args, sql_service: PostgreSQLService, metadata_table_name: str, **kwargs):
+    def __init__(self, *args, sql_service: PostgreSQLService, metadata_table_name: str, case_mode: CaseMode, **kwargs):
         super().__init__('snowglobe', *args, **kwargs)
         self.sql_service = sql_service
+        self.case_mode = case_mode
 
         self.sessions: Dict[str, SnowGlobeSession] = {}  # stores all the live sessions
         self.metadata_table_name = metadata_table_name
 
-        self.query_results: Dict[str, List[Row]] = {}  # stores all the async query results
+        self.query_results: Dict[str, Sequence[Row]] = {}  # stores all the async query results
+
+    def sql_alchemy_result_to_snowglobe_result(self, result: List[Row], known_columns: Container[str])\
+            -> Dict[str, Any]:
+        col_names = result[0]._fields
+        columns = [{'name': self.case_mode.convert(col_name, known_columns), "length": 0, "precision": 0, "scale": 0,
+                    "nullable": False} for col_name in col_names]
+        rows = [list(row) for row in result]
+        for i, col in enumerate(columns):
+            t = None
+            for row in rows:
+                if row[i] is None:
+                    col['nullable'] = True
+                else:
+                    proposed_type = PY_TYPE_TO_SNOW_TYPE.get(type(row[i]))
+                    if proposed_type is None:
+                        # unrecognized type, call it a variant and be done with it
+                        t = VARIANT
+                    elif t is None:
+                        t = proposed_type
+                    elif t != proposed_type:
+                        # type conflict (I don't know if this can even happen), call it a variant
+                        t = VARIANT
+            if t is None:
+                # if no type was found, we default the column type to variant, AFAICT this will only happen for a result
+                # without rows
+                t = VARIANT
+            col['type'] = t.name
+            if t.connector_converter is not None:
+                for row in rows:
+                    row[i] = t.connector_converter(row[i])
+        return {'rowtype': columns, 'rowset': rows}
 
     def session_from_request(self, request):
         """
         Get a request's relevant session
         """
         auth = request.headers.get('Authorization')
         if not auth:
@@ -145,15 +147,15 @@
                 "queryId": query_id,
             }
             if not result:
                 return JSONResponse({'data': data, 'success': True})
             if body.get('asyncExec', False):
                 # we should store the result in the server for when it gets retrieved
                 self.query_results[query_id] = result
-            data.update(sql_alchemy_result_to_snowglobe_result(result))
+            data.update(self.sql_alchemy_result_to_snowglobe_result(result, session.known_columns))
             return JSONResponse({'data': data, 'success': True})
         except Exception as e:
             print_exc()  # we print exec here because the connector + webservice combo doesn't always do a good job of
             # telling us what the error is (or that it's happening)
             return JSONResponse({'success': False, 'message': str(e)})
 
     @class_http_endpoint(['GET'], '/monitoring/queries/{query_id:str}')  # type: ignore[arg-type]
```

### Comparing `yellowbox-snowglobe-0.1.1/yellowbox_snowglobe/service.py` & `yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,43 @@
+from yellowbox import AsyncRunMixin, RunMixin, YellowService
 from yellowbox.extras.postgresql import PostgreSQLService
 from yellowbox.utils import docker_host_name
 
 from yellowbox_snowglobe.api import SnowGlobeAPI
+from yellowbox_snowglobe.case_mode import CaseMode, IgnoreAll
 
 
-class SnowGlobeService(PostgreSQLService):
-    def __init__(self, *args, metadata_table_name: str = '__snowglobe_md', **kwargs):
-        super().__init__(*args, **kwargs)
-        self.api = SnowGlobeAPI(sql_service=self, metadata_table_name=metadata_table_name)
+class SnowGlobeService(YellowService, RunMixin, AsyncRunMixin):
+    def __init__(self, *args, metadata_table_name: str = '__snowglobe_md', case_mode: CaseMode = IgnoreAll(), **kwargs):
+        super().__init__()
+        self.sql_service = PostgreSQLService(*args, **kwargs)
+        self.api = SnowGlobeAPI(sql_service=self.sql_service, metadata_table_name=metadata_table_name,
+                                case_mode=case_mode)
 
     @property
     def api_port(self):
         # the http port snowflake connectors should use to connect
         return self.api.port
 
     def start(self, *args, **kwargs):
-        super().start(*args, **kwargs)
+        self.sql_service.start(*args, **kwargs)
         self.api.start()
         return self
 
     async def astart(self, *args, **kwargs):
-        await super().astart(*args, **kwargs)
+        await self.sql_service.astart(*args, **kwargs)
         self.api.start()
         return self
 
     def stop(self, *args):
         self.api.stop()
-        super().stop(*args)
+        self.sql_service.stop(*args)
+
+    def is_alive(self) -> bool:
+        return self.api.is_alive() and self.sql_service.is_alive()
 
     def _base_connection_kwargs(self):
         return dict(
             port=self.api_port,
             user='MyUser',
             password='MyPass',
             account='MyAccount',
```

### Comparing `yellowbox-snowglobe-0.1.1/yellowbox_snowglobe/session.py` & `yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/session.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, Optional, Sequence, Set
 
 from sqlalchemy import create_engine, text
 from sqlalchemy.engine import Connection, Engine, Row, Transaction
 
 from yellowbox_snowglobe.schema_init import SCHEMA_INITIALIZE_SCRIPT
 
 if TYPE_CHECKING:
     from yellowbox_snowglobe.api import SnowGlobeAPI
 
-QUERY_RESPONSE = Optional[List[Row]]
+QUERY_RESPONSE = Optional[Sequence[Row]]
 
 
 class SnowGlobeSession:
     # a session is an individual connection, containing all the data associated with it.
     next_token = 0  # each session is identified by a token the connector must send on every request
 
     def __init__(self, owner: SnowGlobeAPI, db: Optional[str], schema: str):
@@ -24,14 +24,17 @@
         self.next_token += 1
         self.schema = schema
         # all these fields are set and replaced together when we switch the DB
         self.db: Optional[str] = None
         self.engine: Optional[Engine] = None
         self._connection: Optional[Connection] = None
         self._transaction: Optional[Transaction] = None
+
+        self.known_columns: Set[str] = set()  # stores all the columns we know about, updates when a create or alter
+        # is called
         if db:
             self.switch_db(db, schema)
 
     @property
     def connection(self) -> Connection:
         if not self._connection:
             raise Exception("No connection exists, make sure to use a database first")
@@ -63,15 +66,15 @@
         with self.connection.begin_nested():
             # right now, the only indicator of initialization is the presence of the metadata table
             exists = self.connection.execute(text(f"SELECT EXISTS(SELECT FROM information_schema.tables"
                                                   f" WHERE  table_schema = '{self.schema}'"
                                                   f" AND table_name = '{self.owner.metadata_table_name}')")).scalar()
             if exists:
                 return
-            self.connection.execute(f'SET search_path TO {self.schema};')
+            self.connection.execute(text(f'SET search_path TO {self.schema};'))
             self.connection.execute(SCHEMA_INITIALIZE_SCRIPT)
             self.connection.execute(text(f"CREATE TABLE IF NOT EXISTS {self.owner.metadata_table_name}()"))
 
     def do_query(self, query: str) -> QUERY_RESPONSE:
         # queries are always normalized to be without a semicolon
         query_lower = query.lower()
         prefix_search_root: Any = self.FUNC_BY_PREFIX
@@ -119,14 +122,20 @@
 
     def _do_select(self, query) -> QUERY_RESPONSE:
         result = self.connection.execute(text(query)).all()
         return result
 
     def _do_mutating_noresponse(self, query) -> QUERY_RESPONSE:
         self.connection.execute(text(query))
+        # we need to update the known columns here
+        result = self.connection.execute(text(
+            "select column_name from information_schema.columns c where c.table_schema <> 'pg_catalog'"
+            "AND c.table_schema <> 'information_schema';"
+        ))
+        self.known_columns = set(result.scalars().fetchall())
         return None
 
     # endregion
 
     # here we map SQL keywords to whichever handler we want to use on queries with them
     # think of this like a prefix trie, with NONE as a fallback
     # all keywords beginning with "!" are specially generated by the post_to_snow transpiler.
```

### Comparing `yellowbox-snowglobe-0.1.1/yellowbox_snowglobe/snow_to_post.py` & `yellowbox_snowglobe-0.2.0/yellowbox_snowglobe/snow_to_post.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,16 @@
          " FROM information_schema.tables WHERE table_type = 'BASE TABLE'"),
     # describe table
     Rule(re.compile(r"(?i)(describe|desc)\s+table\s+(" + NAME_PATTERN + r")"),
          "SELECT column_name as name, data_type as type, 'COLUMN' as kind, is_nullable as \"null?\","
          " column_default as default, NULL as primary_key, NULL as unique_key, NULL as check,"
          " NULL as expression, NULL as comment, NULL as \"policy name\" FROM information_schema.columns"
          r" WHERE table_name = '\2'"),
+    # Ignore sample in queries
+    Rule(re.compile(r"(?i)\bsample\s+\(([0-9\.]+)\s+rows\)"), replacement=r"order by random() limit \1"),
 ]
 
 
 def repl_part(part: Union[str, TextLiteral], rules: Iterable[Rule]) -> str:
     if isinstance(part, TextLiteral):
         return part.value
     ret_parts = []
```

### Comparing `yellowbox-snowglobe-0.1.1/PKG-INFO` & `yellowbox_snowglobe-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: yellowbox-snowglobe
-Version: 0.1.1
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: Biocatch LTD
 Author-email: serverteam@biocatch.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: yellowbox[webserver,postgresql] (>=0.7.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: yellowbox[postgresql,webserver] (>=0.7.0)
```

