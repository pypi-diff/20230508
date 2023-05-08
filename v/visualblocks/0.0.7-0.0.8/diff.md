# Comparing `tmp/visualblocks-0.0.7.tar.gz` & `tmp/visualblocks-0.0.8.tar.gz`

## Comparing `visualblocks-0.0.7.tar` & `visualblocks-0.0.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 visualblocks-0.0.7/.editorconfig
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 visualblocks-0.0.7/src/visualblocks/__init__.py
--rw-r--r--   0        0        0    14606 2020-02-02 00:00:00.000000 visualblocks-0.0.7/src/visualblocks/server.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 visualblocks-0.0.7/.gitignore
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 visualblocks-0.0.7/README.pypi.md
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 visualblocks-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 visualblocks-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 visualblocks-0.0.8/.editorconfig
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 visualblocks-0.0.8/src/visualblocks/__init__.py
+-rw-r--r--   0        0        0    14606 2020-02-02 00:00:00.000000 visualblocks-0.0.8/src/visualblocks/server.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 visualblocks-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 visualblocks-0.0.8/README.pypi.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 visualblocks-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 visualblocks-0.0.8/PKG-INFO
```

### Comparing `visualblocks-0.0.7/src/visualblocks/server.py` & `visualblocks-0.0.8/src/visualblocks/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import shutil
 import sys
 import threading
 import traceback
 import urllib.parse
 import zipfile
 
-_VISUAL_BLOCKS_BUNDLE_VERSION = '1683325333'
+_VISUAL_BLOCKS_BUNDLE_VERSION = '1683568957'
 
 # Disable logging from werkzeug.
 #
 # Without this, flask will show a warning about using dev server (which is OK
 # in our usecase).
 logging.getLogger('werkzeug').disabled = True
```

### Comparing `visualblocks-0.0.7/README.pypi.md` & `visualblocks-0.0.8/README.pypi.md`

 * *Files identical despite different names*

### Comparing `visualblocks-0.0.7/pyproject.toml` & `visualblocks-0.0.8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "visualblocks"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Google LLC", email="opensource@google.com" },
 ]
 description = "Visual Blocks for Google Colaboratory"
 readme = "README.pypi.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `visualblocks-0.0.7/PKG-INFO` & `visualblocks-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualblocks
-Version: 0.0.7
+Version: 0.0.8
 Summary: Visual Blocks for Google Colaboratory
 Project-URL: Homepage, https://github.com/google/visualblocks
 Project-URL: Bug Tracker, https://github.com/google/visualblocks/issues
 Author-email: Google LLC <opensource@google.com>
 Classifier: Environment :: Other Environment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

