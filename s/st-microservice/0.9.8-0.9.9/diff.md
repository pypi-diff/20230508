# Comparing `tmp/st_microservice-0.9.8.tar.gz` & `tmp/st_microservice-0.9.9.tar.gz`

## Comparing `st_microservice-0.9.8.tar` & `st_microservice-0.9.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 st_microservice-0.9.8/src/st_microservice/__init__.py
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 st_microservice-0.9.8/src/st_microservice/auth_utils.py
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 st_microservice-0.9.8/src/st_microservice/filter_parser.py
--rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 st_microservice-0.9.8/src/st_microservice/graphql_app.py
--rw-r--r--   0        0        0     8086 2020-02-02 00:00:00.000000 st_microservice-0.9.8/src/st_microservice/graphql_utils.py
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 st_microservice-0.9.8/src/st_microservice/starlettebackend.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 st_microservice-0.9.8/.gitignore
--rw-r--r--   0        0        0    35182 2020-02-02 00:00:00.000000 st_microservice-0.9.8/LICENSE.txt
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 st_microservice-0.9.8/README.md
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 st_microservice-0.9.8/pyproject.toml
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 st_microservice-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 st_microservice-0.9.9/src/st_microservice/__init__.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 st_microservice-0.9.9/src/st_microservice/auth_utils.py
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 st_microservice-0.9.9/src/st_microservice/filter_parser.py
+-rw-r--r--   0        0        0     8081 2020-02-02 00:00:00.000000 st_microservice-0.9.9/src/st_microservice/graphql_app.py
+-rw-r--r--   0        0        0     8086 2020-02-02 00:00:00.000000 st_microservice-0.9.9/src/st_microservice/graphql_utils.py
+-rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 st_microservice-0.9.9/src/st_microservice/starlettebackend.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 st_microservice-0.9.9/.gitignore
+-rw-r--r--   0        0        0    35182 2020-02-02 00:00:00.000000 st_microservice-0.9.9/LICENSE.txt
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 st_microservice-0.9.9/README.md
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 st_microservice-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 st_microservice-0.9.9/PKG-INFO
```

### Comparing `st_microservice-0.9.8/src/st_microservice/auth_utils.py` & `st_microservice-0.9.9/src/st_microservice/auth_utils.py`

 * *Files identical despite different names*

### Comparing `st_microservice-0.9.8/src/st_microservice/filter_parser.py` & `st_microservice-0.9.9/src/st_microservice/filter_parser.py`

 * *Files identical despite different names*

### Comparing `st_microservice-0.9.8/src/st_microservice/graphql_app.py` & `st_microservice-0.9.9/src/st_microservice/graphql_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Union, List, Any, Mapping
 import asyncio
 from datetime import date, datetime
-from graphql import GraphQLField, GraphQLObjectType, GraphQLInterfaceType, GraphQLResolveInfo
+from graphql import GraphQLField, GraphQLObjectType, GraphQLInterfaceType, GraphQLResolveInfo, MiddlewareManager
 from ariadne import load_schema_from_path, make_executable_schema, SchemaDirectiveVisitor, FallbackResolversSetter, \
     ScalarType
 from ariadne.graphql import GraphQLError
 from ariadne.asgi import GraphQL
+from ariadne.asgi.handlers import GraphQLHTTPHandler, GraphQLWSHandler
 from ariadne.types import Extension, SchemaBindable
 
 from .auth_utils import get_token_from_header, get_user_from_token, JWTAuthBackend, AuthCredentials
 
 
 # Directives
 
@@ -224,9 +225,16 @@
         'need_permission': NeedPermissionDirective,
         'db_model': DBModelDirective,
         'all_filter': AllFilterDirective,
         'filter': FilterDirective,
         'no_filter': NoFilterDirective
     })
 
-    return GraphQL(schema, debug=debug, middleware=[check_permission_middleware], extensions=[DBRollbackExtension],
-                   on_connect=on_websocket_connect)
+    return GraphQL(
+        schema,
+        debug=debug,
+        http_handler=GraphQLHTTPHandler(
+            middleware=[MiddlewareManager(check_permission_middleware)],
+            extensions=[DBRollbackExtension]
+        ),
+        websocket_handler=GraphQLWSHandler(on_connect=on_websocket_connect)
+    )
```

### Comparing `st_microservice-0.9.8/src/st_microservice/graphql_utils.py` & `st_microservice-0.9.9/src/st_microservice/graphql_utils.py`

 * *Files identical despite different names*

### Comparing `st_microservice-0.9.8/src/st_microservice/starlettebackend.py` & `st_microservice-0.9.9/src/st_microservice/starlettebackend.py`

 * *Files identical despite different names*

### Comparing `st_microservice-0.9.8/LICENSE.txt` & `st_microservice-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_microservice-0.9.8/pyproject.toml` & `st_microservice-0.9.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "st-microservice"
-version = "0.9.8"
+version = "0.9.9"
 authors = [
     {name = "Robert Trad", email = "roberttrad@gmail.com" }
 ]
 description = "Tools to build Microservice Backends"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent"
 ]
 dependencies = [
-    "ariadne==0.15.1",
-    "starlette<0.20",
+    "ariadne==0.16.0",
+    "starlette<0.21",
     "websockets<11",
     "PyJWT>=2.1.0,<3",
     "sqlalchemy<1.5",
     "pyparsing>=3.0.0,<4"
 ]
 
 [project.urls]
```

### Comparing `st_microservice-0.9.8/PKG-INFO` & `st_microservice-0.9.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: st-microservice
-Version: 0.9.8
+Version: 0.9.9
 Summary: Tools to build Microservice Backends
 Project-URL: Homepage, https://github.com/rouppart/ST-Microservice
 Author-email: Robert Trad <roberttrad@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
-Requires-Dist: ariadne==0.15.1
+Requires-Dist: ariadne==0.16.0
 Requires-Dist: pyjwt<3,>=2.1.0
 Requires-Dist: pyparsing<4,>=3.0.0
 Requires-Dist: sqlalchemy<1.5
-Requires-Dist: starlette<0.20
+Requires-Dist: starlette<0.21
 Requires-Dist: websockets<11
 Description-Content-Type: text/markdown
 
 # Tools to build microservice
 
 Backend of the Saad & Trad microservices architecture based on Graphql, Starlette and SQLAlchemy
```

