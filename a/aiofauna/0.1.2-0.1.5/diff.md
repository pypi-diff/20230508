# Comparing `tmp/aiofauna-0.1.2.tar.gz` & `tmp/aiofauna-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiofauna-0.1.2.tar", max compression
+gzip compressed data, was "aiofauna-0.1.5.tar", max compression
```

## Comparing `aiofauna-0.1.2.tar` & `aiofauna-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,18 @@
--rw-r--r--   0        0        0     3619 2023-05-05 14:04:33.858503 aiofauna-0.1.2/aiofauna/__init__.py
--rw-r--r--   0        0        0    17190 2023-05-05 14:01:54.151818 aiofauna-0.1.2/aiofauna/api.py
--rw-r--r--   0        0        0      819 2023-05-06 04:21:31.770848 aiofauna-0.1.2/aiofauna/cli.py
--rw-r--r--   0        0        0     4014 2023-05-05 14:00:20.387576 aiofauna-0.1.2/aiofauna/client.py
--rw-r--r--   0        0        0      529 2023-05-05 14:00:19.927579 aiofauna-0.1.2/aiofauna/deprecated.py
--rw-r--r--   0        0        0     8161 2023-05-05 14:00:19.463582 aiofauna-0.1.2/aiofauna/errors.py
--rw-r--r--   0        0        0     6673 2023-05-05 14:00:19.003585 aiofauna-0.1.2/aiofauna/json.py
--rw-r--r--   0        0        0     5861 2023-05-05 14:00:18.547588 aiofauna-0.1.2/aiofauna/objects.py
--rw-r--r--   0        0        0    14595 2023-05-06 08:00:24.709545 aiofauna-0.1.2/aiofauna/odm.py
--rw-r--r--   0        0        0     2760 2023-05-05 14:00:17.607594 aiofauna-0.1.2/aiofauna/page.py
--rw-r--r--   0        0        0    41588 2023-05-05 14:00:16.947598 aiofauna-0.1.2/aiofauna/query.py
--rw-r--r--   0        0        0      515 2023-05-06 08:02:13.509398 aiofauna-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      859 2023-05-06 08:02:46.814771 aiofauna-0.1.2/setup.py
--rw-r--r--   0        0        0      677 2023-05-06 08:02:46.815555 aiofauna-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1126 2023-05-08 06:43:22.972944 aiofauna-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2678 2023-05-08 04:44:25.192212 aiofauna-0.1.5/README.md
+-rw-r--r--   0        0        0     3656 2023-05-08 06:40:40.439634 aiofauna-0.1.5/aiofauna/__init__.py
+-rw-r--r--   0        0        0    16481 2023-05-08 06:40:40.591631 aiofauna-0.1.5/aiofauna/api.py
+-rw-r--r--   0        0        0     3304 2023-05-08 02:52:55.686757 aiofauna-0.1.5/aiofauna/asgi.py
+-rw-r--r--   0        0        0     7679 2023-05-08 06:40:32.547771 aiofauna-0.1.5/aiofauna/client.py
+-rw-r--r--   0        0        0     3678 2023-05-08 02:23:17.855099 aiofauna-0.1.5/aiofauna/datastructures.py
+-rw-r--r--   0        0        0      493 2023-05-06 09:16:36.202849 aiofauna-0.1.5/aiofauna/deprecated.py
+-rw-r--r--   0        0        0     8153 2023-05-08 02:23:18.327095 aiofauna-0.1.5/aiofauna/errors.py
+-rw-r--r--   0        0        0     4056 2023-05-08 06:40:40.455633 aiofauna-0.1.5/aiofauna/helpers.py
+-rw-r--r--   0        0        0     6728 2023-05-08 03:17:10.714267 aiofauna-0.1.5/aiofauna/json.py
+-rw-r--r--   0        0        0     5841 2023-05-08 02:23:18.171096 aiofauna-0.1.5/aiofauna/objects.py
+-rw-r--r--   0        0        0    14615 2023-05-08 06:40:40.567632 aiofauna-0.1.5/aiofauna/odm.py
+-rw-r--r--   0        0        0     2672 2023-05-08 02:26:21.521409 aiofauna-0.1.5/aiofauna/page.py
+-rw-r--r--   0        0        0    41561 2023-05-08 02:26:13.437479 aiofauna-0.1.5/aiofauna/query.py
+-rw-r--r--   0        0        0      660 2023-05-08 06:43:53.392466 aiofauna-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3597 2023-05-08 06:46:50.972162 aiofauna-0.1.5/setup.py
+-rw-r--r--   0        0        0     3697 2023-05-08 06:46:50.972446 aiofauna-0.1.5/PKG-INFO
```

### Comparing `aiofauna-0.1.2/aiofauna/__init__.py` & `aiofauna-0.1.5/aiofauna/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,81 +1,80 @@
-"""
----
-title: AioFauna
----
-
-# AioFauna
- 
- 🚀 Introducing aiofauna: A full-stack framework for FaunaDB, industry performant with a seamless user experience! 🔥 Take your Backend Development to the next level dramatically improving productivity, performance and development experience.
-
-🌟 Features:
-
-✅ Inspired by FastAPI: DX (Developer Experience) first. Based on Pydantic, Aiohttp, and FaunaDB. CORS support, query and path parameters, request body parsing, most of the features you love from FastAPI are available in aiofauna.
-
-✅ Blazingly Fast!: Industry performant http server while having the fastest python based http client allowing exceptional integrations with third party APIs, forget about installing dozens of SDKs.
-
-✅ Async/await coroutines: Leverage the power of async programming for enhanced performance and responsiveness. 
-
-✅ Automatic Swagger UI generation: Automatic documentation and manual testing UI following industry standard without further effort!.
-
-✅ Live reload and SSE (Server-Sent Events) support: Stream data in real-time to your clients and experience effortless development with live reload.
-
-✅ Pydantic-based Document Object Mapper (DOM): Define and validate your data models with ease. Summarize complex FQL expressions into pythonic, fully typed asynchronous methods for all CRUD operations.
-
-✅ Auto-provisioning: Automatic management of indexes, unique indexes, and collections.
-
-✅ Full JSON communication: Custom encoders to ensure seamless data exchange between your application and FaunaDB backend.
-
-💡 With aiofauna, you can build fast, scalable, and reliable applications using the power of FaunaDB and modern asynchronous Python with its out of the box aiohttp based web framework. Say goodbye to the hassle of manually managing indexes and collections and hello to a seamless data driven development experience with FaunaModel.
-
-🌐 aiofauna is independent and allows native interaction with external services like Docker API, GCP API, AWS API among others, implementing a lightweight stack with aiohttp server capabilities and fauna backend (to be enhanced soon).
-
-📚 Check out the aiofauna library, and start building your next-gen applications today! 🚀
-#Python #FaunaDB #Async #Pydantic #aiofauna
-
-⚙️ If you are using a synchronous framework check out [Faudantic](https://github.com/obahamonde/faudantic) for a similar experience with FaunaDB and Pydantic.
-
-📚 [Documentation](https://aiofauna.smartpro.solutions)
-
-📦 [PyPi](https://pypi.org/project/aiofauna/)
-
-📦 [GitHub](https://github.com/obahamonde/aiofauna)
-
-📦 [Demo](https://aiofaunastreams-fwuw7gz7oq-uc.a.run.app/) (Stream data in real-time to your clients)
-
-"""
-
-__version__ = (0, 1, 0)
-__author__ = "obahamonde"
-__license__ = "MIT"
-
-import json
-from datetime import datetime
-from typing import Any, AsyncGenerator, Callable, Dict, List, Optional, Union
-from uuid import UUID, uuid4
-
-import asyncio
-import aiohttp_cors
-
-from pydantic import BaseModel,BaseConfig, BaseSettings, Field  # pylint: disable=no-name-in-module
-
-from aiohttp.web import (
-    Application,
-    AppRunner,
-    Request,
-    Response,
-    RouteDef,
-    TCPSite,
-    json_response,
-)
-from aiohttp.web_middlewares import middleware
-from aiohttp_sse import sse_response
-from .client import ClientSession, AsyncFaunaClient as FaunaClient
-from .errors import AioFaunaException as FaunaException
-from . import query as q
-from .json import (
-    FaunaJSONEncoder as JSONEncoder,
-    to_json as dumps,
-    parse_json_or_none as loads,
-)
-from .odm import AsyncFaunaModel as FaunaModel
-from .api import Api
+"""
+---
+title: AioFauna
+---
+# AioFauna
+
+🚀 Introducing aiofauna: A full-stack framework built on top of Aiohttp, Pydantic and FaunaDB.
+
+🔥 Inspired by FastAPI focuses on Developer Experience, Productivity and Versatility.
+
+🌟 Features:
+
+✅ Supports Python 3.7+, comes with an opinionated ODM (Object Document Mapper) out of the box for FaunaDB that abstracts out complex FQL expressions into pythonic, fully typed asynchronous methods for all CRUD operations.
+
+✅ Performant and scalable: Built on top of Aiohttp a powerful http server and client and FaunaDB an scalable serverless database for modern applications.
+
+✅ Async/await coroutines: Leverage the power of async programming for enhanced performance and responsiveness, being ASGI compliant is compatible with most async python frameworks.
+
+✅ Automatic Swagger UI generation: Automatic generation of interactive Swagger UI documentation for instant testing of your API.
+
+✅ SSE (Server Sent Events): Built-in support for SSE (Server Sent Events) for real-time streaming of data from FaunaDB to your application.
+
+✅ Robust data validation: Built-in support for Pydantic models for robust data validation and serialization.
+
+✅ Auto-provisioning: Automatic management of indexes, unique indexes, and collections with FaunaModel ODM.
+
+✅ Full JSON communication: Custom encoder to ensure seamless data exchange between your application and FaunaDB backend.
+
+✅ Markdown and Jinja support with live reload: experiment an smooth frontend devserver experience without leaving your backend code.
+
+✅ Inspired by fastapi, you will work with almost the same syntax and features like path operations, path parameters, query parameters, request body, status codes and more.
+
+💡 With aiofauna, you can build fast, scalable, and reliable modern applications, while building seamless integrations thanks to the fastest http client aiohttp and the most versatile database FaunaDB, you will enjoy integrating with third party services such as APIs, Data Sources and Cloud Services.
+
+📚 Check out the aiofauna library, and start building your next-gen applications today! 🚀
+
+#Python #FaunaDB #Async #Pydantic #aiofauna
+
+⚙️ If you are using a synchronous framework check out [Faudantic](https://github.com/obahamonde/faudantic) for a similar experience with FaunaDB and Pydantic.
+
+📚 [Documentation](https://obahamonde-aiofauna-docs.smartpro.solutions) (Built with aiofauna)
+
+📦 [PyPi](https://pypi.org/project/aiofauna/)
+
+📦 [GitHub](https://github.com/obahamonde/aiofauna)
+
+📦 [Demo](https://aiofaunastreams-fwuw7gz7oq-uc.a.run.app/) (Real time Latency Monitoring between FaunaDB and Google Cloud Run)
+
+"""
+
+__version__ = (0, 1, 5)
+__author__ = "obahamonde"
+__license__ = "MIT"
+
+import json
+from datetime import datetime
+from typing import Any, AsyncGenerator, Callable, Dict, List, Optional, Union
+from uuid import UUID, uuid4
+
+import asyncio
+import aiohttp_cors
+from pydantic import (
+    BaseModel,
+    BaseConfig,
+    BaseSettings,
+    Field,
+)  # pylint: disable=no-name-in-module
+from aiohttp.web import json_response as jsonify, Request, Response
+from aiohttp_sse import sse_response
+from .client import ClientSession, AsyncFaunaClient as FaunaClient
+from .errors import AioFaunaException as FaunaException
+from . import query as q
+from .json import (
+    FaunaJSONEncoder as JSONEncoder,
+    to_json as dumps,
+    parse_json_or_none as loads,
+)
+from .odm import AsyncFaunaModel as FaunaModel
+from .api import Api
+from .helpers import render_template, make_response, markdown_it, redirect
```

### Comparing `aiofauna-0.1.2/aiofauna/api.py` & `aiofauna-0.1.5/aiofauna/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,18 @@
 """REST API Module with automatic OpenAPI generation."""
 import json
 import base64
 import asyncio
