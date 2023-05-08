# Comparing `tmp/modelbase_pde-0.2.8.tar.gz` & `tmp/modelbase_pde-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelbase_pde-0.2.8.tar", max compression
+gzip compressed data, was "modelbase_pde-0.2.9.tar", max compression
```

## Comparing `modelbase_pde-0.2.8.tar` & `modelbase_pde-0.2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35753 2022-12-12 08:42:35.099220 modelbase_pde-0.2.8/LICENSE
--rw-r--r--   0        0        0      816 2022-12-12 08:42:35.099220 modelbase_pde-0.2.8/README.md
--rw-r--r--   0        0        0      513 2022-12-12 08:42:35.099220 modelbase_pde-0.2.8/build.py
--rw-r--r--   0        0        0     1186 2022-12-12 08:42:35.101220 modelbase_pde-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      144 2022-12-12 08:42:35.101220 modelbase_pde-0.2.8/src/modelbase_pde/__init__.py
--rw-r--r--   0        0        0    13347 2022-12-12 08:42:35.101220 modelbase_pde-0.2.8/src/modelbase_pde/basemodels.py
--rw-r--r--   0        0        0    19838 2022-12-12 08:42:35.101220 modelbase_pde-0.2.8/src/modelbase_pde/leafmodels.py
--rw-r--r--   0        0        0      150 2022-12-12 08:42:35.101220 modelbase_pde-0.2.8/src/modelbase_pde/utils/__init__.py
--rw-r--r--   0        0        0    14344 2022-12-12 08:42:35.101220 modelbase_pde-0.2.8/src/modelbase_pde/utils/coordinates.py
--rw-r--r--   0        0        0     3270 2022-12-12 08:42:35.101220 modelbase_pde-0.2.8/src/modelbase_pde/utils/perffuncs.cpp
--rw-r--r--   0        0        0     1974 2022-12-12 08:42:35.101220 modelbase_pde-0.2.8/src/modelbase_pde/utils/perffuncs.py
--rw-r--r--   0        0        0     5007 2022-12-12 08:42:35.101220 modelbase_pde-0.2.8/src/modelbase_pde/utils/plotting.py
--rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 modelbase_pde-0.2.8/setup.py
--rw-r--r--   0        0        0     1464 1970-01-01 00:00:00.000000 modelbase_pde-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    35753 2022-12-27 08:49:10.519823 modelbase_pde-0.2.9/LICENSE
+-rw-r--r--   0        0        0      816 2022-12-27 08:49:10.519823 modelbase_pde-0.2.9/README.md
+-rw-r--r--   0        0        0      513 2022-12-27 08:49:10.520823 modelbase_pde-0.2.9/build.py
+-rw-r--r--   0        0        0     1186 2022-12-27 08:49:10.522823 modelbase_pde-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      144 2022-12-27 08:49:10.522823 modelbase_pde-0.2.9/src/modelbase_pde/__init__.py
+-rw-r--r--   0        0        0    13347 2022-12-27 08:49:10.522823 modelbase_pde-0.2.9/src/modelbase_pde/basemodels.py
+-rw-r--r--   0        0        0    19838 2022-12-27 08:49:10.522823 modelbase_pde-0.2.9/src/modelbase_pde/leafmodels.py
+-rw-r--r--   0        0        0      150 2022-12-27 08:49:10.522823 modelbase_pde-0.2.9/src/modelbase_pde/utils/__init__.py
+-rw-r--r--   0        0        0    14344 2022-12-27 08:49:10.522823 modelbase_pde-0.2.9/src/modelbase_pde/utils/coordinates.py
+-rw-r--r--   0        0        0     3270 2022-12-27 08:49:10.522823 modelbase_pde-0.2.9/src/modelbase_pde/utils/perffuncs.cpp
+-rw-r--r--   0        0        0     1974 2022-12-27 08:49:10.522823 modelbase_pde-0.2.9/src/modelbase_pde/utils/perffuncs.py
+-rw-r--r--   0        0        0     5007 2022-12-27 08:49:10.522823 modelbase_pde-0.2.9/src/modelbase_pde/utils/plotting.py
+-rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 modelbase_pde-0.2.9/setup.py
+-rw-r--r--   0        0        0     1464 1970-01-01 00:00:00.000000 modelbase_pde-0.2.9/PKG-INFO
```

### Comparing `modelbase_pde-0.2.8/LICENSE` & `modelbase_pde-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `modelbase_pde-0.2.8/README.md` & `modelbase_pde-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `modelbase_pde-0.2.8/build.py` & `modelbase_pde-0.2.9/build.py`

 * *Files identical despite different names*

### Comparing `modelbase_pde-0.2.8/pyproject.toml` & `modelbase_pde-0.2.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelbase-pde"
-version = "0.2.8"
+version = "0.2.9"
 description = "A subpackage of modelbase that enables investigation of PDE models"
 authors = ["Marvin van Aalst <marvin.vanaalst@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "modelbase_pde", from = "src" }
 ]
