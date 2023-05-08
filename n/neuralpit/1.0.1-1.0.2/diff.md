# Comparing `tmp/neuralpit-1.0.1.tar.gz` & `tmp/neuralpit-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralpit-1.0.1.tar", last modified: Mon May  8 14:25:37 2023, max compression
+gzip compressed data, was "neuralpit-1.0.2.tar", last modified: Mon May  8 17:13:59 2023, max compression
```

## Comparing `neuralpit-1.0.1.tar` & `neuralpit-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:25:37.209286 neuralpit-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 14:25:04.000000 neuralpit-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      520 2023-05-08 14:25:37.209286 neuralpit-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      130 2023-05-08 14:25:04.000000 neuralpit-1.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)      982 2023-05-08 14:25:04.000000 neuralpit-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 14:25:37.209286 neuralpit-1.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:25:37.209286 neuralpit-1.0.1/src/
--rw-r--r--   0 root         (0) root         (0)       61 2023-05-08 14:25:04.000000 neuralpit-1.0.1/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:25:37.209286 neuralpit-1.0.1/src/chat/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 14:25:04.000000 neuralpit-1.0.1/src/chat/config.toml
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-08 14:25:04.000000 neuralpit-1.0.1/src/chat/document.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:25:37.209286 neuralpit-1.0.1/src/neuralpit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      520 2023-05-08 14:25:37.000000 neuralpit-1.0.1/src/neuralpit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      278 2023-05-08 14:25:37.000000 neuralpit-1.0.1/src/neuralpit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 14:25:37.000000 neuralpit-1.0.1/src/neuralpit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-08 14:25:37.000000 neuralpit-1.0.1/src/neuralpit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-08 14:25:37.000000 neuralpit-1.0.1/src/neuralpit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:13:59.200994 neuralpit-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 17:13:20.000000 neuralpit-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      574 2023-05-08 17:13:59.200994 neuralpit-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      184 2023-05-08 17:13:20.000000 neuralpit-1.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      982 2023-05-08 17:13:20.000000 neuralpit-1.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 17:13:59.200994 neuralpit-1.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:13:59.200994 neuralpit-1.0.2/src/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-08 17:13:20.000000 neuralpit-1.0.2/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:13:59.200994 neuralpit-1.0.2/src/neuralpit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 17:13:20.000000 neuralpit-1.0.2/src/neuralpit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:13:59.200994 neuralpit-1.0.2/src/neuralpit/chat/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 17:13:20.000000 neuralpit-1.0.2/src/neuralpit/chat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-08 17:13:20.000000 neuralpit-1.0.2/src/neuralpit/chat/chatwithdocument.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:13:59.200994 neuralpit-1.0.2/src/neuralpit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      574 2023-05-08 17:13:59.000000 neuralpit-1.0.2/src/neuralpit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      332 2023-05-08 17:13:59.000000 neuralpit-1.0.2/src/neuralpit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 17:13:59.000000 neuralpit-1.0.2/src/neuralpit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-08 17:13:59.000000 neuralpit-1.0.2/src/neuralpit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-08 17:13:59.000000 neuralpit-1.0.2/src/neuralpit.egg-info/top_level.txt
```

### Comparing `neuralpit-1.0.1/PKG-INFO` & `neuralpit-1.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 1.0.1
+Version: 1.0.2
 Summary: NeuralPit API
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -12,7 +12,10 @@
 Provides-Extra: dev
 
 # Update version
 python -m pip install pip-tools
 pip install bumpver
 pip-compile --extra dev pyproject.toml
 bumpver update --minor
+
+# Install package locally
+python -m pip install -e .
```

### Comparing `neuralpit-1.0.1/pyproject.toml` & `neuralpit-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neuralpit"
-version = "1.0.1"
+version = "1.0.2"
 description = "NeuralPit API"
 readme = "README.md"
 authors = [{ name = "Quang Nguyen", email = "quang.nguyen@neuralpit.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `neuralpit-1.0.1/src/neuralpit.egg-info/PKG-INFO` & `neuralpit-1.0.2/src/neuralpit.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 1.0.1
+Version: 1.0.2
 Summary: NeuralPit API
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -12,7 +12,10 @@
 Provides-Extra: dev
 
 # Update version
 python -m pip install pip-tools
 pip install bumpver
 pip-compile --extra dev pyproject.toml
 bumpver update --minor
+
+# Install package locally
+python -m pip install -e .
```

