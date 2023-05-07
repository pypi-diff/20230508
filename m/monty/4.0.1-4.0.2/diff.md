# Comparing `tmp/monty-4.0.1.tar.gz` & `tmp/monty-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/monty-4.0.1.tar", last modified: Mon Oct 12 14:43:02 2020, max compression
+gzip compressed data, was "dist/monty-4.0.2.tar", last modified: Mon Oct 12 16:59:02 2020, max compression
```

## Comparing `monty-4.0.1.tar` & `monty-4.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2020-10-12 14:43:02.341287 monty-4.0.1/
--rw-r--r--   0 shyue      (501) staff       (20)     1088 2020-09-11 04:40:36.000000 monty-4.0.1/LICENSE.rst
--rw-r--r--   0 shyue      (501) staff       (20)       66 2020-09-11 04:40:36.000000 monty-4.0.1/MANIFEST.in
--rw-r--r--   0 shyue      (501) staff       (20)     2537 2020-10-12 14:43:02.341536 monty-4.0.1/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)     1466 2020-09-11 04:40:36.000000 monty-4.0.1/README.rst
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2020-10-12 14:43:02.336903 monty-4.0.1/monty/
--rw-r--r--   0 shyue      (501) staff       (20)      504 2020-10-12 14:41:04.000000 monty-4.0.1/monty/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     1489 2020-09-11 04:40:36.000000 monty-4.0.1/monty/bisect.py
--rw-r--r--   0 shyue      (501) staff       (20)     6623 2020-09-11 04:40:36.000000 monty-4.0.1/monty/collections.py
--rw-r--r--   0 shyue      (501) staff       (20)     3510 2020-09-11 04:40:36.000000 monty-4.0.1/monty/design_patterns.py
--rw-r--r--   0 shyue      (501) staff       (20)     6372 2020-10-12 14:38:29.000000 monty-4.0.1/monty/dev.py
--rw-r--r--   0 shyue      (501) staff       (20)     1474 2020-09-11 04:40:36.000000 monty-4.0.1/monty/fnmatch.py
--rw-r--r--   0 shyue      (501) staff       (20)     1370 2020-09-11 04:40:36.000000 monty-4.0.1/monty/fractions.py
--rw-r--r--   0 shyue      (501) staff       (20)    14265 2020-09-11 04:40:36.000000 monty-4.0.1/monty/functools.py
--rw-r--r--   0 shyue      (501) staff       (20)     3123 2020-09-11 04:40:36.000000 monty-4.0.1/monty/inspect.py
--rw-r--r--   0 shyue      (501) staff       (20)     9024 2020-09-11 04:40:36.000000 monty-4.0.1/monty/io.py
--rw-r--r--   0 shyue      (501) staff       (20)     2755 2020-09-11 04:40:36.000000 monty-4.0.1/monty/itertools.py
--rw-r--r--   0 shyue      (501) staff       (20)    15350 2020-09-11 04:40:36.000000 monty-4.0.1/monty/json.py
--rw-r--r--   0 shyue      (501) staff       (20)     2196 2020-09-11 04:40:36.000000 monty-4.0.1/monty/logging.py
--rw-r--r--   0 shyue      (501) staff       (20)      505 2020-09-11 04:40:36.000000 monty-4.0.1/monty/math.py
--rw-r--r--   0 shyue      (501) staff       (20)      672 2020-09-11 04:40:36.000000 monty-4.0.1/monty/msgpack.py
--rw-r--r--   0 shyue      (501) staff       (20)     1110 2020-09-11 04:40:36.000000 monty-4.0.1/monty/multiprocessing.py
--rw-r--r--   0 shyue      (501) staff       (20)      642 2020-09-11 04:40:36.000000 monty-4.0.1/monty/operator.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2020-10-12 14:43:02.340889 monty-4.0.1/monty/os/
--rw-r--r--   0 shyue      (501) staff       (20)     1233 2020-09-11 04:40:36.000000 monty-4.0.1/monty/os/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     3687 2020-09-11 04:40:36.000000 monty-4.0.1/monty/os/path.py
--rw-r--r--   0 shyue      (501) staff       (20)     2361 2020-09-11 04:40:36.000000 monty-4.0.1/monty/pprint.py
--rw-r--r--   0 shyue      (501) staff       (20)     1910 2020-09-11 04:40:36.000000 monty-4.0.1/monty/re.py
--rw-r--r--   0 shyue      (501) staff       (20)     5071 2020-09-11 04:40:36.000000 monty-4.0.1/monty/serialization.py
--rw-r--r--   0 shyue      (501) staff       (20)     4846 2020-09-11 04:40:36.000000 monty-4.0.1/monty/shutil.py
--rw-r--r--   0 shyue      (501) staff       (20)     3123 2020-09-11 04:40:36.000000 monty-4.0.1/monty/string.py
--rw-r--r--   0 shyue      (501) staff       (20)     2643 2020-09-11 04:40:36.000000 monty-4.0.1/monty/subprocess.py
--rw-r--r--   0 shyue      (501) staff       (20)     4235 2020-09-11 04:40:36.000000 monty-4.0.1/monty/tempfile.py
--rw-r--r--   0 shyue      (501) staff       (20)     5652 2020-09-11 04:40:36.000000 monty-4.0.1/monty/termcolor.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2020-10-12 14:43:02.339855 monty-4.0.1/monty.egg-info/
--rw-r--r--   0 shyue      (501) staff       (20)     2537 2020-10-12 14:43:02.000000 monty-4.0.1/monty.egg-info/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)      676 2020-10-12 14:43:02.000000 monty-4.0.1/monty.egg-info/SOURCES.txt
--rw-r--r--   0 shyue      (501) staff       (20)        1 2020-10-12 14:43:02.000000 monty-4.0.1/monty.egg-info/dependency_links.txt
--rw-r--r--   0 shyue      (501) staff       (20)       20 2020-10-12 14:43:02.000000 monty-4.0.1/monty.egg-info/requires.txt
--rw-r--r--   0 shyue      (501) staff       (20)       12 2020-10-12 14:43:02.000000 monty-4.0.1/monty.egg-info/top_level.txt
--rw-r--r--   0 shyue      (501) staff       (20)      619 2020-10-12 14:43:02.342717 monty-4.0.1/setup.cfg
--rw-r--r--   0 shyue      (501) staff       (20)     1200 2020-10-12 14:41:08.000000 monty-4.0.1/setup.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2020-10-12 16:59:02.757045 monty-4.0.2/
+-rw-r--r--   0 shyue      (501) staff       (20)     1088 2020-09-11 04:40:36.000000 monty-4.0.2/LICENSE.rst
+-rw-r--r--   0 shyue      (501) staff       (20)       66 2020-09-11 04:40:36.000000 monty-4.0.2/MANIFEST.in
+-rw-r--r--   0 shyue      (501) staff       (20)     2537 2020-10-12 16:59:02.757220 monty-4.0.2/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)     1466 2020-09-11 04:40:36.000000 monty-4.0.2/README.rst
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2020-10-12 16:59:02.754227 monty-4.0.2/monty/
+-rw-r--r--   0 shyue      (501) staff       (20)      505 2020-10-12 16:58:26.000000 monty-4.0.2/monty/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1489 2020-09-11 04:40:36.000000 monty-4.0.2/monty/bisect.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6623 2020-09-11 04:40:36.000000 monty-4.0.2/monty/collections.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3510 2020-09-11 04:40:36.000000 monty-4.0.2/monty/design_patterns.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6846 2020-10-12 16:53:38.000000 monty-4.0.2/monty/dev.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1474 2020-09-11 04:40:36.000000 monty-4.0.2/monty/fnmatch.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1370 2020-09-11 04:40:36.000000 monty-4.0.2/monty/fractions.py
+-rw-r--r--   0 shyue      (501) staff       (20)    14265 2020-09-11 04:40:36.000000 monty-4.0.2/monty/functools.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3123 2020-09-11 04:40:36.000000 monty-4.0.2/monty/inspect.py
+-rw-r--r--   0 shyue      (501) staff       (20)     9024 2020-09-11 04:40:36.000000 monty-4.0.2/monty/io.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2755 2020-09-11 04:40:36.000000 monty-4.0.2/monty/itertools.py
+-rw-r--r--   0 shyue      (501) staff       (20)    15350 2020-09-11 04:40:36.000000 monty-4.0.2/monty/json.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2196 2020-09-11 04:40:36.000000 monty-4.0.2/monty/logging.py
+-rw-r--r--   0 shyue      (501) staff       (20)      505 2020-09-11 04:40:36.000000 monty-4.0.2/monty/math.py
+-rw-r--r--   0 shyue      (501) staff       (20)      672 2020-09-11 04:40:36.000000 monty-4.0.2/monty/msgpack.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1110 2020-09-11 04:40:36.000000 monty-4.0.2/monty/multiprocessing.py
+-rw-r--r--   0 shyue      (501) staff       (20)      642 2020-09-11 04:40:36.000000 monty-4.0.2/monty/operator.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2020-10-12 16:59:02.756739 monty-4.0.2/monty/os/
+-rw-r--r--   0 shyue      (501) staff       (20)     1233 2020-09-11 04:40:36.000000 monty-4.0.2/monty/os/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3687 2020-09-11 04:40:36.000000 monty-4.0.2/monty/os/path.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2361 2020-09-11 04:40:36.000000 monty-4.0.2/monty/pprint.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1910 2020-09-11 04:40:36.000000 monty-4.0.2/monty/re.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5071 2020-09-11 04:40:36.000000 monty-4.0.2/monty/serialization.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4846 2020-09-11 04:40:36.000000 monty-4.0.2/monty/shutil.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3123 2020-09-11 04:40:36.000000 monty-4.0.2/monty/string.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2643 2020-09-11 04:40:36.000000 monty-4.0.2/monty/subprocess.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4235 2020-09-11 04:40:36.000000 monty-4.0.2/monty/tempfile.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5652 2020-09-11 04:40:36.000000 monty-4.0.2/monty/termcolor.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2020-10-12 16:59:02.755948 monty-4.0.2/monty.egg-info/
+-rw-r--r--   0 shyue      (501) staff       (20)     2537 2020-10-12 16:59:02.000000 monty-4.0.2/monty.egg-info/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)      676 2020-10-12 16:59:02.000000 monty-4.0.2/monty.egg-info/SOURCES.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        1 2020-10-12 16:59:02.000000 monty-4.0.2/monty.egg-info/dependency_links.txt
+-rw-r--r--   0 shyue      (501) staff       (20)       20 2020-10-12 16:59:02.000000 monty-4.0.2/monty.egg-info/requires.txt
+-rw-r--r--   0 shyue      (501) staff       (20)       12 2020-10-12 16:59:02.000000 monty-4.0.2/monty.egg-info/top_level.txt
+-rw-r--r--   0 shyue      (501) staff       (20)      619 2020-10-12 16:59:02.757985 monty-4.0.2/setup.cfg
+-rw-r--r--   0 shyue      (501) staff       (20)     1200 2020-10-12 16:54:08.000000 monty-4.0.2/setup.py
```

### Comparing `monty-4.0.1/LICENSE.rst` & `monty-4.0.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/PKG-INFO` & `monty-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monty
-Version: 4.0.1
+Version: 4.0.2
 Summary: Monty is the missing complement to Python.
 Home-page: https://github.com/materialsvirtuallab/monty
 Author: Shyue Ping Ong
 Author-email: ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 License: MIT
 Description: Monty: Python Made Even Easier