```

### Comparing `modelbase_pde-0.2.8/src/modelbase_pde/basemodels.py` & `modelbase_pde-0.2.9/src/modelbase_pde/basemodels.py`

 * *Files identical despite different names*

### Comparing `modelbase_pde-0.2.8/src/modelbase_pde/leafmodels.py` & `modelbase_pde-0.2.9/src/modelbase_pde/leafmodels.py`

 * *Files identical despite different names*

### Comparing `modelbase_pde-0.2.8/src/modelbase_pde/utils/coordinates.py` & `modelbase_pde-0.2.9/src/modelbase_pde/utils/coordinates.py`

 * *Files identical despite different names*

### Comparing `modelbase_pde-0.2.8/src/modelbase_pde/utils/perffuncs.cpp` & `modelbase_pde-0.2.9/src/modelbase_pde/utils/perffuncs.cpp`

 * *Files identical despite different names*

### Comparing `modelbase_pde-0.2.8/src/modelbase_pde/utils/perffuncs.py` & `modelbase_pde-0.2.9/src/modelbase_pde/utils/perffuncs.py`

 * *Files identical despite different names*

### Comparing `modelbase_pde-0.2.8/src/modelbase_pde/utils/plotting.py` & `modelbase_pde-0.2.9/src/modelbase_pde/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `modelbase_pde-0.2.8/setup.py` & `modelbase_pde-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 install_requires = \
 ['modelbase>=1.18.9,<2.0.0',
  'pybind11>=2.10.0,<3.0.0',
  'setuptools>=65.4.0,<66.0.0']
 
 setup_kwargs = {
     'name': 'modelbase-pde',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'A subpackage of modelbase that enables investigation of PDE models',
     'long_description': '# modelbase pde\n\n[![pipeline status](https://gitlab.com/marvin.vanaalst/modelbase-pde/badges/main/pipeline.svg)](https://gitlab.com/marvin.vanaalst/modelbase-pde/-/commits/main)\n[![coverage report](https://gitlab.com/marvin.vanaalst/modelbase-pde/badges/main/coverage.svg)](https://gitlab.com/marvin.vanaalst/modelbase-pde/-/commits/main)\n[![PyPi](https://img.shields.io/pypi/v/modelbase-pde)](https://pypi.org/project/modelbase-pde/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n[![Downloads](https://pepy.tech/badge/modelbase-pde)](https://pepy.tech/project/modelbase-pde)\n\nSubpackage of the [modelbase](https://gitlab.com/ebenhoeh/modelbase) package.\n',
     'author': 'Marvin van Aalst',
     'author_email': 'marvin.vanaalst@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `modelbase_pde-0.2.8/PKG-INFO` & `modelbase_pde-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelbase-pde
-Version: 0.2.8
+Version: 0.2.9
 Summary: A subpackage of modelbase that enables investigation of PDE models
 Author: Marvin van Aalst
 Author-email: marvin.vanaalst@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

