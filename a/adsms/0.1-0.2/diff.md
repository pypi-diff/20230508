# Comparing `tmp/adsms-0.1.tar.gz` & `tmp/adsms-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adsms-0.1.tar", last modified: Mon May  8 15:12:22 2023, max compression
+gzip compressed data, was "adsms-0.2.tar", last modified: Mon May  8 17:10:33 2023, max compression
```

## Comparing `adsms-0.1.tar` & `adsms-0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 kj7rrv    (1000) kj7rrv    (1000)        0 2023-05-08 15:12:22.979833 adsms-0.1/
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)    34020 2023-05-04 19:33:40.000000 adsms-0.1/LICENSE
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)     2701 2023-05-08 15:12:22.979833 adsms-0.1/PKG-INFO
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)     2192 2023-05-06 01:37:05.000000 adsms-0.1/README.md
-drwxrwxr-x   0 kj7rrv    (1000) kj7rrv    (1000)        0 2023-05-08 15:12:22.979833 adsms-0.1/adsms/
--rwxrwxr-x   0 kj7rrv    (1000) kj7rrv    (1000)     2263 2023-05-08 01:47:00.000000 adsms-0.1/adsms/__init__.py
-drwxrwxr-x   0 kj7rrv    (1000) kj7rrv    (1000)        0 2023-05-08 15:12:22.979833 adsms-0.1/adsms.egg-info/
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)     2701 2023-05-08 15:12:22.000000 adsms-0.1/adsms.egg-info/PKG-INFO
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)      226 2023-05-08 15:12:22.000000 adsms-0.1/adsms.egg-info/SOURCES.txt
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)        1 2023-05-08 15:12:22.000000 adsms-0.1/adsms.egg-info/dependency_links.txt
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)       37 2023-05-08 15:12:22.000000 adsms-0.1/adsms.egg-info/entry_points.txt
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)        9 2023-05-08 15:12:22.000000 adsms-0.1/adsms.egg-info/requires.txt
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)        6 2023-05-08 15:12:22.000000 adsms-0.1/adsms.egg-info/top_level.txt
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)      700 2023-05-08 15:12:10.000000 adsms-0.1/pyproject.toml
--rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)       38 2023-05-08 15:12:22.979833 adsms-0.1/setup.cfg
+drwxrwxr-x   0 kj7rrv    (1000) kj7rrv    (1000)        0 2023-05-08 17:10:33.879735 adsms-0.2/
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)    34020 2023-05-04 19:33:40.000000 adsms-0.2/LICENSE
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)        8 2023-05-08 17:09:57.000000 adsms-0.2/MANIFEST.in
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)     2701 2023-05-08 17:10:33.879735 adsms-0.2/PKG-INFO
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)     2192 2023-05-06 01:37:05.000000 adsms-0.2/README.md
+drwxrwxr-x   0 kj7rrv    (1000) kj7rrv    (1000)        0 2023-05-08 17:10:33.875735 adsms-0.2/adsms/
+-rwxrwxr-x   0 kj7rrv    (1000) kj7rrv    (1000)     2263 2023-05-08 01:47:00.000000 adsms-0.2/adsms/__init__.py
+drwxrwxr-x   0 kj7rrv    (1000) kj7rrv    (1000)        0 2023-05-08 17:10:33.875735 adsms-0.2/adsms.egg-info/
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)     2701 2023-05-08 17:10:33.000000 adsms-0.2/adsms.egg-info/PKG-INFO
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)      238 2023-05-08 17:10:33.000000 adsms-0.2/adsms.egg-info/SOURCES.txt
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)        1 2023-05-08 17:10:33.000000 adsms-0.2/adsms.egg-info/dependency_links.txt
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)       37 2023-05-08 17:10:33.000000 adsms-0.2/adsms.egg-info/entry_points.txt
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)        9 2023-05-08 17:10:33.000000 adsms-0.2/adsms.egg-info/requires.txt
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)        6 2023-05-08 17:10:33.000000 adsms-0.2/adsms.egg-info/top_level.txt
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)      700 2023-05-08 17:10:19.000000 adsms-0.2/pyproject.toml
+-rw-rw-r--   0 kj7rrv    (1000) kj7rrv    (1000)       38 2023-05-08 17:10:33.879735 adsms-0.2/setup.cfg
```

### Comparing `adsms-0.1/LICENSE` & `adsms-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adsms-0.1/PKG-INFO` & `adsms-0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsms
-Version: 0.1
+Version: 0.2
 Summary: Send SMS aircraft alerts based on ADS-B data
 Author-email: Samuel Sloniker <sam@kj7rrv.com>
 Project-URL: Homepage, https://git.kj7rrv.com/kj7rrv/adsms
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `adsms-0.1/README.md` & `adsms-0.2/README.md`

 * *Files identical despite different names*

### Comparing `adsms-0.1/adsms/__init__.py` & `adsms-0.2/adsms/__init__.py`

 * *Files identical despite different names*

### Comparing `adsms-0.1/adsms.egg-info/PKG-INFO` & `adsms-0.2/adsms.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsms
-Version: 0.1
+Version: 0.2
 Summary: Send SMS aircraft alerts based on ADS-B data
 Author-email: Samuel Sloniker <sam@kj7rrv.com>
 Project-URL: Homepage, https://git.kj7rrv.com/kj7rrv/adsms
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `adsms-0.1/pyproject.toml` & `adsms-0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "adsms"
-version = "0.1"
+version = "0.2"
 description = "Send SMS aircraft alerts based on ADS-B data"
 readme = "README.md"
 authors = [{ name = "Samuel Sloniker", email = "sam@kj7rrv.com"}]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 2 - Pre-Alpha",
```

