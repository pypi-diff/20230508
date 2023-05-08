# Comparing `tmp/sparkverse-0.0.1.tar.gz` & `tmp/sparkverse-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkverse-0.0.1.tar", last modified: Mon May  8 11:44:05 2023, max compression
+gzip compressed data, was "sparkverse-0.0.2.tar", last modified: Mon May  8 19:09:26 2023, max compression
```

## Comparing `sparkverse-0.0.1.tar` & `sparkverse-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-08 11:44:05.799536 sparkverse-0.0.1/
--rw-r--r--   0 root         (0) staff       (20)     1070 2023-05-08 11:23:02.000000 sparkverse-0.0.1/LICENSE
--rw-r--r--   0 root         (0) staff       (20)       37 2023-05-08 11:23:02.000000 sparkverse-0.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      423 2023-05-08 11:23:02.000000 sparkverse-0.0.1/NEWS.txt
--rw-r--r--   0 root         (0) staff       (20)     1031 2023-05-08 11:44:05.799269 sparkverse-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1023 2023-05-08 11:23:02.000000 sparkverse-0.0.1/README.md
--rw-r--r--   0 root         (0) staff       (20)       38 2023-05-08 11:44:05.799614 sparkverse-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     1425 2023-05-08 11:23:02.000000 sparkverse-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-08 11:44:05.791059 sparkverse-0.0.1/src/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-08 11:44:05.793742 sparkverse-0.0.1/src/sparkverse/
--rw-r--r--   0 root         (0) staff       (20)       84 2023-05-08 11:23:02.000000 sparkverse-0.0.1/src/sparkverse/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-08 11:44:05.798919 sparkverse-0.0.1/src/sparkverse/data/
--rwxr-xr-x   0 root         (0) staff       (20)    28453 2023-05-08 11:23:02.000000 sparkverse-0.0.1/src/sparkverse/data/Cropps1.png
--rwxr-xr-x   0 root         (0) staff       (20)    28684 2023-05-08 11:23:02.000000 sparkverse-0.0.1/src/sparkverse/data/Cropps2.png
--rwxr-xr-x   0 root         (0) staff       (20)    26184 2023-05-08 11:23:02.000000 sparkverse-0.0.1/src/sparkverse/data/LaneKeeper1.png
--rwxr-xr-x   0 root         (0) staff       (20)    26228 2023-05-08 11:23:02.000000 sparkverse-0.0.1/src/sparkverse/data/LaneKeeper2.png
--rwxr-xr-x   0 root         (0) staff       (20)    25273 2023-05-08 11:23:02.000000 sparkverse-0.0.1/src/sparkverse/data/LaneKeeper3.png
--rwxr-xr-x   0 root         (0) staff       (20)    76717 2023-05-08 11:23:02.000000 sparkverse-0.0.1/src/sparkverse/data/LineFollower1.png
--rwxr-xr-x   0 root         (0) staff       (20)    17710 2023-05-08 11:23:02.000000 sparkverse-0.0.1/src/sparkverse/data/LineFollower2.png
--rwxr-xr-x   0 root         (0) staff       (20)      152 2023-05-08 11:23:02.000000 sparkverse-0.0.1/src/sparkverse/data/player.png
--rw-r--r--   0 root         (0) staff       (20)      586 2023-05-08 11:23:02.000000 sparkverse-0.0.1/src/sparkverse/external_data.py
--rw-r--r--   0 root         (0) staff       (20)    10597 2023-05-08 11:23:02.000000 sparkverse-0.0.1/src/sparkverse/simulator.py
--rw-r--r--   0 root         (0) staff       (20)     2656 2023-05-08 11:23:02.000000 sparkverse-0.0.1/src/sparkverse/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-08 11:44:05.796135 sparkverse-0.0.1/src/sparkverse.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     1031 2023-05-08 11:44:05.000000 sparkverse-0.0.1/src/sparkverse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      704 2023-05-08 11:44:05.000000 sparkverse-0.0.1/src/sparkverse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-08 11:44:05.000000 sparkverse-0.0.1/src/sparkverse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       48 2023-05-08 11:44:05.000000 sparkverse-0.0.1/src/sparkverse.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-08 11:23:51.000000 sparkverse-0.0.1/src/sparkverse.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) staff       (20)       21 2023-05-08 11:44:05.000000 sparkverse-0.0.1/src/sparkverse.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       11 2023-05-08 11:44:05.000000 sparkverse-0.0.1/src/sparkverse.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-08 19:09:26.237297 sparkverse-0.0.2/
+-rw-r--r--   0 root         (0) staff       (20)     1070 2023-05-08 11:23:02.000000 sparkverse-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)       37 2023-05-08 11:23:02.000000 sparkverse-0.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      423 2023-05-08 11:23:02.000000 sparkverse-0.0.2/NEWS.txt
+-rw-r--r--   0 root         (0) staff       (20)     1031 2023-05-08 19:09:26.237025 sparkverse-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1023 2023-05-08 11:23:02.000000 sparkverse-0.0.2/README.md
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-05-08 19:09:26.237381 sparkverse-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     1425 2023-05-08 19:09:12.000000 sparkverse-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-08 19:09:26.228458 sparkverse-0.0.2/src/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-08 19:09:26.231666 sparkverse-0.0.2/src/sparkverse/
+-rw-r--r--   0 root         (0) staff       (20)       84 2023-05-08 11:23:02.000000 sparkverse-0.0.2/src/sparkverse/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-08 19:09:26.236667 sparkverse-0.0.2/src/sparkverse/data/
+-rwxr-xr-x   0 root         (0) staff       (20)    28453 2023-05-08 11:23:02.000000 sparkverse-0.0.2/src/sparkverse/data/Cropps1.png
+-rwxr-xr-x   0 root         (0) staff       (20)    28684 2023-05-08 11:23:02.000000 sparkverse-0.0.2/src/sparkverse/data/Cropps2.png
+-rwxr-xr-x   0 root         (0) staff       (20)    26184 2023-05-08 11:23:02.000000 sparkverse-0.0.2/src/sparkverse/data/LaneKeeper1.png
+-rwxr-xr-x   0 root         (0) staff       (20)    26228 2023-05-08 11:23:02.000000 sparkverse-0.0.2/src/sparkverse/data/LaneKeeper2.png
+-rwxr-xr-x   0 root         (0) staff       (20)    25273 2023-05-08 11:23:02.000000 sparkverse-0.0.2/src/sparkverse/data/LaneKeeper3.png
+-rwxr-xr-x   0 root         (0) staff       (20)    76717 2023-05-08 11:23:02.000000 sparkverse-0.0.2/src/sparkverse/data/LineFollower1.png
+-rwxr-xr-x   0 root         (0) staff       (20)    17710 2023-05-08 11:23:02.000000 sparkverse-0.0.2/src/sparkverse/data/LineFollower2.png
+-rwxr-xr-x   0 root         (0) staff       (20)      152 2023-05-08 11:23:02.000000 sparkverse-0.0.2/src/sparkverse/data/player.png
+-rw-r--r--   0 root         (0) staff       (20)      586 2023-05-08 11:23:02.000000 sparkverse-0.0.2/src/sparkverse/external_data.py
+-rw-r--r--   0 root         (0) staff       (20)    10597 2023-05-08 11:23:02.000000 sparkverse-0.0.2/src/sparkverse/simulator.py
+-rw-r--r--   0 root         (0) staff       (20)     2656 2023-05-08 11:23:02.000000 sparkverse-0.0.2/src/sparkverse/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-08 19:09:26.233867 sparkverse-0.0.2/src/sparkverse.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     1031 2023-05-08 19:09:26.000000 sparkverse-0.0.2/src/sparkverse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      704 2023-05-08 19:09:26.000000 sparkverse-0.0.2/src/sparkverse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-08 19:09:26.000000 sparkverse-0.0.2/src/sparkverse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       48 2023-05-08 19:09:26.000000 sparkverse-0.0.2/src/sparkverse.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-08 11:23:51.000000 sparkverse-0.0.2/src/sparkverse.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) staff       (20)       21 2023-05-08 19:09:26.000000 sparkverse-0.0.2/src/sparkverse.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       11 2023-05-08 19:09:26.000000 sparkverse-0.0.2/src/sparkverse.egg-info/top_level.txt
```

### Comparing `sparkverse-0.0.1/LICENSE` & `sparkverse-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.1/PKG-INFO` & `sparkverse-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkverse
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple python3 simulator for advance driving systems
 Home-page: https://github.com/Amporu/SparkVerse
 Author: Tucudean Adrian-Ionut
 Author-email: Tucudean.Adrian.Ionut0@gmail.com
 License: MIT
 Keywords: Simulator computer vision Advanced Driving
 Classifier: Development Status :: 1 - Planning
