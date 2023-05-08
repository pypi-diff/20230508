# Comparing `tmp/quart-schema-0.8.0.tar.gz` & `tmp/quart-schema-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quart-schema-0.8.0.tar", last modified: Tue May 11 21:15:50 2021, max compression
+gzip compressed data, was "quart-schema-0.9.0.tar", last modified: Wed Jul 21 20:21:45 2021, max compression
```

## Comparing `quart-schema-0.8.0.tar` & `quart-schema-0.9.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1050 2020-12-08 17:38:25.231388 quart-schema-0.8.0/LICENSE
--rw-r--r--   0        0        0     3400 2020-12-13 15:08:48.789883 quart-schema-0.8.0/README.rst
--rw-r--r--   0        0        0     1612 2021-05-11 21:15:29.662659 quart-schema-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      538 2021-02-28 13:45:44.992703 quart-schema-0.8.0/src/quart_schema/__init__.py
--rw-r--r--   0        0        0    12332 2021-05-11 21:15:29.662659 quart-schema-0.8.0/src/quart_schema/extension.py
--rw-r--r--   0        0        0     3233 2021-05-11 21:15:29.662659 quart-schema-0.8.0/src/quart_schema/mixins.py
--rw-r--r--   0        0        0        7 2020-12-08 17:38:25.231388 quart-schema-0.8.0/src/quart_schema/py.typed
--rw-r--r--   0        0        0     1714 2021-05-11 21:15:29.662659 quart-schema-0.8.0/src/quart_schema/typing.py
--rw-r--r--   0        0        0     6432 2021-05-11 21:15:29.662659 quart-schema-0.8.0/src/quart_schema/validation.py
--rw-r--r--   0        0        0     4382 2021-05-11 21:15:50.255917 quart-schema-0.8.0/setup.py
--rw-r--r--   0        0        0     4526 2021-05-11 21:15:50.256391 quart-schema-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1050 2020-12-08 17:38:25.231388 quart-schema-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3396 2021-07-21 20:20:48.721843 quart-schema-0.9.0/README.rst
+-rw-r--r--   0        0        0     1623 2021-07-21 20:20:48.721843 quart-schema-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      605 2021-07-21 20:20:48.721843 quart-schema-0.9.0/src/quart_schema/__init__.py
+-rw-r--r--   0        0        0    12332 2021-05-11 21:15:29.662659 quart-schema-0.9.0/src/quart_schema/extension.py
+-rw-r--r--   0        0        0     3233 2021-05-11 21:15:29.662659 quart-schema-0.9.0/src/quart_schema/mixins.py
+-rw-r--r--   0        0        0        7 2020-12-08 17:38:25.231388 quart-schema-0.9.0/src/quart_schema/py.typed
+-rw-r--r--   0        0        0     2227 2021-07-21 20:20:48.721843 quart-schema-0.9.0/src/quart_schema/typing.py
+-rw-r--r--   0        0        0     6995 2021-07-21 20:20:48.721843 quart-schema-0.9.0/src/quart_schema/validation.py
+-rw-r--r--   0        0        0     4378 2021-07-21 20:21:45.677743 quart-schema-0.9.0/setup.py
+-rw-r--r--   0        0        0     4522 2021-07-21 20:21:45.678376 quart-schema-0.9.0/PKG-INFO
```

### Comparing `quart-schema-0.8.0/LICENSE` & `quart-schema-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quart-schema-0.8.0/README.rst` & `quart-schema-0.9.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 Quickstart
 ----------
 
 Quart-Schema can validate an existing Quart route by decorating it
 with ``validate_querystring``, ``validate_request``, or
 ``validate_response``. It can also validate the JSON data sent and
 received over websockets using the ``send_as`` and ``receive_as``
-methods,
+methods.
 
 .. code-block:: python
 
+    from dataclasses import dataclass
     from datetime import datetime
     from typing import Optional
 
-    from pydantic.dataclasses import dataclass
-    from quart import Quart
+    from quart import Quart, websocket
     from quart_schema import QuartSchema, validate_request, validate_response
 
     app = Quart(__name__)
     QuartSchema(app)
 
     @dataclass
     class Todo:
@@ -44,15 +44,15 @@
     async def ws() -> None:
         while True:
             data = await websocket.receive_as(Todo)
             ... # Do something with data, e.g. save to the DB
             await websocket.send_as(data, Todo)
 
 The documentation is served by default at ``/openapi.json`` according
