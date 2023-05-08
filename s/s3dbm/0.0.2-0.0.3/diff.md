# Comparing `tmp/s3dbm-0.0.2.tar.gz` & `tmp/s3dbm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3dbm-0.0.2.tar", last modified: Sun May  7 22:43:00 2023, max compression
+gzip compressed data, was "s3dbm-0.0.3.tar", last modified: Mon May  8 01:41:04 2023, max compression
```

## Comparing `s3dbm-0.0.2.tar` & `s3dbm-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-07 22:43:00.427883 s3dbm-0.0.2/
--rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-05 20:34:52.000000 s3dbm-0.0.2/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-07 22:43:00.427883 s3dbm-0.0.2/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)       78 2023-05-07 22:33:06.000000 s3dbm-0.0.2/README.rst
--rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-06 23:57:50.000000 s3dbm-0.0.2/pyproject.toml
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-07 22:43:00.427883 s3dbm-0.0.2/s3dbm/
--rw-rw-r--   0 mike      (1000) mike      (1000)      111 2023-05-07 22:26:45.000000 s3dbm-0.0.2/s3dbm/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    12767 2023-05-07 22:31:35.000000 s3dbm-0.0.2/s3dbm/main.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-07 22:43:00.427883 s3dbm-0.0.2/s3dbm/tests/
--rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-06 23:57:50.000000 s3dbm-0.0.2/s3dbm/tests/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    13297 2023-05-07 22:42:24.000000 s3dbm-0.0.2/s3dbm/utils.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-07 22:43:00.427883 s3dbm-0.0.2/s3dbm.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-07 22:43:00.000000 s3dbm-0.0.2/s3dbm.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      267 2023-05-07 22:43:00.000000 s3dbm-0.0.2/s3dbm.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-07 22:43:00.000000 s3dbm-0.0.2/s3dbm.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       36 2023-05-07 22:43:00.000000 s3dbm-0.0.2/s3dbm.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        6 2023-05-07 22:43:00.000000 s3dbm-0.0.2/s3dbm.egg-info/top_level.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-07 22:43:00.431883 s3dbm-0.0.2/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     7162 2023-05-07 22:42:48.000000 s3dbm-0.0.2/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 01:41:04.517390 s3dbm-0.0.3/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-05 20:34:52.000000 s3dbm-0.0.3/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-08 01:41:04.517390 s3dbm-0.0.3/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)       78 2023-05-07 22:33:06.000000 s3dbm-0.0.3/README.rst
+-rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-06 23:57:50.000000 s3dbm-0.0.3/pyproject.toml
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 01:41:04.513390 s3dbm-0.0.3/s3dbm/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      111 2023-05-08 01:40:14.000000 s3dbm-0.0.3/s3dbm/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    12767 2023-05-08 01:40:08.000000 s3dbm-0.0.3/s3dbm/main.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 01:41:04.517390 s3dbm-0.0.3/s3dbm/tests/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-06 23:57:50.000000 s3dbm-0.0.3/s3dbm/tests/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    13297 2023-05-07 22:42:24.000000 s3dbm-0.0.3/s3dbm/utils.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 01:41:04.517390 s3dbm-0.0.3/s3dbm.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-08 01:41:04.000000 s3dbm-0.0.3/s3dbm.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      267 2023-05-08 01:41:04.000000 s3dbm-0.0.3/s3dbm.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-08 01:41:04.000000 s3dbm-0.0.3/s3dbm.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       36 2023-05-08 01:41:04.000000 s3dbm-0.0.3/s3dbm.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        6 2023-05-08 01:41:04.000000 s3dbm-0.0.3/s3dbm.egg-info/top_level.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-08 01:41:04.517390 s3dbm-0.0.3/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7162 2023-05-08 01:40:38.000000 s3dbm-0.0.3/setup.py
```

### Comparing `s3dbm-0.0.2/LICENSE` & `s3dbm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `s3dbm-0.0.2/PKG-INFO` & `s3dbm-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3dbm
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python dbm-style interface to S3
 Home-page: https://github.com/mullenkamp/s3dbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm s3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `s3dbm-0.0.2/s3dbm/main.py` & `s3dbm-0.0.3/s3dbm/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from . import utils
 
 #######################################################
 ### Classes
 
 
 
-class S3dbm(MutableMapping):
+class S3DBM(MutableMapping):
     """
 
     """
     def __init__(self, bucket: str, client: botocore.client.BaseClient=None, connection_config: utils.ConnectionConfig=None, public_url: HttpUrl=None, flag: str = "r", buffer_size: int=524288, retries: int=3, read_timeout: int=120, provider: str=None, threads: int=30, compression=True, cache: MutableMapping=None):
         """
 
         """
@@ -320,8 +320,8 @@
     +---------+-------------------------------------------+
     | ``'n'`` | Always create a new, empty database, open |
     |         | for reading and writing                   |
     +---------+-------------------------------------------+
 
     """
 
-    return S3dbm(bucket, client, connection_config, public_url, flag, buffer_size, retries, read_timeout, provider, threads, compression, cache)
+    return S3DBM(bucket, client, connection_config, public_url, flag, buffer_size, retries, read_timeout, provider, threads, compression, cache)
```

### Comparing `s3dbm-0.0.2/s3dbm/utils.py` & `s3dbm-0.0.3/s3dbm/utils.py`

 * *Files identical despite different names*

### Comparing `s3dbm-0.0.2/s3dbm.egg-info/PKG-INFO` & `s3dbm-0.0.3/s3dbm.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3dbm
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python dbm-style interface to S3
 Home-page: https://github.com/mullenkamp/s3dbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm s3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `s3dbm-0.0.2/setup.py` & `s3dbm-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # General parameters
 name = 's3dbm'
 main_package = 's3dbm'
-version = '0.0.2'
+version = '0.0.3'
 descrip = 'A python dbm-style interface to S3'
 
 # The below code is for readthedocs. To have sphinx/readthedocs interact with
 # the contained package, readthedocs needs to build the package. But the dependencies
 # should be installed via the conda yml env file rather than during the package build.
 if os.environ.get('READTHEDOCS', False) == 'True':
     INSTALL_REQUIRES = []
```