-from typing import (
-    Any,
-    Dict,
-)
+from typing import Any, Dict, List, Union
 from inspect import signature
 from uuid import UUID
 from datetime import datetime, date, time
 from functools import singledispatch
 from enum import Enum
-from aiohttp.web import (
-    Application,
-    Request,
-    Response,
-    json_response,
-    AppRunner,
-    TCPSite,
-)
+from aiohttp.web import Application, Request, Response, json_response
 from json import JSONDecoder
 from aiohttp.web_request import FileField
 from .odm import AsyncFaunaModel
 from pydantic import BaseModel  # pylint: disable=no-name-in-module
 from .json import FaunaJSONEncoder as JSONEncoder, to_json, parse_json_or_none
 
 
@@ -217,115 +207,125 @@
             open_api["paths"].setdefault(path, {})[method.lower()] = {
                 "summary": func.__name__,
                 "description": func.__doc__,
                 "parameters": _scalars,
                 "requestBody": _body,
                 "responses": {"200": {"description": "OK"}},
             }
-            open_api["components"]["schemas"].update(param["schema"])
+            open_api["components"]["schemas"].update(param["schema"])  # type: ignore
 
         else:
             open_api["paths"].setdefault(path, {})[method.lower()] = {
                 "summary": func.__name__,
                 "description": func.__doc__,
                 "parameters": _scalars,
                 "responses": {"200": {"description": "OK"}},
             }
 
 
 @singledispatch
