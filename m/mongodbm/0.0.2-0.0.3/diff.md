# Comparing `tmp/mongodbm-0.0.2.tar.gz` & `tmp/mongodbm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodbm-0.0.2.tar", last modified: Sun Apr 30 23:46:47 2023, max compression
+gzip compressed data, was "mongodbm-0.0.3.tar", last modified: Sun May  7 22:13:22 2023, max compression
```

## Comparing `mongodbm-0.0.2.tar` & `mongodbm-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-04-30 23:46:47.471091 mongodbm-0.0.2/
--rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-04-30 23:17:54.000000 mongodbm-0.0.2/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)     1748 2023-04-30 23:46:47.471091 mongodbm-0.0.2/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)     1231 2023-04-30 23:40:58.000000 mongodbm-0.0.2/README.rst
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-04-30 23:46:47.471091 mongodbm-0.0.2/mongodbm/
--rw-rw-r--   0 mike      (1000) mike      (1000)       74 2023-04-30 23:17:54.000000 mongodbm-0.0.2/mongodbm/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     7862 2023-04-30 23:44:13.000000 mongodbm-0.0.2/mongodbm/main.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-04-30 23:46:47.471091 mongodbm-0.0.2/mongodbm/tests/
--rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-04-30 23:17:54.000000 mongodbm-0.0.2/mongodbm/tests/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     2369 2023-04-30 23:32:23.000000 mongodbm-0.0.2/mongodbm/utils.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-04-30 23:46:47.471091 mongodbm-0.0.2/mongodbm.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)     1748 2023-04-30 23:46:47.000000 mongodbm-0.0.2/mongodbm.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      294 2023-04-30 23:46:47.000000 mongodbm-0.0.2/mongodbm.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-04-30 23:46:47.000000 mongodbm-0.0.2/mongodbm.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        8 2023-04-30 23:46:47.000000 mongodbm-0.0.2/mongodbm.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        9 2023-04-30 23:46:47.000000 mongodbm-0.0.2/mongodbm.egg-info/top_level.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-04-30 23:17:54.000000 mongodbm-0.0.2/pyproject.toml
--rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-04-30 23:46:47.471091 mongodbm-0.0.2/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     7132 2023-04-30 23:46:36.000000 mongodbm-0.0.2/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-07 22:13:22.795692 mongodbm-0.0.3/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-04-30 23:17:54.000000 mongodbm-0.0.3/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1916 2023-05-07 22:13:22.795692 mongodbm-0.0.3/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1399 2023-05-01 01:52:26.000000 mongodbm-0.0.3/README.rst
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-07 22:13:22.795692 mongodbm-0.0.3/mongodbm/
+-rw-rw-r--   0 mike      (1000) mike      (1000)       74 2023-04-30 23:17:54.000000 mongodbm-0.0.3/mongodbm/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7915 2023-05-07 22:06:29.000000 mongodbm-0.0.3/mongodbm/main.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-07 22:13:22.795692 mongodbm-0.0.3/mongodbm/tests/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-04-30 23:17:54.000000 mongodbm-0.0.3/mongodbm/tests/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2369 2023-04-30 23:32:23.000000 mongodbm-0.0.3/mongodbm/utils.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-07 22:13:22.795692 mongodbm-0.0.3/mongodbm.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1916 2023-05-07 22:13:22.000000 mongodbm-0.0.3/mongodbm.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      294 2023-05-07 22:13:22.000000 mongodbm-0.0.3/mongodbm.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-07 22:13:22.000000 mongodbm-0.0.3/mongodbm.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        8 2023-05-07 22:13:22.000000 mongodbm-0.0.3/mongodbm.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        9 2023-05-07 22:13:22.000000 mongodbm-0.0.3/mongodbm.egg-info/top_level.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-04-30 23:17:54.000000 mongodbm-0.0.3/pyproject.toml
+-rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-07 22:13:22.795692 mongodbm-0.0.3/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7132 2023-05-07 22:12:48.000000 mongodbm-0.0.3/setup.py
```

### Comparing `mongodbm-0.0.2/LICENSE` & `mongodbm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mongodbm-0.0.2/PKG-INFO` & `mongodbm-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodbm
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python key-value MongoDB database
 Home-page: https://github.com/mullenkamp/mongodbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm
 Classifier: Development Status :: 3 - Alpha
