# Comparing `tmp/dh_facebook_client-0.2.1.tar.gz` & `tmp/dh_facebook_client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dh_facebook_client-0.2.1.tar", max compression
+gzip compressed data, was "dh_facebook_client-0.2.2.tar", max compression
```

## Comparing `dh_facebook_client-0.2.1.tar` & `dh_facebook_client-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1086 2023-05-03 19:25:20.013300 dh_facebook_client-0.2.1/dh_facebook_client/__init__.py
--rw-r--r--   0        0        0    11071 2023-05-03 19:25:20.013488 dh_facebook_client-0.2.1/dh_facebook_client/client.py
--rw-r--r--   0        0        0      260 2023-05-04 15:33:07.172663 dh_facebook_client-0.2.1/dh_facebook_client/constants.py
--rw-r--r--   0        0        0     5353 2023-05-03 19:25:20.013782 dh_facebook_client-0.2.1/dh_facebook_client/dataclasses.py
--rw-r--r--   0        0        0      521 2023-05-03 19:25:20.013909 dh_facebook_client-0.2.1/dh_facebook_client/error_code.py
--rw-r--r--   0        0        0     4502 2023-05-03 19:25:20.014061 dh_facebook_client-0.2.1/dh_facebook_client/exceptions.py
--rw-r--r--   0        0        0     2902 2023-05-04 15:33:14.240260 dh_facebook_client-0.2.1/dh_facebook_client/helpers.py
--rw-r--r--   0        0        0     1049 2023-05-03 19:25:20.014307 dh_facebook_client-0.2.1/dh_facebook_client/page_client.py
--rw-r--r--   0        0        0      435 2023-05-03 19:25:20.014436 dh_facebook_client-0.2.1/dh_facebook_client/typings.py
--rw-r--r--   0        0        0     1894 2023-05-03 19:25:20.014566 dh_facebook_client-0.2.1/dh_facebook_client/user_client.py
--rw-r--r--   0        0        0      651 2023-05-04 15:33:18.662056 dh_facebook_client-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 dh_facebook_client-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-05-03 19:25:20.013300 dh_facebook_client-0.2.2/dh_facebook_client/__init__.py
+-rw-r--r--   0        0        0    11071 2023-05-03 19:25:20.013488 dh_facebook_client-0.2.2/dh_facebook_client/client.py
+-rw-r--r--   0        0        0      260 2023-05-04 15:33:07.172663 dh_facebook_client-0.2.2/dh_facebook_client/constants.py
+-rw-r--r--   0        0        0     5353 2023-05-03 19:25:20.013782 dh_facebook_client-0.2.2/dh_facebook_client/dataclasses.py
+-rw-r--r--   0        0        0      521 2023-05-03 19:25:20.013909 dh_facebook_client-0.2.2/dh_facebook_client/error_code.py
+-rw-r--r--   0        0        0     4502 2023-05-03 19:25:20.014061 dh_facebook_client-0.2.2/dh_facebook_client/exceptions.py
+-rw-r--r--   0        0        0     2903 2023-05-08 15:18:15.116678 dh_facebook_client-0.2.2/dh_facebook_client/helpers.py
+-rw-r--r--   0        0        0     1049 2023-05-03 19:25:20.014307 dh_facebook_client-0.2.2/dh_facebook_client/page_client.py
+-rw-r--r--   0        0        0      435 2023-05-03 19:25:20.014436 dh_facebook_client-0.2.2/dh_facebook_client/typings.py
+-rw-r--r--   0        0        0     1894 2023-05-03 19:25:20.014566 dh_facebook_client-0.2.2/dh_facebook_client/user_client.py
+-rw-r--r--   0        0        0      651 2023-05-08 15:18:15.117219 dh_facebook_client-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 dh_facebook_client-0.2.2/PKG-INFO
```

### Comparing `dh_facebook_client-0.2.1/dh_facebook_client/__init__.py` & `dh_facebook_client-0.2.2/dh_facebook_client/__init__.py`

 * *Files identical despite different names*

### Comparing `dh_facebook_client-0.2.1/dh_facebook_client/client.py` & `dh_facebook_client-0.2.2/dh_facebook_client/client.py`

 * *Files identical despite different names*

### Comparing `dh_facebook_client-0.2.1/dh_facebook_client/dataclasses.py` & `dh_facebook_client-0.2.2/dh_facebook_client/dataclasses.py`

 * *Files identical despite different names*

### Comparing `dh_facebook_client-0.2.1/dh_facebook_client/error_code.py` & `dh_facebook_client-0.2.2/dh_facebook_client/error_code.py`

 * *Files identical despite different names*

### Comparing `dh_facebook_client-0.2.1/dh_facebook_client/exceptions.py` & `dh_facebook_client-0.2.2/dh_facebook_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `dh_facebook_client-0.2.1/dh_facebook_client/helpers.py` & `dh_facebook_client-0.2.2/dh_facebook_client/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Any, Callable, Iterable, Optional, Final
+from typing import Any, Callable, Final, Iterable, Optional
 
 from typing_extensions import NotRequired, TypedDict
 
 # TODO: Recursive type hints not yet available in mypy,
 #  should change sub_fields hint to Optional[List[FieldConfig]] when possible:
 #  https://github.com/python/mypy/issues/731
 FieldConfig = TypedDict(
@@ -31,15 +31,15 @@
     https://developers.facebook.com/docs/graph-api/field-expansion
     :param fields_config: The field configurations you want contained in string format
     :return: A formatted fields string
     """
     fields_str = ''
     for config in fields_config:
         # Prep the base sub string for a field w/ params (i.e. foo.limit(5).after(BAR))
-        fields_str = f'{config["field_name"]}'
+        fields_str += f'{config["field_name"]}'
         for param_name in ACCEPTED_SUB_PARAM_NAMES:
             fields_str += _format_sub_parameter_str(config, param_name)
         # If sub-fields exist, prep the nested sub-field(s) strings
         sub_fields = config.get('sub_fields')
         if sub_fields:
             fields_str += f'{{{format_fields_str(sub_fields)}}}'
```

### Comparing `dh_facebook_client-0.2.1/dh_facebook_client/page_client.py` & `dh_facebook_client-0.2.2/dh_facebook_client/page_client.py`

 * *Files identical despite different names*

### Comparing `dh_facebook_client-0.2.1/dh_facebook_client/user_client.py` & `dh_facebook_client-0.2.2/dh_facebook_client/user_client.py`

 * *Files identical despite different names*

### Comparing `dh_facebook_client-0.2.1/pyproject.toml` & `dh_facebook_client-0.2.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dh-facebook-client"
-version = "0.2.1"
+version = "0.2.2"
 description = "Simple client for interacting with the Facebook Graph API"
 authors = ["pchisholm <chisholm.p@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.26.0"
 backoff = "^1.11.1"
```

