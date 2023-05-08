# Comparing `tmp/tuneflow-devkit-py-0.7.0.tar.gz` & `tmp/tuneflow-devkit-py-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneflow-devkit-py-0.7.0.tar", last modified: Sat Apr 29 04:46:42 2023, max compression
+gzip compressed data, was "tuneflow-devkit-py-0.8.0.tar", last modified: Mon May  8 19:37:43 2023, max compression
```

## Comparing `tuneflow-devkit-py-0.7.0.tar` & `tuneflow-devkit-py-0.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:46:42.680899 tuneflow-devkit-py-0.7.0/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1086 2023-01-11 08:37:26.000000 tuneflow-devkit-py-0.7.0/LICENSE
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-04-29 04:46:42.680899 tuneflow-devkit-py-0.7.0/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-03-29 06:56:17.000000 tuneflow-devkit-py-0.7.0/README.md
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1376 2023-04-29 04:12:56.000000 tuneflow-devkit-py-0.7.0/pyproject.toml
--rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-04-29 04:46:42.680899 tuneflow-devkit-py-0.7.0/setup.cfg
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:46:42.680899 tuneflow-devkit-py-0.7.0/src/
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:46:42.680899 tuneflow-devkit-py-0.7.0/src/tuneflow_devkit/
--rw-r--r--   0 panacea   (1000) panacea   (1000)       88 2023-03-05 07:33:21.000000 tuneflow-devkit-py-0.7.0/src/tuneflow_devkit/__init__.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     7077 2023-03-10 22:44:35.000000 tuneflow-devkit-py-0.7.0/src/tuneflow_devkit/debugger.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     8064 2023-04-01 02:37:00.000000 tuneflow-devkit-py-0.7.0/src/tuneflow_devkit/runner.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      921 2023-02-28 00:11:56.000000 tuneflow-devkit-py-0.7.0/src/tuneflow_devkit/translate_utils.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1280 2023-03-05 07:33:30.000000 tuneflow-devkit-py-0.7.0/src/tuneflow_devkit/validation_utils.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:46:42.680899 tuneflow-devkit-py-0.7.0/src/tuneflow_devkit_py.egg-info/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-04-29 04:46:42.000000 tuneflow-devkit-py-0.7.0/src/tuneflow_devkit_py.egg-info/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)      484 2023-04-29 04:46:42.000000 tuneflow-devkit-py-0.7.0/src/tuneflow_devkit_py.egg-info/SOURCES.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-04-29 04:46:42.000000 tuneflow-devkit-py-0.7.0/src/tuneflow_devkit_py.egg-info/dependency_links.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)      119 2023-04-29 04:46:42.000000 tuneflow-devkit-py-0.7.0/src/tuneflow_devkit_py.egg-info/requires.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       16 2023-04-29 04:46:42.000000 tuneflow-devkit-py-0.7.0/src/tuneflow_devkit_py.egg-info/top_level.txt
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:46:42.680899 tuneflow-devkit-py-0.7.0/test/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4192 2023-03-30 01:44:09.000000 tuneflow-devkit-py-0.7.0/test/test_runner.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2686 2023-03-05 07:52:40.000000 tuneflow-devkit-py-0.7.0/test/test_validation_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-08 19:37:43.486639 tuneflow-devkit-py-0.8.0/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1086 2023-01-11 08:37:26.000000 tuneflow-devkit-py-0.8.0/LICENSE
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-05-08 19:37:43.486639 tuneflow-devkit-py-0.8.0/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-03-29 06:56:17.000000 tuneflow-devkit-py-0.8.0/README.md
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1376 2023-05-08 19:33:39.000000 tuneflow-devkit-py-0.8.0/pyproject.toml
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-05-08 19:37:43.486639 tuneflow-devkit-py-0.8.0/setup.cfg
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-08 19:37:43.486639 tuneflow-devkit-py-0.8.0/src/
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-08 19:37:43.486639 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       88 2023-03-05 07:33:21.000000 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit/__init__.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     7077 2023-03-10 22:44:35.000000 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit/debugger.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     8064 2023-04-01 02:37:00.000000 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit/runner.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      921 2023-02-28 00:11:56.000000 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit/translate_utils.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1280 2023-03-05 07:33:30.000000 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit/validation_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-08 19:37:43.486639 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit_py.egg-info/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-05-08 19:37:43.000000 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit_py.egg-info/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      484 2023-05-08 19:37:43.000000 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit_py.egg-info/SOURCES.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-05-08 19:37:43.000000 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit_py.egg-info/dependency_links.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      119 2023-05-08 19:37:43.000000 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit_py.egg-info/requires.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       16 2023-05-08 19:37:43.000000 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit_py.egg-info/top_level.txt
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-08 19:37:43.486639 tuneflow-devkit-py-0.8.0/test/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4192 2023-03-30 01:44:09.000000 tuneflow-devkit-py-0.8.0/test/test_runner.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2686 2023-03-05 07:52:40.000000 tuneflow-devkit-py-0.8.0/test/test_validation_utils.py
```

### Comparing `tuneflow-devkit-py-0.7.0/LICENSE` & `tuneflow-devkit-py-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.7.0/PKG-INFO` & `tuneflow-devkit-py-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-devkit-py
-Version: 0.7.0
+Version: 0.8.0
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: Andantei <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-devkit-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-devkit-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis,SDK,devkit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-devkit-py-0.7.0/README.md` & `tuneflow-devkit-py-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.7.0/pyproject.toml` & `tuneflow-devkit-py-0.8.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "tuneflow-devkit-py"
-version = "0.7.0"
+version = "0.8.0"
 authors = [{ name = "Andantei", email = "contact@info.tuneflow.com" }]
 description = "Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = [
     "AI",
     "music",
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     'python-socketio >= 5.7.2',
     'uvicorn[standard] >= 0.20.0',
-    'tuneflow-py >= 0.7.0',
+    'tuneflow-py >= 0.8.0',
     'msgpack == 1.0.4',
     'fastapi == 0.92.0',
     'msgpack-asgi == 1.1.0'
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/tuneflow/tuneflow-devkit-py"
```

### Comparing `tuneflow-devkit-py-0.7.0/src/tuneflow_devkit/debugger.py` & `tuneflow-devkit-py-0.8.0/src/tuneflow_devkit/debugger.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.7.0/src/tuneflow_devkit/runner.py` & `tuneflow-devkit-py-0.8.0/src/tuneflow_devkit/runner.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.7.0/src/tuneflow_devkit/translate_utils.py` & `tuneflow-devkit-py-0.8.0/src/tuneflow_devkit/translate_utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.7.0/src/tuneflow_devkit/validation_utils.py` & `tuneflow-devkit-py-0.8.0/src/tuneflow_devkit/validation_utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.7.0/src/tuneflow_devkit_py.egg-info/PKG-INFO` & `tuneflow-devkit-py-0.8.0/src/tuneflow_devkit_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-devkit-py
-Version: 0.7.0
+Version: 0.8.0
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: Andantei <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-devkit-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-devkit-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis,SDK,devkit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-devkit-py-0.7.0/test/test_runner.py` & `tuneflow-devkit-py-0.8.0/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.7.0/test/test_validation_utils.py` & `tuneflow-devkit-py-0.8.0/test/test_validation_utils.py`

 * *Files identical despite different names*