```

### Comparing `monty-4.0.1/README.rst` & `monty-4.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/bisect.py` & `monty-4.0.2/monty/bisect.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/collections.py` & `monty-4.0.2/monty/collections.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/design_patterns.py` & `monty-4.0.2/monty/design_patterns.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/dev.py` & `monty-4.0.2/monty/dev.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,22 +11,28 @@
 import subprocess
 import multiprocessing
 import functools
 
 logger = logging.getLogger(__name__)
 
 
-def deprecated(replacement=None, message=None):
+def deprecated(replacement=None, message=None, category=FutureWarning):
     """
     Decorator to mark classes or functions as deprecated,
     with a possible replacement.
 
     Args:
         replacement (callable): A replacement class or method.
         message (str): A warning message to be displayed.
+        category (Warning): Choose the category of the warning to issue. Defaults
+            to FutureWarning. Another choice can be DeprecationWarning. NOte that
+            FutureWarning is meant for end users and is always shown unless silenced.
+            DeprecationWarning is meant for developers and is never shown unless
+            python is run in developmental mode or the filter is changed. Make
+            the choice accordingly.
 
     Returns:
         Original function, but with a warning to use the updated class.
     """
 
     def wrap(old):
         def wrapped(*args, **kwargs):
@@ -37,15 +43,15 @@
                 elif isinstance(replacement, (classmethod, staticmethod)):
                     r = replacement.__func__
                 else:
                     r = replacement
                 msg += "; use %s in %s instead." % (r.__name__, r.__module__)
             if message is not None:
                 msg += "\n" + message