-def make_response(response: Any) -> Response:
+def do_response(response: Any) -> Response:
     """
-    FastAPIesque function to make a response from a function.
+    Flask-esque function to make a response from a function.
     """
     return response
 
 
-@make_response.register(BaseModel)
+@do_response.register(BaseModel)
 def _(response: BaseModel) -> Response:
     return Response(
         status=200,
         body=json.dumps(response.dict()),
         content_type="application/json",
     )
 
 
-@make_response.register(AsyncFaunaModel)
+@do_response.register(AsyncFaunaModel)
 def _(response: AsyncFaunaModel) -> Response:
     response.ref = str(response.ref)
     return Response(
         status=200,
         body=json.dumps(response.dict()),
         content_type="application/json",
     )
 
 
-@make_response.register(list)
-def _(response: list) -> Response:
-    return Response(
-        status=200,
-        body=json.dumps(list(response)),
-        content_type="application/json",
-    )
-
-
-@make_response.register(dict)
+@do_response.register(dict)
 def _(response: dict) -> Response:
     return Response(
         status=200,
         body=json.dumps(response),
         content_type="application/json",
     )
 
 
-@make_response.register(str)
+@do_response.register(str)
 def _(response: str) -> Response:
     return Response(
         status=200,
         body=response.encode(),
         content_type="text/plain",
     )
 
 