-tot eh OpenAPI standard, or at ``/docs`` for a `SwaggerUI
+to the OpenAPI standard, or at ``/docs`` for a `SwaggerUI
 <https://swagger.io/tools/swagger-ui/>`_ interface, or ``/redocs`` for
 a `redoc <https://github.com/Redocly/redoc>`_ interface. Note that
 there is currently no documentation standard for WebSockets.
 
 Contributing
 ------------
 
@@ -85,21 +85,21 @@
 start, after that try searching `stack overflow
 <https://stackoverflow.com/questions/tagged/quart>`_ or ask for help
 `on gitter <https://gitter.im/python-quart/lobby>`_. If you still
 can't find an answer please `open an issue
 <https://gitlab.com/pgjones/quart-schema/issues>`_.
 
 
-.. |Build Status| image:: https://gitlab.com/pgjones/quart-schema/badges/master/pipeline.svg
-   :target: https://gitlab.com/pgjones/quart-schema/commits/master
+.. |Build Status| image:: https://gitlab.com/pgjones/quart-schema/badges/main/pipeline.svg
+   :target: https://gitlab.com/pgjones/quart-schema/commits/main
 
 .. |docs| image:: https://img.shields.io/badge/docs-passing-brightgreen.svg
    :target: https://pgjones.gitlab.io/quart-schema/
 
 .. |pypi| image:: https://img.shields.io/pypi/v/quart-schema.svg
    :target: https://pypi.python.org/pypi/Quart-Schema/
 
 .. |python| image:: https://img.shields.io/pypi/pyversions/quart-schema.svg
    :target: https://pypi.python.org/pypi/Quart-Schema/
 
 .. |license| image:: https://img.shields.io/badge/license-MIT-blue.svg
