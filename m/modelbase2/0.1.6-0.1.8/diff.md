# Comparing `tmp/modelbase2-0.1.6.tar.gz` & `tmp/modelbase2-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelbase2-0.1.6.tar", max compression
+gzip compressed data, was "modelbase2-0.1.8.tar", max compression
```

## Comparing `modelbase2-0.1.6.tar` & `modelbase2-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35079 2022-10-31 08:32:05.477088 modelbase2-0.1.6/LICENSE
--rw-r--r--   0        0        0     2596 2022-10-31 08:32:05.479088 modelbase2-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      723 2022-10-31 08:32:05.479088 modelbase2-0.1.6/src/modelbase2/__init__.py
--rw-r--r--   0        0        0      690 2022-10-31 08:32:05.479088 modelbase2-0.1.6/src/modelbase2/core/__init__.py
--rw-r--r--   0        0        0     4493 2022-10-31 08:32:05.479088 modelbase2-0.1.6/src/modelbase2/core/algebraic_module_container.py
--rw-r--r--   0        0        0     4609 2022-10-31 08:32:05.479088 modelbase2-0.1.6/src/modelbase2/core/constant_container.py
--rw-r--r--   0        0        0     2452 2022-10-31 08:32:05.479088 modelbase2-0.1.6/src/modelbase2/core/data.py
--rw-r--r--   0        0        0      889 2022-10-31 08:32:05.479088 modelbase2-0.1.6/src/modelbase2/core/name_container.py
--rw-r--r--   0        0        0     4832 2022-10-31 08:32:05.479088 modelbase2-0.1.6/src/modelbase2/core/reaction_container.py
--rw-r--r--   0        0        0      857 2022-10-31 08:32:05.479088 modelbase2-0.1.6/src/modelbase2/core/utils.py
--rw-r--r--   0        0        0      736 2022-10-31 08:32:05.479088 modelbase2-0.1.6/src/modelbase2/core/variable_container.py
--rw-r--r--   0        0        0      217 2022-10-31 08:32:05.480088 modelbase2-0.1.6/src/modelbase2/ode/__init__.py
--rw-r--r--   0        0        0     2259 2022-10-31 08:32:05.480088 modelbase2-0.1.6/src/modelbase2/ode/integrator.py
--rw-r--r--   0        0        0     8378 2022-10-31 08:32:05.480088 modelbase2-0.1.6/src/modelbase2/ode/mca.py
--rw-r--r--   0        0        0    15494 2022-10-31 08:32:05.480088 modelbase2-0.1.6/src/modelbase2/ode/model.py
--rw-r--r--   0        0        0     4784 2022-10-31 08:32:05.480088 modelbase2-0.1.6/src/modelbase2/ode/simulator.py
--rw-r--r--   0        0        0        0 2022-10-31 08:32:05.480088 modelbase2-0.1.6/src/modelbase2/py.typed
--rw-r--r--   0        0        0      407 2022-10-31 08:32:05.480088 modelbase2-0.1.6/src/modelbase2/types.py
--rw-r--r--   0        0        0        0 2022-10-31 08:32:05.480088 modelbase2-0.1.6/src/modelbase2/utils/__init__.py
--rw-r--r--   0        0        0    12258 2022-10-31 08:32:05.480088 modelbase2-0.1.6/src/modelbase2/utils/plotting.py
--rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 modelbase2-0.1.6/setup.py
--rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 modelbase2-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35079 2022-11-21 09:18:31.668037 modelbase2-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2596 2022-11-21 09:18:31.670037 modelbase2-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      723 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/__init__.py
+-rw-r--r--   0        0        0      690 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/core/__init__.py
+-rw-r--r--   0        0        0     4493 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/core/algebraic_module_container.py
+-rw-r--r--   0        0        0     4609 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/core/constant_container.py
+-rw-r--r--   0        0        0     2452 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/core/data.py
+-rw-r--r--   0        0        0      889 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/core/name_container.py
+-rw-r--r--   0        0        0     4832 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/core/reaction_container.py
+-rw-r--r--   0        0        0      857 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/core/utils.py
+-rw-r--r--   0        0        0      736 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/core/variable_container.py
+-rw-r--r--   0        0        0      217 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/ode/__init__.py
+-rw-r--r--   0        0        0     2259 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/ode/integrator.py
+-rw-r--r--   0        0        0     8378 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/ode/mca.py
+-rw-r--r--   0        0        0    15494 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/ode/model.py
+-rw-r--r--   0        0        0     4784 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/ode/simulator.py
+-rw-r--r--   0        0        0        0 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/py.typed
+-rw-r--r--   0        0        0      407 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/types.py
+-rw-r--r--   0        0        0        0 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/utils/__init__.py
+-rw-r--r--   0        0        0    12258 2022-11-21 09:18:31.671037 modelbase2-0.1.8/src/modelbase2/utils/plotting.py
+-rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 modelbase2-0.1.8/setup.py
+-rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 modelbase2-0.1.8/PKG-INFO
```

### Comparing `modelbase2-0.1.6/LICENSE` & `modelbase2-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `modelbase2-0.1.6/pyproject.toml` & `modelbase2-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelbase2"
-version = "0.1.6"
+version = "0.1.8"
 description = "A package to build metabolic models"
 license = "GPL-3.0-or-later"
 authors = ["Marvin van Aalst <marvin.vanaalst@gmail.com>", "Oliver Ebenhöh <oliver.ebenhoeh@hhu.de>"]
 maintainers = ["Marvin van Aalst <marvin.vanaalst@gmail.com>"]
 repository = "https://gitlab.com/qtb-hhu/modelbase-software"
 documentation = "https://modelbase.readthedocs.io/en/latest/"
 keywords = ["modelling", "ode", "metabolic"]
```