-@make_response.register(bytes)
+@do_response.register(bytes)
 def _(response: bytes) -> Response:
     return Response(
         status=200,
         body=response,
         content_type="application/octet-stream",
     )
 
 
-@make_response.register(int)
+@do_response.register(int)
 def _(response: int) -> Response:
     return Response(
         status=200,
         body=str(response).encode(),
         content_type="text/plain",
     )
 
 
-@make_response.register(float)
+@do_response.register(float)
 def _(response: float) -> Response:
     return Response(
         status=200,
         body=str(response).encode(),
         content_type="text/plain",
     )
 
 
-@make_response.register(bool)
+@do_response.register(bool)
 def _(response: bool) -> Response:
     return Response(
         status=200,
         body=str(response).encode(),
         content_type="text/plain",
     )
 
 
+@do_response.register(list)
+def _(
+    response: List[Union[AsyncFaunaModel, BaseModel, dict, str, int, float]]
+) -> Response:
+    processed_response = []
+
+    for item in response:
+        if isinstance(item, (BaseModel, AsyncFaunaModel)):
+            processed_response.append(item.dict())
+        else:
+            processed_response.append(item)
+
+    return Response(
+        status=200,
+        body=json.dumps(processed_response),
+        content_type="application/json",
+    )
+
+
 async def inject_signature(request: Request, params: dict):
     """
     FastAPIesque function to shape the signature of a function to the request.
     """
     args_to_apply = {}
 
     for name, param in params.items():
@@ -459,15 +459,15 @@
                         raise ValueError(
                             f"Missing parameter {name} for {func.__name__}"
                         )
                 if asyncio.iscoroutinefunction(func):
                     response = await func(*args, **kwargs, **definitive_args)
                 else:
                     response = func(*args, **kwargs, **definitive_args)
-                return make_response(response)
+                return do_response(response)
 
             wrapper._handler = func
             return wrapper
 
         return decorator
 
     def get(self, path: str, **kwargs):
@@ -517,42 +517,14 @@
             self.router.add_options(
                 path, self.document(path, "OPTIONS")(func), **kwargs
             )
             return func
 
         return decorator
 
