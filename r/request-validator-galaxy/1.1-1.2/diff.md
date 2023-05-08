# Comparing `tmp/request_validator_galaxy-1.1.tar.gz` & `tmp/request_validator_galaxy-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "request_validator_galaxy-1.1.tar", last modified: Mon May  8 13:39:58 2023, max compression
+gzip compressed data, was "request_validator_galaxy-1.2.tar", last modified: Mon May  8 13:48:47 2023, max compression
```

## Comparing `request_validator_galaxy-1.1.tar` & `request_validator_galaxy-1.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:39:58.151530 request_validator_galaxy-1.1/
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      171 2023-05-08 13:39:58.151530 request_validator_galaxy-1.1/PKG-INFO
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      782 2023-05-08 12:56:18.000000 request_validator_galaxy-1.1/README.rst
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:39:58.151530 request_validator_galaxy-1.1/pk_src/
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:39:58.151530 request_validator_galaxy-1.1/pk_src/request_validator_galaxy/
--rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2022-01-08 23:56:05.000000 request_validator_galaxy-1.1/pk_src/request_validator_galaxy/__init__.py
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:39:58.151530 request_validator_galaxy-1.1/pk_src/request_validator_galaxy/example/
--rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2022-01-08 23:56:05.000000 request_validator_galaxy-1.1/pk_src/request_validator_galaxy/example/__init__.py
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:39:58.151530 request_validator_galaxy-1.1/pk_src/request_validator_galaxy/example/common/
--rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:37:26.000000 request_validator_galaxy-1.1/pk_src/request_validator_galaxy/example/common/__init__.py
--rw-rw-r--   0 gwl       (1000) gwl       (1000)       83 2023-05-08 12:39:40.000000 request_validator_galaxy-1.1/pk_src/request_validator_galaxy/example/common/base.py
--rw-rw-r--   0 gwl       (1000) gwl       (1000)     4280 2023-05-08 13:23:27.000000 request_validator_galaxy-1.1/pk_src/request_validator_galaxy/example/custom_sklearn.py
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:39:58.151530 request_validator_galaxy-1.1/pk_src/request_validator_galaxy.egg-info/
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      171 2023-05-08 13:39:58.000000 request_validator_galaxy-1.1/pk_src/request_validator_galaxy.egg-info/PKG-INFO
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      571 2023-05-08 13:39:58.000000 request_validator_galaxy-1.1/pk_src/request_validator_galaxy.egg-info/SOURCES.txt
--rw-rw-r--   0 gwl       (1000) gwl       (1000)        1 2023-05-08 13:39:58.000000 request_validator_galaxy-1.1/pk_src/request_validator_galaxy.egg-info/dependency_links.txt
--rw-rw-r--   0 gwl       (1000) gwl       (1000)        6 2023-05-08 13:39:58.000000 request_validator_galaxy-1.1/pk_src/request_validator_galaxy.egg-info/requires.txt
--rw-rw-r--   0 gwl       (1000) gwl       (1000)       25 2023-05-08 13:39:58.000000 request_validator_galaxy-1.1/pk_src/request_validator_galaxy.egg-info/top_level.txt
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      107 2023-05-08 13:39:58.151530 request_validator_galaxy-1.1/setup.cfg
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      372 2023-05-08 13:39:46.000000 request_validator_galaxy-1.1/setup.py
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:48:47.548102 request_validator_galaxy-1.2/
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      171 2023-05-08 13:48:47.548102 request_validator_galaxy-1.2/PKG-INFO
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      782 2023-05-08 12:56:18.000000 request_validator_galaxy-1.2/README.rst
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:48:47.544102 request_validator_galaxy-1.2/pk_src/
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:48:47.548102 request_validator_galaxy-1.2/pk_src/request_validator_galaxy/
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2022-01-08 23:56:05.000000 request_validator_galaxy-1.2/pk_src/request_validator_galaxy/__init__.py
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:48:47.548102 request_validator_galaxy-1.2/pk_src/request_validator_galaxy/example/
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2022-01-08 23:56:05.000000 request_validator_galaxy-1.2/pk_src/request_validator_galaxy/example/__init__.py
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:48:47.548102 request_validator_galaxy-1.2/pk_src/request_validator_galaxy/example/common/
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:37:26.000000 request_validator_galaxy-1.2/pk_src/request_validator_galaxy/example/common/__init__.py
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)       83 2023-05-08 12:39:40.000000 request_validator_galaxy-1.2/pk_src/request_validator_galaxy/example/common/base.py
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)     4401 2023-05-08 13:48:34.000000 request_validator_galaxy-1.2/pk_src/request_validator_galaxy/example/custom_sklearn.py
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:48:47.548102 request_validator_galaxy-1.2/pk_src/request_validator_galaxy.egg-info/
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      171 2023-05-08 13:48:47.000000 request_validator_galaxy-1.2/pk_src/request_validator_galaxy.egg-info/PKG-INFO
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      517 2023-05-08 13:48:47.000000 request_validator_galaxy-1.2/pk_src/request_validator_galaxy.egg-info/SOURCES.txt
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)        1 2023-05-08 13:48:47.000000 request_validator_galaxy-1.2/pk_src/request_validator_galaxy.egg-info/dependency_links.txt
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)       25 2023-05-08 13:48:47.000000 request_validator_galaxy-1.2/pk_src/request_validator_galaxy.egg-info/top_level.txt
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      107 2023-05-08 13:48:47.548102 request_validator_galaxy-1.2/setup.cfg
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      374 2023-05-08 13:48:45.000000 request_validator_galaxy-1.2/setup.py
```

### Comparing `request_validator_galaxy-1.1/README.rst` & `request_validator_galaxy-1.2/README.rst`

 * *Files identical despite different names*

### Comparing `request_validator_galaxy-1.1/pk_src/request_validator_galaxy/example/custom_sklearn.py` & `request_validator_galaxy-1.2/pk_src/request_validator_galaxy/example/custom_sklearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,18 @@
                     list to the function.
                 **kw (dict): Pass a variable number of keyword arguments to
                     the function.
 
             Returns:
                 The error_response if the header is not present or null.
             """
+            headers = {"name":"preetam"}
             for header_key in header_param:
-                if header_key not in req.headers or \
-                        not req.headers.get(header_key):
+                if header_key not in headers or \
+                        not headers.get(header_key):
                     return {"error" : "error"}
             return function(*args, **kw)
 
         return check_argument
 
     return decorator
 
@@ -105,18 +106,22 @@
                 **kw (dict): Pass a variable number of keyword arguments to
                     the function.
 
             Returns:
                 function (func): The function if the required parameters
                     are present in the request.
             """
