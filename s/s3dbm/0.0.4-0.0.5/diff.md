# Comparing `tmp/s3dbm-0.0.4.tar.gz` & `tmp/s3dbm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3dbm-0.0.4.tar", last modified: Mon May  8 06:27:57 2023, max compression
+gzip compressed data, was "s3dbm-0.0.5.tar", last modified: Mon May  8 08:23:55 2023, max compression
```

## Comparing `s3dbm-0.0.4.tar` & `s3dbm-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 06:27:57.959893 s3dbm-0.0.4/
--rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-05 20:34:52.000000 s3dbm-0.0.4/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-08 06:27:57.959893 s3dbm-0.0.4/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)       78 2023-05-07 22:33:06.000000 s3dbm-0.0.4/README.rst
--rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-06 23:57:50.000000 s3dbm-0.0.4/pyproject.toml
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 06:27:57.959893 s3dbm-0.0.4/s3dbm/
--rw-rw-r--   0 mike      (1000) mike      (1000)      111 2023-05-08 01:40:14.000000 s3dbm-0.0.4/s3dbm/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    12767 2023-05-08 01:40:08.000000 s3dbm-0.0.4/s3dbm/main.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 06:27:57.959893 s3dbm-0.0.4/s3dbm/tests/
--rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-06 23:57:50.000000 s3dbm-0.0.4/s3dbm/tests/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    13753 2023-05-08 06:16:26.000000 s3dbm-0.0.4/s3dbm/utils.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 06:27:57.959893 s3dbm-0.0.4/s3dbm.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-08 06:27:57.000000 s3dbm-0.0.4/s3dbm.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      267 2023-05-08 06:27:57.000000 s3dbm-0.0.4/s3dbm.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-08 06:27:57.000000 s3dbm-0.0.4/s3dbm.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       36 2023-05-08 06:27:57.000000 s3dbm-0.0.4/s3dbm.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        6 2023-05-08 06:27:57.000000 s3dbm-0.0.4/s3dbm.egg-info/top_level.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-08 06:27:57.959893 s3dbm-0.0.4/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     7162 2023-05-08 06:24:12.000000 s3dbm-0.0.4/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 08:23:55.567186 s3dbm-0.0.5/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-05 20:34:52.000000 s3dbm-0.0.5/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-08 08:23:55.567186 s3dbm-0.0.5/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)       78 2023-05-07 22:33:06.000000 s3dbm-0.0.5/README.rst
+-rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-06 23:57:50.000000 s3dbm-0.0.5/pyproject.toml
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 08:23:55.567186 s3dbm-0.0.5/s3dbm/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      111 2023-05-08 01:40:14.000000 s3dbm-0.0.5/s3dbm/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    12767 2023-05-08 01:40:08.000000 s3dbm-0.0.5/s3dbm/main.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 08:23:55.567186 s3dbm-0.0.5/s3dbm/tests/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-06 23:57:50.000000 s3dbm-0.0.5/s3dbm/tests/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    13755 2023-05-08 08:23:10.000000 s3dbm-0.0.5/s3dbm/utils.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 08:23:55.567186 s3dbm-0.0.5/s3dbm.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-08 08:23:55.000000 s3dbm-0.0.5/s3dbm.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      267 2023-05-08 08:23:55.000000 s3dbm-0.0.5/s3dbm.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-08 08:23:55.000000 s3dbm-0.0.5/s3dbm.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       36 2023-05-08 08:23:55.000000 s3dbm-0.0.5/s3dbm.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        6 2023-05-08 08:23:55.000000 s3dbm-0.0.5/s3dbm.egg-info/top_level.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-08 08:23:55.567186 s3dbm-0.0.5/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7162 2023-05-08 08:23:36.000000 s3dbm-0.0.5/setup.py
```

### Comparing `s3dbm-0.0.4/LICENSE` & `s3dbm-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `s3dbm-0.0.4/PKG-INFO` & `s3dbm-0.0.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3dbm
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python dbm-style interface to S3
 Home-page: https://github.com/mullenkamp/s3dbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm s3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `s3dbm-0.0.4/s3dbm/main.py` & `s3dbm-0.0.5/s3dbm/main.py`

 * *Files identical despite different names*

### Comparing `s3dbm-0.0.4/s3dbm/utils.py` & `s3dbm-0.0.5/s3dbm/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
     """
 
     """
     if hasattr(stream, '_buffer_size'):
         buffer_size = stream._buffer_size
     dctx = zstd.ZstdDecompressor()
     reader = dctx.stream_reader(stream, read_size=buffer_size)
-    reader._buffer_size = buffer_size
+    # reader._buffer_size = buffer_size
 
     return reader
 
 
 def zstd_stream_writer(stream, buffer_size: int=524288):
     """
```

### Comparing `s3dbm-0.0.4/s3dbm.egg-info/PKG-INFO` & `s3dbm-0.0.5/s3dbm.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3dbm
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python dbm-style interface to S3
 Home-page: https://github.com/mullenkamp/s3dbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm s3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `s3dbm-0.0.4/setup.py` & `s3dbm-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # General parameters
 name = 's3dbm'
 main_package = 's3dbm'
-version = '0.0.4'
+version = '0.0.5'
 descrip = 'A python dbm-style interface to S3'
 
 # The below code is for readthedocs. To have sphinx/readthedocs interact with
 # the contained package, readthedocs needs to build the package. But the dependencies
 # should be installed via the conda yml env file rather than during the package build.
 if os.environ.get('READTHEDOCS', False) == 'True':
     INSTALL_REQUIRES = []
```