-    def static(self, path: str, directory: str, **kwargs):
-        def decorator(func):
-            self.router.add_static(path, directory, **kwargs)
-            return func
-
-        return decorator
-
-    async def listen(self, host: str = "0.0.0.0", port: int = 8000, **kwargs):
-        for route in list(self.router.routes()):
-            handler = route.handler._handler  # pylint: disable=protected-access
-            path = route.resource.canonical  # type: ignore
-            method = route.method.lower()
-            open_api_params = self._route_open_api_params.get((path, method), {})
-            update_open_api(self.openapi, path, method, handler, open_api_params)
-
-        runner = AppRunner(self)
-
-        await runner.setup()
-
-        site = TCPSite(runner, host, port)
-
-        await site.start()
-
-        print(f"http://{host}:{port}/docs")
-
-        while True:
-            await asyncio.sleep(3600)
-
     def on_event(self, event: str):
         def decorator(func):
             if event not in ["startup", "shutdown"]:
                 raise ValueError("Event must be startup or shutdown")
             elif event == "startup":
                 self.on_startup.append(func)
             else:
```

### Comparing `aiofauna-0.1.2/aiofauna/errors.py` & `aiofauna-0.1.5/aiofauna/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Error types that methods in the FaunaDB client throw."""
 
 # pylint: disable=redefined-builtin
 
 from builtins import object
 
+from typing import Union
+
 from pydantic import ValidationError
 
 from aiohttp.web_exceptions import HTTPException
 
 
 class codes:
 
@@ -337,12 +339,7 @@
     ProcessLookupError,
     TimeoutError,
     BlockingIOError,
     ChildProcessError,
     ConnectionError,
     BrokenPipeError,
 )
-
-
-"""
-(c) 2016 Fauna, Inc.
-"""
```

### Comparing `aiofauna-0.1.2/aiofauna/json.py` & `aiofauna-0.1.5/aiofauna/json.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import asyncio
 from base64 import urlsafe_b64decode, urlsafe_b64encode
 from datetime import date, datetime
 from json import JSONEncoder, dumps, loads
+from typing import overload
 from typing_extensions import override
 from iso8601 import parse_date
 from pydantic import BaseModel  # pylint: disable=no-name-in-module
-from .objects import FaunaTime, Native, Query, Ref, SetRef
-from .query import Expr
-from aiohttp.web import Request
+from aiofauna.objects import FaunaTime, Native, Query, Ref, SetRef
+from aiofauna.query import Expr
+from aiohttp.web import Request, Response
 
 
 def parse_json(json_string):
     """
 
     Parses a JSON string into python values.
```

### Comparing `aiofauna-0.1.2/aiofauna/objects.py` & `aiofauna-0.1.5/aiofauna/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Types used in queries and responses.
 See the `docs <https://app.fauna.com/documentation/reference/queryapi#simple-type>`__.
 """
 from datetime import datetime
 from iso8601 import parse_date
-from .deprecated import deprecated
-from .query import Expr
+from aiofauna.deprecated import deprecated
+from aiofauna.query import Expr
 
 
 class Ref(Expr):
     """
     ```python
     Ref(id, cls=None, db=None)
     ```
@@ -204,12 +204,7 @@
 
     def __eq__(self, other):
         return isinstance(other, Query) and self.value == other.value
 
     def __ne__(self, other):
         # pylint: disable=unneeded-not
         return not self == other
-
-
-"""
-(c) 2016 Fauna, Inc.
-"""
```

### Comparing `aiofauna-0.1.2/aiofauna/odm.py` & `aiofauna-0.1.5/aiofauna/odm.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import asyncio
 
 
 from typing import List, Optional, Any, Callable, Union
 
 try:
-    import query as q # type: ignore
+    import query as q  # type: ignore
 except ImportError:
     from . import query as q
 
 from .errors import AioFaunaException
 
 
 from .json import JSONModel  # pylint: disable=no-name-in-module
