# Comparing `tmp/pyghostdb-0.0.3.tar.gz` & `tmp/pyghostdb-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyghostdb-0.0.3.tar", last modified: Sun May  7 03:59:51 2023, max compression
+gzip compressed data, was "pyghostdb-0.0.4.tar", last modified: Sun May  7 22:51:06 2023, max compression
```

## Comparing `pyghostdb-0.0.3.tar` & `pyghostdb-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-07 03:59:51.022441 pyghostdb-0.0.3/
--rw-r--r--   0 fedorshabashev   (501) staff       (20)      189 2023-05-07 03:59:51.022306 pyghostdb-0.0.3/PKG-INFO
--rw-r--r--   0 fedorshabashev   (501) staff       (20)      783 2023-05-04 00:59:20.000000 pyghostdb-0.0.3/README.md
-drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-07 03:59:51.021443 pyghostdb-0.0.3/pyghostdb/
--rw-r--r--   0 fedorshabashev   (501) staff       (20)        0 2023-05-05 14:29:31.000000 pyghostdb-0.0.3/pyghostdb/__init__.py
--rw-r--r--   0 fedorshabashev   (501) staff       (20)     2756 2023-05-07 03:58:29.000000 pyghostdb-0.0.3/pyghostdb/ghost_storage.py
--rw-r--r--   0 fedorshabashev   (501) staff       (20)     3068 2023-05-07 00:07:50.000000 pyghostdb-0.0.3/pyghostdb/hnswlib_index.py
--rw-r--r--   0 fedorshabashev   (501) staff       (20)     2281 2023-05-07 02:28:04.000000 pyghostdb-0.0.3/pyghostdb/parquet_conversion.py
--rw-r--r--   0 fedorshabashev   (501) staff       (20)     2376 2023-05-07 02:28:04.000000 pyghostdb-0.0.3/pyghostdb/test_hnsw.py
--rw-r--r--   0 fedorshabashev   (501) staff       (20)     2284 2023-05-07 02:28:04.000000 pyghostdb-0.0.3/pyghostdb/text_storage.py
-drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-07 03:59:51.022164 pyghostdb-0.0.3/pyghostdb.egg-info/
--rw-r--r--   0 fedorshabashev   (501) staff       (20)      189 2023-05-07 03:59:51.000000 pyghostdb-0.0.3/pyghostdb.egg-info/PKG-INFO
--rw-r--r--   0 fedorshabashev   (501) staff       (20)      345 2023-05-07 03:59:51.000000 pyghostdb-0.0.3/pyghostdb.egg-info/SOURCES.txt
--rw-r--r--   0 fedorshabashev   (501) staff       (20)        1 2023-05-07 03:59:51.000000 pyghostdb-0.0.3/pyghostdb.egg-info/dependency_links.txt
--rw-r--r--   0 fedorshabashev   (501) staff       (20)       58 2023-05-07 03:59:51.000000 pyghostdb-0.0.3/pyghostdb.egg-info/requires.txt
--rw-r--r--   0 fedorshabashev   (501) staff       (20)       10 2023-05-07 03:59:51.000000 pyghostdb-0.0.3/pyghostdb.egg-info/top_level.txt
--rw-r--r--   0 fedorshabashev   (501) staff       (20)      347 2023-05-07 03:59:42.000000 pyghostdb-0.0.3/pyproject.toml
--rw-r--r--   0 fedorshabashev   (501) staff       (20)       38 2023-05-07 03:59:51.022480 pyghostdb-0.0.3/setup.cfg
+drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-07 22:51:06.694245 pyghostdb-0.0.4/
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)      189 2023-05-07 22:51:06.694075 pyghostdb-0.0.4/PKG-INFO
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)      783 2023-05-04 00:59:20.000000 pyghostdb-0.0.4/README.md
+drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-07 22:51:06.693239 pyghostdb-0.0.4/pyghostdb/
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)        0 2023-05-05 14:29:31.000000 pyghostdb-0.0.4/pyghostdb/__init__.py
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)     2753 2023-05-07 22:31:44.000000 pyghostdb-0.0.4/pyghostdb/ghost_storage.py
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)     3068 2023-05-07 00:07:50.000000 pyghostdb-0.0.4/pyghostdb/hnswlib_index.py
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)     2281 2023-05-07 02:28:04.000000 pyghostdb-0.0.4/pyghostdb/parquet_conversion.py
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)     2376 2023-05-07 02:28:04.000000 pyghostdb-0.0.4/pyghostdb/test_hnsw.py
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)     2284 2023-05-07 02:28:04.000000 pyghostdb-0.0.4/pyghostdb/text_storage.py
+drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-07 22:51:06.693938 pyghostdb-0.0.4/pyghostdb.egg-info/
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)      189 2023-05-07 22:51:06.000000 pyghostdb-0.0.4/pyghostdb.egg-info/PKG-INFO
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)      345 2023-05-07 22:51:06.000000 pyghostdb-0.0.4/pyghostdb.egg-info/SOURCES.txt
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)        1 2023-05-07 22:51:06.000000 pyghostdb-0.0.4/pyghostdb.egg-info/dependency_links.txt
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)       58 2023-05-07 22:51:06.000000 pyghostdb-0.0.4/pyghostdb.egg-info/requires.txt
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)       10 2023-05-07 22:51:06.000000 pyghostdb-0.0.4/pyghostdb.egg-info/top_level.txt
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)      347 2023-05-07 22:51:00.000000 pyghostdb-0.0.4/pyproject.toml
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)       38 2023-05-07 22:51:06.694286 pyghostdb-0.0.4/setup.cfg
```

### Comparing `pyghostdb-0.0.3/README.md` & `pyghostdb-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyghostdb-0.0.3/pyghostdb/ghost_storage.py` & `pyghostdb-0.0.4/pyghostdb/ghost_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     def __init__(self, dim=1536, max_elements=10**5, persist_dir="ghost_dir"):
         self.hnsw_index = HNSWIndex(dim=dim, max_elements=max_elements, ef=200, M=16)
         self.hnsw_index.init_index()
         self.persist_dir = persist_dir
         if not os.path.exists(self.persist_dir):
             os.makedirs(self.persist_dir)
-        self.text_storage_db = TextStorbuiage(self.text_storage_filepath())
+        self.text_storage_db = TextStorage(self.text_storage_filepath())
         if self.hnws_index_filepath_exists():
             self.load()
 
     def add(self, text_id, text, embedding):
         if not isinstance(embedding, np.ndarray):
             try:
                 embedding = np.array(embedding)
```

### Comparing `pyghostdb-0.0.3/pyghostdb/hnswlib_index.py` & `pyghostdb-0.0.4/pyghostdb/hnswlib_index.py`

 * *Files identical despite different names*

### Comparing `pyghostdb-0.0.3/pyghostdb/parquet_conversion.py` & `pyghostdb-0.0.4/pyghostdb/parquet_conversion.py`

 * *Files identical despite different names*

### Comparing `pyghostdb-0.0.3/pyghostdb/test_hnsw.py` & `pyghostdb-0.0.4/pyghostdb/test_hnsw.py`

 * *Files identical despite different names*

### Comparing `pyghostdb-0.0.3/pyghostdb/text_storage.py` & `pyghostdb-0.0.4/pyghostdb/text_storage.py`

 * *Files identical despite different names*

