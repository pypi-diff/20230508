# Comparing `tmp/turbine-py-1.8.0.tar.gz` & `tmp/turbine-py-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbine-py-1.8.0.tar", last modified: Tue May  2 15:36:12 2023, max compression
+gzip compressed data, was "turbine-py-1.8.1.tar", last modified: Mon May  8 18:27:55 2023, max compression
```

## Comparing `turbine-py-1.8.0.tar` & `turbine-py-1.8.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:36:12.006059 turbine-py-1.8.0/
--rw-r--r--   0 root         (0) root         (0)      168 2023-05-02 15:36:01.000000 turbine-py-1.8.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      161 2023-05-02 15:36:01.000000 turbine-py-1.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8663 2023-05-02 15:36:12.006059 turbine-py-1.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8098 2023-05-02 15:36:01.000000 turbine-py-1.8.0/README.md
--rw-r--r--   0 root         (0) root         (0)      315 2023-05-02 15:36:01.000000 turbine-py-1.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1148 2023-05-02 15:36:12.006059 turbine-py-1.8.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:36:12.002059 turbine-py-1.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:36:12.002059 turbine-py-1.8.0/src/turbine/
--rw-r--r--   0 root         (0) root         (0)       83 2023-05-02 15:36:02.000000 turbine-py-1.8.0/src/turbine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4248 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:36:12.002059 turbine-py-1.8.0/src/turbine/function_deploy/
--rw-r--r--   0 root         (0) root         (0)      548 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/function_deploy/Dockerfile
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/function_deploy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:36:12.002059 turbine-py-1.8.0/src/turbine/function_deploy/data_app/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/function_deploy/data_app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:36:12.002059 turbine-py-1.8.0/src/turbine/function_deploy/function_app/
--rw-r--r--   0 root         (0) root         (0)     2460 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/function_deploy/function_app/README.md
--rw-r--r--   0 root         (0) root         (0)      247 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/function_deploy/function_app/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3142 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/function_deploy/function_app/function_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:36:12.002059 turbine-py-1.8.0/src/turbine/function_deploy/function_app/protos/
--rw-r--r--   0 root         (0) root         (0)      406 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/function_deploy/function_app/protos/service.proto
--rw-r--r--   0 root         (0) root         (0)     1023 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/function_deploy/function_app/record.py
--rw-r--r--   0 root         (0) root         (0)      144 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/function_deploy/function_app/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     2895 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/function_deploy/function_app/service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2498 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/function_deploy/function_app/service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:36:12.002059 turbine-py-1.8.0/src/turbine/runner/
--rw-r--r--   0 root         (0) root         (0)      153 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/runner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1045 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/runner/app_generate.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/runner/baserunner.py
--rw-r--r--   0 root         (0) root         (0)     3213 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/runner/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:36:12.006059 turbine-py-1.8.0/src/turbine/runtime/
--rw-r--r--   0 root         (0) root         (0)      780 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/runtime/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1835 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/runtime/info.py
--rw-r--r--   0 root         (0) root         (0)     3924 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/runtime/intermediate.py
--rw-r--r--   0 root         (0) root         (0)     2865 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/runtime/local.py
--rw-r--r--   0 root         (0) root         (0)    11804 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/runtime/platform.py
--rw-r--r--   0 root         (0) root         (0)     2729 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/runtime/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:36:12.002059 turbine-py-1.8.0/src/turbine/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:36:12.006059 turbine-py-1.8.0/src/turbine/templates/python/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/templates/python/.gitignore
--rw-r--r--   0 root         (0) root         (0)     6438 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/templates/python/README.md
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/templates/python/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/templates/python/app.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:36:12.006059 turbine-py-1.8.0/src/turbine/templates/python/fixtures/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/templates/python/fixtures/.gitkeep
--rw-r--r--   0 root         (0) root         (0)     8360 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/templates/python/fixtures/demo-cdc.json
--rw-r--r--   0 root         (0) root         (0)     4691 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/templates/python/fixtures/demo-no-cdc.json
--rw-r--r--   0 root         (0) root         (0)     3128 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/templates/python/main.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-02 15:36:01.000000 turbine-py-1.8.0/src/turbine/templates/python/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:36:12.006059 turbine-py-1.8.0/src/turbine_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8663 2023-05-02 15:36:11.000000 turbine-py-1.8.0/src/turbine_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1637 2023-05-02 15:36:11.000000 turbine-py-1.8.0/src/turbine_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 15:36:11.000000 turbine-py-1.8.0/src/turbine_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-05-02 15:36:11.000000 turbine-py-1.8.0/src/turbine_py.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-02 15:36:11.000000 turbine-py-1.8.0/src/turbine_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-02 15:36:11.000000 turbine-py-1.8.0/src/turbine_py.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:36:12.006059 turbine-py-1.8.0/tests/
--rw-r--r--   0 root         (0) root         (0)     3822 2023-05-02 15:36:01.000000 turbine-py-1.8.0/tests/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:27:55.294124 turbine-py-1.8.1/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-05-08 18:27:45.000000 turbine-py-1.8.1/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      161 2023-05-08 18:27:45.000000 turbine-py-1.8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8663 2023-05-08 18:27:55.294124 turbine-py-1.8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8098 2023-05-08 18:27:45.000000 turbine-py-1.8.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      315 2023-05-08 18:27:45.000000 turbine-py-1.8.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-05-08 18:27:55.294124 turbine-py-1.8.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:27:55.286124 turbine-py-1.8.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:27:55.290124 turbine-py-1.8.1/src/turbine/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-05-08 18:27:46.000000 turbine-py-1.8.1/src/turbine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:27:55.290124 turbine-py-1.8.1/src/turbine/function_deploy/
+-rw-r--r--   0 root         (0) root         (0)      548 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/function_deploy/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/function_deploy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:27:55.290124 turbine-py-1.8.1/src/turbine/function_deploy/data_app/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/function_deploy/data_app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:27:55.290124 turbine-py-1.8.1/src/turbine/function_deploy/function_app/
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/function_deploy/function_app/README.md
+-rw-r--r--   0 root         (0) root         (0)      247 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/function_deploy/function_app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/function_deploy/function_app/function_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:27:55.290124 turbine-py-1.8.1/src/turbine/function_deploy/function_app/protos/
+-rw-r--r--   0 root         (0) root         (0)      406 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/function_deploy/function_app/protos/service.proto
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/function_deploy/function_app/record.py
+-rw-r--r--   0 root         (0) root         (0)      144 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/function_deploy/function_app/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     2895 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/function_deploy/function_app/service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/function_deploy/function_app/service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:27:55.290124 turbine-py-1.8.1/src/turbine/runner/
+-rw-r--r--   0 root         (0) root         (0)      153 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/runner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1045 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/runner/app_generate.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/runner/baserunner.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/runner/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:27:55.290124 turbine-py-1.8.1/src/turbine/runtime/
+-rw-r--r--   0 root         (0) root         (0)      780 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/runtime/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1835 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/runtime/info.py
+-rw-r--r--   0 root         (0) root         (0)     3924 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/runtime/intermediate.py
+-rw-r--r--   0 root         (0) root         (0)     2865 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/runtime/local.py
+-rw-r--r--   0 root         (0) root         (0)    11804 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/runtime/platform.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/runtime/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:27:55.286124 turbine-py-1.8.1/src/turbine/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:27:55.294124 turbine-py-1.8.1/src/turbine/templates/python/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/templates/python/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     6438 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/templates/python/README.md
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/templates/python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/templates/python/app.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:27:55.294124 turbine-py-1.8.1/src/turbine/templates/python/fixtures/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/templates/python/fixtures/.gitkeep
+-rw-r--r--   0 root         (0) root         (0)     8360 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/templates/python/fixtures/demo-cdc.json
+-rw-r--r--   0 root         (0) root         (0)     4691 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/templates/python/fixtures/demo-no-cdc.json
+-rw-r--r--   0 root         (0) root         (0)     3128 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/templates/python/main.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-08 18:27:45.000000 turbine-py-1.8.1/src/turbine/templates/python/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:27:55.294124 turbine-py-1.8.1/src/turbine_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8663 2023-05-08 18:27:55.000000 turbine-py-1.8.1/src/turbine_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1637 2023-05-08 18:27:55.000000 turbine-py-1.8.1/src/turbine_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 18:27:55.000000 turbine-py-1.8.1/src/turbine_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-08 18:27:55.000000 turbine-py-1.8.1/src/turbine_py.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-08 18:27:55.000000 turbine-py-1.8.1/src/turbine_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-08 18:27:55.000000 turbine-py-1.8.1/src/turbine_py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:27:55.294124 turbine-py-1.8.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     3822 2023-05-08 18:27:45.000000 turbine-py-1.8.1/tests/test_cli.py
```

### Comparing `turbine-py-1.8.0/PKG-INFO` & `turbine-py-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbine-py
-Version: 1.8.0
+Version: 1.8.1
 Summary: Meroxa Turbine data application framework
 Home-page: https://meroxa.io/
 Author: Eric Cheatham
 Author-email: eric@meroxa.io
 License: MIT
 Project-URL: Source Code, https://github.com/meroxa/turbine-py/
 Project-URL: Issue Tracker, https://github.com/meroxa/turbine-py/issues
