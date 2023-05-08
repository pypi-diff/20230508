# Comparing `tmp/request_validator_galaxy-1.3.tar.gz` & `tmp/request_validator_galaxy-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "request_validator_galaxy-1.3.tar", last modified: Mon May  8 13:59:27 2023, max compression
+gzip compressed data, was "request_validator_galaxy-1.4.tar", last modified: Mon May  8 14:02:13 2023, max compression
```

## Comparing `request_validator_galaxy-1.3.tar` & `request_validator_galaxy-1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:59:27.801827 request_validator_galaxy-1.3/
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      171 2023-05-08 13:59:27.801827 request_validator_galaxy-1.3/PKG-INFO
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      782 2023-05-08 12:56:18.000000 request_validator_galaxy-1.3/README.rst
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:59:27.801827 request_validator_galaxy-1.3/pk_src/
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:59:27.801827 request_validator_galaxy-1.3/pk_src/request_validator_galaxy/
--rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2022-01-08 23:56:05.000000 request_validator_galaxy-1.3/pk_src/request_validator_galaxy/__init__.py
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:59:27.801827 request_validator_galaxy-1.3/pk_src/request_validator_galaxy/example/
--rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2022-01-08 23:56:05.000000 request_validator_galaxy-1.3/pk_src/request_validator_galaxy/example/__init__.py
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:59:27.801827 request_validator_galaxy-1.3/pk_src/request_validator_galaxy/example/common/
--rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:37:26.000000 request_validator_galaxy-1.3/pk_src/request_validator_galaxy/example/common/__init__.py
--rw-rw-r--   0 gwl       (1000) gwl       (1000)       83 2023-05-08 12:39:40.000000 request_validator_galaxy-1.3/pk_src/request_validator_galaxy/example/common/base.py
--rw-rw-r--   0 gwl       (1000) gwl       (1000)     4432 2023-05-08 13:59:02.000000 request_validator_galaxy-1.3/pk_src/request_validator_galaxy/example/custom_sklearn.py
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 13:59:27.801827 request_validator_galaxy-1.3/pk_src/request_validator_galaxy.egg-info/
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      171 2023-05-08 13:59:27.000000 request_validator_galaxy-1.3/pk_src/request_validator_galaxy.egg-info/PKG-INFO
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      571 2023-05-08 13:59:27.000000 request_validator_galaxy-1.3/pk_src/request_validator_galaxy.egg-info/SOURCES.txt
--rw-rw-r--   0 gwl       (1000) gwl       (1000)        1 2023-05-08 13:59:27.000000 request_validator_galaxy-1.3/pk_src/request_validator_galaxy.egg-info/dependency_links.txt
--rw-rw-r--   0 gwl       (1000) gwl       (1000)        6 2023-05-08 13:59:27.000000 request_validator_galaxy-1.3/pk_src/request_validator_galaxy.egg-info/requires.txt
--rw-rw-r--   0 gwl       (1000) gwl       (1000)       25 2023-05-08 13:59:27.000000 request_validator_galaxy-1.3/pk_src/request_validator_galaxy.egg-info/top_level.txt
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      107 2023-05-08 13:59:27.801827 request_validator_galaxy-1.3/setup.cfg
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      372 2023-05-08 13:59:24.000000 request_validator_galaxy-1.3/setup.py
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 14:02:13.289042 request_validator_galaxy-1.4/
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      171 2023-05-08 14:02:13.289042 request_validator_galaxy-1.4/PKG-INFO
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      782 2023-05-08 12:56:18.000000 request_validator_galaxy-1.4/README.rst
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 14:02:13.285041 request_validator_galaxy-1.4/pk_src/
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 14:02:13.285041 request_validator_galaxy-1.4/pk_src/request_validator_galaxy/
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2022-01-08 23:56:05.000000 request_validator_galaxy-1.4/pk_src/request_validator_galaxy/__init__.py
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 14:02:13.289042 request_validator_galaxy-1.4/pk_src/request_validator_galaxy/example/
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2022-01-08 23:56:05.000000 request_validator_galaxy-1.4/pk_src/request_validator_galaxy/example/__init__.py
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 14:02:13.289042 request_validator_galaxy-1.4/pk_src/request_validator_galaxy/example/common/
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:37:26.000000 request_validator_galaxy-1.4/pk_src/request_validator_galaxy/example/common/__init__.py
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)       83 2023-05-08 12:39:40.000000 request_validator_galaxy-1.4/pk_src/request_validator_galaxy/example/common/base.py
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)     4305 2023-05-08 14:01:47.000000 request_validator_galaxy-1.4/pk_src/request_validator_galaxy/example/custom_sklearn.py
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 14:02:13.285041 request_validator_galaxy-1.4/pk_src/request_validator_galaxy.egg-info/
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      171 2023-05-08 14:02:13.000000 request_validator_galaxy-1.4/pk_src/request_validator_galaxy.egg-info/PKG-INFO
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      571 2023-05-08 14:02:13.000000 request_validator_galaxy-1.4/pk_src/request_validator_galaxy.egg-info/SOURCES.txt
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)        1 2023-05-08 14:02:13.000000 request_validator_galaxy-1.4/pk_src/request_validator_galaxy.egg-info/dependency_links.txt
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)        6 2023-05-08 14:02:13.000000 request_validator_galaxy-1.4/pk_src/request_validator_galaxy.egg-info/requires.txt
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)       25 2023-05-08 14:02:13.000000 request_validator_galaxy-1.4/pk_src/request_validator_galaxy.egg-info/top_level.txt
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      107 2023-05-08 14:02:13.289042 request_validator_galaxy-1.4/setup.cfg
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      372 2023-05-08 14:02:00.000000 request_validator_galaxy-1.4/setup.py
```

### Comparing `request_validator_galaxy-1.3/README.rst` & `request_validator_galaxy-1.4/README.rst`

 * *Files identical despite different names*

### Comparing `request_validator_galaxy-1.3/pk_src/request_validator_galaxy/example/custom_sklearn.py` & `request_validator_galaxy-1.4/pk_src/request_validator_galaxy/example/custom_sklearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,15 @@
                     list to the function.
                 **kw (dict): Pass a variable number of keyword arguments to
                     the function.
 
             Returns:
                 The error_response if the header is not present or null.
             """
-            print(req.headers)
-            headers = {"name":"preetam"}
+            headers = req.headers
             for header_key in header_param:
                 if header_key not in headers or \
                         not headers.get(header_key):
                     return {"error" : "error"}
             return function(*args, **kw)
 
         return check_argument
@@ -107,19 +106,15 @@
                 **kw (dict): Pass a variable number of keyword arguments to
                     the function.
 
             Returns:
                 function (func): The function if the required parameters
                     are present in the request.
             """
-            request_param = {
-                "req_param": {
-                    "names": "preetam"
-                }
-            }
+            request_param = req.get_json()
             if "req_param" not in request_param:
                 error_response = {"error": "error"}
                 return error_response
             for json_key in param:
                 if json_key not in request_param["req_param"]:
                     error_response = {"error": "error"}
                     return error_response
```

### Comparing `request_validator_galaxy-1.3/pk_src/request_validator_galaxy.egg-info/SOURCES.txt` & `request_validator_galaxy-1.4/pk_src/request_validator_galaxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

