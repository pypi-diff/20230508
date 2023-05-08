# Comparing `tmp/python_fast_grpc-0.1.0.tar.gz` & `tmp/python_fast_grpc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_fast_grpc-0.1.0.tar", max compression
+gzip compressed data, was "python_fast_grpc-0.1.1.tar", max compression
```

## Comparing `python_fast_grpc-0.1.0.tar` & `python_fast_grpc-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-05-07 10:06:20.785302 python_fast_grpc-0.1.0/LICENSE
--rw-r--r--   0        0        0      939 2023-05-07 14:19:57.365038 python_fast_grpc-0.1.0/README.md
--rw-r--r--   0        0        0      127 2023-05-07 10:04:32.688620 python_fast_grpc-0.1.0/fast_grpc/__init__.py
--rw-r--r--   0        0        0     3625 2023-05-07 10:52:12.919455 python_fast_grpc-0.1.0/fast_grpc/app.py
--rw-r--r--   0        0        0      242 2023-05-07 08:52:13.078197 python_fast_grpc-0.1.0/fast_grpc/base.py
--rw-r--r--   0        0        0      981 2023-05-07 08:52:17.786157 python_fast_grpc-0.1.0/fast_grpc/exceptions.py
--rw-r--r--   0        0        0      570 2023-05-07 08:53:00.804651 python_fast_grpc-0.1.0/fast_grpc/middleware/__init__.py
--rw-r--r--   0        0        0     1657 2023-05-07 10:04:32.670718 python_fast_grpc-0.1.0/fast_grpc/middleware/base.py
--rw-r--r--   0        0        0       24 2023-05-07 08:53:11.397718 python_fast_grpc-0.1.0/fast_grpc/middleware/exception.py
--rw-r--r--   0        0        0     6739 2023-05-07 10:04:32.682092 python_fast_grpc-0.1.0/fast_grpc/proto.py
--rw-r--r--   0        0        0     4751 2023-05-07 10:04:32.640862 python_fast_grpc-0.1.0/fast_grpc/service.py
--rw-r--r--   0        0        0      139 2023-04-22 16:02:22.806235 python_fast_grpc-0.1.0/fast_grpc/signals.py
--rw-r--r--   0        0        0     3315 2023-05-07 10:04:32.698387 python_fast_grpc-0.1.0/fast_grpc/types.py
--rw-r--r--   0        0        0     2146 2023-05-07 10:53:17.310012 python_fast_grpc-0.1.0/fast_grpc/utils.py
--rw-r--r--   0        0        0     1340 2023-05-07 14:16:00.326875 python_fast_grpc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1653 1970-01-01 00:00:00.000000 python_fast_grpc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-07 10:06:20.785302 python_fast_grpc-0.1.1/LICENSE
+-rw-r--r--   0        0        0      939 2023-05-08 16:51:46.015329 python_fast_grpc-0.1.1/README.md
+-rw-r--r--   0        0        0     6148 2023-05-08 16:48:47.382250 python_fast_grpc-0.1.1/fast_grpc/.DS_Store
+-rw-r--r--   0        0        0      127 2023-05-07 10:04:32.688620 python_fast_grpc-0.1.1/fast_grpc/__init__.py
+-rw-r--r--   0        0        0     3639 2023-05-08 16:11:07.098108 python_fast_grpc-0.1.1/fast_grpc/app.py
+-rw-r--r--   0        0        0      242 2023-05-07 08:52:13.078197 python_fast_grpc-0.1.1/fast_grpc/base.py
+-rw-r--r--   0        0        0      981 2023-05-07 08:52:17.786157 python_fast_grpc-0.1.1/fast_grpc/exceptions.py
+-rw-r--r--   0        0        0      570 2023-05-07 08:53:00.804651 python_fast_grpc-0.1.1/fast_grpc/middleware/__init__.py
+-rw-r--r--   0        0        0     1657 2023-05-07 10:04:32.670718 python_fast_grpc-0.1.1/fast_grpc/middleware/base.py
+-rw-r--r--   0        0        0       24 2023-05-07 08:53:11.397718 python_fast_grpc-0.1.1/fast_grpc/middleware/exception.py
+-rw-r--r--   0        0        0     6817 2023-05-08 16:45:44.765150 python_fast_grpc-0.1.1/fast_grpc/proto.py
+-rw-r--r--   0        0        0     5022 2023-05-08 16:25:53.094255 python_fast_grpc-0.1.1/fast_grpc/service.py
+-rw-r--r--   0        0        0      139 2023-04-22 16:02:22.806235 python_fast_grpc-0.1.1/fast_grpc/signals.py
+-rw-r--r--   0        0        0     3313 2023-05-08 16:08:10.646222 python_fast_grpc-0.1.1/fast_grpc/types.py
+-rw-r--r--   0        0        0     2103 2023-05-08 16:13:38.796925 python_fast_grpc-0.1.1/fast_grpc/utils.py
+-rw-r--r--   0        0        0     1339 2023-05-08 16:48:33.384703 python_fast_grpc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1707 1970-01-01 00:00:00.000000 python_fast_grpc-0.1.1/PKG-INFO
```

### Comparing `python_fast_grpc-0.1.0/LICENSE` & `python_fast_grpc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_fast_grpc-0.1.0/README.md` & `python_fast_grpc-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # fast-grpc
-fast to code grpc in Python 3.9+
+fast to code grpc in Python 3.7+
 
 # Installation
