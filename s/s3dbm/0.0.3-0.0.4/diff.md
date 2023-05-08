# Comparing `tmp/s3dbm-0.0.3.tar.gz` & `tmp/s3dbm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3dbm-0.0.3.tar", last modified: Mon May  8 01:41:04 2023, max compression
+gzip compressed data, was "s3dbm-0.0.4.tar", last modified: Mon May  8 06:27:57 2023, max compression
```

## Comparing `s3dbm-0.0.3.tar` & `s3dbm-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 01:41:04.517390 s3dbm-0.0.3/
--rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-05 20:34:52.000000 s3dbm-0.0.3/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-08 01:41:04.517390 s3dbm-0.0.3/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)       78 2023-05-07 22:33:06.000000 s3dbm-0.0.3/README.rst
--rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-06 23:57:50.000000 s3dbm-0.0.3/pyproject.toml
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 01:41:04.513390 s3dbm-0.0.3/s3dbm/
--rw-rw-r--   0 mike      (1000) mike      (1000)      111 2023-05-08 01:40:14.000000 s3dbm-0.0.3/s3dbm/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    12767 2023-05-08 01:40:08.000000 s3dbm-0.0.3/s3dbm/main.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 01:41:04.517390 s3dbm-0.0.3/s3dbm/tests/
--rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-06 23:57:50.000000 s3dbm-0.0.3/s3dbm/tests/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    13297 2023-05-07 22:42:24.000000 s3dbm-0.0.3/s3dbm/utils.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 01:41:04.517390 s3dbm-0.0.3/s3dbm.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-08 01:41:04.000000 s3dbm-0.0.3/s3dbm.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      267 2023-05-08 01:41:04.000000 s3dbm-0.0.3/s3dbm.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-08 01:41:04.000000 s3dbm-0.0.3/s3dbm.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       36 2023-05-08 01:41:04.000000 s3dbm-0.0.3/s3dbm.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        6 2023-05-08 01:41:04.000000 s3dbm-0.0.3/s3dbm.egg-info/top_level.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-08 01:41:04.517390 s3dbm-0.0.3/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     7162 2023-05-08 01:40:38.000000 s3dbm-0.0.3/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 06:27:57.959893 s3dbm-0.0.4/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-05 20:34:52.000000 s3dbm-0.0.4/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-08 06:27:57.959893 s3dbm-0.0.4/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)       78 2023-05-07 22:33:06.000000 s3dbm-0.0.4/README.rst
+-rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-06 23:57:50.000000 s3dbm-0.0.4/pyproject.toml
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 06:27:57.959893 s3dbm-0.0.4/s3dbm/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      111 2023-05-08 01:40:14.000000 s3dbm-0.0.4/s3dbm/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    12767 2023-05-08 01:40:08.000000 s3dbm-0.0.4/s3dbm/main.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 06:27:57.959893 s3dbm-0.0.4/s3dbm/tests/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-06 23:57:50.000000 s3dbm-0.0.4/s3dbm/tests/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    13753 2023-05-08 06:16:26.000000 s3dbm-0.0.4/s3dbm/utils.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 06:27:57.959893 s3dbm-0.0.4/s3dbm.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-08 06:27:57.000000 s3dbm-0.0.4/s3dbm.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      267 2023-05-08 06:27:57.000000 s3dbm-0.0.4/s3dbm.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-08 06:27:57.000000 s3dbm-0.0.4/s3dbm.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       36 2023-05-08 06:27:57.000000 s3dbm-0.0.4/s3dbm.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        6 2023-05-08 06:27:57.000000 s3dbm-0.0.4/s3dbm.egg-info/top_level.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-08 06:27:57.959893 s3dbm-0.0.4/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7162 2023-05-08 06:24:12.000000 s3dbm-0.0.4/setup.py
```

### Comparing `s3dbm-0.0.3/LICENSE` & `s3dbm-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `s3dbm-0.0.3/PKG-INFO` & `s3dbm-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3dbm
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python dbm-style interface to S3
 Home-page: https://github.com/mullenkamp/s3dbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm s3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `s3dbm-0.0.3/s3dbm/main.py` & `s3dbm-0.0.4/s3dbm/main.py`

 * *Files identical despite different names*

### Comparing `s3dbm-0.0.3/s3dbm/utils.py` & `s3dbm-0.0.4/s3dbm/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,26 +130,32 @@
     return s3
 
 
 def zstd_stream_reader(stream, buffer_size: int=524288):
     """
 
     """