@@ -21,14 +21,16 @@
 ------------
 mongodbm is a Python package to use a MongoDB server as a python dbm-style key/value database. It implements all of the MutableMapping methods in Python and is implemented in MongoDB using the GridFS spec to allow for values of any size. Keys must be strings (as the filename in GridFS) and values can be set as either bytes or file-like objects. Values returned by mongodbm are always file-like objects (specifically the GridOut object from pymongo).
 
 This package was primarily made to be a fast and persistent key/value store that can have multiple readers and writers across multiple Python instances. MongoDB handles the race conditions so that I don't have to. The initial primary use-case is as a local cache for web apps where the source data are stored in remote S3 systems.
 
 A MongoDB server must be running and accessible for mongodbm to work.
 
+If someone is brave enough to try this out, take a look at the doc strings of the mongodbm.open function to find out what you need to do. It's pretty straightforward.
+
 Installation
 ------------
 Install via pip::
 
   pip install mongodbm
 
 Or conda::
```

### Comparing `mongodbm-0.0.2/README.rst` & `mongodbm-0.0.3/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 ------------
 mongodbm is a Python package to use a MongoDB server as a python dbm-style key/value database. It implements all of the MutableMapping methods in Python and is implemented in MongoDB using the GridFS spec to allow for values of any size. Keys must be strings (as the filename in GridFS) and values can be set as either bytes or file-like objects. Values returned by mongodbm are always file-like objects (specifically the GridOut object from pymongo).
 
 This package was primarily made to be a fast and persistent key/value store that can have multiple readers and writers across multiple Python instances. MongoDB handles the race conditions so that I don't have to. The initial primary use-case is as a local cache for web apps where the source data are stored in remote S3 systems.
 
 A MongoDB server must be running and accessible for mongodbm to work.
 
+If someone is brave enough to try this out, take a look at the doc strings of the mongodbm.open function to find out what you need to do. It's pretty straightforward.
+
 Installation
 ------------
 Install via pip::
 
   pip install mongodbm
 
 Or conda::
```

### Comparing `mongodbm-0.0.2/mongodbm/main.py` & `mongodbm-0.0.3/mongodbm/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
             raise ValueError("Invalid flag")
 
         if write:
             utils.set_indexes(self._db, ttl)
 
         self._ttl = ttl
         self._write = write
+        self._chunk_size = gridfs.DEFAULT_CHUNK_SIZE
 
 
     def keys(self):
         fs = gridfs.GridFS(self._db)
 
         for key in fs.list():
             yield key
```

### Comparing `mongodbm-0.0.2/mongodbm/utils.py` & `mongodbm-0.0.3/mongodbm/utils.py`

 * *Files identical despite different names*

### Comparing `mongodbm-0.0.2/mongodbm.egg-info/PKG-INFO` & `mongodbm-0.0.3/mongodbm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodbm
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python key-value MongoDB database
 Home-page: https://github.com/mullenkamp/mongodbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm
 Classifier: Development Status :: 3 - Alpha
@@ -21,14 +21,16 @@
 ------------
 mongodbm is a Python package to use a MongoDB server as a python dbm-style key/value database. It implements all of the MutableMapping methods in Python and is implemented in MongoDB using the GridFS spec to allow for values of any size. Keys must be strings (as the filename in GridFS) and values can be set as either bytes or file-like objects. Values returned by mongodbm are always file-like objects (specifically the GridOut object from pymongo).
 
 This package was primarily made to be a fast and persistent key/value store that can have multiple readers and writers across multiple Python instances. MongoDB handles the race conditions so that I don't have to. The initial primary use-case is as a local cache for web apps where the source data are stored in remote S3 systems.
 
 A MongoDB server must be running and accessible for mongodbm to work.
 
+If someone is brave enough to try this out, take a look at the doc strings of the mongodbm.open function to find out what you need to do. It's pretty straightforward.
+
 Installation
 ------------
 Install via pip::
 
   pip install mongodbm
 
 Or conda::
```

### Comparing `mongodbm-0.0.2/setup.py` & `mongodbm-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # General parameters
 name = 'mongodbm'
 main_package = 'mongodbm'
-version = '0.0.2'
+version = '0.0.3'
 descrip = 'A python key-value MongoDB database'
 
 # The below code is for readthedocs. To have sphinx/readthedocs interact with
 # the contained package, readthedocs needs to build the package. But the dependencies
 # should be installed via the conda yml env file rather than during the package build.
 if os.environ.get('READTHEDOCS', False) == 'True':
     INSTALL_REQUIRES = []
```

