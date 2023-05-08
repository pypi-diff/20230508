# Comparing `tmp/mechanical_bull-0.0.6.tar.gz` & `tmp/mechanical_bull-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mechanical_bull-0.0.6.tar", max compression
+gzip compressed data, was "mechanical_bull-0.0.7.tar", max compression
```

## Comparing `mechanical_bull-0.0.6.tar` & `mechanical_bull-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1062 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/LICENSE
--rw-r--r--   0        0        0     3110 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/README.md
--rw-r--r--   0        0        0        0 2023-04-23 12:23:50.009197 mechanical_bull-0.0.6/mechanical_bull/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 12:23:50.009197 mechanical_bull-0.0.6/mechanical_bull/actions/__init__.py
--rw-r--r--   0        0        0      196 2023-04-23 12:24:23.137503 mechanical_bull-0.0.6/mechanical_bull/actions/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1206 2023-04-23 12:24:23.141503 mechanical_bull-0.0.6/mechanical_bull/actions/__pycache__/accept_follow_request.cpython-311.pyc
--rw-r--r--   0        0        0      930 2023-04-23 12:24:23.153503 mechanical_bull-0.0.6/mechanical_bull/actions/__pycache__/log_to_file.cpython-311.pyc
--rw-r--r--   0        0        0     1236 2023-04-23 12:24:23.141503 mechanical_bull-0.0.6/mechanical_bull/actions/__pycache__/reject_follow_request.cpython-311.pyc
--rw-r--r--   0        0        0     1985 2023-04-23 12:24:23.141503 mechanical_bull-0.0.6/mechanical_bull/actions/__pycache__/test_accept_reject_follow_request.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      491 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/mechanical_bull/actions/accept_follow_request.py
--rw-r--r--   0        0        0      225 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/mechanical_bull/actions/log_to_file.py
--rw-r--r--   0        0        0      521 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/mechanical_bull/actions/reject_follow_request.py
--rw-r--r--   0        0        0      847 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/mechanical_bull/actions/test_accept_reject_follow_request.py
--rw-r--r--   0        0        0     1604 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/mechanical_bull/add_user.py
--rw-r--r--   0        0        0      787 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/mechanical_bull/event_loop.py
--rw-r--r--   0        0        0      335 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/mechanical_bull/handlers.py
--rw-r--r--   0        0        0      685 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/mechanical_bull/run.py
--rw-r--r--   0        0        0      542 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/mechanical_bull/test_event_loop.py
--rw-r--r--   0        0        0      484 2023-04-23 12:23:49.933196 mechanical_bull-0.0.6/mechanical_bull/test_handlers.py
--rw-r--r--   0        0        0      896 2023-04-23 12:23:49.937196 mechanical_bull-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3853 1970-01-01 00:00:00.000000 mechanical_bull-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-08 17:56:14.029019 mechanical_bull-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3110 2023-05-08 17:56:14.029019 mechanical_bull-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 17:56:14.117020 mechanical_bull-0.0.7/mechanical_bull/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 17:56:14.117020 mechanical_bull-0.0.7/mechanical_bull/actions/__init__.py
+-rw-r--r--   0        0        0      196 2023-05-08 17:56:47.057360 mechanical_bull-0.0.7/mechanical_bull/actions/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1206 2023-05-08 17:56:47.061360 mechanical_bull-0.0.7/mechanical_bull/actions/__pycache__/accept_follow_request.cpython-311.pyc
+-rw-r--r--   0        0        0      930 2023-05-08 17:56:47.073360 mechanical_bull-0.0.7/mechanical_bull/actions/__pycache__/log_to_file.cpython-311.pyc
+-rw-r--r--   0        0        0     1236 2023-05-08 17:56:47.061360 mechanical_bull-0.0.7/mechanical_bull/actions/__pycache__/reject_follow_request.cpython-311.pyc
+-rw-r--r--   0        0        0     1985 2023-05-08 17:56:47.061360 mechanical_bull-0.0.7/mechanical_bull/actions/__pycache__/test_accept_reject_follow_request.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      491 2023-05-08 17:56:14.029019 mechanical_bull-0.0.7/mechanical_bull/actions/accept_follow_request.py
+-rw-r--r--   0        0        0      225 2023-05-08 17:56:14.029019 mechanical_bull-0.0.7/mechanical_bull/actions/log_to_file.py
+-rw-r--r--   0        0        0      521 2023-05-08 17:56:14.029019 mechanical_bull-0.0.7/mechanical_bull/actions/reject_follow_request.py
+-rw-r--r--   0        0        0      847 2023-05-08 17:56:14.029019 mechanical_bull-0.0.7/mechanical_bull/actions/test_accept_reject_follow_request.py
+-rw-r--r--   0        0        0     1604 2023-05-08 17:56:14.029019 mechanical_bull-0.0.7/mechanical_bull/add_user.py
+-rw-r--r--   0        0        0      787 2023-05-08 17:56:14.029019 mechanical_bull-0.0.7/mechanical_bull/event_loop.py
+-rw-r--r--   0        0        0      335 2023-05-08 17:56:14.029019 mechanical_bull-0.0.7/mechanical_bull/handlers.py
+-rw-r--r--   0        0        0      685 2023-05-08 17:56:14.029019 mechanical_bull-0.0.7/mechanical_bull/run.py
+-rw-r--r--   0        0        0      542 2023-05-08 17:56:14.029019 mechanical_bull-0.0.7/mechanical_bull/test_event_loop.py
+-rw-r--r--   0        0        0      484 2023-05-08 17:56:14.029019 mechanical_bull-0.0.7/mechanical_bull/test_handlers.py
+-rw-r--r--   0        0        0      896 2023-05-08 17:56:14.029019 mechanical_bull-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3853 1970-01-01 00:00:00.000000 mechanical_bull-0.0.7/PKG-INFO
```

### Comparing `mechanical_bull-0.0.6/LICENSE` & `mechanical_bull-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.6/README.md` & `mechanical_bull-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.6/mechanical_bull/actions/__pycache__/accept_follow_request.cpython-311.pyc` & `mechanical_bull-0.0.7/mechanical_bull/actions/__pycache__/accept_follow_request.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x55234564 (Sun Apr 23 12:23:49 2023 UTC)
+moddate:  0xbe375964 (Mon May  8 17:56:14 2023 UTC)
 files sz: 491
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `mechanical_bull-0.0.6/mechanical_bull/actions/__pycache__/log_to_file.cpython-311.pyc` & `mechanical_bull-0.0.7/mechanical_bull/actions/__pycache__/log_to_file.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x55234564 (Sun Apr 23 12:23:49 2023 UTC)
+moddate:  0xbe375964 (Mon May  8 17:56:14 2023 UTC)
 files sz: 225
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `mechanical_bull-0.0.6/mechanical_bull/actions/__pycache__/reject_follow_request.cpython-311.pyc` & `mechanical_bull-0.0.7/mechanical_bull/actions/__pycache__/reject_follow_request.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x55234564 (Sun Apr 23 12:23:49 2023 UTC)
+moddate:  0xbe375964 (Mon May  8 17:56:14 2023 UTC)
 files sz: 521
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `mechanical_bull-0.0.6/mechanical_bull/actions/__pycache__/test_accept_reject_follow_request.cpython-311-pytest-7.3.1.pyc` & `mechanical_bull-0.0.7/mechanical_bull/actions/__pycache__/test_accept_reject_follow_request.cpython-311-pytest-7.3.1.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x55234564 (Sun Apr 23 12:23:49 2023 UTC)
+moddate:  0xbe375964 (Mon May  8 17:56:14 2023 UTC)
 files sz: 847
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `mechanical_bull-0.0.6/mechanical_bull/actions/reject_follow_request.py` & `mechanical_bull-0.0.7/mechanical_bull/actions/reject_follow_request.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.6/mechanical_bull/actions/test_accept_reject_follow_request.py` & `mechanical_bull-0.0.7/mechanical_bull/actions/test_accept_reject_follow_request.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.6/mechanical_bull/add_user.py` & `mechanical_bull-0.0.7/mechanical_bull/add_user.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.6/mechanical_bull/event_loop.py` & `mechanical_bull-0.0.7/mechanical_bull/event_loop.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.6/mechanical_bull/run.py` & `mechanical_bull-0.0.7/mechanical_bull/run.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.6/mechanical_bull/test_event_loop.py` & `mechanical_bull-0.0.7/mechanical_bull/test_event_loop.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.6/pyproject.toml` & `mechanical_bull-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mechanical-bull"
-version = "0.0.6"
+version = "0.0.7"
 description = "A framework to automate reacting to ActivityStreams events."
 authors = ["Helge <helge.krueger@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "mechanical_bull"}]
 repository = "https://codeberg.org/bovine/mechanical_bull"
 documentation = "https://mechanical-bull.readthedocs.io/en/latest/"
```

### Comparing `mechanical_bull-0.0.6/PKG-INFO` & `mechanical_bull-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mechanical-bull
-Version: 0.0.6
+Version: 0.0.7
 Summary: A framework to automate reacting to ActivityStreams events.
 Home-page: https://codeberg.org/bovine/mechanical_bull
 License: MIT
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

