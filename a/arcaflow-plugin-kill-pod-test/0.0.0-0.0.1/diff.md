# Comparing `tmp/arcaflow_plugin_kill_pod_test-0.0.0.tar.gz` & `tmp/arcaflow_plugin_kill_pod_test-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcaflow_plugin_kill_pod_test-0.0.0.tar", max compression
+gzip compressed data, was "arcaflow_plugin_kill_pod_test-0.0.1.tar", max compression
```

## Comparing `arcaflow_plugin_kill_pod_test-0.0.0.tar` & `arcaflow_plugin_kill_pod_test-0.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1558 2023-03-16 16:07:00.104462 arcaflow_plugin_kill_pod_test-0.0.0/Dockerfile
--rw-r--r--   0        0        0    10174 2023-01-25 15:49:28.000000 arcaflow_plugin_kill_pod_test-0.0.0/LICENSE
--rw-r--r--   0        0        0      673 2023-01-25 15:49:28.000000 arcaflow_plugin_kill_pod_test-0.0.0/README.md
--rwxr-xr-x   0        0        0     9786 2023-05-08 13:05:05.064232 arcaflow_plugin_kill_pod_test-0.0.0/arcaflow_plugin_kill_pod.py
--rw-r--r--   0        0        0      105 2023-03-16 16:07:00.105462 arcaflow_plugin_kill_pod_test-0.0.0/docker-compose.yaml
--rw-r--r--   0        0        0    52658 2023-05-04 14:41:52.873263 arcaflow_plugin_kill_pod_test-0.0.0/poetry.lock
--rw-r--r--   0        0        0     1002 2023-05-08 13:07:12.980341 arcaflow_plugin_kill_pod_test-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     6495 2023-01-25 15:49:28.000000 arcaflow_plugin_kill_pod_test-0.0.0/tests/test_arcaflow_plugin_kill_pod.py
--rw-r--r--   0        0        0     1417 1970-01-01 00:00:00.000000 arcaflow_plugin_kill_pod_test-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1558 2023-03-16 16:07:00.104462 arcaflow_plugin_kill_pod_test-0.0.1/Dockerfile
+-rw-r--r--   0        0        0    10174 2023-01-25 15:49:28.000000 arcaflow_plugin_kill_pod_test-0.0.1/LICENSE
+-rw-r--r--   0        0        0      673 2023-01-25 15:49:28.000000 arcaflow_plugin_kill_pod_test-0.0.1/README.md
+-rwxr-xr-x   0        0        0     9968 2023-05-08 13:22:47.883454 arcaflow_plugin_kill_pod_test-0.0.1/arcaflow_plugin_kill_pod.py
+-rw-r--r--   0        0        0      105 2023-03-16 16:07:00.105462 arcaflow_plugin_kill_pod_test-0.0.1/docker-compose.yaml
+-rw-r--r--   0        0        0    52658 2023-05-04 14:41:52.873263 arcaflow_plugin_kill_pod_test-0.0.1/poetry.lock
+-rw-r--r--   0        0        0     1002 2023-05-08 13:23:31.638836 arcaflow_plugin_kill_pod_test-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6495 2023-01-25 15:49:28.000000 arcaflow_plugin_kill_pod_test-0.0.1/tests/test_arcaflow_plugin_kill_pod.py
+-rw-r--r--   0        0        0     1417 1970-01-01 00:00:00.000000 arcaflow_plugin_kill_pod_test-0.0.1/PKG-INFO
```

### Comparing `arcaflow_plugin_kill_pod_test-0.0.0/Dockerfile` & `arcaflow_plugin_kill_pod_test-0.0.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `arcaflow_plugin_kill_pod_test-0.0.0/LICENSE` & `arcaflow_plugin_kill_pod_test-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arcaflow_plugin_kill_pod_test-0.0.0/README.md` & `arcaflow_plugin_kill_pod_test-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `arcaflow_plugin_kill_pod_test-0.0.0/arcaflow_plugin_kill_pod.py` & `arcaflow_plugin_kill_pod_test-0.0.1/arcaflow_plugin_kill_pod.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,7 +304,16 @@
                     return "error", PodErrorOutput(
                         "timeout while waiting for pods to come up"
                     )
     except Exception:
         return "error", PodErrorOutput(format_exc())
 
 
+if __name__ == "__main__":
+    sys.exit(
+        plugin.run(
+            plugin.build_schema(
+                kill_pods,
+                wait_for_pods,
+            )
+        )
+    )
```

### Comparing `arcaflow_plugin_kill_pod_test-0.0.0/poetry.lock` & `arcaflow_plugin_kill_pod_test-0.0.1/poetry.lock`

 * *Files identical despite different names*

### Comparing `arcaflow_plugin_kill_pod_test-0.0.0/pyproject.toml` & `arcaflow_plugin_kill_pod_test-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "arcaflow_plugin_kill_pod_test"
 # Do not change, the version is automatically updated in CI.
-version = "0.0.0"
+version = "0.0.1"
 description = "Chaos Engineering Kill Pod Plugin for Arcaflow"
 authors = []
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `arcaflow_plugin_kill_pod_test-0.0.0/tests/test_arcaflow_plugin_kill_pod.py` & `arcaflow_plugin_kill_pod_test-0.0.1/tests/test_arcaflow_plugin_kill_pod.py`

 * *Files identical despite different names*

### Comparing `arcaflow_plugin_kill_pod_test-0.0.0/PKG-INFO` & `arcaflow_plugin_kill_pod_test-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcaflow-plugin-kill-pod-test
-Version: 0.0.0
+Version: 0.0.1
 Summary: Chaos Engineering Kill Pod Plugin for Arcaflow
 Home-page: https://github.com/redhat-chaos/arcaflow-plugin-kill-pod
 License: Apache-2.0
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

