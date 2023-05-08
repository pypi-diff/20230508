# Comparing `tmp/request_validator_galaxy-0.7.tar.gz` & `tmp/request_validator_galaxy-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "request_validator_galaxy-0.7.tar", last modified: Mon May  8 12:46:48 2023, max compression
+gzip compressed data, was "request_validator_galaxy-0.8.tar", last modified: Mon May  8 12:57:05 2023, max compression
```

## Comparing `request_validator_galaxy-0.7.tar` & `request_validator_galaxy-0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:46:48.867422 request_validator_galaxy-0.7/
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      171 2023-05-08 12:46:48.867422 request_validator_galaxy-0.7/PKG-INFO
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      566 2023-05-05 05:38:44.000000 request_validator_galaxy-0.7/README.rst
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      107 2023-05-08 12:46:48.867422 request_validator_galaxy-0.7/setup.cfg
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      375 2023-05-08 12:46:36.000000 request_validator_galaxy-0.7/setup.py
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:46:48.867422 request_validator_galaxy-0.7/src/
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:46:48.867422 request_validator_galaxy-0.7/src/request_validator_galaxy/
--rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2022-01-08 23:56:05.000000 request_validator_galaxy-0.7/src/request_validator_galaxy/__init__.py
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:46:48.867422 request_validator_galaxy-0.7/src/request_validator_galaxy/example/
--rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2022-01-08 23:56:05.000000 request_validator_galaxy-0.7/src/request_validator_galaxy/example/__init__.py
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:46:48.867422 request_validator_galaxy-0.7/src/request_validator_galaxy/example/common/
--rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:37:26.000000 request_validator_galaxy-0.7/src/request_validator_galaxy/example/common/__init__.py
--rw-rw-r--   0 gwl       (1000) gwl       (1000)       83 2023-05-08 12:39:40.000000 request_validator_galaxy-0.7/src/request_validator_galaxy/example/common/base.py
--rw-rw-r--   0 gwl       (1000) gwl       (1000)     4405 2023-05-08 12:34:04.000000 request_validator_galaxy-0.7/src/request_validator_galaxy/example/custom_sklearn.py
-drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:46:48.867422 request_validator_galaxy-0.7/src/request_validator_galaxy.egg-info/
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      171 2023-05-08 12:46:48.000000 request_validator_galaxy-0.7/src/request_validator_galaxy.egg-info/PKG-INFO
--rw-rw-r--   0 gwl       (1000) gwl       (1000)      490 2023-05-08 12:46:48.000000 request_validator_galaxy-0.7/src/request_validator_galaxy.egg-info/SOURCES.txt
--rw-rw-r--   0 gwl       (1000) gwl       (1000)        1 2023-05-08 12:46:48.000000 request_validator_galaxy-0.7/src/request_validator_galaxy.egg-info/dependency_links.txt
--rw-rw-r--   0 gwl       (1000) gwl       (1000)       25 2023-05-08 12:46:48.000000 request_validator_galaxy-0.7/src/request_validator_galaxy.egg-info/top_level.txt
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:57:05.100621 request_validator_galaxy-0.8/
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      171 2023-05-08 12:57:05.100621 request_validator_galaxy-0.8/PKG-INFO
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      782 2023-05-08 12:56:18.000000 request_validator_galaxy-0.8/README.rst
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:57:05.096621 request_validator_galaxy-0.8/pk_src/
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:57:05.096621 request_validator_galaxy-0.8/pk_src/request_validator_galaxy/
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2022-01-08 23:56:05.000000 request_validator_galaxy-0.8/pk_src/request_validator_galaxy/__init__.py
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:57:05.100621 request_validator_galaxy-0.8/pk_src/request_validator_galaxy/example/
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2022-01-08 23:56:05.000000 request_validator_galaxy-0.8/pk_src/request_validator_galaxy/example/__init__.py
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:57:05.100621 request_validator_galaxy-0.8/pk_src/request_validator_galaxy/example/common/
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:37:26.000000 request_validator_galaxy-0.8/pk_src/request_validator_galaxy/example/common/__init__.py
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)       83 2023-05-08 12:39:40.000000 request_validator_galaxy-0.8/pk_src/request_validator_galaxy/example/common/base.py
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)     4243 2023-05-08 12:49:05.000000 request_validator_galaxy-0.8/pk_src/request_validator_galaxy/example/custom_sklearn.py
+drwxrwxr-x   0 gwl       (1000) gwl       (1000)        0 2023-05-08 12:57:05.100621 request_validator_galaxy-0.8/pk_src/request_validator_galaxy.egg-info/
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      171 2023-05-08 12:57:05.000000 request_validator_galaxy-0.8/pk_src/request_validator_galaxy.egg-info/PKG-INFO
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      517 2023-05-08 12:57:05.000000 request_validator_galaxy-0.8/pk_src/request_validator_galaxy.egg-info/SOURCES.txt
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)        1 2023-05-08 12:57:05.000000 request_validator_galaxy-0.8/pk_src/request_validator_galaxy.egg-info/dependency_links.txt
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)       25 2023-05-08 12:57:05.000000 request_validator_galaxy-0.8/pk_src/request_validator_galaxy.egg-info/top_level.txt
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      107 2023-05-08 12:57:05.100621 request_validator_galaxy-0.8/setup.cfg
+-rw-rw-r--   0 gwl       (1000) gwl       (1000)      381 2023-05-08 12:56:39.000000 request_validator_galaxy-0.8/setup.py
```

### Comparing `request_validator_galaxy-0.7/src/request_validator_galaxy/example/custom_sklearn.py` & `request_validator_galaxy-0.8/pk_src/request_validator_galaxy/example/custom_sklearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,14 @@
     - validate_header(function): Validate the username header from the api
         request headers.
     - validate_arguments(param): Check for the arguments keys exist or not
         in api request.
 """
 
 from functools import wraps
-
-from flask import (
-    request,
-)
-
-# import constants as settings
-# from views.utility import (
-#     get_error_response,
-#     get_error_message_response
-# )
-
 def validate_headers(header_param, request_headers):
     """Check for the headers keys exist or not in api request.
 
     The validate_headers_list function is a decorator that checks if the
     required headers are present in the request. If any of them are
     missing, it returns an error response with status code 400 and error code
     EMPLOYEE_HEADER_VALIDATION_ERROR.
```

