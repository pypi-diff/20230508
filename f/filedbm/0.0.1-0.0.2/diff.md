# Comparing `tmp/filedbm-0.0.1.tar.gz` & `tmp/filedbm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filedbm-0.0.1.tar", last modified: Mon May  8 05:12:53 2023, max compression
+gzip compressed data, was "filedbm-0.0.2.tar", last modified: Mon May  8 06:23:12 2023, max compression
```

## Comparing `filedbm-0.0.1.tar` & `filedbm-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 05:12:53.391148 filedbm-0.0.1/
--rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-08 01:46:02.000000 filedbm-0.0.1/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)      663 2023-05-08 05:12:53.391148 filedbm-0.0.1/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      152 2023-05-08 01:50:12.000000 filedbm-0.0.1/README.rst
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 05:12:53.391148 filedbm-0.0.1/filedbm/
--rw-rw-r--   0 mike      (1000) mike      (1000)       70 2023-05-08 05:12:10.000000 filedbm-0.0.1/filedbm/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     6560 2023-05-08 05:09:06.000000 filedbm-0.0.1/filedbm/main.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 05:12:53.391148 filedbm-0.0.1/filedbm/tests/
--rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-08 01:48:21.000000 filedbm-0.0.1/filedbm/tests/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4931 2023-05-08 05:04:34.000000 filedbm-0.0.1/filedbm/utils.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 05:12:53.391148 filedbm-0.0.1/filedbm.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)      663 2023-05-08 05:12:53.000000 filedbm-0.0.1/filedbm.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      255 2023-05-08 05:12:53.000000 filedbm-0.0.1/filedbm.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-08 05:12:53.000000 filedbm-0.0.1/filedbm.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        8 2023-05-08 05:12:53.000000 filedbm-0.0.1/filedbm.egg-info/top_level.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-08 01:48:21.000000 filedbm-0.0.1/pyproject.toml
--rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-08 05:12:53.391148 filedbm-0.0.1/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     7116 2023-05-08 05:11:02.000000 filedbm-0.0.1/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 06:23:12.078271 filedbm-0.0.2/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-08 01:46:02.000000 filedbm-0.0.2/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)      663 2023-05-08 06:23:12.078271 filedbm-0.0.2/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      152 2023-05-08 01:50:12.000000 filedbm-0.0.2/README.rst
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 06:23:12.074271 filedbm-0.0.2/filedbm/
+-rw-rw-r--   0 mike      (1000) mike      (1000)       70 2023-05-08 05:12:10.000000 filedbm-0.0.2/filedbm/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6560 2023-05-08 05:09:06.000000 filedbm-0.0.2/filedbm/main.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 06:23:12.078271 filedbm-0.0.2/filedbm/tests/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-08 01:48:21.000000 filedbm-0.0.2/filedbm/tests/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5043 2023-05-08 06:16:54.000000 filedbm-0.0.2/filedbm/utils.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 06:23:12.078271 filedbm-0.0.2/filedbm.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      663 2023-05-08 06:23:12.000000 filedbm-0.0.2/filedbm.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      255 2023-05-08 06:23:12.000000 filedbm-0.0.2/filedbm.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-08 06:23:12.000000 filedbm-0.0.2/filedbm.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        8 2023-05-08 06:23:12.000000 filedbm-0.0.2/filedbm.egg-info/top_level.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-08 01:48:21.000000 filedbm-0.0.2/pyproject.toml
+-rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-08 06:23:12.078271 filedbm-0.0.2/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7116 2023-05-08 06:23:05.000000 filedbm-0.0.2/setup.py
```

### Comparing `filedbm-0.0.1/LICENSE` & `filedbm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `filedbm-0.0.1/PKG-INFO` & `filedbm-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filedbm
-Version: 0.0.1
+Version: 0.0.2
 Summary: A persistent key-value database
 Home-page: https://github.com/mullenkamp/filedbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `filedbm-0.0.1/filedbm/main.py` & `filedbm-0.0.2/filedbm/main.py`

 * *Files identical despite different names*

### Comparing `filedbm-0.0.1/filedbm/utils.py` & `filedbm-0.0.2/filedbm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from typing import Any, Generic, Iterator, Union
 import mmap
 
 ############################################
 ### Parameters
 
 key_hash_len = 13
-write_buffer_size = 512000
+default_write_buffer_size = 512000
 
 
 ############################################
 ### Classes
 
 
 class FileObjectSlice(io.IOBase):
@@ -172,22 +172,26 @@
     write_init_bytes = int_to_bytes(key_bytes_len, n_bytes_key) + int_to_bytes(value_bytes_len, n_bytes_value) + key
 
     file_path = db_path.joinpath(key_hash.hex())
 
     file = io.open(file_path, 'w+b')
     _ = file.write(write_init_bytes)
 
-    chunk = value.read(write_buffer_size)
+    if hasattr(value, '_buffer_size'):
+        buffer_size = value._buffer_size
+    else:
+        buffer_size = default_write_buffer_size
+
+    chunk = value.read(buffer_size)
     while chunk:
         file.write(chunk)
-        chunk = value.read(write_buffer_size)
+        chunk = value.read(buffer_size)
 
     file.close()
 
-    # return file_path
```

### Comparing `filedbm-0.0.1/filedbm.egg-info/PKG-INFO` & `filedbm-0.0.2/filedbm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filedbm
-Version: 0.0.1
+Version: 0.0.2
 Summary: A persistent key-value database
 Home-page: https://github.com/mullenkamp/filedbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `filedbm-0.0.1/setup.py` & `filedbm-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # General parameters
 name = 'filedbm'
 main_package = 'filedbm'
-version = '0.0.1'
+version = '0.0.2'
 descrip = 'A persistent key-value database'
 
 # The below code is for readthedocs. To have sphinx/readthedocs interact with
 # the contained package, readthedocs needs to build the package. But the dependencies
 # should be installed via the conda yml env file rather than during the package build.
 if os.environ.get('READTHEDOCS', False) == 'True':
     INSTALL_REQUIRES = []
```

