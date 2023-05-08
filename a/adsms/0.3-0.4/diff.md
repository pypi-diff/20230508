# Comparing `tmp/adsms-0.3.tar.gz` & `tmp/adsms-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adsms-0.3.tar", last modified: Mon May  8 17:16:39 2023, max compression
+gzip compressed data, was "adsms-0.4.tar", last modified: Mon May  8 17:32:57 2023, max compression
```

## Comparing `adsms-0.3.tar` & `adsms-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kj7rrv    (1000) kj7rrv    (1000)        0 2023-05-08 17:16:39.316400 adsms-0.3/
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)    34020 2023-05-04 19:33:40.000000 adsms-0.3/LICENSE
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)       16 2023-05-08 17:14:34.000000 adsms-0.3/MANIFEST.in
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)     2701 2023-05-08 17:16:39.316400 adsms-0.3/PKG-INFO
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)     2192 2023-05-06 01:37:05.000000 adsms-0.3/README.md
-drwxrwxr-x   0 kj7rrv    (1000) kj7rrv    (1000)        0 2023-05-08 17:16:39.316400 adsms-0.3/adsms/
--rwxrwxr-x   0 kj7rrv    (1000) kj7rrv    (1000)     2263 2023-05-08 01:47:00.000000 adsms-0.3/adsms/__init__.py
-drwxrwxr-x   0 kj7rrv    (1000) kj7rrv    (1000)        0 2023-05-08 17:16:39.316400 adsms-0.3/adsms.egg-info/
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)     2701 2023-05-08 17:16:39.000000 adsms-0.3/adsms.egg-info/PKG-INFO
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)      238 2023-05-08 17:16:39.000000 adsms-0.3/adsms.egg-info/SOURCES.txt
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)        1 2023-05-08 17:16:39.000000 adsms-0.3/adsms.egg-info/dependency_links.txt
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)       37 2023-05-08 17:16:39.000000 adsms-0.3/adsms.egg-info/entry_points.txt
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)        9 2023-05-08 17:16:39.000000 adsms-0.3/adsms.egg-info/requires.txt
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)        6 2023-05-08 17:16:39.000000 adsms-0.3/adsms.egg-info/top_level.txt
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)      700 2023-05-08 17:14:40.000000 adsms-0.3/pyproject.toml
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)       38 2023-05-08 17:16:39.316400 adsms-0.3/setup.cfg
+drwxrwxr-x   0 kj7rrv    (1000) kj7rrv    (1000)        0 2023-05-08 17:32:57.592751 adsms-0.4/
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)    34020 2023-05-04 19:33:40.000000 adsms-0.4/LICENSE
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)       16 2023-05-08 17:14:34.000000 adsms-0.4/MANIFEST.in
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)     2701 2023-05-08 17:32:57.592751 adsms-0.4/PKG-INFO
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)     2192 2023-05-06 01:37:05.000000 adsms-0.4/README.md
+drwxrwxr-x   0 kj7rrv    (1000) kj7rrv    (1000)        0 2023-05-08 17:32:57.592751 adsms-0.4/adsms/
+-rwxrwxr-x   0 kj7rrv    (1000) kj7rrv    (1000)     2263 2023-05-08 01:47:00.000000 adsms-0.4/adsms/__init__.py
+drwxrwxr-x   0 kj7rrv    (1000) kj7rrv    (1000)        0 2023-05-08 17:32:57.592751 adsms-0.4/adsms.egg-info/
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)     2701 2023-05-08 17:32:57.000000 adsms-0.4/adsms.egg-info/PKG-INFO
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)      238 2023-05-08 17:32:57.000000 adsms-0.4/adsms.egg-info/SOURCES.txt
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)        1 2023-05-08 17:32:57.000000 adsms-0.4/adsms.egg-info/dependency_links.txt
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)       37 2023-05-08 17:32:57.000000 adsms-0.4/adsms.egg-info/entry_points.txt
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)        9 2023-05-08 17:32:57.000000 adsms-0.4/adsms.egg-info/requires.txt
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)        6 2023-05-08 17:32:57.000000 adsms-0.4/adsms.egg-info/top_level.txt
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)      700 2023-05-08 17:32:50.000000 adsms-0.4/pyproject.toml
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)       38 2023-05-08 17:32:57.592751 adsms-0.4/setup.cfg
```

### Comparing `adsms-0.3/LICENSE` & `adsms-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adsms-0.3/PKG-INFO` & `adsms-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsms
-Version: 0.3
+Version: 0.4
 Summary: Send SMS aircraft alerts based on ADS-B data
 Author-email: Samuel Sloniker <sam@kj7rrv.com>
 Project-URL: Homepage, https://git.kj7rrv.com/kj7rrv/adsms
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `adsms-0.3/README.md` & `adsms-0.4/README.md`

 * *Files identical despite different names*

### Comparing `adsms-0.3/adsms/__init__.py` & `adsms-0.4/adsms/__init__.py`

 * *Files identical despite different names*

### Comparing `adsms-0.3/adsms.egg-info/PKG-INFO` & `adsms-0.4/adsms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsms
-Version: 0.3
+Version: 0.4
 Summary: Send SMS aircraft alerts based on ADS-B data
 Author-email: Samuel Sloniker <sam@kj7rrv.com>
 Project-URL: Homepage, https://git.kj7rrv.com/kj7rrv/adsms
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `adsms-0.3/pyproject.toml` & `adsms-0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "adsms"
-version = "0.3"
+version = "0.4"
 description = "Send SMS aircraft alerts based on ADS-B data"
 readme = "README.md"
 authors = [{ name = "Samuel Sloniker", email = "sam@kj7rrv.com"}]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 2 - Pre-Alpha",
```