### Comparing `modelbase2-0.1.6/src/modelbase2/__init__.py` & `modelbase2-0.1.8/src/modelbase2/__init__.py`

 * *Files identical despite different names*

### Comparing `modelbase2-0.1.6/src/modelbase2/core/__init__.py` & `modelbase2-0.1.8/src/modelbase2/core/__init__.py`

 * *Files identical despite different names*

### Comparing `modelbase2-0.1.6/src/modelbase2/core/algebraic_module_container.py` & `modelbase2-0.1.8/src/modelbase2/core/algebraic_module_container.py`

 * *Files identical despite different names*

### Comparing `modelbase2-0.1.6/src/modelbase2/core/constant_container.py` & `modelbase2-0.1.8/src/modelbase2/core/constant_container.py`

 * *Files identical despite different names*

### Comparing `modelbase2-0.1.6/src/modelbase2/core/data.py` & `modelbase2-0.1.8/src/modelbase2/core/data.py`

 * *Files identical despite different names*

### Comparing `modelbase2-0.1.6/src/modelbase2/core/name_container.py` & `modelbase2-0.1.8/src/modelbase2/core/name_container.py`

 * *Files identical despite different names*

### Comparing `modelbase2-0.1.6/src/modelbase2/core/reaction_container.py` & `modelbase2-0.1.8/src/modelbase2/core/reaction_container.py`

 * *Files identical despite different names*

### Comparing `modelbase2-0.1.6/src/modelbase2/core/utils.py` & `modelbase2-0.1.8/src/modelbase2/core/utils.py`

 * *Files identical despite different names*

### Comparing `modelbase2-0.1.6/src/modelbase2/core/variable_container.py` & `modelbase2-0.1.8/src/modelbase2/core/variable_container.py`

 * *Files identical despite different names*

### Comparing `modelbase2-0.1.6/src/modelbase2/ode/integrator.py` & `modelbase2-0.1.8/src/modelbase2/ode/integrator.py`

 * *Files identical despite different names*

### Comparing `modelbase2-0.1.6/src/modelbase2/ode/mca.py` & `modelbase2-0.1.8/src/modelbase2/ode/mca.py`

 * *Files identical despite different names*

### Comparing `modelbase2-0.1.6/src/modelbase2/ode/model.py` & `modelbase2-0.1.8/src/modelbase2/ode/model.py`

 * *Files identical despite different names*

### Comparing `modelbase2-0.1.6/src/modelbase2/ode/simulator.py` & `modelbase2-0.1.8/src/modelbase2/ode/simulator.py`

 * *Files identical despite different names*

### Comparing `modelbase2-0.1.6/src/modelbase2/utils/plotting.py` & `modelbase2-0.1.8/src/modelbase2/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `modelbase2-0.1.6/setup.py` & `modelbase2-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'scipy>=1.7.2,<2.0.0',
  'sympy>=1.9,<2.0',
  'tqdm>=4.62.3,<5.0.0',
  'typing-extensions>=4.0.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'modelbase2',
-    'version': '0.1.6',
+    'version': '0.1.8',
     'description': 'A package to build metabolic models',
     'long_description': 'None',
     'author': 'Marvin van Aalst',
     'author_email': 'marvin.vanaalst@gmail.com',
     'maintainer': 'Marvin van Aalst',
     'maintainer_email': 'marvin.vanaalst@gmail.com',
     'url': 'https://gitlab.com/qtb-hhu/modelbase-software',
```

### Comparing `modelbase2-0.1.6/PKG-INFO` & `modelbase2-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelbase2
-Version: 0.1.6
+Version: 0.1.8
 Summary: A package to build metabolic models
 Home-page: https://gitlab.com/qtb-hhu/modelbase-software
 License: GPL-3.0-or-later
 Keywords: modelling,ode,metabolic
 Author: Marvin van Aalst
 Author-email: marvin.vanaalst@gmail.com
 Maintainer: Marvin van Aalst
```