```

### Comparing `turbine-py-1.8.0/README.md` & `turbine-py-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/setup.cfg` & `turbine-py-1.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/src/turbine/cli.py` & `turbine-py-1.8.1/src/turbine/cli.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/src/turbine/function_deploy/Dockerfile` & `turbine-py-1.8.1/src/turbine/function_deploy/Dockerfile`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/src/turbine/function_deploy/function_app/README.md` & `turbine-py-1.8.1/src/turbine/function_deploy/function_app/README.md`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/src/turbine/function_deploy/function_app/function_server.py` & `turbine-py-1.8.1/src/turbine/function_deploy/function_app/function_server.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/src/turbine/function_deploy/function_app/record.py` & `turbine-py-1.8.1/src/turbine/function_deploy/function_app/record.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/src/turbine/function_deploy/function_app/service_pb2.py` & `turbine-py-1.8.1/src/turbine/function_deploy/function_app/service_pb2.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/src/turbine/function_deploy/function_app/service_pb2_grpc.py` & `turbine-py-1.8.1/src/turbine/function_deploy/function_app/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/src/turbine/runner/app_generate.py` & `turbine-py-1.8.1/src/turbine/runner/app_generate.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/src/turbine/runner/baserunner.py` & `turbine-py-1.8.1/src/turbine/runner/baserunner.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,17 @@
         self.info_runtime = InfoRuntime(self.app_config, self.path_to_data_app)
         self.local_runtime = LocalRuntime(self.app_config, self.path_to_data_app)
 
     @property
     def app_config(self):
         config = {}
         try:
