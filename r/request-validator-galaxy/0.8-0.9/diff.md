# Comparing `tmp/request_validator_galaxy-0.8.tar.gz` & `tmp/request_validator_galaxy-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "request_validator_galaxy-0.8.tar", last modified: Mon May  8 12:57:05 2023, max compression
+gzip compressed data, was "request_validator_galaxy-0.9.tar", last modified: Mon May  8 13:24:49 2023, max compression
```

## Comparing `request_validator_galaxy-0.8.tar` & `request_validator_galaxy-0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:57:05.100621 request_validator_galaxy-0.8/
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      171 2023-05-08 12:57:05.100621 request_validator_galaxy-0.8/PKG-INFO
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      782 2023-05-08 12:56:18.000000 request_validator_galaxy-0.8/README.rst
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:57:05.096621 request_validator_galaxy-0.8/pk_src/
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:57:05.096621 request_validator_galaxy-0.8/pk_src/request_validator_galaxy/
--rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2022-01-08 23:56:05.000000 request_validator_galaxy-0.8/pk_src/request_validator_galaxy/__init__.py
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:57:05.100621 request_validator_galaxy-0.8/pk_src/request_validator_galaxy/example/
--rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2022-01-08 23:56:05.000000 request_validator_galaxy-0.8/pk_src/request_validator_galaxy/example/__init__.py
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:57:05.100621 request_validator_galaxy-0.8/pk_src/request_validator_galaxy/example/common/
--rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:37:26.000000 request_validator_galaxy-0.8/pk_src/request_validator_galaxy/example/common/__init__.py
--rw-rw-r--   0 gwl       (1000) gwl       (1000)       83 2023-05-08 12:39:40.000000 request_validator_galaxy-0.8/pk_src/request_validator_galaxy/example/common/base.py
--rw-rw-r--   0 gwl       (1000) gwl       (1000)     4243 2023-05-08 12:49:05.000000 request_validator_galaxy-0.8/pk_src/request_validator_galaxy/example/custom_sklearn.py
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:57:05.100621 request_validator_galaxy-0.8/pk_src/request_validator_galaxy.egg-info/
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      171 2023-05-08 12:57:05.000000 request_validator_galaxy-0.8/pk_src/request_validator_galaxy.egg-info/PKG-INFO
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      517 2023-05-08 12:57:05.000000 request_validator_galaxy-0.8/pk_src/request_validator_galaxy.egg-info/SOURCES.txt
--rw-rw-r--   0 gwl       (1000) gwl       (1000)        1 2023-05-08 12:57:05.000000 request_validator_galaxy-0.8/pk_src/request_validator_galaxy.egg-info/dependency_links.txt
--rw-rw-r--   0 gwl       (1000) gwl       (1000)       25 2023-05-08 12:57:05.000000 request_validator_galaxy-0.8/pk_src/request_validator_galaxy.egg-info/top_level.txt
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      107 2023-05-08 12:57:05.100621 request_validator_galaxy-0.8/setup.cfg
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      381 2023-05-08 12:56:39.000000 request_validator_galaxy-0.8/setup.py
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:24:49.057771 request_validator_galaxy-0.9/
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      171 2023-05-08 13:24:49.061771 request_validator_galaxy-0.9/PKG-INFO
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      782 2023-05-08 12:56:18.000000 request_validator_galaxy-0.9/README.rst
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:24:49.057771 request_validator_galaxy-0.9/pk_src/
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:24:49.057771 request_validator_galaxy-0.9/pk_src/request_validator_galaxy/
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2022-01-08 23:56:05.000000 request_validator_galaxy-0.9/pk_src/request_validator_galaxy/__init__.py
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:24:49.057771 request_validator_galaxy-0.9/pk_src/request_validator_galaxy/example/
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2022-01-08 23:56:05.000000 request_validator_galaxy-0.9/pk_src/request_validator_galaxy/example/__init__.py
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:24:49.057771 request_validator_galaxy-0.9/pk_src/request_validator_galaxy/example/common/
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:37:26.000000 request_validator_galaxy-0.9/pk_src/request_validator_galaxy/example/common/__init__.py
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)       83 2023-05-08 12:39:40.000000 request_validator_galaxy-0.9/pk_src/request_validator_galaxy/example/common/base.py
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)     4280 2023-05-08 13:23:27.000000 request_validator_galaxy-0.9/pk_src/request_validator_galaxy/example/custom_sklearn.py
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:24:49.057771 request_validator_galaxy-0.9/pk_src/request_validator_galaxy.egg-info/
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      171 2023-05-08 13:24:49.000000 request_validator_galaxy-0.9/pk_src/request_validator_galaxy.egg-info/PKG-INFO
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      517 2023-05-08 13:24:49.000000 request_validator_galaxy-0.9/pk_src/request_validator_galaxy.egg-info/SOURCES.txt
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)        1 2023-05-08 13:24:49.000000 request_validator_galaxy-0.9/pk_src/request_validator_galaxy.egg-info/dependency_links.txt
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)       25 2023-05-08 13:24:49.000000 request_validator_galaxy-0.9/pk_src/request_validator_galaxy.egg-info/top_level.txt
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      107 2023-05-08 13:24:49.061771 request_validator_galaxy-0.9/setup.cfg
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      381 2023-05-08 13:23:42.000000 request_validator_galaxy-0.9/setup.py
```

### Comparing `request_validator_galaxy-0.8/README.rst` & `request_validator_galaxy-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `request_validator_galaxy-0.8/pk_src/request_validator_galaxy/example/custom_sklearn.py` & `request_validator_galaxy-0.9/pk_src/request_validator_galaxy/example/custom_sklearn.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,17 @@
     - validate_header(function): Validate the username header from the api
         request headers.
     - validate_arguments(param): Check for the arguments keys exist or not
         in api request.
 """
 
 from functools import wraps
-def validate_headers(header_param, request_headers):
+from flask import request as req
+
+def validate_headers(header_param):
     """Check for the headers keys exist or not in api request.
 
     The validate_headers_list function is a decorator that checks if the
     required headers are present in the request. If any of them are
     missing, it returns an error response with status code 400 and error code
     EMPLOYEE_HEADER_VALIDATION_ERROR.
 
@@ -49,25 +51,25 @@
                 **kw (dict): Pass a variable number of keyword arguments to
                     the function.
 
             Returns:
                 The error_response if the header is not present or null.
             """
             for header_key in header_param:
-                if header_key not in request_headers or \
-                        not request_headers.get(header_key):
+                if header_key not in req.headers or \
+                        not req.headers.get(header_key):
                     return {"error" : "error"}
             return function(*args, **kw)
 
         return check_argument
 
     return decorator
 
 
-def validate_arguments(param, request_param):
+def validate_arguments(param):
     """Check for the arguments keys exist or not in api request.
 
     The validate_arguments function is a decorator that checks if the
     required parameters are present in the request. If not, it returns an
     error response with status code 400 and error code 1002.
 
     Args:
@@ -103,18 +105,18 @@
                 **kw (dict): Pass a variable number of keyword arguments to
                     the function.
 
             Returns:
                 function (func): The function if the required parameters
                     are present in the request.
             """
-            if "req_param" not in request_param:
+            if "req_param" not in req.get_json():
                 error_response = {"error": "error"}
                 return error_response
-
+            request_param = req.get_json()
             for json_key in param:
                 if json_key not in request_param["req_param"]:
                     error_response = {"error": "error"}
                     return error_response
             return function(*args, **kw)
 
         return check_argument
```

### Comparing `request_validator_galaxy-0.8/pk_src/request_validator_galaxy.egg-info/SOURCES.txt` & `request_validator_galaxy-0.9/pk_src/request_validator_galaxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

