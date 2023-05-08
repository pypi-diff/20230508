# Comparing `tmp/inorbit_edge-1.9.1.tar.gz` & `tmp/inorbit_edge-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inorbit_edge-1.9.1.tar", last modified: Tue May  2 16:39:28 2023, max compression
+gzip compressed data, was "inorbit_edge-1.9.2.tar", last modified: Tue May  2 22:04:31 2023, max compression
```

## Comparing `inorbit_edge-1.9.1.tar` & `inorbit_edge-1.9.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:39:28.177492 inorbit_edge-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-02 16:39:28.177492 inorbit_edge-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:39:28.173492 inorbit_edge-1.9.1/inorbit_edge/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/inorbit_edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/inorbit_edge/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)   120194 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/inorbit_edge/inorbit_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18434 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/inorbit_edge/missions.py
--rw-r--r--   0 runner    (1001) docker     (123)    40986 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/inorbit_edge/robot.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/inorbit_edge/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/inorbit_edge/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/inorbit_edge/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:39:28.177492 inorbit_edge-1.9.1/inorbit_edge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-02 16:39:28.000000 inorbit_edge-1.9.1/inorbit_edge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-02 16:39:28.000000 inorbit_edge-1.9.1/inorbit_edge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:39:28.000000 inorbit_edge-1.9.1/inorbit_edge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:39:28.000000 inorbit_edge-1.9.1/inorbit_edge.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-02 16:39:28.000000 inorbit_edge-1.9.1/inorbit_edge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 16:39:28.000000 inorbit_edge-1.9.1/inorbit_edge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-02 16:39:28.177492 inorbit_edge-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:04:31.657637 inorbit_edge-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-02 22:04:23.000000 inorbit_edge-1.9.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-02 22:04:23.000000 inorbit_edge-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-02 22:04:23.000000 inorbit_edge-1.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-02 22:04:31.657637 inorbit_edge-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-02 22:04:23.000000 inorbit_edge-1.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:04:31.653637 inorbit_edge-1.9.2/inorbit_edge/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-02 22:04:23.000000 inorbit_edge-1.9.2/inorbit_edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-02 22:04:23.000000 inorbit_edge-1.9.2/inorbit_edge/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120194 2023-05-02 22:04:23.000000 inorbit_edge-1.9.2/inorbit_edge/inorbit_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18434 2023-05-02 22:04:23.000000 inorbit_edge-1.9.2/inorbit_edge/missions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40989 2023-05-02 22:04:23.000000 inorbit_edge-1.9.2/inorbit_edge/robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-02 22:04:23.000000 inorbit_edge-1.9.2/inorbit_edge/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-02 22:04:23.000000 inorbit_edge-1.9.2/inorbit_edge/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-05-02 22:04:23.000000 inorbit_edge-1.9.2/inorbit_edge/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:04:31.657637 inorbit_edge-1.9.2/inorbit_edge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-02 22:04:31.000000 inorbit_edge-1.9.2/inorbit_edge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-02 22:04:31.000000 inorbit_edge-1.9.2/inorbit_edge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 22:04:31.000000 inorbit_edge-1.9.2/inorbit_edge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 22:04:31.000000 inorbit_edge-1.9.2/inorbit_edge.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-02 22:04:31.000000 inorbit_edge-1.9.2/inorbit_edge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 22:04:31.000000 inorbit_edge-1.9.2/inorbit_edge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-02 22:04:31.657637 inorbit_edge-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-02 22:04:23.000000 inorbit_edge-1.9.2/setup.py
```

### Comparing `inorbit_edge-1.9.1/CONTRIBUTING.md` & `inorbit_edge-1.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `inorbit_edge-1.9.1/LICENSE` & `inorbit_edge-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inorbit_edge-1.9.1/PKG-INFO` & `inorbit_edge-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inorbit_edge
-Version: 1.9.1
+Version: 1.9.2
 Summary: InOrbit Python Edge SDK
 Home-page: https://github.com/inorbit-ai/edge-sdk-python
 Author: InOrbit
 Author-email: support@inorbit.ai
 License: UNKNOWN
 Keywords: inorbit_edge
 Platform: UNKNOWN
```

### Comparing `inorbit_edge-1.9.1/README.md` & `inorbit_edge-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `inorbit_edge-1.9.1/inorbit_edge/inorbit_pb2.py` & `inorbit_edge-1.9.2/inorbit_edge/inorbit_pb2.py`

 * *Files identical despite different names*

### Comparing `inorbit_edge-1.9.1/inorbit_edge/missions.py` & `inorbit_edge-1.9.2/inorbit_edge/missions.py`

 * *Files identical despite different names*

### Comparing `inorbit_edge-1.9.1/inorbit_edge/robot.py` & `inorbit_edge-1.9.2/inorbit_edge/robot.py`

 * *Files 0% similar despite different names*

```diff
@@ -788,15 +788,15 @@
             return False
         return (
             math.sqrt(
                 (self._last_pose.x - waypoint.x) ** 2
                 + (self._last_pose.y - waypoint.y) ** 2,
             )
             <= tolerance.positionMeters
-            and (self._last_pose.theta - waypoint.theta) % (2 * math.pi)
+            and abs(self._last_pose.theta - waypoint.theta) % (2 * math.pi)
             <= tolerance.angularRadians
         )
 
     def publish_key_values(self, key_values, custom_field="0", is_event=False):
         """Publish key value pairs
 
         Args:
```

### Comparing `inorbit_edge-1.9.1/inorbit_edge/utils.py` & `inorbit_edge-1.9.2/inorbit_edge/utils.py`

 * *Files identical despite different names*

### Comparing `inorbit_edge-1.9.1/inorbit_edge/video.py` & `inorbit_edge-1.9.2/inorbit_edge/video.py`

 * *Files identical despite different names*

### Comparing `inorbit_edge-1.9.1/inorbit_edge.egg-info/PKG-INFO` & `inorbit_edge-1.9.2/inorbit_edge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inorbit-edge
-Version: 1.9.1
+Version: 1.9.2
 Summary: InOrbit Python Edge SDK
 Home-page: https://github.com/inorbit-ai/edge-sdk-python
 Author: InOrbit
 Author-email: support@inorbit.ai
 License: UNKNOWN
 Keywords: inorbit_edge
 Platform: UNKNOWN
```

### Comparing `inorbit_edge-1.9.1/inorbit_edge.egg-info/requires.txt` & `inorbit_edge-1.9.2/inorbit_edge.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `inorbit_edge-1.9.1/setup.py` & `inorbit_edge-1.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,10 +89,10 @@
     setup_requires=setup_requirements,
     test_suite="inorbit_edge/tests",
     tests_require=test_requirements,
     extras_require=extra_requirements,
     url="https://github.com/inorbit-ai/edge-sdk-python",
     # Do not edit this string manually, always use bumpversion
     # Details in CONTRIBUTING.rst
-    version="1.9.1",
+    version="1.9.2",
     zip_safe=False,
 )
```

