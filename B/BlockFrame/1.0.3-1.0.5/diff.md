# Comparing `tmp/BlockFrame-1.0.3.tar.gz` & `tmp/BlockFrame-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlockFrame-1.0.3.tar", last modified: Mon May  8 13:36:33 2023, max compression
+gzip compressed data, was "BlockFrame-1.0.5.tar", last modified: Mon May  8 15:12:17 2023, max compression
```

## Comparing `BlockFrame-1.0.3.tar` & `BlockFrame-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 13:36:33.150899 BlockFrame-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-05-08 13:36:33.120074 BlockFrame-1.0.3/BlockFrame/
--rw-rw-rw-   0        0        0       75 2023-05-07 16:54:53.000000 BlockFrame-1.0.3/BlockFrame/__init__.py
--rw-rw-rw-   0        0        0      832 2023-05-07 18:26:27.000000 BlockFrame-1.0.3/BlockFrame/block_frame.py
-drwxrwxrwx   0        0        0        0 2023-05-08 13:36:33.141363 BlockFrame-1.0.3/BlockFrame/chunking_service/
--rw-rw-rw-   0        0        0        0 2023-04-01 11:41:46.000000 BlockFrame-1.0.3/BlockFrame/chunking_service/__init__.py
--rw-rw-rw-   0        0        0     8573 2023-05-08 13:32:16.000000 BlockFrame-1.0.3/BlockFrame/chunking_service/chunking.py
--rw-rw-rw-   0        0        0     1095 2023-05-07 18:26:27.000000 BlockFrame-1.0.3/BlockFrame/chunking_service/config.py
--rw-rw-rw-   0        0        0     1657 2023-05-07 15:14:26.000000 BlockFrame-1.0.3/BlockFrame/chunking_service/fetcher.py
-drwxrwxrwx   0        0        0        0 2023-05-08 13:36:33.148891 BlockFrame-1.0.3/BlockFrame/database_service/
--rw-rw-rw-   0        0        0        0 2023-04-01 11:35:37.000000 BlockFrame-1.0.3/BlockFrame/database_service/__init__.py
--rw-rw-rw-   0        0        0     1137 2023-05-08 13:13:55.000000 BlockFrame-1.0.3/BlockFrame/database_service/database.py
--rw-rw-rw-   0        0        0     1599 2023-05-08 13:09:22.000000 BlockFrame-1.0.3/BlockFrame/database_service/defaultmodel.py
--rw-rw-rw-   0        0        0      377 2023-04-30 09:16:12.000000 BlockFrame-1.0.3/BlockFrame/database_service/getters.py
--rw-rw-rw-   0        0        0     1518 2023-05-07 17:44:18.000000 BlockFrame-1.0.3/BlockFrame/database_service/initalisation.py
--rw-rw-rw-   0        0        0      241 2023-03-26 14:17:13.000000 BlockFrame-1.0.3/BlockFrame/database_service/setters.py
-drwxrwxrwx   0        0        0        0 2023-05-08 13:36:33.135858 BlockFrame-1.0.3/BlockFrame.egg-info/
--rw-rw-rw-   0        0        0     5313 2023-05-08 13:36:32.000000 BlockFrame-1.0.3/BlockFrame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      630 2023-05-08 13:36:33.000000 BlockFrame-1.0.3/BlockFrame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 13:36:32.000000 BlockFrame-1.0.3/BlockFrame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-08 13:36:32.000000 BlockFrame-1.0.3/BlockFrame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-08 13:36:32.000000 BlockFrame-1.0.3/BlockFrame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5313 2023-05-08 13:36:33.150899 BlockFrame-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-08 13:36:33.150899 BlockFrame-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1412 2023-05-08 13:36:16.000000 BlockFrame-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:12:17.135266 BlockFrame-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-05-08 15:12:17.100678 BlockFrame-1.0.5/BlockFrame/
+-rw-rw-rw-   0        0        0       75 2023-05-07 16:54:53.000000 BlockFrame-1.0.5/BlockFrame/__init__.py
+-rw-rw-rw-   0        0        0      832 2023-05-07 18:26:27.000000 BlockFrame-1.0.5/BlockFrame/block_frame.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:12:17.125228 BlockFrame-1.0.5/BlockFrame/chunking_service/
+-rw-rw-rw-   0        0        0        0 2023-04-01 11:41:46.000000 BlockFrame-1.0.5/BlockFrame/chunking_service/__init__.py
+-rw-rw-rw-   0        0        0     8877 2023-05-08 15:10:57.000000 BlockFrame-1.0.5/BlockFrame/chunking_service/chunking.py
+-rw-rw-rw-   0        0        0     1106 2023-05-08 15:11:18.000000 BlockFrame-1.0.5/BlockFrame/chunking_service/config.py
+-rw-rw-rw-   0        0        0     1657 2023-05-07 15:14:26.000000 BlockFrame-1.0.5/BlockFrame/chunking_service/fetcher.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:12:17.133259 BlockFrame-1.0.5/BlockFrame/database_service/
+-rw-rw-rw-   0        0        0        0 2023-04-01 11:35:37.000000 BlockFrame-1.0.5/BlockFrame/database_service/__init__.py
+-rw-rw-rw-   0        0        0     1193 2023-05-08 15:11:50.000000 BlockFrame-1.0.5/BlockFrame/database_service/database.py
+-rw-rw-rw-   0        0        0     1599 2023-05-08 13:09:22.000000 BlockFrame-1.0.5/BlockFrame/database_service/defaultmodel.py
+-rw-rw-rw-   0        0        0      377 2023-04-30 09:16:12.000000 BlockFrame-1.0.5/BlockFrame/database_service/getters.py
+-rw-rw-rw-   0        0        0     1518 2023-05-07 17:44:18.000000 BlockFrame-1.0.5/BlockFrame/database_service/initalisation.py
+-rw-rw-rw-   0        0        0      241 2023-03-26 14:17:13.000000 BlockFrame-1.0.5/BlockFrame/database_service/setters.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:12:17.122328 BlockFrame-1.0.5/BlockFrame.egg-info/
+-rw-rw-rw-   0        0        0     5313 2023-05-08 15:12:16.000000 BlockFrame-1.0.5/BlockFrame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      630 2023-05-08 15:12:17.000000 BlockFrame-1.0.5/BlockFrame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 15:12:16.000000 BlockFrame-1.0.5/BlockFrame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-08 15:12:16.000000 BlockFrame-1.0.5/BlockFrame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-08 15:12:16.000000 BlockFrame-1.0.5/BlockFrame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5313 2023-05-08 15:12:17.134259 BlockFrame-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-08 15:12:17.135266 BlockFrame-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1412 2023-05-08 15:12:08.000000 BlockFrame-1.0.5/setup.py
```

### Comparing `BlockFrame-1.0.3/BlockFrame/block_frame.py` & `BlockFrame-1.0.5/BlockFrame/block_frame.py`

 * *Files identical despite different names*

### Comparing `BlockFrame-1.0.3/BlockFrame/chunking_service/chunking.py` & `BlockFrame-1.0.5/BlockFrame/chunking_service/chunking.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,34 +33,41 @@
         custom_chunker: callable = None,
     ):
         self.custom_chunker = custom_chunker
         self.primary_uuid = uuid.uuid4()
         self.original_file_hash = ""
         self.chunk_file_hashes = []
         self.file_name = file_name
