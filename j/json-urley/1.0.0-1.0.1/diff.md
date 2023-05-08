# Comparing `tmp/json-urley-1.0.0.tar.gz` & `tmp/json-urley-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/json-urley-1.0.0.tar", last modified: Mon Dec 26 03:08:17 2022, max compression
+gzip compressed data, was "json-urley-1.0.1.tar", last modified: Mon May  8 04:50:07 2023, max compression
```

## Comparing `json-urley-1.0.0.tar` & `json-urley-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2022-12-26 03:08:17.967374 json-urley-1.0.0/
--rw-r--r--   0 tofarr     (501) staff       (20)     5249 2022-12-26 03:08:17.966985 json-urley-1.0.0/PKG-INFO
--rw-r--r--   0 tofarr     (501) staff       (20)     4824 2022-12-26 03:01:46.000000 json-urley-1.0.0/README.md
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2022-12-26 03:08:17.962160 json-urley-1.0.0/json_urley/
--rw-r--r--   0 tofarr     (501) staff       (20)     5501 2022-12-26 02:42:50.000000 json-urley-1.0.0/json_urley/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3491 2022-12-25 05:40:19.000000 json-urley-1.0.0/json_urley/_path_element.py
--rw-r--r--   0 tofarr     (501) staff       (20)       44 2022-12-23 19:13:52.000000 json-urley-1.0.0/json_urley/json_urley_error.py
--rw-r--r--   0 tofarr     (501) staff       (20)       22 2022-12-26 03:00:50.000000 json-urley-1.0.0/json_urley/version.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2022-12-26 03:08:17.966373 json-urley-1.0.0/json_urley.egg-info/
--rw-r--r--   0 tofarr     (501) staff       (20)     5249 2022-12-26 03:08:17.000000 json-urley-1.0.0/json_urley.egg-info/PKG-INFO
--rw-r--r--   0 tofarr     (501) staff       (20)      258 2022-12-26 03:08:17.000000 json-urley-1.0.0/json_urley.egg-info/SOURCES.txt
--rw-r--r--   0 tofarr     (501) staff       (20)        1 2022-12-26 03:08:17.000000 json-urley-1.0.0/json_urley.egg-info/dependency_links.txt
--rw-r--r--   0 tofarr     (501) staff       (20)       11 2022-12-26 03:08:17.000000 json-urley-1.0.0/json_urley.egg-info/top_level.txt
--rw-r--r--   0 tofarr     (501) staff       (20)       38 2022-12-26 03:08:17.967499 json-urley-1.0.0/setup.cfg
--rw-r--r--   0 tofarr     (501) staff       (20)      757 2022-12-26 03:01:00.000000 json-urley-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:50:07.197854 json-urley-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-08 04:49:54.000000 json-urley-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-08 04:50:07.197854 json-urley-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:50:07.197854 json-urley-1.0.1/json_urley/
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-05-08 04:49:54.000000 json-urley-1.0.1/json_urley/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-08 04:49:54.000000 json-urley-1.0.1/json_urley/_path_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-08 04:49:54.000000 json-urley-1.0.1/json_urley/json_urley_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:50:07.197854 json-urley-1.0.1/json_urley.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-08 04:50:07.000000 json-urley-1.0.1/json_urley.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-08 04:50:07.000000 json-urley-1.0.1/json_urley.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 04:50:07.000000 json-urley-1.0.1/json_urley.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-08 04:50:07.000000 json-urley-1.0.1/json_urley.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 04:50:07.000000 json-urley-1.0.1/json_urley.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 04:50:07.197854 json-urley-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-08 04:49:54.000000 json-urley-1.0.1/setup.py
```

### Comparing `json-urley-1.0.0/PKG-INFO` & `json-urley-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: json-urley
-Version: 1.0.0
+Version: 1.0.1
 Summary: A tight standard for converting json objects to and from URL parameters.
 Home-page: https://github.com/tofarr/json-urley
 Author: Tim O'Farrell
 Author-email: tofarr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 
 # JSON URLEY: A Tight Standard for Json / URL Parameter Conversion
 
 Json Urley provides a tight standard for converting json objects to and from URL parameters.
 
 ## Aims:
 
