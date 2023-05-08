# Comparing `tmp/did-py-0.0.7.tar.gz` & `tmp/did-py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "did-py-0.0.7.tar", last modified: Tue Jan 31 21:02:06 2023, max compression
+gzip compressed data, was "did-py-0.0.9.tar", last modified: Tue Jan 31 21:13:11 2023, max compression
```

## Comparing `did-py-0.0.7.tar` & `did-py-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 21:02:06.510486 did-py-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-31 21:01:53.000000 did-py-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-31 21:01:53.000000 did-py-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-01-31 21:02:06.510486 did-py-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-01-31 21:01:53.000000 did-py-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 21:02:06.510486 did-py-0.0.7/did/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 21:01:53.000000 did-py-0.0.7/did/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-01-31 21:01:53.000000 did-py-0.0.7/did/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-01-31 21:01:53.000000 did-py-0.0.7/did/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 21:02:06.510486 did-py-0.0.7/did_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-01-31 21:02:06.000000 did-py-0.0.7/did_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-01-31 21:02:06.000000 did-py-0.0.7/did_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 21:02:06.000000 did-py-0.0.7/did_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 21:02:06.000000 did-py-0.0.7/did_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-01-31 21:02:06.000000 did-py-0.0.7/did_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-01-31 21:01:53.000000 did-py-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 21:02:06.510486 did-py-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-31 21:01:53.000000 did-py-0.0.7/vulcan.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 21:13:11.240305 did-py-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-31 21:12:57.000000 did-py-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-31 21:12:57.000000 did-py-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-01-31 21:13:11.240305 did-py-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-01-31 21:12:57.000000 did-py-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 21:13:11.240305 did-py-0.0.9/did/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 21:12:57.000000 did-py-0.0.9/did/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-01-31 21:12:57.000000 did-py-0.0.9/did/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-01-31 21:12:57.000000 did-py-0.0.9/did/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 21:13:11.240305 did-py-0.0.9/did_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-01-31 21:13:11.000000 did-py-0.0.9/did_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-01-31 21:13:11.000000 did-py-0.0.9/did_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 21:13:11.000000 did-py-0.0.9/did_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 21:13:11.000000 did-py-0.0.9/did_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-01-31 21:13:11.000000 did-py-0.0.9/did_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-01-31 21:12:57.000000 did-py-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 21:13:11.240305 did-py-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-31 21:12:57.000000 did-py-0.0.9/vulcan.lock
```

### Comparing `did-py-0.0.7/LICENSE` & `did-py-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `did-py-0.0.7/PKG-INFO` & `did-py-0.0.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,12 @@
-Metadata-Version: 2.1
-Name: did-py
-Version: 0.0.7
-Summary: what did i do?
-Author-email: Casey Williams <caseyjw@mail.com>
-License: MIT
-Project-URL: github, https://github.com/shnupta/did
-Keywords: time-management,tasks,productivity
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # did
 a simple task manager
 
 [![Build](https://github.com/shnupta/did/actions/workflows/python-app.yml/badge.svg)](https://github.com/shnupta/did/actions/workflows/python-app.yml)
-[![PyPI version](https://badge.fury.io/py/did-py.svg)](https://badge.fury.io/py/did-py)
+[![PyPI version](https://badge.fury.io/py/did-py.svg?dummy=unused)](https://badge.fury.io/py/did-py)
 
 ## install
 ```
 pip install did-py
 ```
 
 ## usage
```

### Comparing `did-py-0.0.7/README.md` & `did-py-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,24 @@
+Metadata-Version: 2.1
+Name: did-py
+Version: 0.0.9
+Summary: what did i do?
+Author-email: Casey Williams <caseyjw@mail.com>
+License: MIT
+Project-URL: github, https://github.com/shnupta/did
+Keywords: time-management,tasks,productivity
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # did
 a simple task manager
 
 [![Build](https://github.com/shnupta/did/actions/workflows/python-app.yml/badge.svg)](https://github.com/shnupta/did/actions/workflows/python-app.yml)
-[![PyPI version](https://badge.fury.io/py/did-py.svg)](https://badge.fury.io/py/did-py)
+[![PyPI version](https://badge.fury.io/py/did-py.svg?dummy=unused)](https://badge.fury.io/py/did-py)
 
 ## install
 ```
 pip install did-py
 ```
 
 ## usage
```

### Comparing `did-py-0.0.7/did/colors.py` & `did-py-0.0.9/did/colors.py`

 * *Files identical despite different names*

### Comparing `did-py-0.0.7/did/main.py` & `did-py-0.0.9/did/main.py`

 * *Files identical despite different names*

### Comparing `did-py-0.0.7/did_py.egg-info/PKG-INFO` & `did-py-0.0.9/did_py.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: did-py
-Version: 0.0.7
+Version: 0.0.9
 Summary: what did i do?
 Author-email: Casey Williams <caseyjw@mail.com>
 License: MIT
 Project-URL: github, https://github.com/shnupta/did
 Keywords: time-management,tasks,productivity
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # did
 a simple task manager
 
 [![Build](https://github.com/shnupta/did/actions/workflows/python-app.yml/badge.svg)](https://github.com/shnupta/did/actions/workflows/python-app.yml)
-[![PyPI version](https://badge.fury.io/py/did-py.svg)](https://badge.fury.io/py/did-py)
+[![PyPI version](https://badge.fury.io/py/did-py.svg?dummy=unused)](https://badge.fury.io/py/did-py)
 
 ## install
 ```
 pip install did-py
 ```
 
 ## usage
```

### Comparing `did-py-0.0.7/pyproject.toml` & `did-py-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "did-py"
-version = "0.0.7"
+version = "0.0.9"
 description = "what did i do?"
 authors = [{name="Casey Williams", email="caseyjw@mail.com"}]
 urls = {github="https://github.com/shnupta/did"}
 license = {text="MIT"}
 keywords = [ "time-management", "tasks", "productivity" ]
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.7"
```

