# Comparing `tmp/s3dbm-0.0.1.tar.gz` & `tmp/s3dbm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3dbm-0.0.1.tar", last modified: Sun May  7 22:33:17 2023, max compression
+gzip compressed data, was "s3dbm-0.0.2.tar", last modified: Sun May  7 22:43:00 2023, max compression
```

## Comparing `s3dbm-0.0.1.tar` & `s3dbm-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-07 22:33:17.777493 s3dbm-0.0.1/
--rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-05 20:34:52.000000 s3dbm-0.0.1/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-07 22:33:17.777493 s3dbm-0.0.1/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)       78 2023-05-07 22:33:06.000000 s3dbm-0.0.1/README.rst
--rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-06 23:57:50.000000 s3dbm-0.0.1/pyproject.toml
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-07 22:33:17.777493 s3dbm-0.0.1/s3dbm/
--rw-rw-r--   0 mike      (1000) mike      (1000)      111 2023-05-07 22:26:45.000000 s3dbm-0.0.1/s3dbm/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    12767 2023-05-07 22:31:35.000000 s3dbm-0.0.1/s3dbm/main.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-07 22:33:17.777493 s3dbm-0.0.1/s3dbm/tests/
--rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-06 23:57:50.000000 s3dbm-0.0.1/s3dbm/tests/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    13211 2023-05-07 22:22:11.000000 s3dbm-0.0.1/s3dbm/utils.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-07 22:33:17.777493 s3dbm-0.0.1/s3dbm.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-07 22:33:17.000000 s3dbm-0.0.1/s3dbm.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      267 2023-05-07 22:33:17.000000 s3dbm-0.0.1/s3dbm.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-07 22:33:17.000000 s3dbm-0.0.1/s3dbm.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       36 2023-05-07 22:33:17.000000 s3dbm-0.0.1/s3dbm.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        6 2023-05-07 22:33:17.000000 s3dbm-0.0.1/s3dbm.egg-info/top_level.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-07 22:33:17.777493 s3dbm-0.0.1/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     7162 2023-05-07 22:24:25.000000 s3dbm-0.0.1/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-07 22:43:00.427883 s3dbm-0.0.2/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-05 20:34:52.000000 s3dbm-0.0.2/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-07 22:43:00.427883 s3dbm-0.0.2/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)       78 2023-05-07 22:33:06.000000 s3dbm-0.0.2/README.rst
+-rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-06 23:57:50.000000 s3dbm-0.0.2/pyproject.toml
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-07 22:43:00.427883 s3dbm-0.0.2/s3dbm/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      111 2023-05-07 22:26:45.000000 s3dbm-0.0.2/s3dbm/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    12767 2023-05-07 22:31:35.000000 s3dbm-0.0.2/s3dbm/main.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-07 22:43:00.427883 s3dbm-0.0.2/s3dbm/tests/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-06 23:57:50.000000 s3dbm-0.0.2/s3dbm/tests/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    13297 2023-05-07 22:42:24.000000 s3dbm-0.0.2/s3dbm/utils.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-07 22:43:00.427883 s3dbm-0.0.2/s3dbm.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-07 22:43:00.000000 s3dbm-0.0.2/s3dbm.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      267 2023-05-07 22:43:00.000000 s3dbm-0.0.2/s3dbm.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-07 22:43:00.000000 s3dbm-0.0.2/s3dbm.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       36 2023-05-07 22:43:00.000000 s3dbm-0.0.2/s3dbm.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        6 2023-05-07 22:43:00.000000 s3dbm-0.0.2/s3dbm.egg-info/top_level.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-07 22:43:00.431883 s3dbm-0.0.2/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7162 2023-05-07 22:42:48.000000 s3dbm-0.0.2/setup.py
```

### Comparing `s3dbm-0.0.1/LICENSE` & `s3dbm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `s3dbm-0.0.1/PKG-INFO` & `s3dbm-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3dbm
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python dbm-style interface to S3
 Home-page: https://github.com/mullenkamp/s3dbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm s3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `s3dbm-0.0.1/s3dbm/main.py` & `s3dbm-0.0.2/s3dbm/main.py`

 * *Files identical despite different names*

### Comparing `s3dbm-0.0.1/s3dbm/utils.py` & `s3dbm-0.0.2/s3dbm/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,22 +239,24 @@
     if cache is not None:
         if '_chunk_size' in cache:
             buffer_size = cache._chunk_size
         try:
             file_obj = cache[obj_key]
         except:
             file_obj = get_object_s3(obj_key, bucket, s3, public_url, buffer_size, read_timeout, provider)
-            cache[obj_key] = file_obj
-            file_obj = cache[obj_key]
+            if file_obj is not None:
+                cache[obj_key] = file_obj
+                file_obj = cache[obj_key]
     else:
         file_obj = get_object_s3(obj_key, bucket, s3, public_url, buffer_size, read_timeout, provider)
 
-    if compression:
-        if obj_key.endswith('.zstd') or obj_key.endswith('.zst'):
-            file_obj = zstd_stream_reader(file_obj, buffer_size)
+    if file_obj is not None:
+        if compression:
+            if obj_key.endswith('.zstd') or obj_key.endswith('.zst'):
+                file_obj = zstd_stream_reader(file_obj, buffer_size)
 
     return file_obj
 
 
 def put_object_s3(s3: botocore.client.BaseClient, bucket: str, obj_key: str, file_obj: io.BufferedIOBase, buffer_size: int=524288, compression=True):
     """
     Function to upload data to an S3 bucket. This function will iteratively write the input file_obj in chunks ensuring that little memory is needed writing the object.
```

### Comparing `s3dbm-0.0.1/s3dbm.egg-info/PKG-INFO` & `s3dbm-0.0.2/s3dbm.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3dbm
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python dbm-style interface to S3
 Home-page: https://github.com/mullenkamp/s3dbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm s3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `s3dbm-0.0.1/setup.py` & `s3dbm-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # General parameters
 name = 's3dbm'
 main_package = 's3dbm'
-version = '0.0.1'
+version = '0.0.2'
 descrip = 'A python dbm-style interface to S3'
 
 # The below code is for readthedocs. To have sphinx/readthedocs interact with
 # the contained package, readthedocs needs to build the package. But the dependencies
 # should be installed via the conda yml env file rather than during the package build.
 if os.environ.get('READTHEDOCS', False) == 'True':
     INSTALL_REQUIRES = []
```