@@ -55,45 +55,39 @@
     """
 
     ref: Optional[str] = None
 
     ts: Optional[str] = None
 
     def __init__(self, **data: Any) -> None:
-
         super().__init__(**data)
 
         for field in self.__fields__.values():
             try:
                 one_of = field.field_info.extra.get("oneOf")
 
                 if isinstance(one_of, list):
                     if data.get(field.name) not in one_of:
                         raise ValueError(f"{field.name} must be one of {one_of}")
 
             except Exception:  # pylint: disable=broad-except
                 continue
 
-
-
     @classmethod
     def client(cls) -> AsyncFaunaClient:
-        
         fauna_secret = os.getenv("FAUNA_SECRET")
-              
+
         return AsyncFaunaClient(secret=fauna_secret)
 
     @classmethod
     def q(cls) -> Callable:
-        
         return cls.client().query
 
     @classmethod
     async def provision(cls) -> bool:
-        
         _q = cls.q()
         try:
             if not await _q(q.exists(q.collection(cls.__name__.lower()))):
                 await _q(q.create_collection({"name": cls.__name__.lower()}))
 
                 print("Created collection %s", cls.__name__.lower())
 
@@ -148,17 +142,15 @@
                                     "name": f"{cls.__name__.lower()}_{field.name}",
                                     "source": q.collection(cls.__name__.lower()),
                                     "terms": [{"field": ["data", field.name]}],
                                 }
                             )
                         )
 
-                        print(
-                            "Created index %s_%s", cls.__name__.lower(), field.name
-                        )
+                        print("Created index %s_%s", cls.__name__.lower(), field.name)
                         continue
 
             return True
 
         except AioFaunaException as exc:
             logging.error(exc)
 
@@ -363,15 +355,15 @@
 
         except AioFaunaException as exc:
             logging.error(exc)
 
             raise ValueError(f"{ref} not found")
 
     @classmethod
-    async def find_all(cls, limit: int, offset: int) -> List[AsyncFaunaModel]:
+    async def all(cls) -> List[AsyncFaunaModel]:
         """
 
 
         Finds all documents of the model in FaunaDB.
 
 
 
@@ -507,27 +499,33 @@
 
             An instance of the model if created successfully, None otherwise.
         """
 
         try:
             for field in self.__fields__.values():
                 if field.field_info.extra.get("unique"):
-                    instance = await self.find_unique(field.name, getattr(self, field.name))
+                    instance = await self.find_unique(
+                        field.name, getattr(self, field.name)
+                    )
                     if instance is None:
                         continue
-                    else:
-                        await instance.__class__.q()(q.create(q.collection(self.__class__.__name__.lower()), {"data": self.dict()})) # type: ignore
-                        return instance # type: ignore
-            self.__class__.q()(q.create(q.collection(self.__class__.__name__.lower()), {"data": self.dict()}))
+                    await instance.__class__.q()(q.create(q.collection(self.__class__.__name__.lower()), {"data": self.dict()}))  # type: ignore
+                    return instance  # type: ignore
+            data = await self.__class__.q()(
+                q.create(
+                    q.collection(self.__class__.__name__.lower()), {"data": self.dict()}
+                )
+            )
+            self.ref = data["ref"]["@ref"]["id"]
+            self.ts = data["ts"] / 1000
             return self
-        
+
         except AioFaunaException as exc:
-            
             logging.error(exc)
-            
+
             raise ValueError(exc)
 
     @classmethod
     async def query(cls, query: str) -> List[AsyncFaunaModel]:
         """
 
 
@@ -605,8 +603,7 @@
 
             An instance of the model if saved successfully, None otherwise.
         """
 
         if isinstance(self.ref, str) and len(self.ref) == 18:
             return await self.update(self.ref, kwargs=self.dict())
         return await self.create()
-
```

### Comparing `aiofauna-0.1.2/aiofauna/page.py` & `aiofauna-0.1.5/aiofauna/page.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-try:
-    import query as q
-except ImportError:
-    from . import query as q
+from aiofauna import query
 
 
 class Page(object):
     """
     Represents a single pagination result.
     See ``paginate`` in the `docs <https://app.fauna.com/documentation/reference/queryapi#read-functions>`__.
     You must convert to Page yourself using :py:meth:`from_raw`.
@@ -72,12 +69,7 @@
 
         while getattr(page, next_cursor) is not None:
             page = get_page(
                 **{"size": page_size, next_cursor: getattr(page, next_cursor)}
             )
             for val in page.data:
                 yield val if mapper is None else mapper(val)
-
-
-"""
-(c) 2016 Fauna, Inc.
-"""
```

### Comparing `aiofauna-0.1.2/aiofauna/query.py` & `aiofauna-0.1.5/aiofauna/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 For example: ``select("a", {"a": Ref("123", Ref("widgets", Native.CLASSES))})``.
 """
 
 # pylint: disable=invalid-name, redefined-builtin
 
 from types import FunctionType
-from . import deprecated
+from aiofauna import deprecated
 
 # region Basic forms
 
 
 def abort(msg):
     """See the `docs <https://docs.fauna.com/fauna/current/api/fql/functions/abort>`__."""
     return _fn({"abort": msg})
@@ -1284,11 +1284,7 @@
     This ensures that a single value passed is not put in an array, so
     ``query.add([1, 2])`` will work as well as ``query.add(1, 2)``.
     """
     return values[0] if len(values) == 1 else values
 
 
 # endregion
-
-"""
-(c) 2016 Fauna, Inc.
-"""
```

