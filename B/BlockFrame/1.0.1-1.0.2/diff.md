# Comparing `tmp/BlockFrame-1.0.1.tar.gz` & `tmp/BlockFrame-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlockFrame-1.0.1.tar", last modified: Sun May  7 18:45:27 2023, max compression
+gzip compressed data, was "BlockFrame-1.0.2.tar", last modified: Mon May  8 13:15:46 2023, max compression
```

## Comparing `BlockFrame-1.0.1.tar` & `BlockFrame-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 18:45:27.392899 BlockFrame-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-07 18:45:27.362312 BlockFrame-1.0.1/BlockFrame/
--rw-rw-rw-   0        0        0       75 2023-05-07 16:54:53.000000 BlockFrame-1.0.1/BlockFrame/__init__.py
--rw-rw-rw-   0        0        0      832 2023-05-07 18:26:27.000000 BlockFrame-1.0.1/BlockFrame/block_frame.py
-drwxrwxrwx   0        0        0        0 2023-05-07 18:45:27.380359 BlockFrame-1.0.1/BlockFrame/chunking_service/
--rw-rw-rw-   0        0        0        0 2023-04-01 11:41:46.000000 BlockFrame-1.0.1/BlockFrame/chunking_service/__init__.py
--rw-rw-rw-   0        0        0     8233 2023-05-07 18:26:27.000000 BlockFrame-1.0.1/BlockFrame/chunking_service/chunking.py
--rw-rw-rw-   0        0        0     1095 2023-05-07 18:26:27.000000 BlockFrame-1.0.1/BlockFrame/chunking_service/config.py
--rw-rw-rw-   0        0        0     1657 2023-05-07 15:14:26.000000 BlockFrame-1.0.1/BlockFrame/chunking_service/fetcher.py
-drwxrwxrwx   0        0        0        0 2023-05-07 18:45:27.390228 BlockFrame-1.0.1/BlockFrame/database_service/
--rw-rw-rw-   0        0        0        0 2023-04-01 11:35:37.000000 BlockFrame-1.0.1/BlockFrame/database_service/__init__.py
--rw-rw-rw-   0        0        0     1061 2023-05-07 17:47:32.000000 BlockFrame-1.0.1/BlockFrame/database_service/database.py
--rw-rw-rw-   0        0        0     1599 2023-05-07 11:12:22.000000 BlockFrame-1.0.1/BlockFrame/database_service/defaultmodel.py
--rw-rw-rw-   0        0        0      377 2023-04-30 09:16:12.000000 BlockFrame-1.0.1/BlockFrame/database_service/getters.py
--rw-rw-rw-   0        0        0     1518 2023-05-07 17:44:18.000000 BlockFrame-1.0.1/BlockFrame/database_service/initalisation.py
--rw-rw-rw-   0        0        0      241 2023-03-26 14:17:13.000000 BlockFrame-1.0.1/BlockFrame/database_service/setters.py
-drwxrwxrwx   0        0        0        0 2023-05-07 18:45:27.377367 BlockFrame-1.0.1/BlockFrame.egg-info/
--rw-rw-rw-   0        0        0     5209 2023-05-07 18:45:27.000000 BlockFrame-1.0.1/BlockFrame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      630 2023-05-07 18:45:27.000000 BlockFrame-1.0.1/BlockFrame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 18:45:27.000000 BlockFrame-1.0.1/BlockFrame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-07 18:45:27.000000 BlockFrame-1.0.1/BlockFrame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-07 18:45:27.000000 BlockFrame-1.0.1/BlockFrame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5209 2023-05-07 18:45:27.391386 BlockFrame-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-07 18:45:27.392899 BlockFrame-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1310 2023-05-07 18:45:16.000000 BlockFrame-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:15:46.909382 BlockFrame-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-08 13:15:46.884918 BlockFrame-1.0.2/BlockFrame/
+-rw-rw-rw-   0        0        0       75 2023-05-07 16:54:53.000000 BlockFrame-1.0.2/BlockFrame/__init__.py
+-rw-rw-rw-   0        0        0      832 2023-05-07 18:26:27.000000 BlockFrame-1.0.2/BlockFrame/block_frame.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:15:46.899476 BlockFrame-1.0.2/BlockFrame/chunking_service/
+-rw-rw-rw-   0        0        0        0 2023-04-01 11:41:46.000000 BlockFrame-1.0.2/BlockFrame/chunking_service/__init__.py
+-rw-rw-rw-   0        0        0     8257 2023-05-08 09:30:34.000000 BlockFrame-1.0.2/BlockFrame/chunking_service/chunking.py
+-rw-rw-rw-   0        0        0     1095 2023-05-07 18:26:27.000000 BlockFrame-1.0.2/BlockFrame/chunking_service/config.py
+-rw-rw-rw-   0        0        0     1657 2023-05-07 15:14:26.000000 BlockFrame-1.0.2/BlockFrame/chunking_service/fetcher.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:15:46.905861 BlockFrame-1.0.2/BlockFrame/database_service/
+-rw-rw-rw-   0        0        0        0 2023-04-01 11:35:37.000000 BlockFrame-1.0.2/BlockFrame/database_service/__init__.py
+-rw-rw-rw-   0        0        0     1137 2023-05-08 13:13:55.000000 BlockFrame-1.0.2/BlockFrame/database_service/database.py
+-rw-rw-rw-   0        0        0     1599 2023-05-08 13:09:22.000000 BlockFrame-1.0.2/BlockFrame/database_service/defaultmodel.py
+-rw-rw-rw-   0        0        0      377 2023-04-30 09:16:12.000000 BlockFrame-1.0.2/BlockFrame/database_service/getters.py
+-rw-rw-rw-   0        0        0     1518 2023-05-07 17:44:18.000000 BlockFrame-1.0.2/BlockFrame/database_service/initalisation.py
+-rw-rw-rw-   0        0        0      241 2023-03-26 14:17:13.000000 BlockFrame-1.0.2/BlockFrame/database_service/setters.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:15:46.895027 BlockFrame-1.0.2/BlockFrame.egg-info/
+-rw-rw-rw-   0        0        0     5209 2023-05-08 13:15:46.000000 BlockFrame-1.0.2/BlockFrame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      630 2023-05-08 13:15:46.000000 BlockFrame-1.0.2/BlockFrame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 13:15:46.000000 BlockFrame-1.0.2/BlockFrame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-08 13:15:46.000000 BlockFrame-1.0.2/BlockFrame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-08 13:15:46.000000 BlockFrame-1.0.2/BlockFrame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5209 2023-05-08 13:15:46.909382 BlockFrame-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-08 13:15:46.909382 BlockFrame-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1310 2023-05-08 13:15:18.000000 BlockFrame-1.0.2/setup.py
```

### Comparing `BlockFrame-1.0.1/BlockFrame/block_frame.py` & `BlockFrame-1.0.2/BlockFrame/block_frame.py`

 * *Files identical despite different names*

### Comparing `BlockFrame-1.0.1/BlockFrame/chunking_service/chunking.py` & `BlockFrame-1.0.2/BlockFrame/chunking_service/chunking.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,26 +23,28 @@
         self.chunk_counter = 0
         self.window_size = 10
         self.chunk_time_estimate = timedelta(seconds=1)
 
     def target(
         self, file_name, size=None, files: list = None, custom_chunker: callable = None
     ):
