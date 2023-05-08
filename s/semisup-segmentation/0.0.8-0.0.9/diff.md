# Comparing `tmp/semisup-segmentation-0.0.8.tar.gz` & `tmp/semisup-segmentation-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/semisup-segmentation-0.0.8.tar", last modified: Wed May  3 11:40:43 2023, max compression
+gzip compressed data, was "dist/semisup-segmentation-0.0.9.tar", last modified: Wed May  3 11:47:54 2023, max compression
```

## Comparing `semisup-segmentation-0.0.8.tar` & `semisup-segmentation-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 11:40:43.000000 semisup-segmentation-0.0.8/
--rw-rw-r--   0 adines    (1000) adines    (1000)      635 2023-05-03 11:40:43.000000 semisup-segmentation-0.0.8/PKG-INFO
--rw-rw-r--   0 adines    (1000) adines    (1000)     1071 2020-12-11 12:52:05.000000 semisup-segmentation-0.0.8/LICENSE.txt
--rw-rw-r--   0 adines    (1000) adines    (1000)     1197 2020-12-16 16:41:18.000000 semisup-segmentation-0.0.8/README.rst
-drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 11:40:43.000000 semisup-segmentation-0.0.8/semisup_segmentation.egg-info/
--rw-rw-r--   0 adines    (1000) adines    (1000)      635 2023-05-03 11:40:43.000000 semisup-segmentation-0.0.8/semisup_segmentation.egg-info/PKG-INFO
--rw-rw-r--   0 adines    (1000) adines    (1000)       87 2023-05-03 11:40:43.000000 semisup-segmentation-0.0.8/semisup_segmentation.egg-info/requires.txt
--rw-rw-r--   0 adines    (1000) adines    (1000)        1 2023-05-03 11:40:43.000000 semisup-segmentation-0.0.8/semisup_segmentation.egg-info/dependency_links.txt
--rw-rw-r--   0 adines    (1000) adines    (1000)      344 2023-05-03 11:40:43.000000 semisup-segmentation-0.0.8/semisup_segmentation.egg-info/SOURCES.txt
--rw-rw-r--   0 adines    (1000) adines    (1000)       11 2023-05-03 11:40:43.000000 semisup-segmentation-0.0.8/semisup_segmentation.egg-info/top_level.txt
--rw-rw-r--   0 adines    (1000) adines    (1000)     8410 2023-05-03 11:40:40.000000 semisup-segmentation-0.0.8/setup.py
--rw-rw-r--   0 adines    (1000) adines    (1000)       46 2020-12-11 12:52:32.000000 semisup-segmentation-0.0.8/MANIFEST.in
--rw-rw-r--   0 adines    (1000) adines    (1000)       67 2023-05-03 11:40:43.000000 semisup-segmentation-0.0.8/setup.cfg
-drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 11:40:43.000000 semisup-segmentation-0.0.8/SemiSegAPI/
--rw-rw-r--   0 adines    (1000) adines    (1000)     8342 2023-05-02 16:24:16.000000 semisup-segmentation-0.0.8/SemiSegAPI/semiSupervised.py
--rw-rw-r--   0 adines    (1000) adines    (1000)      249 2023-05-03 11:25:10.000000 semisup-segmentation-0.0.8/SemiSegAPI/__init__.py
--rw-rw-r--   0 adines    (1000) adines    (1000)    10397 2023-05-03 07:51:02.000000 semisup-segmentation-0.0.8/SemiSegAPI/utils.py
+drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 11:47:54.000000 semisup-segmentation-0.0.9/
+-rw-rw-r--   0 adines    (1000) adines    (1000)      635 2023-05-03 11:47:54.000000 semisup-segmentation-0.0.9/PKG-INFO
+-rw-rw-r--   0 adines    (1000) adines    (1000)     1071 2020-12-11 12:52:05.000000 semisup-segmentation-0.0.9/LICENSE.txt
+-rw-rw-r--   0 adines    (1000) adines    (1000)     1197 2020-12-16 16:41:18.000000 semisup-segmentation-0.0.9/README.rst
+drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 11:47:54.000000 semisup-segmentation-0.0.9/semisup_segmentation.egg-info/
+-rw-rw-r--   0 adines    (1000) adines    (1000)      635 2023-05-03 11:47:53.000000 semisup-segmentation-0.0.9/semisup_segmentation.egg-info/PKG-INFO
+-rw-rw-r--   0 adines    (1000) adines    (1000)       93 2023-05-03 11:47:53.000000 semisup-segmentation-0.0.9/semisup_segmentation.egg-info/requires.txt
+-rw-rw-r--   0 adines    (1000) adines    (1000)        1 2023-05-03 11:47:53.000000 semisup-segmentation-0.0.9/semisup_segmentation.egg-info/dependency_links.txt
+-rw-rw-r--   0 adines    (1000) adines    (1000)      344 2023-05-03 11:47:53.000000 semisup-segmentation-0.0.9/semisup_segmentation.egg-info/SOURCES.txt
+-rw-rw-r--   0 adines    (1000) adines    (1000)       11 2023-05-03 11:47:53.000000 semisup-segmentation-0.0.9/semisup_segmentation.egg-info/top_level.txt
+-rw-rw-r--   0 adines    (1000) adines    (1000)     8410 2023-05-03 11:47:49.000000 semisup-segmentation-0.0.9/setup.py
+-rw-rw-r--   0 adines    (1000) adines    (1000)       46 2020-12-11 12:52:32.000000 semisup-segmentation-0.0.9/MANIFEST.in
+-rw-rw-r--   0 adines    (1000) adines    (1000)       67 2023-05-03 11:47:54.000000 semisup-segmentation-0.0.9/setup.cfg
+drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 11:47:54.000000 semisup-segmentation-0.0.9/SemiSegAPI/
+-rw-rw-r--   0 adines    (1000) adines    (1000)     8342 2023-05-02 16:24:16.000000 semisup-segmentation-0.0.9/SemiSegAPI/semiSupervised.py
+-rw-rw-r--   0 adines    (1000) adines    (1000)      249 2023-05-03 11:25:10.000000 semisup-segmentation-0.0.9/SemiSegAPI/__init__.py
+-rw-rw-r--   0 adines    (1000) adines    (1000)    10397 2023-05-03 07:51:02.000000 semisup-segmentation-0.0.9/SemiSegAPI/utils.py
```

### Comparing `semisup-segmentation-0.0.8/PKG-INFO` & `semisup-segmentation-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semisup-segmentation
-Version: 0.0.8
+Version: 0.0.9
 Summary: API that provides methods to construct deep segmentation models using semi-supervised methods.
 Home-page: https://github.com/adines/SemiSeg
 Author: Adrian Ines
 Author-email: adines@unirioja.es
 License: UNKNOWN
 Keywords: segmentation,deep learning,semi-supervised
 Platform: UNKNOWN
