# Comparing `tmp/elefantolib_fastapi-0.2.0.tar.gz` & `tmp/elefantolib_fastapi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefantolib_fastapi-0.2.0.tar", max compression
+gzip compressed data, was "elefantolib_fastapi-0.2.1.tar", max compression
```

## Comparing `elefantolib_fastapi-0.2.0.tar` & `elefantolib_fastapi-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      904 2023-04-24 17:24:20.772908 elefantolib_fastapi-0.2.0/README.md
--rw-r--r--   0        0        0       22 2023-04-24 17:24:20.772908 elefantolib_fastapi-0.2.0/elefantolib_fastapi/__init__.py
--rw-r--r--   0        0        0      179 2023-04-24 17:24:20.772908 elefantolib_fastapi-0.2.0/elefantolib_fastapi/requests.py
--rw-r--r--   0        0        0      821 2023-04-24 17:24:20.772908 elefantolib_fastapi-0.2.0/elefantolib_fastapi/routes.py
--rw-r--r--   0        0        0      872 2023-04-24 17:24:37.081065 elefantolib_fastapi-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.2.0/setup.py
--rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      878 2023-05-08 21:24:10.556377 elefantolib_fastapi-0.2.1/README.md
+-rw-r--r--   0        0        0       22 2023-05-08 21:24:10.556377 elefantolib_fastapi-0.2.1/elefantolib_fastapi/__init__.py
+-rw-r--r--   0        0        0      247 2023-05-08 21:24:10.556377 elefantolib_fastapi-0.2.1/elefantolib_fastapi/requests.py
+-rw-r--r--   0        0        0      898 2023-05-08 21:24:10.556377 elefantolib_fastapi-0.2.1/elefantolib_fastapi/routes.py
+-rw-r--r--   0        0        0      889 2023-05-08 21:24:22.816527 elefantolib_fastapi-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1605 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.2.1/setup.py
+-rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.2.1/PKG-INFO
```

### Comparing `elefantolib_fastapi-0.2.0/README.md` & `elefantolib_fastapi-0.2.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -35,24 +35,24 @@
     - ISSUER=Consumer
 
 ### Create it
 
 * Create a file `main.py` with:
 
 ```Python
-from elefantolib_fastapi.requests import ElefantoRequest
-from elefantolib_fastapi.routes import ElefantoRoute
+from elefantolib_fastapi.requests import Request
+from elefantolib_fastapi.routes import APIRoute
 
 from fastapi import FastAPI
 
 app = FastAPI()
 
-app.router.route_class = ElefantoRoute
+app.router.route_class = APIRoute
 
 
 @app.get('/')
-def index(request: ElefantoRequest):
+def index(request: Request):
     # TODO something
     response = request.pfm.services.some_service_name.get('path-to-endpoint')
     return response
 
 ```
```

### Comparing `elefantolib_fastapi-0.2.0/elefantolib_fastapi/routes.py` & `elefantolib_fastapi-0.2.1/elefantolib_fastapi/routes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-from typing import Any, Callable, Coroutine
+import os
+from typing import Callable
 
 from elefantolib import context
 from elefantolib.provider import fastapi_provider
 
-from fastapi import Request, Response
-from fastapi.routing import APIRoute
+import fastapi
+from fastapi import routing
 
-from .requests import ElefantoRequest
+from redis import asyncio as aioredis
 
+from .requests import Request
 
-class ElefantoRoute(APIRoute):
 
-    def get_route_handler(self) -> \
-            Callable[[Request], Coroutine[Any, Any, Response]]:
+class APIRoute(routing.APIRoute):
+
+    def get_route_handler(self) -> Callable:
         original_route_handler = super().get_route_handler()
 
-        async def custom_route_handler(request: Request) -> Response:
+        async def custom_route_handler(request: fastapi.Request) -> fastapi.Response:
             pvr = fastapi_provider.FastAPIProvider(request=request)
             request.scope['pfm'] = context.AsyncPlatformContext(pvr=pvr)
-            new_request = ElefantoRequest(request.scope, request.receive)
+
+            if redis_url := os.environ.get('REDIS_URL'):
+                request.scope['redis'] = aioredis.from_url(redis_url)
+
+            new_request = Request(request.scope, request.receive)
             return await original_route_handler(new_request)
         return custom_route_handler