-        self.file_name = file_name
-        self.size = size
+        self.custom_chunker = custom_chunker
         self.primary_uuid = uuid.uuid4()
         self.original_file_hash = ""
         self.chunk_file_hashes = []
+        self.file_name = file_name
         self.chunk_file_uid = []
         self.files = files
-        self.custom_chunker = custom_chunker
+        self.size = size
+        
+        
         if not pathlib.Path(self.file_name) or not pathlib.Path(self.file_name).exists:
             raise FileNotFoundError
         return "correctly targeted"
-
+    
     def generic_chunks(self):
         _size = os.stat(self.file_name).st_size // self.size
         with open(self.file_name, "rb") as f:
             while content := f.read(_size):
                 yield content
 
     def time_based_chunks(self):
```

### Comparing `BlockFrame-1.0.1/BlockFrame/chunking_service/config.py` & `BlockFrame-1.0.2/BlockFrame/chunking_service/config.py`

 * *Files identical despite different names*

### Comparing `BlockFrame-1.0.1/BlockFrame/chunking_service/fetcher.py` & `BlockFrame-1.0.2/BlockFrame/chunking_service/fetcher.py`

 * *Files identical despite different names*

### Comparing `BlockFrame-1.0.1/BlockFrame/database_service/database.py` & `BlockFrame-1.0.2/BlockFrame/database_service/database.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,12 +18,15 @@
             if custom_uri := self.config["database"]["uri"]:
                 DatabaseInterface.custom_uri(custom_uri)
                 self.database_obj = self.get_db()
 
         if not self.database_obj:
             self.database_obj = self.get_db()
 
+        # create the table
+        self.create_table(DefaultChunkModel)
+
         super().__init__(
             class_model=self.class_model,
             database_obj=self.database_obj,
             config=self.config,
         )
```

### Comparing `BlockFrame-1.0.1/BlockFrame/database_service/defaultmodel.py` & `BlockFrame-1.0.2/BlockFrame/database_service/defaultmodel.py`

 * *Files identical despite different names*

### Comparing `BlockFrame-1.0.1/BlockFrame/database_service/initalisation.py` & `BlockFrame-1.0.2/BlockFrame/database_service/initalisation.py`

 * *Files identical despite different names*

### Comparing `BlockFrame-1.0.1/BlockFrame.egg-info/PKG-INFO` & `BlockFrame-1.0.2/BlockFrame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlockFrame
-Version: 1.0.1
+Version: 1.0.2
 Summary: File Chunking Library to work as a data-store solution alongside webapps and software.
 Home-page: https://github.com/Wizock/BlockFrame/
 Author: Rohaan Ahmed
 Author-email: silent.death3500@gmail.com
 Project-URL: Bug Tracker, https://github.com/Wizock/BlockFrame/issues
 Project-URL: Documentation, https://blockframe.readthedocs.io/
 Project-URL: Source Code, https://github.com/Wizock/BlockFrame/
```

### Comparing `BlockFrame-1.0.1/BlockFrame.egg-info/SOURCES.txt` & `BlockFrame-1.0.2/BlockFrame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BlockFrame-1.0.1/PKG-INFO` & `BlockFrame-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlockFrame
-Version: 1.0.1
+Version: 1.0.2
 Summary: File Chunking Library to work as a data-store solution alongside webapps and software.
 Home-page: https://github.com/Wizock/BlockFrame/
 Author: Rohaan Ahmed
 Author-email: silent.death3500@gmail.com
 Project-URL: Bug Tracker, https://github.com/Wizock/BlockFrame/issues
 Project-URL: Documentation, https://blockframe.readthedocs.io/
 Project-URL: Source Code, https://github.com/Wizock/BlockFrame/
```

### Comparing `BlockFrame-1.0.1/setup.py` & `BlockFrame-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="BlockFrame",
-    version="1.0.1",
+    version="1.0.2",
     author="Rohaan Ahmed",
     author_email="silent.death3500@gmail.com",
     description="File Chunking Library to work as a data-store solution alongside webapps and software.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

