# Comparing `tmp/circuitpython-ArrowLine-1.0.0.tar.gz` & `tmp/circuitpython-ArrowLine-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-ArrowLine-1.0.0.tar", last modified: Mon May  8 02:39:07 2023, max compression
+gzip compressed data, was "circuitpython-ArrowLine-1.0.1.tar", last modified: Mon May  8 01:51:14 2023, max compression
```

## Comparing `circuitpython-ArrowLine-1.0.0.tar` & `circuitpython-ArrowLine-1.0.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 02:39:07.849213 circuitpython-ArrowLine-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 02:39:07.841213 circuitpython-ArrowLine-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 02:39:07.845213 circuitpython-ArrowLine-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 02:39:07.845213 circuitpython-ArrowLine-1.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-08 02:39:07.849213 circuitpython-ArrowLine-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/README.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (123)    10952 2023-05-08 02:38:59.000000 circuitpython-ArrowLine-1.0.0/arrowline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 02:39:07.845213 circuitpython-ArrowLine-1.0.0/circuitpython_ArrowLine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-08 02:39:07.000000 circuitpython-ArrowLine-1.0.0/circuitpython_ArrowLine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-08 02:39:07.000000 circuitpython-ArrowLine-1.0.0/circuitpython_ArrowLine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 02:39:07.000000 circuitpython-ArrowLine-1.0.0/circuitpython_ArrowLine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 02:39:07.000000 circuitpython-ArrowLine-1.0.0/circuitpython_ArrowLine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-08 02:39:07.000000 circuitpython-ArrowLine-1.0.0/circuitpython_ArrowLine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 02:39:07.845213 circuitpython-ArrowLine-1.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 02:39:07.845213 circuitpython-ArrowLine-1.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 02:39:07.849213 circuitpython-ArrowLine-1.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-08 02:38:59.000000 circuitpython-ArrowLine-1.0.0/examples/arrowline_dotted.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-08 02:38:59.000000 circuitpython-ArrowLine-1.0.0/examples/arrowline_multiple_arrows.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-08 02:38:59.000000 circuitpython-ArrowLine-1.0.0/examples/arrowline_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-08 02:38:59.000000 circuitpython-ArrowLine-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-08 02:38:45.000000 circuitpython-ArrowLine-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 02:39:07.849213 circuitpython-ArrowLine-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.028372 circuitpython-ArrowLine-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.020372 circuitpython-ArrowLine-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.024371 circuitpython-ArrowLine-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.024371 circuitpython-ArrowLine-1.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-08 01:51:14.028372 circuitpython-ArrowLine-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/README.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10952 2023-05-08 01:51:03.000000 circuitpython-ArrowLine-1.0.1/arrowline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.024371 circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-08 01:51:13.000000 circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-08 01:51:14.000000 circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 01:51:13.000000 circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 01:51:13.000000 circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 01:51:13.000000 circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.028372 circuitpython-ArrowLine-1.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.028372 circuitpython-ArrowLine-1.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.028372 circuitpython-ArrowLine-1.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-08 01:51:03.000000 circuitpython-ArrowLine-1.0.1/examples/arrowline_dotted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-08 01:51:03.000000 circuitpython-ArrowLine-1.0.1/examples/arrowline_multiple_arrows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-08 01:51:03.000000 circuitpython-ArrowLine-1.0.1/examples/arrowline_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-08 01:51:03.000000 circuitpython-ArrowLine-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 01:51:14.028372 circuitpython-ArrowLine-1.0.1/setup.cfg
```

### Comparing `circuitpython-ArrowLine-1.0.0/.pre-commit-config.yaml` & `circuitpython-ArrowLine-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.0/.pylintrc` & `circuitpython-ArrowLine-1.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.0/CODE_OF_CONDUCT.md` & `circuitpython-ArrowLine-1.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.0/LICENSE` & `circuitpython-ArrowLine-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.0/LICENSES/CC-BY-4.0.txt` & `circuitpython-ArrowLine-1.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.0/LICENSES/MIT.txt` & `circuitpython-ArrowLine-1.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.0/LICENSES/Unlicense.txt` & `circuitpython-ArrowLine-1.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.0/PKG-INFO` & `circuitpython-ArrowLine-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-ArrowLine
-Version: 1.0.0
+Version: 1.0.1
 Summary: CircuitPython library to draw Arrowlines.
 Author-email: "Jose D. Montoya" <arrowline@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_ArrowLine.git
 Keywords: hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-ArrowLine-1.0.0/README.rst` & `circuitpython-ArrowLine-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.0/arrowline.py` & `circuitpython-ArrowLine-1.0.1/arrowline.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from vectorio import Polygon, Circle
 
 try:
     from typing import Optional
 except ImportError:
     pass
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __repo__ = "https://github.com/jposada202020/CircuitPython_ArrowLine.git"
 
 
 class Line:
 
     """A Line Arrow utility.
```

### Comparing `circuitpython-ArrowLine-1.0.0/circuitpython_ArrowLine.egg-info/PKG-INFO` & `circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-ArrowLine
-Version: 1.0.0
+Version: 1.0.1
 Summary: CircuitPython library to draw Arrowlines.
 Author-email: "Jose D. Montoya" <arrowline@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_ArrowLine.git
 Keywords: hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-ArrowLine-1.0.0/circuitpython_ArrowLine.egg-info/SOURCES.txt` & `circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.0/docs/_static/favicon.ico` & `circuitpython-ArrowLine-1.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.0/docs/conf.py` & `circuitpython-ArrowLine-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.0/docs/examples.rst` & `circuitpython-ArrowLine-1.0.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.0/examples/arrowline_dotted.py` & `circuitpython-ArrowLine-1.0.1/examples/arrowline_dotted.py`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.0/examples/arrowline_multiple_arrows.py` & `circuitpython-ArrowLine-1.0.1/examples/arrowline_multiple_arrows.py`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.0/examples/arrowline_simpletest.py` & `circuitpython-ArrowLine-1.0.1/examples/arrowline_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.0/pyproject.toml` & `circuitpython-ArrowLine-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-ArrowLine"
 description = "CircuitPython library to draw Arrowlines."
-version = "1.0.0"
+version = "1.0.1"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "arrowline@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_ArrowLine.git"}
 keywords = [
     "hardware",
@@ -31,12 +31,12 @@
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["CircuitPython_Arrowline"]
+py-modules = ["arrowline"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 optional-dependencies = {optional = {file = ["optional_requirements.txt"]}}
```