-            warnings.warn(msg, FutureWarning, stacklevel=2)
+            warnings.warn(msg, category=category, stacklevel=2)
             return old(*args, **kwargs)
 
         return wrapped
 
     return wrap
```

### Comparing `monty-4.0.1/monty/fnmatch.py` & `monty-4.0.2/monty/fnmatch.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/fractions.py` & `monty-4.0.2/monty/fractions.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/functools.py` & `monty-4.0.2/monty/functools.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/inspect.py` & `monty-4.0.2/monty/inspect.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/io.py` & `monty-4.0.2/monty/io.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/itertools.py` & `monty-4.0.2/monty/itertools.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/json.py` & `monty-4.0.2/monty/json.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/logging.py` & `monty-4.0.2/monty/logging.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/msgpack.py` & `monty-4.0.2/monty/msgpack.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/multiprocessing.py` & `monty-4.0.2/monty/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/operator.py` & `monty-4.0.2/monty/operator.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/os/__init__.py` & `monty-4.0.2/monty/os/__init__.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/os/path.py` & `monty-4.0.2/monty/os/path.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/pprint.py` & `monty-4.0.2/monty/pprint.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/re.py` & `monty-4.0.2/monty/re.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/serialization.py` & `monty-4.0.2/monty/serialization.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/shutil.py` & `monty-4.0.2/monty/shutil.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/string.py` & `monty-4.0.2/monty/string.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/subprocess.py` & `monty-4.0.2/monty/subprocess.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/tempfile.py` & `monty-4.0.2/monty/tempfile.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty/termcolor.py` & `monty-4.0.2/monty/termcolor.py`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/monty.egg-info/PKG-INFO` & `monty-4.0.2/monty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monty
-Version: 4.0.1
+Version: 4.0.2
 Summary: Monty is the missing complement to Python.
 Home-page: https://github.com/materialsvirtuallab/monty
 Author: Shyue Ping Ong
 Author-email: ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 License: MIT
 Description: Monty: Python Made Even Easier
```

### Comparing `monty-4.0.1/monty.egg-info/SOURCES.txt` & `monty-4.0.2/monty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/setup.cfg` & `monty-4.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `monty-4.0.1/setup.py` & `monty-4.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with io.open(os.path.join(current_dir, "README.rst"), "rt") as f:
     long_desc = f.read()
 
 setup(
     name="monty",
     packages=find_packages(),
-    version="4.0.1",
+    version="4.0.2",
     extras_require={"yaml": ["ruamel.yaml"], },
     package_data={},
     author="Shyue Ping Ong",
     author_email="ongsp@ucsd.edu",
     maintainer="Shyue Ping Ong",
     url="https://github.com/materialsvirtuallab/monty",
     license="MIT",
```