+    if hasattr(stream, '_buffer_size'):
+        buffer_size = stream._buffer_size
     dctx = zstd.ZstdDecompressor()
     reader = dctx.stream_reader(stream, read_size=buffer_size)
+    reader._buffer_size = buffer_size
 
     return reader
 
 
 def zstd_stream_writer(stream, buffer_size: int=524288):
     """
 
     """
+    if hasattr(stream, '_buffer_size'):
+        buffer_size = stream._buffer_size
     dctx = zstd.ZstdCompressor(1)
     writer = dctx.stream_writer(stream, write_size=buffer_size)
+    writer._buffer_size = buffer_size
 
     return writer
 
 
 def url_to_stream(url: HttpUrl, buffer_size: int=524288, read_timeout: int=120):
     """
     Function to create a file object from a file stored via http(s). This function will return a file object of the object in the url location. This file object does not contain any data until data is read from it, which ensures large files are not completely read into memory.
@@ -171,14 +177,15 @@
         file object of the S3 object.
     """
     transport_params = {'buffer_size': buffer_size, 'timeout': read_timeout}
 
     ## Get the object
     try:
         file_obj = smart_open.open(url, 'rb', transport_params=transport_params, compression='disable')
+        file_obj._buffer_size = buffer_size
     except Exception as err:
         file_obj = None
 
     return file_obj
 
 
 def get_object_s3(obj_key: str, bucket: str, s3: botocore.client.BaseClient = None, public_url: HttpUrl=None, buffer_size: int=524288, read_timeout: int=120, provider: str=None):
@@ -217,14 +224,15 @@
 
     elif isinstance(s3, botocore.client.BaseClient):
         s3_url = s3_url_base.format(bucket=bucket, key=obj_key)
         transport_params['client'] = s3
 
         try:
             file_obj = smart_open.open(s3_url, 'rb', transport_params=transport_params, compression='disable')
+            file_obj._buffer_size = buffer_size
         except Exception as err:
             # print('smart_open could not open url with the following error:')
             # print(err)
             file_obj = None
 
     else:
         raise TypeError('One of client or public_url needs to be correctly defined.')
@@ -233,16 +241,16 @@
 
 
 def get_object_final(obj_key: str, bucket: str, s3: botocore.client.BaseClient = None, public_url: HttpUrl=None, buffer_size: int=524288, read_timeout: int=120, provider: str=None, compression: bool=True, cache: MutableMapping=None):
     """
 
     """
     if cache is not None:
-        if '_chunk_size' in cache:
-            buffer_size = cache._chunk_size
+        if hasattr(cache, '_buffer_size'):
+            buffer_size = cache._buffer_size
         try:
             file_obj = cache[obj_key]
         except:
             file_obj = get_object_s3(obj_key, bucket, s3, public_url, buffer_size, read_timeout, provider)
             if file_obj is not None:
                 cache[obj_key] = file_obj
                 file_obj = cache[obj_key]
@@ -274,17 +282,20 @@
     buffer_size: int
         The amount of bytes to use in memory for processing the object.
 
     Returns
     -------
     None
     """
+    if hasattr(file_obj, '_buffer_size'):
+        buffer_size = file_obj._buffer_size
+
     s3_url = s3_url_base.format(bucket=bucket, key=obj_key)
 
-    transport_params = {'client': s3}
+    transport_params = {'client': s3, 'buffer_size': buffer_size}
 
     obj_size = determine_file_obj_size(file_obj)
 
     if obj_size > multipart_size:
         transport_params['multipart_upload'] = True
     else:
         transport_params['multipart_upload'] = False
```

### Comparing `s3dbm-0.0.3/s3dbm.egg-info/PKG-INFO` & `s3dbm-0.0.4/s3dbm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3dbm
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python dbm-style interface to S3
 Home-page: https://github.com/mullenkamp/s3dbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm s3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `s3dbm-0.0.3/setup.py` & `s3dbm-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # General parameters
 name = 's3dbm'
 main_package = 's3dbm'
-version = '0.0.3'
+version = '0.0.4'
 descrip = 'A python dbm-style interface to S3'
 
 # The below code is for readthedocs. To have sphinx/readthedocs interact with
 # the contained package, readthedocs needs to build the package. But the dependencies
 # should be installed via the conda yml env file rather than during the package build.
 if os.environ.get('READTHEDOCS', False) == 'True':
     INSTALL_REQUIRES = []
```

