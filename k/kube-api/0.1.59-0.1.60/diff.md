# Comparing `tmp/kube_api-0.1.59.tar.gz` & `tmp/kube_api-0.1.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kube_api-0.1.59.tar", last modified: Thu May  4 17:11:06 2023, max compression
+gzip compressed data, was "kube_api-0.1.60.tar", last modified: Mon May  8 00:54:02 2023, max compression
```

## Comparing `kube_api-0.1.59.tar` & `kube_api-0.1.60.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:11:06.547321 kube_api-0.1.59/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-04 17:11:06.547321 kube_api-0.1.59/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:11:06.547321 kube_api-0.1.59/kube_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:54.000000 kube_api-0.1.59/kube_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-04 17:10:54.000000 kube_api-0.1.59/kube_api/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    25366 2023-05-04 17:10:54.000000 kube_api-0.1.59/kube_api/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-04 17:10:54.000000 kube_api-0.1.59/kube_api/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-04 17:10:54.000000 kube_api-0.1.59/kube_api/pods.py
--rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-05-04 17:10:54.000000 kube_api-0.1.59/kube_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-04 17:10:54.000000 kube_api-0.1.59/kube_api/volumeclaims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:11:06.547321 kube_api-0.1.59/kube_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-04 17:11:06.000000 kube_api-0.1.59/kube_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-04 17:11:06.000000 kube_api-0.1.59/kube_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:11:06.000000 kube_api-0.1.59/kube_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 17:11:06.000000 kube_api-0.1.59/kube_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 17:11:06.000000 kube_api-0.1.59/kube_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 17:11:06.547321 kube_api-0.1.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-04 17:10:54.000000 kube_api-0.1.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:54:02.738541 kube_api-0.1.60/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-08 00:54:02.738541 kube_api-0.1.60/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:54:02.738541 kube_api-0.1.60/kube_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:53:54.000000 kube_api-0.1.60/kube_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-08 00:53:54.000000 kube_api-0.1.60/kube_api/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25447 2023-05-08 00:53:54.000000 kube_api-0.1.60/kube_api/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-08 00:53:54.000000 kube_api-0.1.60/kube_api/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-08 00:53:54.000000 kube_api-0.1.60/kube_api/pods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-05-08 00:53:54.000000 kube_api-0.1.60/kube_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-08 00:53:54.000000 kube_api-0.1.60/kube_api/volumeclaims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:54:02.738541 kube_api-0.1.60/kube_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-08 00:54:02.000000 kube_api-0.1.60/kube_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-08 00:54:02.000000 kube_api-0.1.60/kube_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 00:54:02.000000 kube_api-0.1.60/kube_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 00:54:02.000000 kube_api-0.1.60/kube_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 00:54:02.000000 kube_api-0.1.60/kube_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 00:54:02.738541 kube_api-0.1.60/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-08 00:53:54.000000 kube_api-0.1.60/setup.py
```

### Comparing `kube_api-0.1.59/PKG-INFO` & `kube_api-0.1.60/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kube_api
-Version: 0.1.59
+Version: 0.1.60
 Summary: A simple Kubernetes Python API
 Home-page: https://github.com/labdave/kube_api
 Author: Qiu Qin
 Author-email: qiuosier@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kube_api-0.1.59/kube_api/config.py` & `kube_api-0.1.60/kube_api/config.py`

 * *Files identical despite different names*

### Comparing `kube_api-0.1.59/kube_api/jobs.py` & `kube_api-0.1.60/kube_api/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -381,26 +381,27 @@
 
     "workspace" and "outputs" volumes are shared by all containers.
 
     Attributes:
         workspace_path: The mount path for workspace volume.
         outputs_path: The mount path for outputs volume
     """
-    def __init__(self, job_name, namespace='default', workspace_path="/workspace/", output_path=None, workspace_size="1", output_size="1", shared_claim_name=None, backoff_limit=0):
+    def __init__(self, job_name, namespace='default', workspace_path="/workspace/", output_path=None, workspace_size="1", output_size="1", shared_claim_name=None, backoff_limit=0, shared_tier='filestore-hdd'):
         super().__init__(job_name, namespace)
         self.workspace_path = workspace_path
         if not self.workspace_path.endswith("/"):
             self.workspace_path += "/"
         self.outputs_path = output_path
         if isinstance(self.outputs_path, str) and not self.outputs_path.endswith("/"):
             self.outputs_path += "/"
 
         self.workspace_size = workspace_size
         self.output_size = output_size
         self.shared_claim_name = shared_claim_name
+        self.shared_claim_tier = shared_tier
 
         self.job_spec = dict(backoff_limit=backoff_limit)
         self.workspace_vc = None
         self.outputs_vc = None
         # envs will be shared by all jobs.
         self.envs = dict()
         if self.outputs_path:
@@ -436,15 +437,15 @@
                         claim_name=self.job_name+"-ovc"
                     )
                 )
                 volume_mounts.append(
                     client.V1VolumeMount(mount_path=self.outputs_path, name="outputs"),
                 )
         else:
-            self.workspace_vc = VolumeClaim(self.shared_claim_name, self.workspace_size, self.namespace, "filestore-hdd", ['ReadWriteMany'], True)
+            self.workspace_vc = VolumeClaim(self.shared_claim_name, self.workspace_size, self.namespace, self.shared_claim_tier, ['ReadWriteMany'], True)
             self.add_volume(
                 name="workspace",
                 persistent_volume_claim=client.V1PersistentVolumeClaimVolumeSource(
                     claim_name=self.shared_claim_name
                 )
             )
```

### Comparing `kube_api-0.1.59/kube_api/namespaces.py` & `kube_api-0.1.60/kube_api/namespaces.py`

 * *Files identical despite different names*

### Comparing `kube_api-0.1.59/kube_api/pods.py` & `kube_api-0.1.60/kube_api/pods.py`

 * *Files identical despite different names*

### Comparing `kube_api-0.1.59/kube_api/utils.py` & `kube_api-0.1.60/kube_api/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,28 +152,28 @@
                 created = True
                 break
             else:
                 raise RuntimeError(f"({name}) Failure to create a Persistent Volume on the cluster. Response: {str(pv_response)}")
     return created
 
 
-def create_filestore_instance(name, capacity=1024, core_api=None, storage_class="filestore-hdd", namespace="default", vol_name=None, vol_capacity=1024, vol_claim_name=None):
+def create_filestore_instance(name, capacity=1024, core_api=None, storage_class="filestore-hdd", namespace="default", vol_name=None, vol_capacity=1024, vol_claim_name=None, tier=filestore_v1.Instance.Tier.BASIC_HDD):
     # Create a client
     client = filestore_v1.CloudFilestoreManagerClient()
 
     inst_request = filestore_v1.GetInstanceRequest(name=f"projects/davelab-gcloud/locations/us-east1-b/instances/{name}")
     response = None
     try:
         response = client.get_instance(inst_request)
     except BaseException as e:
         logging.info(f"Filestore Instance {name} does not exist. Creating now.")
 
     if not response:
         instance = filestore_v1.Instance(
-            tier=filestore_v1.Instance.Tier.BASIC_HDD,
+            tier=tier,
             file_shares=[filestore_v1.FileShareConfig(name=name.replace("-", "_"), capacity_gb=capacity)],
             networks=[filestore_v1.NetworkConfig(network="davelab-private")]
         )
 
         # Initialize request argument(s)
         request = filestore_v1.CreateInstanceRequest(
             parent="projects/davelab-gcloud/locations/us-east1-b",
```

### Comparing `kube_api-0.1.59/kube_api/volumeclaims.py` & `kube_api-0.1.60/kube_api/volumeclaims.py`

 * *Files identical despite different names*

### Comparing `kube_api-0.1.59/kube_api.egg-info/PKG-INFO` & `kube_api-0.1.60/kube_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kube-api
-Version: 0.1.59
+Version: 0.1.60
 Summary: A simple Kubernetes Python API
 Home-page: https://github.com/labdave/kube_api
 Author: Qiu Qin
 Author-email: qiuosier@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kube_api-0.1.59/setup.py` & `kube_api-0.1.60/setup.py`

 * *Files identical despite different names*