```

### Comparing `elefantolib_fastapi-0.2.0/pyproject.toml` & `elefantolib_fastapi-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "elefantolib-fastapi"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["gglassota <gglassota2@gmail.com>"]
 readme = "README.md"
 packages = [{include = "elefantolib_fastapi"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 elefantolib = "^0.9.2"
 fastapi = "^0.95.1"
+redis = "^4.5.5"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 pytest-flake8 = "^1.1.1"
```

### Comparing `elefantolib_fastapi-0.2.0/setup.py` & `elefantolib_fastapi-0.2.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['elefantolib_fastapi']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['elefantolib>=0.9.2,<0.10.0', 'fastapi>=0.95.1,<0.96.0']
+['elefantolib>=0.9.2,<0.10.0', 'fastapi>=0.95.1,<0.96.0', 'redis>=4.5.5,<5.0.0']
 
 setup_kwargs = {
     'name': 'elefantolib-fastapi',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': '',
-    'long_description': '## Elefantolib for FastAPI\n\n> **_NOTE:_**  Only for this library developers. After clone this repository you should run command:\n> \n\n ```console \ngit config core.hooksPath .githooks\n```\n\n\n## Installation\n\n<div class="termy">\n\n```console\npoetry add elefantolib-fastapi\n```\n</div>\n\n## Example\n\n### Prepare\n\n* Add environmental variables\n\n```\nSECRET=\nALGORITHM=\nISSUER=\n```\n* Defaults:\n    \n    - SECRET - not set, this is required\n    - ALGORITHM=HS256\n    - ISSUER=Consumer\n\n### Create it\n\n* Create a file `main.py` with:\n\n```Python\nfrom elefantolib_fastapi.requests import ElefantoRequest\nfrom elefantolib_fastapi.routes import ElefantoRoute\n\nfrom fastapi import FastAPI\n\napp = FastAPI()\n\napp.router.route_class = ElefantoRoute\n\n\n@app.get(\'/\')\ndef index(request: ElefantoRequest):\n    # TODO something\n    response = request.pfm.services.some_service_name.get(\'path-to-endpoint\')\n    return response\n\n```',
+    'long_description': '## Elefantolib for FastAPI\n\n> **_NOTE:_**  Only for this library developers. After clone this repository you should run command:\n> \n\n ```console \ngit config core.hooksPath .githooks\n```\n\n\n## Installation\n\n<div class="termy">\n\n```console\npoetry add elefantolib-fastapi\n```\n</div>\n\n## Example\n\n### Prepare\n\n* Add environmental variables\n\n```\nSECRET=\nALGORITHM=\nISSUER=\n```\n* Defaults:\n    \n    - SECRET - not set, this is required\n    - ALGORITHM=HS256\n    - ISSUER=Consumer\n\n### Create it\n\n* Create a file `main.py` with:\n\n```Python\nfrom elefantolib_fastapi.requests import Request\nfrom elefantolib_fastapi.routes import APIRoute\n\nfrom fastapi import FastAPI\n\napp = FastAPI()\n\napp.router.route_class = APIRoute\n\n\n@app.get(\'/\')\ndef index(request: Request):\n    # TODO something\n    response = request.pfm.services.some_service_name.get(\'path-to-endpoint\')\n    return response\n\n```',
     'author': 'gglassota',
     'author_email': 'gglassota2@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `elefantolib_fastapi-0.2.0/PKG-INFO` & `elefantolib_fastapi-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: elefantolib-fastapi
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: gglassota
 Author-email: gglassota2@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: elefantolib (>=0.9.2,<0.10.0)
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
+Requires-Dist: redis (>=4.5.5,<5.0.0)
 Description-Content-Type: text/markdown
 
 ## Elefantolib for FastAPI
 
 > **_NOTE:_**  Only for this library developers. After clone this repository you should run command:
 > 
 
@@ -49,24 +50,24 @@
     - ISSUER=Consumer
 
 ### Create it
 
 * Create a file `main.py` with:
 
 ```Python
-from elefantolib_fastapi.requests import ElefantoRequest
-from elefantolib_fastapi.routes import ElefantoRoute
+from elefantolib_fastapi.requests import Request
+from elefantolib_fastapi.routes import APIRoute
 
 from fastapi import FastAPI
 
 app = FastAPI()
 
-app.router.route_class = ElefantoRoute
+app.router.route_class = APIRoute
 
 
 @app.get('/')
-def index(request: ElefantoRequest):
+def index(request: Request):
     # TODO something
     response = request.pfm.services.some_service_name.get('path-to-endpoint')
     return response
 
 ```
```