-            with open(os.path.abspath(f"{self.path_to_data_app}") + "/app.json") as fd:
+            with open(
+                os.path.abspath(os.path.join(self.path_to_data_app, " app.json"))
+            ) as fd:
                 config = AppConfig(**json.load(fd))
                 if self.app_name != "":
                     config.name = self.app_name
         except OSError as e:
             print(f"Unable to locate app config: {e}", file=sys.stderr)
         return config
```

### Comparing `turbine-py-1.8.0/src/turbine/runner/runner.py` & `turbine-py-1.8.1/src/turbine/runner/runner.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/src/turbine/runtime/__init__.py` & `turbine-py-1.8.1/src/turbine/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/src/turbine/runtime/info.py` & `turbine-py-1.8.1/src/turbine/runtime/info.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/src/turbine/runtime/intermediate.py` & `turbine-py-1.8.1/src/turbine/runtime/intermediate.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/src/turbine/runtime/local.py` & `turbine-py-1.8.1/src/turbine/runtime/local.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/src/turbine/runtime/platform.py` & `turbine-py-1.8.1/src/turbine/runtime/platform.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/src/turbine/runtime/types.py` & `turbine-py-1.8.1/src/turbine/runtime/types.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/src/turbine/templates/python/README.md` & `turbine-py-1.8.1/src/turbine/templates/python/README.md`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/src/turbine/templates/python/fixtures/demo-cdc.json` & `turbine-py-1.8.1/src/turbine/templates/python/fixtures/demo-cdc.json`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/src/turbine/templates/python/fixtures/demo-no-cdc.json` & `turbine-py-1.8.1/src/turbine/templates/python/fixtures/demo-no-cdc.json`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/src/turbine/templates/python/main.py` & `turbine-py-1.8.1/src/turbine/templates/python/main.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/src/turbine_py.egg-info/PKG-INFO` & `turbine-py-1.8.1/src/turbine_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbine-py
-Version: 1.8.0
+Version: 1.8.1
 Summary: Meroxa Turbine data application framework
 Home-page: https://meroxa.io/
 Author: Eric Cheatham
 Author-email: eric@meroxa.io
 License: MIT
 Project-URL: Source Code, https://github.com/meroxa/turbine-py/
 Project-URL: Issue Tracker, https://github.com/meroxa/turbine-py/issues
```

### Comparing `turbine-py-1.8.0/src/turbine_py.egg-info/SOURCES.txt` & `turbine-py-1.8.1/src/turbine_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.0/tests/test_cli.py` & `turbine-py-1.8.1/tests/test_cli.py`

 * *Files identical despite different names*