-            if "req_param" not in req.get_json():
+            request_param = {
+                "req_param": {
+                    "names": "preetam"
+                }
+            }
+            if "req_param" not in request_param:
                 error_response = {"error": "error"}
                 return error_response
-            request_param = req.get_json()
             for json_key in param:
                 if json_key not in request_param["req_param"]:
                     error_response = {"error": "error"}
                     return error_response
             return function(*args, **kw)
 
         return check_argument
```

### Comparing `request_validator_galaxy-1.1/pk_src/request_validator_galaxy.egg-info/SOURCES.txt` & `request_validator_galaxy-1.2/pk_src/request_validator_galaxy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 README.rst
 setup.cfg
 setup.py
 pk_src/request_validator_galaxy/__init__.py
 pk_src/request_validator_galaxy.egg-info/PKG-INFO
 pk_src/request_validator_galaxy.egg-info/SOURCES.txt
 pk_src/request_validator_galaxy.egg-info/dependency_links.txt
-pk_src/request_validator_galaxy.egg-info/requires.txt
 pk_src/request_validator_galaxy.egg-info/top_level.txt
 pk_src/request_validator_galaxy/example/__init__.py
 pk_src/request_validator_galaxy/example/custom_sklearn.py
 pk_src/request_validator_galaxy/example/common/__init__.py
 pk_src/request_validator_galaxy/example/common/base.py
```