-Require Python 3.9+
+Require Python 3.7+
 ```shell
 pip install python-fast-grpc
 ```
 
 # Quick start
 1. Run a gRPC application
 ```python
```

### Comparing `python_fast_grpc-0.1.0/fast_grpc/app.py` & `python_fast_grpc-0.1.1/fast_grpc/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import asyncio
 import inspect
-from typing import Any, Callable, Optional, Sequence, Type
+from typing import Any, Callable, List, Optional, Sequence, Type
 
 import grpc
-from grpc.aio._typing import ChannelArgumentType
+from grpc.aio._typing import ChannelArgumentType  # noqa
 from logzero import logger
 from pydantic import BaseModel
 
 from fast_grpc.middleware import Middleware
 from fast_grpc.middleware.base import BaseRPCMiddleware
 from fast_grpc.service import Service
 from fast_grpc.types import App
@@ -19,17 +19,17 @@
         self,
         default_service_name: str = "FastGRPC",
         middleware: Optional[Sequence[Middleware]] = None,
     ):
         self.default_service_name = default_service_name
         self.service = Service(service_name=self.default_service_name)
 
-        self.rpc_startup_funcs: list[Callable[..., Any]] = []
-        self.rpc_shutdown_funcs: list[Callable[..., Any]] = []
-        self.user_middleware: list[Middleware] = [] if middleware is None else list(middleware)
+        self.rpc_startup_funcs: List[Callable[..., Any]] = []
+        self.rpc_shutdown_funcs: List[Callable[..., Any]] = []
+        self.user_middleware: List[Middleware] = [] if middleware is None else list(middleware)
         self.middleware_stack: App = self.build_middleware_stack()
 
     def setup(self) -> None:
         # build proto
         self.service.gen_and_compile_proto()
 
     def on_startup(self, func: Callable[..., None]):
```

### Comparing `python_fast_grpc-0.1.0/fast_grpc/exceptions.py` & `python_fast_grpc-0.1.1/fast_grpc/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_fast_grpc-0.1.0/fast_grpc/middleware/__init__.py` & `python_fast_grpc-0.1.1/fast_grpc/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `python_fast_grpc-0.1.0/fast_grpc/middleware/base.py` & `python_fast_grpc-0.1.1/fast_grpc/middleware/base.py`

 * *Files identical despite different names*

### Comparing `python_fast_grpc-0.1.0/fast_grpc/proto.py` & `python_fast_grpc-0.1.1/fast_grpc/proto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 import datetime
 from collections import deque
 from enum import IntEnum
-from typing import List, Type, Union, get_args, get_origin
+from typing import List, Set, Type, Union
 
 from grpc_tools import protoc
 from pydantic import BaseModel