+        self.file_bytes = file_bytes
         self.chunk_file_uid = []
         self.files = files
         self.size = size
         if file_bytes:
-            with tempfile.NamedTemporaryFile(delete=False) as temp_file:
-                temp_file.write(file_bytes)
-                self.file_name = temp_file.name
-
-            if (
-                not pathlib.Path(self.file_name)
-                or not pathlib.Path(self.file_name).exists
-            ):
-                raise FileNotFoundError
-            return "correctly targeted"
+            with tempfile.NamedTemporaryFile(delete=True) as temp_file:
+                if file_name and isinstance(file_name, str):
+                    self.file_name = file_name
+                else:
+                    temp_file.write(file_bytes)
+                    self.file_name = temp_file.name
+
+        elif self.file_name is None:
+            raise ValueError("Either file_bytes or file_name must be provided")
+        elif not pathlib.Path(self.file_name).exists:
+            raise FileNotFoundError(f"{self.file_name} does not exist")
 
     def generic_chunks(self):
-        _size = os.stat(self.file_name).st_size // self.size
-        with open(self.file_name, "rb") as f:
-            while content := f.read(_size):
-                yield content
+        if self.file_bytes:
+            _size = len(self.file_bytes) // self.size
+            for i in range(self.size):
+                yield self.file_bytes[i * _size : (i + 1) * _size]
+        else:
+            _size = os.stat(self.file_name).st_size // self.size
+            with open(self.file_name, "rb") as f:
+                while content := f.read(_size):
+                    yield content
 
     def time_based_chunks(self):
         self.chunk_counter = 0
         with open(self.file_name, "rb") as f:
             while True:
                 start_time = (
                     datetime.now()
@@ -79,15 +86,14 @@
                     past_transfers = [transfer_time] * self.window_size
                     transfer_rate = sum(past_transfers, timedelta(0)) / self.window_size
                     # predict the time required to transfer the remaining data
                     remaining_bytes = os.stat(self.file_name).st_size - f.tell()
                     remaining_time_estimate = (
                         remaining_bytes / transfer_rate.total_seconds()
                     )
-                    # adjust the chunk size based on the predicted time to optimize transfer time
                     self.chunk_time_estimate = (
                         remaining_time_estimate / self.window_size
                     )
                     self.chunk_size_estimate = int(
                         max(
                             min(
                                 self.chunk_size_estimate,
@@ -150,15 +156,15 @@
         [
             x
             for x in os.listdir(self.path)
             if x.startswith(f"{self.primary_uuid}_chunk_")
         ]
 
         with self.db as session:
-            if existing_models := (
+            if (
                 session.query(DefaultChunkModel)
                 .filter_by(file_name=self.file_name)
                 .all()
             ):
                 raise ChunksExistsError("file is already chunked")
 
         count = 0
```

### Comparing `BlockFrame-1.0.3/BlockFrame/chunking_service/config.py` & `BlockFrame-1.0.5/BlockFrame/chunking_service/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
-import json
 import xml.etree.ElementTree as ET
 from types import SimpleNamespace
+import tomllib as toml
 
 
 class Config:
     def __init__(self, file_path):
         self.file_path = file_path
         self.option_dict = {
             "json": "from_json",
```

### Comparing `BlockFrame-1.0.3/BlockFrame/chunking_service/fetcher.py` & `BlockFrame-1.0.5/BlockFrame/chunking_service/fetcher.py`

 * *Files identical despite different names*

### Comparing `BlockFrame-1.0.3/BlockFrame/database_service/database.py` & `BlockFrame-1.0.5/BlockFrame/database_service/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import contextlib
 from BlockFrame.database_service.defaultmodel import DefaultChunkModel
 from BlockFrame.database_service.getters import BlockFrameDatabaseGetters
-from BlockFrame.database_service.initalisation import *
+from BlockFrame.database_service.initalisation import (
+    BlockFrameDatabaseInit,
+    DatabaseInterface,
+)
 
 
 class BlockFrameDatabase(BlockFrameDatabaseGetters, BlockFrameDatabaseInit):
     def __init__(self, *args, **kwargs):
         self.class_model = (
             DefaultChunkModel
             if kwargs.get("class_model") is not None
```

### Comparing `BlockFrame-1.0.3/BlockFrame/database_service/defaultmodel.py` & `BlockFrame-1.0.5/BlockFrame/database_service/defaultmodel.py`

 * *Files identical despite different names*

### Comparing `BlockFrame-1.0.3/BlockFrame/database_service/initalisation.py` & `BlockFrame-1.0.5/BlockFrame/database_service/initalisation.py`

 * *Files identical despite different names*

### Comparing `BlockFrame-1.0.3/BlockFrame.egg-info/PKG-INFO` & `BlockFrame-1.0.5/BlockFrame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlockFrame
-Version: 1.0.3
+Version: 1.0.5
 Summary: File Chunking Library to work as a data-store solution alongside webapps and software.
 Home-page: https://github.com/Wizock/BlockFrame/
 Author: Rohaan Ahmed
 Author-email: silent.death3500@gmail.com
 Project-URL: Bug Tracker, https://github.com/Wizock/BlockFrame/issues
 Project-URL: Documentation, https://blockframe.readthedocs.io/
 Project-URL: Source Code, https://github.com/Wizock/BlockFrame/
```

### Comparing `BlockFrame-1.0.3/BlockFrame.egg-info/SOURCES.txt` & `BlockFrame-1.0.5/BlockFrame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BlockFrame-1.0.3/PKG-INFO` & `BlockFrame-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlockFrame
-Version: 1.0.3
+Version: 1.0.5
 Summary: File Chunking Library to work as a data-store solution alongside webapps and software.
 Home-page: https://github.com/Wizock/BlockFrame/
 Author: Rohaan Ahmed
 Author-email: silent.death3500@gmail.com
 Project-URL: Bug Tracker, https://github.com/Wizock/BlockFrame/issues
 Project-URL: Documentation, https://blockframe.readthedocs.io/
 Project-URL: Source Code, https://github.com/Wizock/BlockFrame/
```

### Comparing `BlockFrame-1.0.3/setup.py` & `BlockFrame-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="BlockFrame",
-    version="1.0.3",
+    version="1.0.5",
     author="Rohaan Ahmed",
     author_email="silent.death3500@gmail.com",
     description="File Chunking Library to work as a data-store solution alongside webapps and software.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