@@ -98,17 +100,21 @@
 could command a server to create a data structure to hold trillions of items from the command line? Gross! 
 
 ### Aren't nested arrays still difficult to read?
 
 Yes. Though the spec allows you to define data structures of any complexity, just because you can doesn't mean you 
 should!
 
-## Building The Project
-
-You need an account on pypi before this will work:
+## Installing local development dependencies
 
 ```
-pip install setuptools wheel
-python setup.py sdist bdist_wheel
-pip install twine
-python -m twine upload dist/*
+python setup.py install easy_install "json-urley[dev]"
 ```
+
+## Release Procedure
+
+![status](https://github.com/tofarr/json-urley/actions/workflows/quality.yml/badge.svg?branch=main)
+
+The typical process here is:
+* Create a PR with changes. Merge these to main (The `Quality` workflows make sure that your PR
+  meets the styling, linting, and code coverage standards).
+* New releases created in github are automatically uploaded to pypi
```

### Comparing `json-urley-1.0.0/README.md` & `json-urley-1.0.1/json_urley.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: json-urley
+Version: 1.0.1
+Summary: A tight standard for converting json objects to and from URL parameters.
+Home-page: https://github.com/tofarr/json-urley
+Author: Tim O'Farrell
+Author-email: tofarr@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
 # JSON URLEY: A Tight Standard for Json / URL Parameter Conversion
 
 Json Urley provides a tight standard for converting json objects to and from URL parameters.
 
 ## Aims:
 
 * The resulting URLs should be as readable as possible
@@ -86,17 +100,21 @@
 could command a server to create a data structure to hold trillions of items from the command line? Gross! 
 
 ### Aren't nested arrays still difficult to read?
 
 Yes. Though the spec allows you to define data structures of any complexity, just because you can doesn't mean you 
 should!
 
-## Building The Project
-
-You need an account on pypi before this will work:
+## Installing local development dependencies
 
 ```
-pip install setuptools wheel
-python setup.py sdist bdist_wheel
-pip install twine
-python -m twine upload dist/*
-```
+python setup.py install easy_install "json-urley[dev]"
+```
+
+## Release Procedure
+
+![status](https://github.com/tofarr/json-urley/actions/workflows/quality.yml/badge.svg?branch=main)
+
+The typical process here is:
+* Create a PR with changes. Merge these to main (The `Quality` workflows make sure that your PR
+  meets the styling, linting, and code coverage standards).
+* New releases created in github are automatically uploaded to pypi
```

### Comparing `json-urley-1.0.0/json_urley/_path_element.py` & `json-urley-1.0.1/json_urley/_path_element.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,104 +1,127 @@
+# pylint: disable=R0401
 from dataclasses import dataclass
 from typing import Optional, List
 
 from json_urley import JsonUrleyError
 
 
 @dataclass
 class PathElement:
     key: str
     type_hint: Optional[str] = None
 
     def get_typed_value(self, value: str):
         type_hint = self.type_hint
         if type_hint:
-            if type_hint == 's':
-                return value
-            elif type_hint == 'f':
-                try:
-                    return float(value)
-                except ValueError:
-                    raise JsonUrleyError('not_int:{value}')
-            elif type_hint == 'i':
-                try:
-                    return int(value)
-                except ValueError:
-                    raise JsonUrleyError('not_float:{value}')
-            elif type_hint == 'b':
-                value = value.lower()
-                if value in ('true', '1'):
-                    return True
-                elif value in ('false', '0'):
-                    return False
-                else:
-                    raise JsonUrleyError(f'not_boolean:{value}')
-            elif type_hint == 'n':
-                if value:
-                    raise JsonUrleyError(f'not_empty:{value}')
-                return None
-            elif type_hint == 'a':
-                if value:
-                    raise JsonUrleyError(f'not_empty:{value}')
-                return []
-            elif type_hint == 'o':
-                if value:
-                    raise JsonUrleyError(f'not_empty:{value}')
-                return {}
-            else:
-                raise JsonUrleyError(f'invalid_type_hint:{type_hint}')
-        else:
-            if value == 'null':
-                return None
-            elif value == 'true':
-                return True
-            elif value == 'false':
-                return False
-            try:
-                return int(value)
-            except ValueError:
-                pass
-            try:
-                return float(value)
-            except ValueError:
-                pass
-            return value
+            fn = _TYPE_HINTS.get(type_hint)
+            if not fn:
+                raise JsonUrleyError(f"invalid_type_hint:{type_hint}")
+            return fn(value)
+        return _get_typed_value(value)
 
 
 def parse_path(path: str) -> List[PathElement]:
     elements = []
     current_index = 0
     current_key = []
     while True:
-        next_tilda = _next_index_of(path, '~', current_index)
-        next_dot = _next_index_of(path, '.', current_index)
+        next_tilda = _next_index_of(path, "~", current_index)
+        next_dot = _next_index_of(path, ".", current_index)
         if next_tilda < next_dot:
-            if path[next_tilda + 1] in ('~', '.'):
+            if path[next_tilda + 1] in ("~", "."):
                 current_key.append(path[current_index:next_tilda])
                 current_key.append(path[next_tilda + 1])
                 current_index = next_tilda + 2
             else:
                 current_key.append(path[current_index:next_tilda])
-                elements.append(PathElement(
-                    key=''.join(current_key),
-                    type_hint=path[next_tilda + 1:next_dot]
-                ))
+                elements.append(
+                    PathElement(
+                        key="".join(current_key),
+                        type_hint=path[next_tilda + 1 : next_dot],
+                    )
+                )
                 current_key.clear()
                 current_index = next_dot + 1
         elif next_dot < next_tilda:
             current_key.append(path[current_index:next_dot])
-            elements.append(PathElement(''.join(current_key)))
+            elements.append(PathElement("".join(current_key)))
             current_key.clear()
             current_index = next_dot + 1
         else:
             if current_index < len(path):
                 current_key.append(path[current_index:])
             if current_key:
-                elements.append(PathElement(''.join(current_key)))
+                elements.append(PathElement("".join(current_key)))
             return elements
 
 
 def _next_index_of(path: str, sub: str, from_index: int):
     try:
         return path.index(sub, from_index)
     except ValueError:
         return len(path)
+
+
+def _s(value: str):
+    return value
+
+
+def _f(value: str):
+    try:
+        return float(value)
+    except ValueError as exc:
+        raise JsonUrleyError("not_float:{value}") from exc
+
+
+def _i(value: str):
+    try:
+        return int(value)
+    except ValueError as exc:
+        raise JsonUrleyError("not_int:{value}") from exc
+
+
+def _b(value: str):
+    value = value.lower()
+    if value in ("true", "1"):
+        return True
+    if value in ("false", "0"):
+        return False
+    raise JsonUrleyError(f"not_boolean:{value}")
+
+
+def _n(value: str):
+    if value:
+        raise JsonUrleyError(f"not_empty:{value}")
+
+
+def _a(value: str):
+    if value:
+        raise JsonUrleyError(f"not_empty:{value}")
+    return []
+
+
+def _o(value: str):
+    if value:
+        raise JsonUrleyError(f"not_empty:{value}")
+    return {}
+
+
+def _get_typed_value(value: str):
+    if value == "null":
+        return None
+    if value == "true":
+        return True
+    if value == "false":
+        return False
+    try:
+        return int(value)
+    except ValueError:
+        pass
+    try:
+        return float(value)
+    except ValueError:
+        pass
+    return value
+
+
+_TYPE_HINTS = {"s": _s, "f": _f, "i": _i, "b": _b, "n": _n, "a": _a, "o": _o}
```