+from typing_extensions import get_args, get_origin
 
 from fast_grpc.types import (
     BoolValue,
     BytesValue,
     Double,
     DoubleValue,
     FloatValue,
@@ -86,17 +87,17 @@
 
 class ProtoBuilder:
     def __init__(self, service):
         from fast_grpc.service import Service
 
         self.service: Service = service
         self.queue: deque[Union[Type[BaseModel], Type[IntEnum]]] = deque()
-        self.messages: set[Union[Type[BaseModel], Type[IntEnum]]] = set()
+        self.messages: Set[Union[Type[BaseModel], Type[IntEnum]]] = set()
 
-        self.import_packages: set[str] = set()
+        self.import_packages: Set[str] = set()
 
     def create(self):
         rpc_methods = []
         message_contents = []
         for method in self.service.methods:
             rpc_methods.append(
                 rpc_template.format(
@@ -136,15 +137,16 @@
         index = 0
         for name, field in schema.__fields__.items():
             index += 1
             if field.annotation in _wrapper_types:
                 self.import_packages.add("""import "google/protobuf/wrappers.proto";""")
                 type_name = _wrapper_types[field.annotation]
                 fields.append(field_template.format(type=type_name, name=name, index=index))
-            elif origin := get_origin(field.annotation):
+            elif get_origin(field.annotation):
+                origin = get_origin(field.annotation)
                 if origin not in {list, List}:
                     raise NotImplementedError(f"Unsupported type {field.annotation}")
                 type_arg = get_args(field.annotation)[0]
                 if type_arg in _wrapper_types:
                     self.import_packages.add("""import "google/protobuf/wrappers.proto";""")
                     type_name = _wrapper_types[type_arg]
                     fields.append(field_template.format(type=f"repeated {type_name}", name=name, index=index))
```

### Comparing `python_fast_grpc-0.1.0/fast_grpc/service.py` & `python_fast_grpc-0.1.1/fast_grpc/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 import inspect
 import os
 from concurrent.futures import ThreadPoolExecutor
-from functools import cached_property
 from importlib import import_module
-from typing import Any, Callable, Optional
+from typing import Any, Callable, List, Optional
 
 from google.protobuf.json_format import MessageToDict, Parse, ParseDict
 
 from fast_grpc.proto import ProtoBuilder, protoc_compile
 from fast_grpc.types import Message, ServicerContext
 from fast_grpc.utils import (
     await_sync_function,
@@ -38,15 +37,15 @@
 
         return new_class
 
 
 class Service:
     def __init__(self, service_name: str, package_name: str = "", proto_path="."):
         self.service_name = service_name
-        self.methods: list[Method] = []
+        self.methods: List[Method] = []
         self.proto_path = proto_path
         self.thread_pool: Optional[ThreadPoolExecutor] = None
 
         if is_camel_case(self.service_name):
             self.proto_name = camel_to_snake(self.service_name).lower()
         elif is_snake_case(self.service_name):
             self.proto_name = self.service_name.lower()
@@ -54,27 +53,37 @@
             self.proto_name = self.service_name.lower()
 
         if package_name:
             self.package_name = package_name
         else:
             self.package_name = self.proto_name
 
-    @cached_property
+        self._proto_file = None
+        self._pb2 = None
+        self._pb2_grpc = None
+
+    @property
     def proto_file(self):
-        if not os.path.exists(self.proto_path):
-            os.makedirs(self.proto_path)
-        return os.path.join(self.proto_path, f"{self.proto_name}.proto")
+        if self._proto_file is None:
+            if not os.path.exists(self.proto_path):
+                os.makedirs(self.proto_path)
+            self._proto_file = os.path.join(self.proto_path, f"{self.proto_name}.proto")
+        return self._proto_file
 
-    @cached_property
+    @property
     def pb2(self):
-        return import_module(f"{self.package_name}_pb2")
+        if self._pb2 is None:
+            self._pb2 = import_module(f"{self.package_name}_pb2")
+        return self._pb2
 
-    @cached_property
+    @property
     def pb2_grpc(self):
-        return import_module(f"{self.package_name}_pb2_grpc")
+        if self._pb2_grpc is None:
+            self._pb2_grpc = import_module(f"{self.package_name}_pb2_grpc")
+        return self._pb2_grpc
 
     def gen_and_compile_proto(self):
         builder = ProtoBuilder(self)
         proto = builder.create()
         with open(self.proto_file, "w") as f:
             f.write(proto)
         protoc_compile(self.proto_file)
```

### Comparing `python_fast_grpc-0.1.0/fast_grpc/types.py` & `python_fast_grpc-0.1.1/fast_grpc/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 from enum import IntEnum as _IntEnum
-from typing import TYPE_CHECKING, Awaitable, Callable, Generic, Optional, TypeVar, Union
+from typing import TYPE_CHECKING, Awaitable, Callable, Generic, Optional, TypeVar
 
 from google.protobuf.message import Message
 from grpc.aio import ServicerContext
 from logzero import logger
 from pydantic import ConstrainedInt
 from pydantic.generics import GenericModel
 
@@ -109,12 +109,12 @@
 
     @classmethod
     def __modify_schema__(cls, field_schema):
         field_schema["description"] = "<br>".join([e.swagger_description for e in cls])
 
     @classmethod
     def _missing_(cls, value):
-        logger.info(f"{cls.__qualname__} missing {value=}")
+        logger.info(f"{cls.__qualname__} missing value={value}")
         unknown = cls._value2member_map_.get(0)
         if not isinstance(value, int) and unknown is None:
             raise ValueError("%r is not a valid %s" % (value, cls.__qualname__))
         return unknown
```

### Comparing `python_fast_grpc-0.1.0/fast_grpc/utils.py` & `python_fast_grpc-0.1.1/fast_grpc/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # -*- coding: utf-8 -*-
 import asyncio
 import contextvars
 import functools
-import inspect
 import os
 import re
 import sys
 from importlib import import_module
-from typing import Callable
 
 
 def import_string(dotted_path):
     try:
         module_path, class_name = dotted_path.rsplit(".", 1)
     except ValueError as err:
         raise ImportError("%s doesn't look like a module path" % dotted_path) from err
```

### Comparing `python_fast_grpc-0.1.0/pyproject.toml` & `python_fast_grpc-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 [tool.poetry]
 name = "python-fast-grpc"
-version = "0.1.0"
+version = "0.1.1"
 description = "fast to code grpc in python"
 authors = ["taogeYT <li_yatao@outlook.com>"]
 readme = "README.md"
 packages = [{include = "fast_grpc"}]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.7"
+protobuf = "^4.22.0"
 grpcio = "^1.53.0"
-pydantic = "^1.10.7"
-protobuf = "^4.22.3"
-mypy-protobuf = "^3.4.0"
-grpcio-tools = "^1.54.0"
+grpcio-tools = "^1.53.0"
+pydantic = "^1.10.0"
 logzero = "^1.7.0"
-blinker = "^1.6.2"
+blinker = "^1.6.1"
 
 [tool.poetry.dev-dependencies]
-isort = "^5.10.1"
+isort = "^5.10.0"
 black = "^22.3.0"
 flake8 = "^4.0"
 mypy = "^0.931"
+mypy-protobuf = "^3.4.0"
 pytest = "^7.1.2"
 pytest-asyncio = "^0.18.3"
+ipython = "^6.5.0"
 types-toml = "^0.10.8"
 types-requests = "^2.28.11"
-ipython = "^8.12.0"
 types-protobuf = "3.20.4.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
-python_version = "3.9"
+python_version = "3.7"
 plugins = ["pydantic.mypy"]
 ignore_missing_imports = true
 allow_redefinition = true
 no_implicit_optional = true
 local_partial_types = true
 strict_equality = true
 warn_redundant_casts = true
 warn_unused_configs = true
 warn_unused_ignores = true
 warn_unreachable = true
 
 [tool.black]
-target-version = [ "py39" ]
+target-version = [ "py37" ]
 line-length = 120
 skip-numeric-underscore-normalization = true
 exclude = 'dist|build|\.venv|\.git|\.mypy_cache'
 
 [tool.isort]
 profile = "black"
```

### Comparing `python_fast_grpc-0.1.0/PKG-INFO` & `python_fast_grpc-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: python-fast-grpc
-Version: 0.1.0
+Version: 0.1.1
 Summary: fast to code grpc in python
 Author: taogeYT
 Author-email: li_yatao@outlook.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: blinker (>=1.6.2,<2.0.0)
+Requires-Dist: blinker (>=1.6.1,<2.0.0)
 Requires-Dist: grpcio (>=1.53.0,<2.0.0)
-Requires-Dist: grpcio-tools (>=1.54.0,<2.0.0)
+Requires-Dist: grpcio-tools (>=1.53.0,<2.0.0)
 Requires-Dist: logzero (>=1.7.0,<2.0.0)
-Requires-Dist: mypy-protobuf (>=3.4.0,<4.0.0)
-Requires-Dist: protobuf (>=4.22.3,<5.0.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: protobuf (>=4.22.0,<5.0.0)
+Requires-Dist: pydantic (>=1.10.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # fast-grpc
-fast to code grpc in Python 3.9+
+fast to code grpc in Python 3.7+
 
 # Installation
-Require Python 3.9+
+Require Python 3.7+
 ```shell
 pip install python-fast-grpc
 ```
 
 # Quick start
 1. Run a gRPC application
 ```python
```