-   :target: https://gitlab.com/pgjones/quart-schema/blob/master/LICENSE
+   :target: https://gitlab.com/pgjones/quart-schema/blob/main/LICENSE
```

### Comparing `quart-schema-0.8.0/pyproject.toml` & `quart-schema-0.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quart-schema"
-version = "0.8.0"
+version = "0.9.0"
 description = "A Quart extension to provide schema validation"
 authors = ["pgjones <philip.graham.jones@googlemail.com>"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -49,9 +49,9 @@
 tox = "*"
 
 [tool.pytest.ini_options]
 addopts = "--no-cov-on-fail --showlocals --strict"
 testpaths = ["tests"]
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry_core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `quart-schema-0.8.0/src/quart_schema/extension.py` & `quart-schema-0.9.0/src/quart_schema/extension.py`

 * *Files identical despite different names*

### Comparing `quart-schema-0.8.0/src/quart_schema/mixins.py` & `quart-schema-0.9.0/src/quart_schema/mixins.py`

 * *Files identical despite different names*

### Comparing `quart-schema-0.8.0/src/quart_schema/typing.py` & `quart-schema-0.9.0/src/quart_schema/typing.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,41 @@
 from __future__ import annotations
 
-from typing import Any, AnyStr, Dict, List, Optional, Type, TypeVar, Union
+from typing import Any, AnyStr, Dict, List, Optional, Tuple, Type, TypeVar, Union
 
 from pydantic import BaseModel
 from quart.datastructures import FileStorage
+from quart.typing import (
+    HeadersValue,
+    ResponseReturnValue as QuartResponseReturnValue,
+    ResponseValue as QuartResponseValue,
+    StatusCode,
+)
 from quart.wrappers import Response
 from werkzeug.datastructures import Headers
 
 try:
     from typing import Protocol, TypedDict
 except ImportError:
     from typing_extensions import Protocol, TypedDict  # type: ignore
 
 
+PydanticModel = Union[Type[BaseModel], Type]  # Type[Dataclass] does not work
+
+ResponseValue = Union[QuartResponseValue, PydanticModel]
+
+ResponseReturnValue = Union[
+    QuartResponseReturnValue,
+    ResponseValue,
+    Tuple[ResponseValue, HeadersValue],
+    Tuple[ResponseValue, StatusCode],
+    Tuple[ResponseValue, StatusCode, HeadersValue],
+]
+
+
 class Dataclass(Protocol):
     __pydantic_model__: Type[BaseModel]
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         ...
```

### Comparing `quart-schema-0.8.0/src/quart_schema/validation.py` & `quart-schema-0.9.0/src/quart_schema/validation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from __future__ import annotations
 
 from dataclasses import asdict, is_dataclass
 from enum import auto, Enum
 from functools import wraps
-from typing import Any, Callable, cast, Optional, Type, TYPE_CHECKING, Union
+from typing import Any, Callable, cast, Optional, Union
 
 from pydantic import BaseModel, ValidationError
+from pydantic.dataclasses import dataclass as pydantic_dataclass
 from pydantic.schema import model_schema
-from quart import current_app, request
+from quart import current_app, request, ResponseReturnValue as QuartResponseReturnValue
 from werkzeug.datastructures import Headers
 from werkzeug.exceptions import BadRequest
 
-if TYPE_CHECKING:
-    from pydantic.dataclasses import Dataclass
-
+from .typing import PydanticModel, ResponseReturnValue
 
 QUART_SCHEMA_REQUEST_ATTRIBUTE = "_quart_schema_request_schema"
 QUART_SCHEMA_RESPONSE_ATTRIBUTE = "_quart_schema_response_schemas"
 QUART_SCHEMA_QUERYSTRING_ATTRIBUTE = "_quart_schema_querystring_schema"
 
 
 class SchemaInvalidError(Exception):
@@ -36,26 +35,29 @@
 
 
 class DataSource(Enum):
     FORM = auto()
     JSON = auto()
 
 
-def validate_querystring(model_class: Union[Type[BaseModel], Type[Dataclass]]) -> Callable:
+def validate_querystring(model_class: PydanticModel) -> Callable:
     """Validate the querystring arguments.
 
     This ensures that the query string arguments can be converted to
     the *model_class*. If they cannot a `RequestSchemaValidationError`
     is raised which by default results in a 400 response.
 
     Arguments:
-        model_class: The model to use, either a pydantic dataclass or
-            a class that inherits from pydantic's BaseModel. All the
-            fields must be optional.
+        model_class: The model to use, either a dataclass, pydantic
+            dataclass or a class that inherits from pydantic's
+            BaseModel. All the fields must be optional.
     """
+    if is_dataclass(model_class):
+        model_class = pydantic_dataclass(model_class)
+
     schema = model_schema(model_class)
 
     if len(schema.get("required", [])) != 0:
         raise SchemaInvalidError("Fields must be optional")
 
     def decorator(func: Callable) -> Callable:
         setattr(func, QUART_SCHEMA_QUERYSTRING_ATTRIBUTE, model_class)
@@ -71,31 +73,35 @@
 
         return wrapper
 
     return decorator
 
 
 def validate_request(
-    model_class: Union[Type[BaseModel], Type[Dataclass]],
+    model_class: PydanticModel,
     *,
     source: DataSource = DataSource.JSON,
 ) -> Callable:
     """Validate the request data.
 
     This ensures that the request body is JSON and that the body can
     be converted to the *model_class*. If they cannot a
     `RequestSchemaValidationError` is raised which by default results
     in a 400 response.
 
     Arguments:
-        model_class: The model to use, either a pydantic dataclass or
-            a class that inherits from pydantic's BaseModel.
+        model_class: The model to use, either a dataclass, pydantic
+            dataclass or a class that inherits from pydantic's
+            BaseModel. All the fields must be optional.
         source: The source of the data to validate (json or form
             encoded).
     """
+    if is_dataclass(model_class):
+        model_class = pydantic_dataclass(model_class)
+
     schema = model_schema(model_class)
     if source == DataSource.FORM and any(
         schema["properties"][field]["type"] == "object" for field in schema["properties"]
     ):
         raise SchemaInvalidError("Form must not have nested objects")
 
     def decorator(func: Callable) -> Callable:
@@ -116,34 +122,37 @@
                 return await current_app.ensure_async(func)(*args, data=model, **kwargs)
 
         return wrapper
 
     return decorator
 
 
-def validate_response(
-    model_class: Union[Type[BaseModel], Type[Dataclass]], status_code: int = 200
-) -> Callable:
+def validate_response(model_class: PydanticModel, status_code: int = 200) -> Callable:
     """Validate the response data.
 
     This ensures that the response is a either dictionary that the
     body can be converted to the *model_class* or an instance of the
     *model_class*. If this is not possible a
     `ResponseSchemaValidationError` is raised which by default results
     in a 500 response. The returned value is then a dictionary which
     Quart encodes as JSON.
 
     Arguments:
-        model_class: The model to use, either a pydantic dataclass or
-            a class that inherits from pydantic's BaseModel.
+        model_class: The model to use, either a dataclass, pydantic
+            dataclass or a class that inherits from pydantic's
+            BaseModel. All the fields must be optional.
         status_code: The status code this validation applies
             to. Defaults to 200.
     """
+    if is_dataclass(model_class):
+        model_class = pydantic_dataclass(model_class)
 
-    def decorator(func: Callable) -> Callable:
+    def decorator(
+        func: Callable[..., ResponseReturnValue]
+    ) -> Callable[..., QuartResponseReturnValue]:
         schemas = getattr(func, QUART_SCHEMA_RESPONSE_ATTRIBUTE, {})
         schemas[status_code] = model_class
         setattr(func, QUART_SCHEMA_RESPONSE_ATTRIBUTE, schemas)
 
         @wraps(func)
         async def wrapper(*args: Any, **kwargs: Any) -> Any:
             result = await current_app.ensure_async(func)(*args, **kwargs)
@@ -165,14 +174,16 @@
                 if isinstance(value, dict):
                     try:
                         model_value = model_class(**value)
                     except ValidationError as error:
                         raise ResponseSchemaValidationError(error)
                 elif type(value) == model_class:
                     model_value = value
+                elif is_dataclass(value):
+                    model_value = model_class(**asdict(value))
                 else:
                     raise ResponseSchemaValidationError()
                 if is_dataclass(model_value):
                     return asdict(model_value), status_or_headers, headers
                 else:
                     model_value = cast(BaseModel, model_value)
                     return model_value.dict(), status_or_headers, headers
```

### Comparing `quart-schema-0.8.0/setup.py` & `quart-schema-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ['pydantic>=1.8', 'pyhumps>=1.6.1', 'quart>=0.15']
 
 extras_require = \
 {':python_version < "3.8"': ['typing_extensions']}
 
 setup_kwargs = {
     'name': 'quart-schema',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'A Quart extension to provide schema validation',
-    'long_description': 'Quart-Schema\n============\n\n|Build Status| |docs| |pypi| |python| |license|\n\nQuart-Schema is a Quart extension that provides schema validation and\nauto-generated API documentation. This is particularly useful when\nwriting RESTful APIs.\n\nQuickstart\n----------\n\nQuart-Schema can validate an existing Quart route by decorating it\nwith ``validate_querystring``, ``validate_request``, or\n``validate_response``. It can also validate the JSON data sent and\nreceived over websockets using the ``send_as`` and ``receive_as``\nmethods,\n\n.. code-block:: python\n\n    from datetime import datetime\n    from typing import Optional\n\n    from pydantic.dataclasses import dataclass\n    from quart import Quart\n    from quart_schema import QuartSchema, validate_request, validate_response\n\n    app = Quart(__name__)\n    QuartSchema(app)\n\n    @dataclass\n    class Todo:\n        task: str\n        due: Optional[datetime]\n\n    @app.route("/", methods=["POST"])\n    @validate_request(Todo)\n    @validate_response(Todo, 201)\n    async def create_todo(data: Todo) -> Todo:\n        ... # Do something with data, e.g. save to the DB\n        return data, 201\n\n    @app.websocket("/ws")\n    async def ws() -> None:\n        while True:\n            data = await websocket.receive_as(Todo)\n            ... # Do something with data, e.g. save to the DB\n            await websocket.send_as(data, Todo)\n\nThe documentation is served by default at ``/openapi.json`` according\ntot eh OpenAPI standard, or at ``/docs`` for a `SwaggerUI\n<https://swagger.io/tools/swagger-ui/>`_ interface, or ``/redocs`` for\na `redoc <https://github.com/Redocly/redoc>`_ interface. Note that\nthere is currently no documentation standard for WebSockets.\n\nContributing\n------------\n\nQuart-Schema is developed on `GitLab\n<https://gitlab.com/pgjones/quart-schema>`_. If you come across an\nissue, or have a feature request please open an `issue\n<https://gitlab.com/pgjones/quart-schema/issues>`_. If you want to\ncontribute a fix or the feature-implementation please do (typo fixes\nwelcome), by proposing a `merge request\n<https://gitlab.com/pgjones/quart-schema/merge_requests>`_.\n\nTesting\n~~~~~~~\n\nThe best way to test Quart-Schema is with `Tox\n<https://tox.readthedocs.io>`_,\n\n.. code-block:: console\n\n    $ pip install tox\n    $ tox\n\nthis will check the code style and run the tests.\n\nHelp\n----\n\nThe Quart-Schema `documentation\n<https://pgjones.gitlab.io/quart-schema/>`_ is the best places to\nstart, after that try searching `stack overflow\n<https://stackoverflow.com/questions/tagged/quart>`_ or ask for help\n`on gitter <https://gitter.im/python-quart/lobby>`_. If you still\ncan\'t find an answer please `open an issue\n<https://gitlab.com/pgjones/quart-schema/issues>`_.\n\n\n.. |Build Status| image:: https://gitlab.com/pgjones/quart-schema/badges/master/pipeline.svg\n   :target: https://gitlab.com/pgjones/quart-schema/commits/master\n\n.. |docs| image:: https://img.shields.io/badge/docs-passing-brightgreen.svg\n   :target: https://pgjones.gitlab.io/quart-schema/\n\n.. |pypi| image:: https://img.shields.io/pypi/v/quart-schema.svg\n   :target: https://pypi.python.org/pypi/Quart-Schema/\n\n.. |python| image:: https://img.shields.io/pypi/pyversions/quart-schema.svg\n   :target: https://pypi.python.org/pypi/Quart-Schema/\n\n.. |license| image:: https://img.shields.io/badge/license-MIT-blue.svg\n   :target: https://gitlab.com/pgjones/quart-schema/blob/master/LICENSE\n',
+    'long_description': 'Quart-Schema\n============\n\n|Build Status| |docs| |pypi| |python| |license|\n\nQuart-Schema is a Quart extension that provides schema validation and\nauto-generated API documentation. This is particularly useful when\nwriting RESTful APIs.\n\nQuickstart\n----------\n\nQuart-Schema can validate an existing Quart route by decorating it\nwith ``validate_querystring``, ``validate_request``, or\n``validate_response``. It can also validate the JSON data sent and\nreceived over websockets using the ``send_as`` and ``receive_as``\nmethods.\n\n.. code-block:: python\n\n    from dataclasses import dataclass\n    from datetime import datetime\n    from typing import Optional\n\n    from quart import Quart, websocket\n    from quart_schema import QuartSchema, validate_request, validate_response\n\n    app = Quart(__name__)\n    QuartSchema(app)\n\n    @dataclass\n    class Todo:\n        task: str\n        due: Optional[datetime]\n\n    @app.route("/", methods=["POST"])\n    @validate_request(Todo)\n    @validate_response(Todo, 201)\n    async def create_todo(data: Todo) -> Todo:\n        ... # Do something with data, e.g. save to the DB\n        return data, 201\n\n    @app.websocket("/ws")\n    async def ws() -> None:\n        while True:\n            data = await websocket.receive_as(Todo)\n            ... # Do something with data, e.g. save to the DB\n            await websocket.send_as(data, Todo)\n\nThe documentation is served by default at ``/openapi.json`` according\nto the OpenAPI standard, or at ``/docs`` for a `SwaggerUI\n<https://swagger.io/tools/swagger-ui/>`_ interface, or ``/redocs`` for\na `redoc <https://github.com/Redocly/redoc>`_ interface. Note that\nthere is currently no documentation standard for WebSockets.\n\nContributing\n------------\n\nQuart-Schema is developed on `GitLab\n<https://gitlab.com/pgjones/quart-schema>`_. If you come across an\nissue, or have a feature request please open an `issue\n<https://gitlab.com/pgjones/quart-schema/issues>`_. If you want to\ncontribute a fix or the feature-implementation please do (typo fixes\nwelcome), by proposing a `merge request\n<https://gitlab.com/pgjones/quart-schema/merge_requests>`_.\n\nTesting\n~~~~~~~\n\nThe best way to test Quart-Schema is with `Tox\n<https://tox.readthedocs.io>`_,\n\n.. code-block:: console\n\n    $ pip install tox\n    $ tox\n\nthis will check the code style and run the tests.\n\nHelp\n----\n\nThe Quart-Schema `documentation\n<https://pgjones.gitlab.io/quart-schema/>`_ is the best places to\nstart, after that try searching `stack overflow\n<https://stackoverflow.com/questions/tagged/quart>`_ or ask for help\n`on gitter <https://gitter.im/python-quart/lobby>`_. If you still\ncan\'t find an answer please `open an issue\n<https://gitlab.com/pgjones/quart-schema/issues>`_.\n\n\n.. |Build Status| image:: https://gitlab.com/pgjones/quart-schema/badges/main/pipeline.svg\n   :target: https://gitlab.com/pgjones/quart-schema/commits/main\n\n.. |docs| image:: https://img.shields.io/badge/docs-passing-brightgreen.svg\n   :target: https://pgjones.gitlab.io/quart-schema/\n\n.. |pypi| image:: https://img.shields.io/pypi/v/quart-schema.svg\n   :target: https://pypi.python.org/pypi/Quart-Schema/\n\n.. |python| image:: https://img.shields.io/pypi/pyversions/quart-schema.svg\n   :target: https://pypi.python.org/pypi/Quart-Schema/\n\n.. |license| image:: https://img.shields.io/badge/license-MIT-blue.svg\n   :target: https://gitlab.com/pgjones/quart-schema/blob/main/LICENSE\n',
     'author': 'pgjones',
     'author_email': 'philip.graham.jones@googlemail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/pgjones/quart-schema/',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `quart-schema-0.8.0/PKG-INFO` & `quart-schema-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quart-schema
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Quart extension to provide schema validation
 Home-page: https://gitlab.com/pgjones/quart-schema/
 License: MIT
 Author: pgjones
 Author-email: philip.graham.jones@googlemail.com
 Requires-Python: >=3.7
 Classifier: Development Status :: 3 - Alpha
@@ -38,23 +38,23 @@
 Quickstart
 ----------
 
 Quart-Schema can validate an existing Quart route by decorating it
 with ``validate_querystring``, ``validate_request``, or
 ``validate_response``. It can also validate the JSON data sent and
 received over websockets using the ``send_as`` and ``receive_as``
-methods,
+methods.
 
 .. code-block:: python
 
+    from dataclasses import dataclass
     from datetime import datetime
     from typing import Optional
 
-    from pydantic.dataclasses import dataclass
-    from quart import Quart
+    from quart import Quart, websocket
     from quart_schema import QuartSchema, validate_request, validate_response
 
     app = Quart(__name__)
     QuartSchema(app)
 
     @dataclass
     class Todo:
@@ -72,15 +72,15 @@
     async def ws() -> None:
         while True:
             data = await websocket.receive_as(Todo)
             ... # Do something with data, e.g. save to the DB
             await websocket.send_as(data, Todo)
 
 The documentation is served by default at ``/openapi.json`` according
-tot eh OpenAPI standard, or at ``/docs`` for a `SwaggerUI
+to the OpenAPI standard, or at ``/docs`` for a `SwaggerUI
 <https://swagger.io/tools/swagger-ui/>`_ interface, or ``/redocs`` for
 a `redoc <https://github.com/Redocly/redoc>`_ interface. Note that
 there is currently no documentation standard for WebSockets.
 
 Contributing
 ------------
 
@@ -113,22 +113,22 @@
 start, after that try searching `stack overflow
 <https://stackoverflow.com/questions/tagged/quart>`_ or ask for help
 `on gitter <https://gitter.im/python-quart/lobby>`_. If you still
 can't find an answer please `open an issue
 <https://gitlab.com/pgjones/quart-schema/issues>`_.
 
 
-.. |Build Status| image:: https://gitlab.com/pgjones/quart-schema/badges/master/pipeline.svg
-   :target: https://gitlab.com/pgjones/quart-schema/commits/master
+.. |Build Status| image:: https://gitlab.com/pgjones/quart-schema/badges/main/pipeline.svg
+   :target: https://gitlab.com/pgjones/quart-schema/commits/main
 
 .. |docs| image:: https://img.shields.io/badge/docs-passing-brightgreen.svg
    :target: https://pgjones.gitlab.io/quart-schema/
 
 .. |pypi| image:: https://img.shields.io/pypi/v/quart-schema.svg
    :target: https://pypi.python.org/pypi/Quart-Schema/
 
 .. |python| image:: https://img.shields.io/pypi/pyversions/quart-schema.svg
    :target: https://pypi.python.org/pypi/Quart-Schema/
 
 .. |license| image:: https://img.shields.io/badge/license-MIT-blue.svg
-   :target: https://gitlab.com/pgjones/quart-schema/blob/master/LICENSE
+   :target: https://gitlab.com/pgjones/quart-schema/blob/main/LICENSE
```

