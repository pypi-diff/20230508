# Comparing `tmp/joern_lib-0.8.0.tar.gz` & `tmp/joern_lib-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joern_lib-0.8.0.tar", max compression
+gzip compressed data, was "joern_lib-0.8.1.tar", max compression
```

## Comparing `joern_lib-0.8.0.tar` & `joern_lib-0.8.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-05-05 22:17:31.777335 joern_lib-0.8.0/LICENSE
--rw-r--r--   0        0        0     3909 2023-05-05 22:17:31.777335 joern_lib-0.8.0/README.md
--rw-r--r--   0        0        0       86 2023-05-05 22:17:31.805335 joern_lib-0.8.0/joern_lib/__init__.py
--rw-r--r--   0        0        0    11860 2023-05-05 22:17:31.805335 joern_lib-0.8.0/joern_lib/client.py
--rw-r--r--   0        0        0       61 2023-05-05 22:17:31.805335 joern_lib-0.8.0/joern_lib/detectors/__init__.py
--rw-r--r--   0        0        0      627 2023-05-05 22:17:31.805335 joern_lib-0.8.0/joern_lib/detectors/c.py
--rw-r--r--   0        0        0     9096 2023-05-05 22:17:31.805335 joern_lib-0.8.0/joern_lib/detectors/common.py
--rw-r--r--   0        0        0     2841 2023-05-05 22:17:31.805335 joern_lib-0.8.0/joern_lib/detectors/java.py
--rw-r--r--   0        0        0     3914 2023-05-05 22:17:31.805335 joern_lib-0.8.0/joern_lib/detectors/js.py
--rw-r--r--   0        0        0    12485 2023-05-05 22:17:31.805335 joern_lib-0.8.0/joern_lib/utils.py
--rw-r--r--   0        0        0     4535 2023-05-05 22:17:31.809336 joern_lib-0.8.0/joern_lib/workspace.py
--rw-r--r--   0        0        0     1206 2023-05-05 22:17:31.809336 joern_lib-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5255 1970-01-01 00:00:00.000000 joern_lib-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-08 13:43:18.210812 joern_lib-0.8.1/LICENSE
+-rw-r--r--   0        0        0     3909 2023-05-08 13:43:18.210812 joern_lib-0.8.1/README.md
+-rw-r--r--   0        0        0       86 2023-05-08 13:43:18.238813 joern_lib-0.8.1/joern_lib/__init__.py
+-rw-r--r--   0        0        0    11860 2023-05-08 13:43:18.238813 joern_lib-0.8.1/joern_lib/client.py
+-rw-r--r--   0        0        0       61 2023-05-08 13:43:18.238813 joern_lib-0.8.1/joern_lib/detectors/__init__.py
+-rw-r--r--   0        0        0      627 2023-05-08 13:43:18.238813 joern_lib-0.8.1/joern_lib/detectors/c.py
+-rw-r--r--   0        0        0     9096 2023-05-08 13:43:18.238813 joern_lib-0.8.1/joern_lib/detectors/common.py
+-rw-r--r--   0        0        0     2841 2023-05-08 13:43:18.238813 joern_lib-0.8.1/joern_lib/detectors/java.py
+-rw-r--r--   0        0        0     3914 2023-05-08 13:43:18.238813 joern_lib-0.8.1/joern_lib/detectors/js.py
+-rw-r--r--   0        0        0    12485 2023-05-08 13:43:18.238813 joern_lib-0.8.1/joern_lib/utils.py
+-rw-r--r--   0        0        0     4535 2023-05-08 13:43:18.238813 joern_lib-0.8.1/joern_lib/workspace.py
+-rw-r--r--   0        0        0     1215 2023-05-08 13:43:18.242813 joern_lib-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     5157 1970-01-01 00:00:00.000000 joern_lib-0.8.1/PKG-INFO
```

### Comparing `joern_lib-0.8.0/LICENSE` & `joern_lib-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `joern_lib-0.8.0/README.md` & `joern_lib-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `joern_lib-0.8.0/joern_lib/client.py` & `joern_lib-0.8.1/joern_lib/client.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.8.0/joern_lib/detectors/c.py` & `joern_lib-0.8.1/joern_lib/detectors/c.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.8.0/joern_lib/detectors/common.py` & `joern_lib-0.8.1/joern_lib/detectors/common.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.8.0/joern_lib/detectors/java.py` & `joern_lib-0.8.1/joern_lib/detectors/java.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.8.0/joern_lib/detectors/js.py` & `joern_lib-0.8.1/joern_lib/detectors/js.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.8.0/joern_lib/utils.py` & `joern_lib-0.8.1/joern_lib/utils.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.8.0/joern_lib/workspace.py` & `joern_lib-0.8.1/joern_lib/workspace.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.8.0/pyproject.toml` & `joern_lib-0.8.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "joern-lib"
-version = "0.8.0"
+version = "0.8.1"
 description = "Python library to interact with Joern server"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "joern_lib"}]
 homepage = "https://github.com/AppThreat/joern-lib"
 repository = "https://github.com/AppThreat/joern-lib"
@@ -19,25 +19,25 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
 ]
 exclude = ["contrib", "tests"]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<3.11"
+python = ">=3.8.1,<3.11"
 httpx = "^0.24.0"
 websockets = "^11.0.2"
 uvloop = "^0.17.0"
 orjson = "^3.8.11"
 rich = "^13.3.5"
 
-[tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
-black = "^22.3.0"
-flake8 = "^4.0.1"
-pytest-cov = "^3.0.0"
-pyinstaller = "^5.0.1"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.1"
+black = "^23.3.0"
+flake8 = "^6.0.0"
+pytest-cov = "^4.0.0"
+pyinstaller = "^5.10.1"
 pdoc3 = "^0.10.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `joern_lib-0.8.0/PKG-INFO` & `joern_lib-0.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: joern-lib
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python library to interact with Joern server
 Home-page: https://github.com/AppThreat/joern-lib
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.8.1,<3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
```

