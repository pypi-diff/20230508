# Comparing `tmp/python_client_generator-1.1.3.tar.gz` & `tmp/python_client_generator-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_client_generator-1.1.3.tar", max compression
+gzip compressed data, was "python_client_generator-1.1.4.tar", max compression
```

## Comparing `python_client_generator-1.1.3.tar` & `python_client_generator-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1069 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/LICENSE
--rw-r--r--   0        0        0     1568 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/README.md
--rw-r--r--   0        0        0     1769 2023-05-05 13:01:20.667187 python_client_generator-1.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/__init__.py
--rw-r--r--   0        0        0       32 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/__main__.py
--rw-r--r--   0        0        0       54 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/exceptions.py
--rwxr-xr-x   0        0        0     6598 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/generate_apis.py
--rw-r--r--   0        0        0      493 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/generate_base_client.py
--rwxr-xr-x   0        0        0     6482 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/generate_models.py
--rw-r--r--   0        0        0      593 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/generate_pyproject.py
--rw-r--r--   0        0        0     1797 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/main.py
--rw-r--r--   0        0        0       42 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/templates/__init__.py
--rw-r--r--   0        0        0     2251 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/templates/apis.py.mustache
--rw-r--r--   0        0        0     1817 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/templates/base_client.py.mustache
--rw-r--r--   0        0        0      509 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/templates/models.py.mustache
--rw-r--r--   0        0        0      423 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/templates/pyproject.toml.mustache
--rw-r--r--   0        0        0     3490 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/utils.py
--rw-r--r--   0        0        0     2477 1970-01-01 00:00:00.000000 python_client_generator-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-08 14:37:39.499563 python_client_generator-1.1.4/LICENSE
+-rw-r--r--   0        0        0     1568 2023-05-08 14:37:39.499563 python_client_generator-1.1.4/README.md
+-rw-r--r--   0        0        0     1787 2023-05-08 14:38:06.843759 python_client_generator-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-08 14:37:39.499563 python_client_generator-1.1.4/python_client_generator/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-08 14:37:39.499563 python_client_generator-1.1.4/python_client_generator/__main__.py
+-rw-r--r--   0        0        0       54 2023-05-08 14:37:39.499563 python_client_generator-1.1.4/python_client_generator/exceptions.py
+-rwxr-xr-x   0        0        0     6598 2023-05-08 14:37:39.499563 python_client_generator-1.1.4/python_client_generator/generate_apis.py
+-rw-r--r--   0        0        0      493 2023-05-08 14:37:39.499563 python_client_generator-1.1.4/python_client_generator/generate_base_client.py
+-rwxr-xr-x   0        0        0     6482 2023-05-08 14:37:39.499563 python_client_generator-1.1.4/python_client_generator/generate_models.py
+-rw-r--r--   0        0        0      593 2023-05-08 14:37:39.499563 python_client_generator-1.1.4/python_client_generator/generate_pyproject.py
+-rw-r--r--   0        0        0     1797 2023-05-08 14:37:39.499563 python_client_generator-1.1.4/python_client_generator/main.py
+-rw-r--r--   0        0        0       42 2023-05-08 14:37:39.503563 python_client_generator-1.1.4/python_client_generator/templates/__init__.py
+-rw-r--r--   0        0        0     2251 2023-05-08 14:37:39.503563 python_client_generator-1.1.4/python_client_generator/templates/apis.py.mustache
+-rw-r--r--   0        0        0     1817 2023-05-08 14:37:39.503563 python_client_generator-1.1.4/python_client_generator/templates/base_client.py.mustache
+-rw-r--r--   0        0        0      509 2023-05-08 14:37:39.503563 python_client_generator-1.1.4/python_client_generator/templates/models.py.mustache
+-rw-r--r--   0        0        0      423 2023-05-08 14:37:39.503563 python_client_generator-1.1.4/python_client_generator/templates/pyproject.toml.mustache
+-rw-r--r--   0        0        0     3490 2023-05-08 14:37:39.503563 python_client_generator-1.1.4/python_client_generator/utils.py
+-rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 python_client_generator-1.1.4/PKG-INFO
```

### Comparing `python_client_generator-1.1.3/LICENSE` & `python_client_generator-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_client_generator-1.1.3/README.md` & `python_client_generator-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `python_client_generator-1.1.3/pyproject.toml` & `python_client_generator-1.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "python-client-generator"
-version = "1.1.3"
+version = "1.1.4"
 description = "Python package to generate an httpx-based client off an OpenAPI spec"
 readme = "README.md"
 authors = ["Bogdan Petre <bogdan.petre@sennder.com>", "Trevor Pace <trevor.pace@sennder.com>"]
 repository = "https://github.com/sennder/python-client-generator"
 
 [tool.poetry.urls]
 download = "https://github.com/sennder/python-client-generator/releases"
 tracker = "https://github.com/sennder/python-client-generator/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
 chevron = "^0.14.0"
+semver = "^3.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.1.1"
 coverage = { version = "^5.3", extras = ["toml"]}
 pytest-cov = "^2.10.1"
 flake8 = "^3.8.4"
 mypy = "^0.812"
```

### Comparing `python_client_generator-1.1.3/python_client_generator/generate_apis.py` & `python_client_generator-1.1.4/python_client_generator/generate_apis.py`

 * *Files identical despite different names*

### Comparing `python_client_generator-1.1.3/python_client_generator/generate_models.py` & `python_client_generator-1.1.4/python_client_generator/generate_models.py`

 * *Files identical despite different names*

### Comparing `python_client_generator-1.1.3/python_client_generator/generate_pyproject.py` & `python_client_generator-1.1.4/python_client_generator/generate_pyproject.py`

 * *Files identical despite different names*

### Comparing `python_client_generator-1.1.3/python_client_generator/main.py` & `python_client_generator-1.1.4/python_client_generator/main.py`

 * *Files identical despite different names*

### Comparing `python_client_generator-1.1.3/python_client_generator/templates/apis.py.mustache` & `python_client_generator-1.1.4/python_client_generator/templates/apis.py.mustache`

 * *Files identical despite different names*

### Comparing `python_client_generator-1.1.3/python_client_generator/templates/base_client.py.mustache` & `python_client_generator-1.1.4/python_client_generator/templates/base_client.py.mustache`

 * *Files identical despite different names*

### Comparing `python_client_generator-1.1.3/python_client_generator/utils.py` & `python_client_generator-1.1.4/python_client_generator/utils.py`

 * *Files identical despite different names*

### Comparing `python_client_generator-1.1.3/PKG-INFO` & `python_client_generator-1.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: python-client-generator
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python package to generate an httpx-based client off an OpenAPI spec
 Home-page: https://github.com/sennder/python-client-generator
 Author: Bogdan Petre
 Author-email: bogdan.petre@sennder.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: chevron (>=0.14.0,<0.15.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
+Requires-Dist: semver (>=3.0.0,<4.0.0)
 Project-URL: Repository, https://github.com/sennder/python-client-generator
 Project-URL: download, https://github.com/sennder/python-client-generator/releases
 Project-URL: tracker, https://github.com/sennder/python-client-generator/issues
 Description-Content-Type: text/markdown
 
 # python-client-generator
```

