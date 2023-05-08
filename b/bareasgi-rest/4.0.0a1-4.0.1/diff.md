# Comparing `tmp/bareASGI-rest-4.0.0a1.tar.gz` & `tmp/bareASGI-rest-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bareASGI-rest-4.0.0a1.tar", max compression
+gzip compressed data, was "bareASGI-rest-4.0.1.tar", max compression
```

## Comparing `bareASGI-rest-4.0.0a1.tar` & `bareASGI-rest-4.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     5668 2021-10-11 07:23:58.310185 bareASGI-rest-4.0.0a1/README.md
--rw-r--r--   0        0        0      333 2021-10-11 07:24:17.362472 bareASGI-rest-4.0.0a1/bareasgi_rest/__init__.py
--rw-r--r--   0        0        0     2835 2021-10-11 07:23:58.310185 bareASGI-rest-4.0.0a1/bareasgi_rest/arg_builder.py
--rw-r--r--   0        0        0     1749 2021-10-11 07:55:48.878152 bareASGI-rest-4.0.0a1/bareasgi_rest/constants.py
--rw-r--r--   0        0        0      556 2021-10-11 07:23:58.310185 bareASGI-rest-4.0.0a1/bareasgi_rest/helpers.py
--rw-r--r--   0        0        0        0 2021-10-11 07:23:58.310185 bareASGI-rest-4.0.0a1/bareasgi_rest/py.typed
--rw-r--r--   0        0        0    15157 2021-10-11 08:02:27.536676 bareASGI-rest-4.0.0a1/bareasgi_rest/rest_router.py
--rw-r--r--   0        0        0       20 2021-10-11 07:23:58.310185 bareASGI-rest-4.0.0a1/bareasgi_rest/serialization/__init__.py
--rw-r--r--   0        0        0     3073 2021-10-11 07:23:58.310185 bareASGI-rest-4.0.0a1/bareasgi_rest/serialization/json.py
--rw-r--r--   0        0        0      710 2021-10-11 07:54:31.147125 bareASGI-rest-4.0.0a1/bareasgi_rest/serialization/xml.py
--rw-r--r--   0        0        0      267 2021-10-11 07:23:58.310185 bareASGI-rest-4.0.0a1/bareasgi_rest/swagger/__init__.py
--rw-r--r--   0        0        0     2754 2021-10-11 07:23:58.310185 bareASGI-rest-4.0.0a1/bareasgi_rest/swagger/config.py
--rw-r--r--   0        0        0     2068 2021-10-11 07:24:17.366472 bareASGI-rest-4.0.0a1/bareasgi_rest/swagger/controller.py
--rw-r--r--   0        0        0     1826 2021-10-11 07:23:58.310185 bareASGI-rest-4.0.0a1/bareasgi_rest/swagger/entry.py
--rw-r--r--   0        0        0     1042 2021-10-11 07:23:58.310185 bareASGI-rest-4.0.0a1/bareasgi_rest/swagger/errors.py
--rw-r--r--   0        0        0     4951 2021-10-11 14:12:15.743219 bareASGI-rest-4.0.0a1/bareasgi_rest/swagger/parameters.py
--rw-r--r--   0        0        0      456 2021-10-11 07:23:58.310185 bareASGI-rest-4.0.0a1/bareasgi_rest/swagger/paths.py
--rw-r--r--   0        0        0     5101 2021-10-11 14:11:18.209813 bareASGI-rest-4.0.0a1/bareasgi_rest/swagger/properties.py
--rw-r--r--   0        0        0     2636 2021-10-11 07:23:58.314185 bareASGI-rest-4.0.0a1/bareasgi_rest/swagger/repository.py
--rw-r--r--   0        0        0     1255 2021-10-11 07:23:58.314185 bareASGI-rest-4.0.0a1/bareasgi_rest/swagger/responses.py
--rw-r--r--   0        0        0      590 2021-10-11 07:23:58.314185 bareASGI-rest-4.0.0a1/bareasgi_rest/swagger/utils.py
--rw-r--r--   0        0        0     4487 2021-10-11 07:23:58.314185 bareASGI-rest-4.0.0a1/bareasgi_rest/templates/swagger.html
--rw-r--r--   0        0        0     1071 2021-10-11 07:24:17.366472 bareASGI-rest-4.0.0a1/bareasgi_rest/types.py
--rw-r--r--   0        0        0      279 2021-10-11 07:23:58.314185 bareASGI-rest-4.0.0a1/bareasgi_rest/utils.py
--rw-r--r--   0        0        0      973 2021-10-11 14:12:28.551533 bareASGI-rest-4.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     6905 2021-10-11 14:12:56.095820 bareASGI-rest-4.0.0a1/setup.py
--rw-r--r--   0        0        0     6604 2021-10-11 14:12:56.096597 bareASGI-rest-4.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     5345 2022-10-02 07:16:44.815069 bareASGI-rest-4.0.1/README.md
+-rw-r--r--   0        0        0      333 2022-09-23 16:55:22.067275 bareASGI-rest-4.0.1/bareasgi_rest/__init__.py
+-rw-r--r--   0        0        0     3075 2022-10-02 07:16:01.839182 bareASGI-rest-4.0.1/bareasgi_rest/arg_builder.py
+-rw-r--r--   0        0        0     1749 2022-09-23 16:55:22.067615 bareASGI-rest-4.0.1/bareasgi_rest/constants.py
+-rw-r--r--   0        0        0      556 2022-09-23 16:41:12.116759 bareASGI-rest-4.0.1/bareasgi_rest/helpers.py
+-rw-r--r--   0        0        0        0 2022-09-23 16:41:12.116790 bareASGI-rest-4.0.1/bareasgi_rest/py.typed
+-rw-r--r--   0        0        0    14941 2022-10-01 07:45:39.671215 bareASGI-rest-4.0.1/bareasgi_rest/rest_router.py
+-rw-r--r--   0        0        0       20 2022-09-23 16:41:12.117041 bareASGI-rest-4.0.1/bareasgi_rest/serialization/__init__.py
+-rw-r--r--   0        0        0     3073 2022-09-23 16:41:12.117117 bareASGI-rest-4.0.1/bareasgi_rest/serialization/json.py
+-rw-r--r--   0        0        0      710 2022-09-23 16:55:22.068222 bareASGI-rest-4.0.1/bareasgi_rest/serialization/xml.py
+-rw-r--r--   0        0        0      267 2022-09-23 16:41:12.117299 bareASGI-rest-4.0.1/bareasgi_rest/swagger/__init__.py
+-rw-r--r--   0        0        0     2754 2022-09-23 16:41:12.117385 bareASGI-rest-4.0.1/bareasgi_rest/swagger/config.py
+-rw-r--r--   0        0        0     2068 2022-09-23 16:55:22.068574 bareASGI-rest-4.0.1/bareasgi_rest/swagger/controller.py
+-rw-r--r--   0        0        0     1848 2022-09-24 09:47:02.814216 bareASGI-rest-4.0.1/bareasgi_rest/swagger/entry.py
+-rw-r--r--   0        0        0     1082 2022-10-01 07:49:41.321292 bareASGI-rest-4.0.1/bareasgi_rest/swagger/errors.py
+-rw-r--r--   0        0        0     5007 2022-09-24 09:54:21.151191 bareASGI-rest-4.0.1/bareasgi_rest/swagger/parameters.py
+-rw-r--r--   0        0        0      456 2022-09-23 16:41:12.117844 bareASGI-rest-4.0.1/bareasgi_rest/swagger/paths.py
+-rw-r--r--   0        0        0     5355 2022-09-24 10:12:40.801067 bareASGI-rest-4.0.1/bareasgi_rest/swagger/properties.py
+-rw-r--r--   0        0        0     2640 2022-09-24 09:55:18.753375 bareASGI-rest-4.0.1/bareasgi_rest/swagger/repository.py
+-rw-r--r--   0        0        0     1255 2022-09-23 16:41:12.118078 bareASGI-rest-4.0.1/bareasgi_rest/swagger/responses.py
+-rw-r--r--   0        0        0      590 2022-09-23 16:41:12.118146 bareASGI-rest-4.0.1/bareasgi_rest/swagger/utils.py
+-rw-r--r--   0        0        0     4487 2022-09-23 16:41:12.118294 bareASGI-rest-4.0.1/bareasgi_rest/templates/swagger.html
+-rw-r--r--   0        0        0     1071 2022-09-23 16:55:22.069013 bareASGI-rest-4.0.1/bareasgi_rest/types.py
+-rw-r--r--   0        0        0      279 2022-09-23 16:41:12.118469 bareASGI-rest-4.0.1/bareasgi_rest/utils.py
+-rw-r--r--   0        0        0      945 2023-05-08 06:07:39.874037 bareASGI-rest-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6582 2023-05-08 06:08:09.716897 bareASGI-rest-4.0.1/setup.py
+-rw-r--r--   0        0        0     6355 2023-05-08 06:08:09.717240 bareASGI-rest-4.0.1/PKG-INFO
```

### Comparing `bareASGI-rest-4.0.0a1/README.md` & `bareASGI-rest-4.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,22 @@
 (read the [docs](https://rob-blackbourn.github.io/bareASGI-rest/)).
 
 It includes:
 
 - A router to simplify the creation of REST APIs,
 - A swagger API endpoint
 
-This is a Python 3.7+ package, and is currently pre-release.
-
-## Branch
-
-This is the v3 maintenance branch.
+This is a Python 3.8+ package.
 
 ## Installation
 
-The package can be install from pypi.
-
-It is currently pre-release so you will need the --pre flag.
+The package can be installed from pypi.
 
 ```bash
-$ pip install --pre bareASGI-rest
+$ pip install bareASGI-rest
 ```
 
 An ASGI server will be required to run the code. The examples below use
 [uvicorn](https://www.uvicorn.org/).
 
 ```bash
 $ pip install uvicorn
@@ -41,20 +35,16 @@
 
 ### Creating typed dictionaries
 
 Here is the type of a book. We use `TypedDict` to allow automatic type discovery
 
 ```python
 from datetime import datetime
-try:
-    # Available in 3.8
-    from typing import TypedDict  # type:ignore
-except:
-    # Available in 3.7
-    from typing_extensions import TypedDict
+from typing import TypedDict
+
 
 class Book(TypedDict):
     """A Book
 
     Args:
         book_id (int): The book id
         title (str): The title
@@ -71,15 +61,16 @@
 
 ### Creating the API
 
 Now we can build the API.
 
 ```python
 from typing import Dict, List
-from urllib.error import HTTPError
+
+from bareasgi_rest import RestError
 
 
 BOOKS: Dict[int, Book] = {}
 NEXT_ID: int = 0
 
 async def get_books() -> List[Book]:
     """Get all the books.
@@ -95,22 +86,22 @@
 async def get_book(book_id: int) -> Book:
     """Get a book for a given id
 
     Args:
         book_id (int): The id of the book
 
     Raises:
-        HTTPError: 404, when a book is not found
+        RestError: 404, when a book is not found
 
     Returns:
         Book: The book
     """
 
     if book_id not in BOOKS:
-        raise HTTPError(None, 404, None, None, None)
+        raise RestError(404, "Book not found")
 
     return BOOKS[book_id]
 
 
 async def create_book(
         author: str,
         title: str,
@@ -147,25 +138,25 @@
     Args:
         book_id (int): The id of the book to update
         author (str): The new author
         title (str): The title
         published (datetime): The publication date
 
     Raises:
-        HTTPError: 404, when a book is not found
+        RestError: 404, when a book is not found
     """
     if book_id not in BOOKS:
-        raise HTTPError(None, 404, None, None, None)
+        raise RestError(404, "Book not found")
     BOOKS[book_id]['title'] = title
     BOOKS[book_id]['author'] = author
     BOOKS[book_id]['published'] = published
 ```
 
-We can see that errors are handler by raising HTTPError
-from the `urllib.errors` standard library package. A convention has been applied such that the status code MUST
+We can see that errors are handler by raising ResetError.
+A convention has been applied such that the status code MUST
 appear before the message, separated by a comma.
 
 ### Adding support for the REST router
 
 Now we must create our application and add support for the router.
 
 ```python
```

### Comparing `bareASGI-rest-4.0.0a1/bareasgi_rest/arg_builder.py` & `bareASGI-rest-4.0.1/bareasgi_rest/arg_builder.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,16 +45,20 @@
         else:
             if parameter.name in matches:
                 value = arg_deserializer(
                     matches[parameter.name],
                     parameter.annotation
                 )
             elif parameter.name in query:
-                if typing_inspect.is_list_type(parameter.annotation):
-                    element_type, *_rest = typing_inspect.get_args(
+                if typing_inspect.is_list_type(  # type: ignore
+                        parameter.annotation
+                ) or typing_inspect.is_optional_list_type(  # type: ignore
+                    parameter.annotation
+                ):
+                    element_type, *_rest = typing_inspect.get_args(  # type: ignore
                         parameter.annotation
                     )
                     value = [
                         arg_deserializer(
                             item,
                             element_type
                         )
@@ -62,15 +66,17 @@
                     ]
                 else:
                     value = arg_deserializer(
                         query[parameter.name][0],
                         parameter.annotation
                     )
 
-            elif typing_inspect.is_optional_type(parameter.annotation):
+            elif typing_inspect.is_optional_type(  # type: ignore
+                    parameter.annotation
+            ):
                 value = None
             else:
                 raise KeyError(parameter.name)
 
         if (
                 parameter.kind == Parameter.POSITIONAL_ONLY
                 or parameter.kind == Parameter.POSITIONAL_OR_KEYWORD
```

### Comparing `bareASGI-rest-4.0.0a1/bareasgi_rest/constants.py` & `bareASGI-rest-4.0.1/bareasgi_rest/constants.py`

 * *Files identical despite different names*

### Comparing `bareASGI-rest-4.0.0a1/bareasgi_rest/helpers.py` & `bareASGI-rest-4.0.1/bareasgi_rest/helpers.py`

 * *Files identical despite different names*

### Comparing `bareASGI-rest-4.0.0a1/bareasgi_rest/rest_router.py` & `bareASGI-rest-4.0.1/bareasgi_rest/rest_router.py`

 * *Files 4% similar despite different names*

```diff
@@ -288,33 +288,30 @@
                     signature,
                     route_args,
                     query_args,
                     body_reader,
                     arg_deserializer
                 )
             except BaseException as error:  # pylint: disable=broad-except
-                return HttpResponse(
-                    response_code.BAD_REQUEST,
-                    [(b'content-type', b'text/plain')],
-                    text_writer("Failed to make args:" + ". ".join(error.args))
+                return HttpResponse.from_text(
+                    "Failed to make args:" + ". ".join(error.args),
+                    status=response_code.BAD_REQUEST
                 )
 
             try:
                 body = await callback(*args, **kwargs)
             except RestError as error:
-                return HttpResponse(
-                    error.status,
-                    [(b'content-type', b'text/plain')],
-                    text_writer(error.message)
+                return HttpResponse.from_text(
+                    error.message,
+                    status=error.status
                 )
             except BaseException as error:  # pylint: disable=broad-except
-                return HttpResponse(
-                    response_code.INTERNAL_SERVER_ERROR,
-                    [(b'content-type', b'text/plain')],
-                    text_writer(str(error))
+                return HttpResponse.from_text(
+                    str(error),
+                    status=response_code.INTERNAL_SERVER_ERROR
                 )
 
             accept = header.accept(request.scope['headers'])
             writer = self._make_writer(
                 body,
                 accept,
                 signature.return_annotation,
@@ -327,18 +324,17 @@
                     if content_type in accept:
                         break
                 else:
                     if b'*/*' in accept:
                         # Prefer the first content type that is supported.
                         content_type = produces[0]
                     else:
-                        return HttpResponse(
-                            response_code.UNSUPPORTED_MEDIA_TYPE,
-                            [(b'content-type', b'text/plain')],
-                            text_writer('Unsupported media type')
+                        return HttpResponse.from_text(
+                            'Unsupported media type',
+                            status=response_code.UNSUPPORTED_MEDIA_TYPE
                         )
 
             headers = [
                 (b'content-type', content_type)
             ]
 
             return HttpResponse(status_code, headers, writer)
```

### Comparing `bareASGI-rest-4.0.0a1/bareasgi_rest/serialization/json.py` & `bareASGI-rest-4.0.1/bareasgi_rest/serialization/json.py`

 * *Files identical despite different names*

### Comparing `bareASGI-rest-4.0.0a1/bareasgi_rest/serialization/xml.py` & `bareASGI-rest-4.0.1/bareasgi_rest/serialization/xml.py`

 * *Files identical despite different names*

### Comparing `bareASGI-rest-4.0.0a1/bareasgi_rest/swagger/config.py` & `bareASGI-rest-4.0.1/bareasgi_rest/swagger/config.py`

 * *Files identical despite different names*

### Comparing `bareASGI-rest-4.0.0a1/bareasgi_rest/swagger/controller.py` & `bareASGI-rest-4.0.1/bareasgi_rest/swagger/controller.py`

 * *Files identical despite different names*

### Comparing `bareASGI-rest-4.0.0a1/bareasgi_rest/swagger/entry.py` & `bareASGI-rest-4.0.1/bareasgi_rest/swagger/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         collection_format: str,
         tags: Optional[List[str]],
         ok_status_code: int,
         ok_status_description: str,
         config: SwaggerConfig
 ) -> Dict[str, Any]:
     signature = inspect.signature(callback)
-    docstring = docstring_parser.parse(inspect.getdoc(callback))
+    docstring = docstring_parser.parse(inspect.getdoc(callback) or '')
     params = make_swagger_parameters(
         method,
         consumes,
         path_definition,
         signature.parameters,
         docstring,
         collection_format,
@@ -49,15 +49,15 @@
         docstring.raises if docstring else None,
         ok_status_code,
         ok_status_description,
         collection_format,
         config
     )
 
-    entry = {
+    entry: Dict[str, Any] = {
         'parameters': params,
         'produces': [content_type.decode() for content_type in produces],
         'consumes': [accept.decode() for accept in consumes],
         'responses': responses
     }
 
     if docstring:
```

### Comparing `bareASGI-rest-4.0.0a1/bareasgi_rest/swagger/errors.py` & `bareASGI-rest-4.0.1/bareasgi_rest/swagger/errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 
 from docstring_parser import DocstringRaises
 
 
 def gather_error_responses(docstring_raises: List[DocstringRaises]) -> Dict[int, Any]:
     """Gather error responses
 
-    Looks for exceptions of type `HTTPError` with a description starting with
+    Looks for exceptions of type `RestError` with a description starting with
     the error code: e.g. `"404, when a book is not found"`
 
     Args:
         docstring_raises (List[DocstringRaises]): The raises from the docstring
 
     Returns:
         Dict[int, Any]: The error response schema.
     """
     responses: Dict[int, Any] = {}
     for raises in docstring_raises:
-        if raises.type_name != 'HTTPError':
+        if raises.type_name != 'RestError':
             continue
-        first, sep, rest = raises.description.partition(',')
+        description = raises.description or ''
+        first, sep, rest = description.partition(',')
         if not sep:
             continue
         try:
             error_code = int(first.strip())
             description = rest.strip()
             responses[error_code] = {
                 'description': description
```

### Comparing `bareASGI-rest-4.0.0a1/bareasgi_rest/swagger/parameters.py` & `bareASGI-rest-4.0.1/bareasgi_rest/swagger/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     AbstractSet,
     Any,
     Dict,
     List,
     Mapping,
     Optional,
     Sequence,
-    Set
+    Set,
 )
 
 from bareasgi.basic_router.path_definition import PathDefinition
 from docstring_parser import Docstring, DocstringParam
 import jetblack_serialization.typing_inspect_ex as typing_inspect
 from jetblack_serialization.custom_annotations import (
     is_any_serialization_annotation
@@ -53,15 +53,15 @@
         source: str,
         parameters: Mapping[str, Parameter],
         path_variables: AbstractSet[str],
         docstring: Docstring,
         collection_format: str,
         config: SwaggerConfig
 ) -> List[Dict[str, Any]]:
-    """Make inline paramters for query or form"""
+    """Make inline parameters for query or form"""
     props: List[Dict[str, Any]] = []
     for parameter in parameters.values():
         if parameter.name in path_variables:
             continue
         docstring_param = find_docstring_param(parameter.name, docstring)
         props.append(
             _make_swagger_parameter(
@@ -137,15 +137,17 @@
             )
         )
     else:
         # Fall back to b'application/json'.
         for parameter in available_parameters.values():
             docstring_param = find_docstring_param(parameter.name, docstring)
             if is_any_serialization_annotation(parameter.annotation):
-                body_type = typing_inspect.get_origin(parameter.annotation)
+                body_type = typing_inspect.get_origin(  # type: ignore
+                    parameter.annotation
+                )
                 schema = get_property(
                     body_type,
                     config.serialize_key(parameter.name),
                     None,
                     Parameter.empty,
                     collection_format,
                     config
```

### Comparing `bareASGI-rest-4.0.0a1/bareasgi_rest/swagger/properties.py` & `bareASGI-rest-4.0.1/bareasgi_rest/swagger/properties.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,26 +44,28 @@
 
     Raises:
         TypeError: If the property type is not handled.
 
     Returns:
         Dict[str, Any]: The swagger property.
     """
-    if typing_inspect.is_annotated_type(annotation):
+    if typing_inspect.is_annotated_type(annotation):  # type: ignore
         return get_property(
-            typing_inspect.get_origin(annotation),
+            typing_inspect.get_origin(annotation),  # type: ignore
             name,
             description,
             default,
             collection_format,
             config
         )
 
-    if typing_inspect.is_optional_type(annotation):
-        optional_type = typing_inspect.get_optional_type(annotation)
+    if typing_inspect.is_optional_type(annotation):  # type: ignore
+        optional_type = typing_inspect.get_optional_type(  # type: ignore
+            annotation
+        )
         return get_property(
             optional_type,
             name,
             description,
             default,
             collection_format,
             config
@@ -95,53 +97,59 @@
         prop['format'] = 'date-time'
     elif annotation is timedelta:
         # Note: Swagger has no support for durations. I made up the format.
         prop['type'] = 'string'
         prop['format'] = 'duration'
     elif isclass(annotation) and issubclass(annotation, Enum):
         prop['type'] = 'string'
-        prop['enum'] = [name for name, value in annotation.__members__.items()]
-    elif typing_inspect.is_list_type(annotation):
-        contained_type, *_rest = typing_inspect.get_args(annotation)
+        prop['enum'] = [name for name, _value in annotation.__members__.items()]
+    elif typing_inspect.is_list_type(annotation):  # type: ignore
+        contained_type, *_rest = typing_inspect.get_args(  # type: ignore
+            annotation
+        )
         prop['type'] = 'array'
         prop['collectionFormat'] = collection_format
         prop['items'] = get_property(
             contained_type,
             None,
             None,
             default,
             collection_format,
             config
         )
-    elif typing_inspect.is_dict_type(annotation):
+    elif typing_inspect.is_dict_type(annotation):  # type: ignore
         prop['type'] = 'object'
-    elif typing_inspect.is_typed_dict_type(annotation):
+    elif typing_inspect.is_typed_dict_type(annotation):  # type: ignore
         prop['type'] = 'object'
         prop['properties'] = get_properties(
             annotation,
-            docstring_parser.parse(inspect.getdoc(annotation)),
+            docstring_parser.parse(inspect.getdoc(annotation) or ''),
             collection_format,
             config
         )
     else:
         raise TypeError('Unhandled type annotation')
 
     return prop
 
 
-def _get_default(annotation, member_annotation, name) -> Any:
+def _get_default(
+        annotation: object,
+        member_annotation: Annotation,
+        name: str
+) -> Any:
     if is_any_default_annotation(member_annotation):
         _, default_value = get_default_annotation(member_annotation)
         return default_value.value
 
     return getattr(annotation, name, inspect.Parameter.empty)
 
 
 def get_properties(
-        annotation,
+        annotation: object,
         docstring: Docstring,
         collection_format: str,
         config: SwaggerConfig
 ) -> Dict[str, Any]:
     """Get the properties of a TypedDict
 
     Args:
@@ -149,15 +157,15 @@
             annotations
         docstring (Docstring): The docstring
         collection_format (str): The collection format
 
     Returns:
         Dict[str, Any]: The swagger properties.
     """
-    annotations: Dict[str, Annotation] = typing_inspect.typed_dict_keys(
+    annotations: Dict[str, Annotation] = typing_inspect.typed_dict_keys(  # type: ignore
         annotation
     )
     properties: Dict[str, Any] = {}
     for name, member_annotation in annotations.items():
         camelcase_name = config.serialize_key(name)
         docstring_param = find_docstring_param(name, docstring)
         description = docstring_param.description if docstring_param else None
```

### Comparing `bareASGI-rest-4.0.0a1/bareasgi_rest/swagger/repository.py` & `bareASGI-rest-4.0.1/bareasgi_rest/swagger/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Dict,
     List,
     Mapping,
     Optional,
     Sequence
 )
 
-from bareasgi.basic_router.http_router import PathDefinition
+from bareasgi.basic_router.path_definition import PathDefinition
 
 from ..types import RestCallback
 
 from .config import SwaggerConfig
 from .entry import make_swagger_entry
 from .paths import make_swagger_path
```

### Comparing `bareASGI-rest-4.0.0a1/bareasgi_rest/swagger/responses.py` & `bareASGI-rest-4.0.1/bareasgi_rest/swagger/responses.py`

 * *Files identical despite different names*

### Comparing `bareASGI-rest-4.0.0a1/bareasgi_rest/swagger/utils.py` & `bareASGI-rest-4.0.1/bareasgi_rest/swagger/utils.py`

 * *Files identical despite different names*

### Comparing `bareASGI-rest-4.0.0a1/bareasgi_rest/templates/swagger.html` & `bareASGI-rest-4.0.1/bareasgi_rest/templates/swagger.html`

 * *Files identical despite different names*

### Comparing `bareASGI-rest-4.0.0a1/bareasgi_rest/types.py` & `bareASGI-rest-4.0.1/bareasgi_rest/types.py`

 * *Files identical despite different names*

### Comparing `bareASGI-rest-4.0.0a1/pyproject.toml` & `bareASGI-rest-4.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 [tool.poetry]
 name = "bareASGI-rest"
-version = "4.0.0-alpha.1"
+version = "4.0.1"
 description = "REST support for bareASGI"
 repository = "https://github.com/rob-blackbourn/bareASGI-rest"
 authors = ["Rob Blackbourn <rob.blackbourn@gmail.com>"]
 keywords = ['bareASGI', 'rest', 'swagger']
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
   { include = "bareasgi_rest" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-bareasgi = "^4.0"
+bareasgi = "^4.2"
 bareasgi-jinja2 = "^4.0"
-docstring-parser = "^0.6"
-typing-extensions = "^3.7"
-lxml = "^4.4.2"
-stringcase = "^1.2.0"
-jetblack-serialization = "^3.0.0-alpha.2"
+docstring-parser = "^0.15"
+lxml = "^4.9"
+stringcase = "^1.2"
+jetblack-serialization = "^3.0.1"
+typing-extensions = "^4"
+typing_inspect = "^0.8"
 
 [tool.poetry.dev-dependencies]
-autopep8 = "^1.5"
-hypercorn = "^0.11"
-mypy = "^0.910"
-pylint = "^2.9"
-pytest = "^5.3"
-pytest-asyncio = "^0.10"
-pytest-runner = "^5.2"
-uvicorn = "^0.15"
-rope = "^0.16.0"
-mkdocs = "^1.2"
-mkdocs-material = "^7.2"
-jetblack-markdown = "^0.6"
-mike = "^1.1.1"
-types-setuptools = "^57.0.2"
+autopep8 = "^1"
+hypercorn = "^0.14"
+mypy = "^0.971"
+pylint = "^2"
+pytest = "^7"
+pytest-asyncio = "^0.19"
+pytest-runner = "^6"
+uvicorn = "^0.18"
+mkdocs = "^1.3"
+mkdocs-material = "^8.5"
+jetblack-markdown = "^1.1"
+mike = "^1.1"
+types-setuptools = "^65"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `bareASGI-rest-4.0.0a1/setup.py` & `bareASGI-rest-4.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 ['bareasgi_rest', 'bareasgi_rest.serialization', 'bareasgi_rest.swagger']
 
 package_data = \
 {'': ['*'], 'bareasgi_rest': ['templates/*']}
 
 install_requires = \
 ['bareasgi-jinja2>=4.0,<5.0',
- 'bareasgi>=4.0,<5.0',
- 'docstring-parser>=0.6,<0.7',
- 'jetblack-serialization>=3.0.0-alpha.2,<4.0.0',
- 'lxml>=4.4.2,<5.0.0',
- 'stringcase>=1.2.0,<2.0.0',
- 'typing-extensions>=3.7,<4.0']
+ 'bareasgi>=4.2,<5.0',
+ 'docstring-parser>=0.15,<0.16',
+ 'jetblack-serialization>=3.0.1,<4.0.0',
+ 'lxml>=4.9,<5.0',
+ 'stringcase>=1.2,<2.0',
+ 'typing-extensions>=4,<5',
+ 'typing_inspect>=0.8,<0.9']
 
 setup_kwargs = {
     'name': 'bareasgi-rest',
-    'version': '4.0.0a1',
+    'version': '4.0.1',
     'description': 'REST support for bareASGI',
-    'long_description': '# bareASGI-rest\n\nThis package provides enhanced support for writing REST\nAPIs with [bareASGI](https://bareasgi.com),\n(read the [docs](https://rob-blackbourn.github.io/bareASGI-rest/)).\n\nIt includes:\n\n- A router to simplify the creation of REST APIs,\n- A swagger API endpoint\n\nThis is a Python 3.7+ package, and is currently pre-release.\n\n## Branch\n\nThis is the v3 maintenance branch.\n\n## Installation\n\nThe package can be install from pypi.\n\nIt is currently pre-release so you will need the --pre flag.\n\n```bash\n$ pip install --pre bareASGI-rest\n```\n\nAn ASGI server will be required to run the code. The examples below use\n[uvicorn](https://www.uvicorn.org/).\n\n```bash\n$ pip install uvicorn\n```\n\n## Usage\n\nThe router provided by this package maps the arguments and\ntypes of request handlers.\n\nWe will create a mock book repository.\n\n### Creating typed dictionaries\n\nHere is the type of a book. We use `TypedDict` to allow automatic type discovery\n\n```python\nfrom datetime import datetime\ntry:\n    # Available in 3.8\n    from typing import TypedDict  # type:ignore\nexcept:\n    # Available in 3.7\n    from typing_extensions import TypedDict\n\nclass Book(TypedDict):\n    """A Book\n\n    Args:\n        book_id (int): The book id\n        title (str): The title\n        author (str): The author\n        published (datetime): The publication date\n    """\n    book_id: int\n    title: str\n    author: str\n    published: datetime\n```\n\nNote: the docstring will be used to provide documentation for swagger.\n\n### Creating the API\n\nNow we can build the API.\n\n```python\nfrom typing import Dict, List\nfrom urllib.error import HTTPError\n\n\nBOOKS: Dict[int, Book] = {}\nNEXT_ID: int = 0\n\nasync def get_books() -> List[Book]:\n    """Get all the books.\n\n    This method gets all the books in the shop.\n\n    Returns:\n        List[Book]: All the books\n    """\n    return list(BOOKS.values())\n\n\nasync def get_book(book_id: int) -> Book:\n    """Get a book for a given id\n\n    Args:\n        book_id (int): The id of the book\n\n    Raises:\n        HTTPError: 404, when a book is not found\n\n    Returns:\n        Book: The book\n    """\n\n    if book_id not in BOOKS:\n        raise HTTPError(None, 404, None, None, None)\n\n    return BOOKS[book_id]\n\n\nasync def create_book(\n        author: str,\n        title: str,\n        published: datetime\n) -> int:\n    """Add a book\n\n    Args:\n        author (str): The author\n        title (str): The title\n        published (datetime): The publication date\n\n    Returns:\n        int: The id of the new book\n    """\n    NEXT_ID += 1\n    BOOKS[NEXT_ID] = Book(\n        book_id=NEXT_ID,\n        title=title,\n        author=author,\n        published=published\n    )\n    return NEXT_ID\n\n\nasync def update_book(\n        book_id: int,\n        author: str,\n        title: str,\n        published: datetime\n) -> None:\n    """Update a book\n\n    Args:\n        book_id (int): The id of the book to update\n        author (str): The new author\n        title (str): The title\n        published (datetime): The publication date\n\n    Raises:\n        HTTPError: 404, when a book is not found\n    """\n    if book_id not in BOOKS:\n        raise HTTPError(None, 404, None, None, None)\n    BOOKS[book_id][\'title\'] = title\n    BOOKS[book_id][\'author\'] = author\n    BOOKS[book_id][\'published\'] = published\n```\n\nWe can see that errors are handler by raising HTTPError\nfrom the `urllib.errors` standard library package. A convention has been applied such that the status code MUST\nappear before the message, separated by a comma.\n\n### Adding support for the REST router\n\nNow we must create our application and add support for the router.\n\n```python\nfrom bareasgi import Application\nfrom bareasgi_rest import RestHttpRouter, add_swagger_ui\n\n\nrouter = RestHttpRouter(\n    None,\n    title="Books",\n    version="1",\n    description="A book api",\n    base_path=\'/api/1\',\n    tags=[\n        {\n            \'name\': \'Books\',\n            \'description\': \'The book store API\'\n        }\n    ]\n)\napp = Application(http_router=router)\nadd_swagger_ui(app)\n```\n\nNote the `base_path` argument can be used to prefix all\npaths.\n\nThe `RestHttpRouter` is a subclass of the basic router, so\nall those methods are also available.\n\n### Creating the routes\n\nNow we can create the routes:\n\n```python\ntags = [\'Books\']\nrouter.add_rest({\'GET\'}, \'/books\', get_books,tags=tags)\nrouter.add_rest({\'GET\'}, \'/books/{bookId:int}\', get_book, tags=tags)\nrouter.add_rest({\'POST\'}, \'/books\', create_book, tags=tags, status_code=201)\nrouter.add_rest({\'PUT\'}, \'/books/{bookId:int}\', update_book, tags=tags, status_code=204)\n```\n\nFirst we should note that the paths will be prefixed with the\n`base_path` provided to the router.\n\nReferring back to the implementation of `get_book` we can\nsee that the camel-case path variable `bookId` has been\nmapped to the snake-case `book_id` parameter. The JSON object provided in the body of the `create_book` will\nsimilarly map camel-cased properties to the snake-cased\nfunction parameters.\n\nWe can also see how the status codes have been overridden\nfor the `POST` and `PUT` endpoints, and all the routes\nhave the "Books" tag for grouping in the UI.\n\n### Serving the API\n\nFinally we can serve the API:\n\n```python\nimport uvicorn\n\nuvicorn.run(app, port=9009)\n```\n\nBrowsing to http://localhost/api/1/swagger we should see:\n\n![Top Level](screenshot1.png)\n\nWhen we expand `GET /books/{bookId}` we can see all the\ninformation provided in the docstring and typing has been\npassed through to the swagger UI.\n\n![GET /books/{bookId}](screenshot2.png)\n\n## Thanks\n\nThanks to [rr-](https://github.com/rr-) and contributors\nfor the excellent\n[docstring-parser](https://github.com/rr-/docstring_parser)\npackage.\n',
+    'long_description': '# bareASGI-rest\n\nThis package provides enhanced support for writing REST\nAPIs with [bareASGI](https://bareasgi.com),\n(read the [docs](https://rob-blackbourn.github.io/bareASGI-rest/)).\n\nIt includes:\n\n- A router to simplify the creation of REST APIs,\n- A swagger API endpoint\n\nThis is a Python 3.8+ package.\n\n## Installation\n\nThe package can be installed from pypi.\n\n```bash\n$ pip install bareASGI-rest\n```\n\nAn ASGI server will be required to run the code. The examples below use\n[uvicorn](https://www.uvicorn.org/).\n\n```bash\n$ pip install uvicorn\n```\n\n## Usage\n\nThe router provided by this package maps the arguments and\ntypes of request handlers.\n\nWe will create a mock book repository.\n\n### Creating typed dictionaries\n\nHere is the type of a book. We use `TypedDict` to allow automatic type discovery\n\n```python\nfrom datetime import datetime\nfrom typing import TypedDict\n\n\nclass Book(TypedDict):\n    """A Book\n\n    Args:\n        book_id (int): The book id\n        title (str): The title\n        author (str): The author\n        published (datetime): The publication date\n    """\n    book_id: int\n    title: str\n    author: str\n    published: datetime\n```\n\nNote: the docstring will be used to provide documentation for swagger.\n\n### Creating the API\n\nNow we can build the API.\n\n```python\nfrom typing import Dict, List\n\nfrom bareasgi_rest import RestError\n\n\nBOOKS: Dict[int, Book] = {}\nNEXT_ID: int = 0\n\nasync def get_books() -> List[Book]:\n    """Get all the books.\n\n    This method gets all the books in the shop.\n\n    Returns:\n        List[Book]: All the books\n    """\n    return list(BOOKS.values())\n\n\nasync def get_book(book_id: int) -> Book:\n    """Get a book for a given id\n\n    Args:\n        book_id (int): The id of the book\n\n    Raises:\n        RestError: 404, when a book is not found\n\n    Returns:\n        Book: The book\n    """\n\n    if book_id not in BOOKS:\n        raise RestError(404, "Book not found")\n\n    return BOOKS[book_id]\n\n\nasync def create_book(\n        author: str,\n        title: str,\n        published: datetime\n) -> int:\n    """Add a book\n\n    Args:\n        author (str): The author\n        title (str): The title\n        published (datetime): The publication date\n\n    Returns:\n        int: The id of the new book\n    """\n    NEXT_ID += 1\n    BOOKS[NEXT_ID] = Book(\n        book_id=NEXT_ID,\n        title=title,\n        author=author,\n        published=published\n    )\n    return NEXT_ID\n\n\nasync def update_book(\n        book_id: int,\n        author: str,\n        title: str,\n        published: datetime\n) -> None:\n    """Update a book\n\n    Args:\n        book_id (int): The id of the book to update\n        author (str): The new author\n        title (str): The title\n        published (datetime): The publication date\n\n    Raises:\n        RestError: 404, when a book is not found\n    """\n    if book_id not in BOOKS:\n        raise RestError(404, "Book not found")\n    BOOKS[book_id][\'title\'] = title\n    BOOKS[book_id][\'author\'] = author\n    BOOKS[book_id][\'published\'] = published\n```\n\nWe can see that errors are handler by raising ResetError.\nA convention has been applied such that the status code MUST\nappear before the message, separated by a comma.\n\n### Adding support for the REST router\n\nNow we must create our application and add support for the router.\n\n```python\nfrom bareasgi import Application\nfrom bareasgi_rest import RestHttpRouter, add_swagger_ui\n\n\nrouter = RestHttpRouter(\n    None,\n    title="Books",\n    version="1",\n    description="A book api",\n    base_path=\'/api/1\',\n    tags=[\n        {\n            \'name\': \'Books\',\n            \'description\': \'The book store API\'\n        }\n    ]\n)\napp = Application(http_router=router)\nadd_swagger_ui(app)\n```\n\nNote the `base_path` argument can be used to prefix all\npaths.\n\nThe `RestHttpRouter` is a subclass of the basic router, so\nall those methods are also available.\n\n### Creating the routes\n\nNow we can create the routes:\n\n```python\ntags = [\'Books\']\nrouter.add_rest({\'GET\'}, \'/books\', get_books,tags=tags)\nrouter.add_rest({\'GET\'}, \'/books/{bookId:int}\', get_book, tags=tags)\nrouter.add_rest({\'POST\'}, \'/books\', create_book, tags=tags, status_code=201)\nrouter.add_rest({\'PUT\'}, \'/books/{bookId:int}\', update_book, tags=tags, status_code=204)\n```\n\nFirst we should note that the paths will be prefixed with the\n`base_path` provided to the router.\n\nReferring back to the implementation of `get_book` we can\nsee that the camel-case path variable `bookId` has been\nmapped to the snake-case `book_id` parameter. The JSON object provided in the body of the `create_book` will\nsimilarly map camel-cased properties to the snake-cased\nfunction parameters.\n\nWe can also see how the status codes have been overridden\nfor the `POST` and `PUT` endpoints, and all the routes\nhave the "Books" tag for grouping in the UI.\n\n### Serving the API\n\nFinally we can serve the API:\n\n```python\nimport uvicorn\n\nuvicorn.run(app, port=9009)\n```\n\nBrowsing to http://localhost/api/1/swagger we should see:\n\n![Top Level](screenshot1.png)\n\nWhen we expand `GET /books/{bookId}` we can see all the\ninformation provided in the docstring and typing has been\npassed through to the swagger UI.\n\n![GET /books/{bookId}](screenshot2.png)\n\n## Thanks\n\nThanks to [rr-](https://github.com/rr-) and contributors\nfor the excellent\n[docstring-parser](https://github.com/rr-/docstring_parser)\npackage.\n',
     'author': 'Rob Blackbourn',
     'author_email': 'rob.blackbourn@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/rob-blackbourn/bareASGI-rest',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `bareASGI-rest-4.0.0a1/PKG-INFO` & `bareASGI-rest-4.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,52 @@
 Metadata-Version: 2.1
 Name: bareasgi-rest
-Version: 4.0.0a1
+Version: 4.0.1
 Summary: REST support for bareASGI
 Home-page: https://github.com/rob-blackbourn/bareASGI-rest
 License: Apache-2.0
 Keywords: bareASGI,rest,swagger
 Author: Rob Blackbourn
 Author-email: rob.blackbourn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: bareasgi (>=4.0,<5.0)
+Requires-Dist: bareasgi (>=4.2,<5.0)
 Requires-Dist: bareasgi-jinja2 (>=4.0,<5.0)
-Requires-Dist: docstring-parser (>=0.6,<0.7)
-Requires-Dist: jetblack-serialization (>=3.0.0-alpha.2,<4.0.0)
-Requires-Dist: lxml (>=4.4.2,<5.0.0)
-Requires-Dist: stringcase (>=1.2.0,<2.0.0)
-Requires-Dist: typing-extensions (>=3.7,<4.0)
+Requires-Dist: docstring-parser (>=0.15,<0.16)
+Requires-Dist: jetblack-serialization (>=3.0.1,<4.0.0)
+Requires-Dist: lxml (>=4.9,<5.0)
+Requires-Dist: stringcase (>=1.2,<2.0)
+Requires-Dist: typing-extensions (>=4,<5)
+Requires-Dist: typing_inspect (>=0.8,<0.9)
 Project-URL: Repository, https://github.com/rob-blackbourn/bareASGI-rest
 Description-Content-Type: text/markdown
 
 # bareASGI-rest
 
 This package provides enhanced support for writing REST
 APIs with [bareASGI](https://bareasgi.com),
 (read the [docs](https://rob-blackbourn.github.io/bareASGI-rest/)).
 
 It includes:
 
 - A router to simplify the creation of REST APIs,
 - A swagger API endpoint
 
-This is a Python 3.7+ package, and is currently pre-release.
-
-## Branch
-
-This is the v3 maintenance branch.
+This is a Python 3.8+ package.
 
 ## Installation
 
-The package can be install from pypi.
-
-It is currently pre-release so you will need the --pre flag.
+The package can be installed from pypi.
 
 ```bash
-$ pip install --pre bareASGI-rest
+$ pip install bareASGI-rest
 ```
 
 An ASGI server will be required to run the code. The examples below use
 [uvicorn](https://www.uvicorn.org/).
 
 ```bash
 $ pip install uvicorn
@@ -65,20 +61,16 @@
 
 ### Creating typed dictionaries
 
 Here is the type of a book. We use `TypedDict` to allow automatic type discovery
 
 ```python
 from datetime import datetime
-try:
-    # Available in 3.8
-    from typing import TypedDict  # type:ignore
-except:
-    # Available in 3.7
-    from typing_extensions import TypedDict
+from typing import TypedDict
+
 
 class Book(TypedDict):
     """A Book
 
     Args:
         book_id (int): The book id
         title (str): The title
@@ -95,15 +87,16 @@
 
 ### Creating the API
 
 Now we can build the API.
 
 ```python
 from typing import Dict, List
-from urllib.error import HTTPError
+
+from bareasgi_rest import RestError
 
 
 BOOKS: Dict[int, Book] = {}
 NEXT_ID: int = 0
 
 async def get_books() -> List[Book]:
     """Get all the books.
@@ -119,22 +112,22 @@
 async def get_book(book_id: int) -> Book:
     """Get a book for a given id
 
     Args:
         book_id (int): The id of the book
 
     Raises:
-        HTTPError: 404, when a book is not found
+        RestError: 404, when a book is not found
 
     Returns:
         Book: The book
     """
 
     if book_id not in BOOKS:
-        raise HTTPError(None, 404, None, None, None)
+        raise RestError(404, "Book not found")
 
     return BOOKS[book_id]
 
 
 async def create_book(
         author: str,
         title: str,
@@ -171,25 +164,25 @@
     Args:
         book_id (int): The id of the book to update
         author (str): The new author
         title (str): The title
         published (datetime): The publication date
 
     Raises:
-        HTTPError: 404, when a book is not found
+        RestError: 404, when a book is not found
     """
     if book_id not in BOOKS:
-        raise HTTPError(None, 404, None, None, None)
+        raise RestError(404, "Book not found")
     BOOKS[book_id]['title'] = title
     BOOKS[book_id]['author'] = author
     BOOKS[book_id]['published'] = published
 ```
 
-We can see that errors are handler by raising HTTPError
-from the `urllib.errors` standard library package. A convention has been applied such that the status code MUST
+We can see that errors are handler by raising ResetError.
+A convention has been applied such that the status code MUST
 appear before the message, separated by a comma.
 
 ### Adding support for the REST router
 
 Now we must create our application and add support for the router.
 
 ```python
```