```

### Comparing `semisup-segmentation-0.0.8/LICENSE.txt` & `semisup-segmentation-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `semisup-segmentation-0.0.8/README.rst` & `semisup-segmentation-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `semisup-segmentation-0.0.8/semisup_segmentation.egg-info/PKG-INFO` & `semisup-segmentation-0.0.9/semisup_segmentation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semisup-segmentation
-Version: 0.0.8
+Version: 0.0.9
 Summary: API that provides methods to construct deep segmentation models using semi-supervised methods.
 Home-page: https://github.com/adines/SemiSeg
 Author: Adrian Ines
 Author-email: adines@unirioja.es
 License: UNKNOWN
 Keywords: segmentation,deep learning,semi-supervised
 Platform: UNKNOWN
```

### Comparing `semisup-segmentation-0.0.8/setup.py` & `semisup-segmentation-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.8',  # Required
+    version='0.0.9',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='API that provides methods to construct deep segmentation models using semi-supervised methods.',  # Required
 
     # This is an optional longer description of your project that represents
```

### Comparing `semisup-segmentation-0.0.8/SemiSegAPI/semiSupervised.py` & `semisup-segmentation-0.0.9/SemiSegAPI/semiSupervised.py`

 * *Files identical despite different names*

### Comparing `semisup-segmentation-0.0.8/SemiSegAPI/utils.py` & `semisup-segmentation-0.0.9/SemiSegAPI/utils.py`

 * *Files identical despite different names*

