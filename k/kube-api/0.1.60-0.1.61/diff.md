# Comparing `tmp/kube_api-0.1.60.tar.gz` & `tmp/kube_api-0.1.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kube_api-0.1.60.tar", last modified: Mon May  8 00:54:02 2023, max compression
+gzip compressed data, was "kube_api-0.1.61.tar", last modified: Mon May  8 01:20:14 2023, max compression
```

## Comparing `kube_api-0.1.60.tar` & `kube_api-0.1.61.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:54:02.738541 kube_api-0.1.60/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-08 00:54:02.738541 kube_api-0.1.60/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:54:02.738541 kube_api-0.1.60/kube_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:53:54.000000 kube_api-0.1.60/kube_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-08 00:53:54.000000 kube_api-0.1.60/kube_api/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    25447 2023-05-08 00:53:54.000000 kube_api-0.1.60/kube_api/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-08 00:53:54.000000 kube_api-0.1.60/kube_api/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-08 00:53:54.000000 kube_api-0.1.60/kube_api/pods.py
--rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-05-08 00:53:54.000000 kube_api-0.1.60/kube_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-08 00:53:54.000000 kube_api-0.1.60/kube_api/volumeclaims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:54:02.738541 kube_api-0.1.60/kube_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-08 00:54:02.000000 kube_api-0.1.60/kube_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-08 00:54:02.000000 kube_api-0.1.60/kube_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 00:54:02.000000 kube_api-0.1.60/kube_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 00:54:02.000000 kube_api-0.1.60/kube_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 00:54:02.000000 kube_api-0.1.60/kube_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 00:54:02.738541 kube_api-0.1.60/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-08 00:53:54.000000 kube_api-0.1.60/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:20:14.472102 kube_api-0.1.61/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-08 01:20:14.472102 kube_api-0.1.61/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:20:14.472102 kube_api-0.1.61/kube_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 01:20:04.000000 kube_api-0.1.61/kube_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-08 01:20:04.000000 kube_api-0.1.61/kube_api/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25447 2023-05-08 01:20:04.000000 kube_api-0.1.61/kube_api/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-08 01:20:04.000000 kube_api-0.1.61/kube_api/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-08 01:20:04.000000 kube_api-0.1.61/kube_api/pods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10221 2023-05-08 01:20:04.000000 kube_api-0.1.61/kube_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-08 01:20:04.000000 kube_api-0.1.61/kube_api/volumeclaims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:20:14.472102 kube_api-0.1.61/kube_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-08 01:20:14.000000 kube_api-0.1.61/kube_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-08 01:20:14.000000 kube_api-0.1.61/kube_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 01:20:14.000000 kube_api-0.1.61/kube_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 01:20:14.000000 kube_api-0.1.61/kube_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 01:20:14.000000 kube_api-0.1.61/kube_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 01:20:14.472102 kube_api-0.1.61/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-08 01:20:04.000000 kube_api-0.1.61/setup.py
```

### Comparing `kube_api-0.1.60/PKG-INFO` & `kube_api-0.1.61/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kube_api
-Version: 0.1.60
+Version: 0.1.61
 Summary: A simple Kubernetes Python API
 Home-page: https://github.com/labdave/kube_api
 Author: Qiu Qin
 Author-email: qiuosier@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kube_api-0.1.60/kube_api/config.py` & `kube_api-0.1.61/kube_api/config.py`

 * *Files identical despite different names*

### Comparing `kube_api-0.1.60/kube_api/jobs.py` & `kube_api-0.1.61/kube_api/jobs.py`

 * *Files identical despite different names*

### Comparing `kube_api-0.1.60/kube_api/namespaces.py` & `kube_api-0.1.61/kube_api/namespaces.py`

 * *Files identical despite different names*

### Comparing `kube_api-0.1.60/kube_api/pods.py` & `kube_api-0.1.61/kube_api/pods.py`

 * *Files identical despite different names*

### Comparing `kube_api-0.1.60/kube_api/utils.py` & `kube_api-0.1.61/kube_api/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,18 @@
     response = None
     try:
         response = client.get_instance(inst_request)
     except BaseException as e:
         logging.info(f"Filestore Instance {name} does not exist. Creating now.")
 
     if not response:
+        if storage_class == "filestore-ssd" and capacity < 2560:
+            capacity = 2560
+        elif storage_class == "filestore-hdd" and capacity < 1024:
+            capacity = 1024
         instance = filestore_v1.Instance(
             tier=tier,
             file_shares=[filestore_v1.FileShareConfig(name=name.replace("-", "_"), capacity_gb=capacity)],
             networks=[filestore_v1.NetworkConfig(network="davelab-private")]
         )
 
         # Initialize request argument(s)
```

### Comparing `kube_api-0.1.60/kube_api/volumeclaims.py` & `kube_api-0.1.61/kube_api/volumeclaims.py`

 * *Files identical despite different names*

### Comparing `kube_api-0.1.60/kube_api.egg-info/PKG-INFO` & `kube_api-0.1.61/kube_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kube-api
-Version: 0.1.60
+Version: 0.1.61
 Summary: A simple Kubernetes Python API
 Home-page: https://github.com/labdave/kube_api
 Author: Qiu Qin
 Author-email: qiuosier@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kube_api-0.1.60/setup.py` & `kube_api-0.1.61/setup.py`

 * *Files identical despite different names*

