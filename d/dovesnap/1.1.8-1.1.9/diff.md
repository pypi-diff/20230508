# Comparing `tmp/dovesnap-1.1.8.tar.gz` & `tmp/dovesnap-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dovesnap-1.1.8.tar", max compression
+gzip compressed data, was "dovesnap-1.1.9.tar", max compression
```

## Comparing `dovesnap-1.1.8.tar` & `dovesnap-1.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11374 2023-03-16 05:35:52.492529 dovesnap-1.1.8/LICENSE
--rw-r--r--   0        0        0      599 2023-03-16 05:35:52.496529 dovesnap-1.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-16 05:35:52.496529 dovesnap-1.1.8/src/dovesnap/__init__.py
--rwxr-xr-x   0        0        0     2231 2023-03-16 05:35:52.496529 dovesnap-1.1.8/src/dovesnap/cleanup_dovesnap
--rwxr-xr-x   0        0        0    12055 2023-03-16 05:35:52.496529 dovesnap-1.1.8/src/dovesnap/graph_dovesnap.py
--rw-r--r--   0        0        0      844 2023-03-16 05:37:00.452005 dovesnap-1.1.8/setup.py
--rw-r--r--   0        0        0      630 2023-03-16 05:37:00.452273 dovesnap-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11374 2023-05-03 04:36:38.334870 dovesnap-1.1.9/LICENSE
+-rw-r--r--   0        0        0      599 2023-05-03 04:36:38.338870 dovesnap-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-03 04:36:38.338870 dovesnap-1.1.9/src/dovesnap/__init__.py
+-rwxr-xr-x   0        0        0     2231 2023-05-03 04:36:38.338870 dovesnap-1.1.9/src/dovesnap/cleanup_dovesnap
+-rwxr-xr-x   0        0        0    12055 2023-05-03 04:36:38.338870 dovesnap-1.1.9/src/dovesnap/graph_dovesnap.py
+-rw-r--r--   0        0        0      844 2023-05-03 04:38:02.971518 dovesnap-1.1.9/setup.py
+-rw-r--r--   0        0        0      630 2023-05-03 04:38:02.971876 dovesnap-1.1.9/PKG-INFO
```

### Comparing `dovesnap-1.1.8/LICENSE` & `dovesnap-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dovesnap-1.1.8/pyproject.toml` & `dovesnap-1.1.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "dovesnap"
-version = "1.1.8"
+version = "1.1.9"
 description = "graphviz generator of dovesnap networks"
 authors = ["Charlie Lewis <clewis@iqt.org>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8 <3.11"
 docker = "6.0.1"
-faucetconfrpc = "0.22.52"
+faucetconfrpc = "0.22.53"
 graphviz = "0.20.1"
 
 [tool.poetry.dev-dependencies]
-pytype = "2023.3.13"
-"ruamel.yaml" = "0.17.21"
+pytype = "2023.4.27"
+"ruamel.yaml" = "0.17.22"
 
 [tool.poetry.scripts]
 graph_dovesnap = "dovesnap.graph_dovesnap:main"
 
 [tool.poetry.urls]
 homepage = "https://github.com/IQTLabs/dovesnap"
```

### Comparing `dovesnap-1.1.8/src/dovesnap/cleanup_dovesnap` & `dovesnap-1.1.9/src/dovesnap/cleanup_dovesnap`

 * *Files identical despite different names*

### Comparing `dovesnap-1.1.8/src/dovesnap/graph_dovesnap.py` & `dovesnap-1.1.9/src/dovesnap/graph_dovesnap.py`

 * *Files identical despite different names*

### Comparing `dovesnap-1.1.8/setup.py` & `dovesnap-1.1.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 packages = \
 ['dovesnap']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['docker==6.0.1', 'faucetconfrpc==0.22.52', 'graphviz==0.20.1']
+['docker==6.0.1', 'faucetconfrpc==0.22.53', 'graphviz==0.20.1']
 
 entry_points = \
 {'console_scripts': ['graph_dovesnap = dovesnap.graph_dovesnap:main']}
 
 setup_kwargs = {
     'name': 'dovesnap',
-    'version': '1.1.8',
+    'version': '1.1.9',
     'description': 'graphviz generator of dovesnap networks',
     'long_description': None,
     'author': 'Charlie Lewis',
     'author_email': 'clewis@iqt.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `dovesnap-1.1.8/PKG-INFO` & `dovesnap-1.1.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dovesnap
-Version: 1.1.8
+Version: 1.1.9
 Summary: graphviz generator of dovesnap networks
 License: Apache-2.0
 Author: Charlie Lewis
 Author-email: clewis@iqt.org
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: docker (==6.0.1)
-Requires-Dist: faucetconfrpc (==0.22.52)
+Requires-Dist: faucetconfrpc (==0.22.53)
 Requires-Dist: graphviz (==0.20.1)
 Project-URL: homepage, https://github.com/IQTLabs/dovesnap
```