```

### Comparing `sparkverse-0.0.1/README.md` & `sparkverse-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.1/setup.py` & `sparkverse-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys, os
 
 here = os.path.abspath(os.path.dirname(__file__))
 #README = open(os.path.join(here, 'README-pypi.rst')).read()
 NEWS = open(os.path.join(here, 'NEWS.txt')).read()
 
 
-version = '0.0.1'
+version = '0.0.2'
 
 install_requires = [
     # List your project dependencies here.
     # For more details, see:
     # http://packages.python.org/distribute/setuptools.html#declaring-dependencies
     'requests'	
 ]
```

### Comparing `sparkverse-0.0.1/src/sparkverse/data/Cropps1.png` & `sparkverse-0.0.2/src/sparkverse/data/Cropps1.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.1/src/sparkverse/data/Cropps2.png` & `sparkverse-0.0.2/src/sparkverse/data/Cropps2.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.1/src/sparkverse/data/LaneKeeper1.png` & `sparkverse-0.0.2/src/sparkverse/data/LaneKeeper1.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.1/src/sparkverse/data/LaneKeeper2.png` & `sparkverse-0.0.2/src/sparkverse/data/LaneKeeper2.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.1/src/sparkverse/data/LaneKeeper3.png` & `sparkverse-0.0.2/src/sparkverse/data/LaneKeeper3.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.1/src/sparkverse/data/LineFollower1.png` & `sparkverse-0.0.2/src/sparkverse/data/LineFollower1.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.1/src/sparkverse/data/LineFollower2.png` & `sparkverse-0.0.2/src/sparkverse/data/LineFollower2.png`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.1/src/sparkverse/external_data.py` & `sparkverse-0.0.2/src/sparkverse/external_data.py`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.1/src/sparkverse/simulator.py` & `sparkverse-0.0.2/src/sparkverse/simulator.py`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.1/src/sparkverse/utils.py` & `sparkverse-0.0.2/src/sparkverse/utils.py`

 * *Files identical despite different names*

### Comparing `sparkverse-0.0.1/src/sparkverse.egg-info/PKG-INFO` & `sparkverse-0.0.2/src/sparkverse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkverse
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple python3 simulator for advance driving systems
 Home-page: https://github.com/Amporu/SparkVerse
 Author: Tucudean Adrian-Ionut
 Author-email: Tucudean.Adrian.Ionut0@gmail.com
 License: MIT
 Keywords: Simulator computer vision Advanced Driving
 Classifier: Development Status :: 1 - Planning
```

### Comparing `sparkverse-0.0.1/src/sparkverse.egg-info/SOURCES.txt` & `sparkverse-0.0.2/src/sparkverse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

