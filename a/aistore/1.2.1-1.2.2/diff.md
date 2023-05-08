# Comparing `tmp/aistore-1.2.1.tar.gz` & `tmp/aistore-1.2.2.tar.gz`

## Comparing `aistore-1.2.1.tar` & `aistore-1.2.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/client.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/common_requirements
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/botocore_patch/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/botocore_patch/__init__.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/botocore_patch/botocore.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/botocore_patch/botocore_requirements
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/pytorch/README.md
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/pytorch/__init__.py
--rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/pytorch/aisio.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/pytorch/dataset.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/pytorch/dev_requirements
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/pytorch/utils.py
--rw-r--r--   0        0        0     5511 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/README.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/__init__.py
--rw-r--r--   0        0        0    26239 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/bucket.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/client.py
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/cluster.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/const.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/errors.py
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/etl.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/etl_const.py
--rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/etl_templates.py
--rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/job.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/list_object_flag.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/namespace.py
--rw-r--r--   0        0        0     8204 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/object.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/object_attributes.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/object_iterator.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/object_reader.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/request_client.py
--rw-r--r--   0        0        0    10384 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/types.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/utils.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/multiobj/__init__.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/multiobj/object_collection.py
--rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/multiobj/object_group.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/multiobj/object_names.py
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/multiobj/object_range.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aistore-1.2.1/aistore/sdk/multiobj/object_template.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aistore-1.2.1/LICENSE
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aistore-1.2.1/.gitignore
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 aistore-1.2.1/README.md
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 aistore-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 aistore-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/client.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/common_requirements
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/botocore_patch/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/botocore_patch/__init__.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/botocore_patch/botocore.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/botocore_patch/botocore_requirements
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/pytorch/README.md
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/pytorch/__init__.py
+-rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/pytorch/aisio.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/pytorch/dataset.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/pytorch/dev_requirements
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/pytorch/utils.py
+-rw-r--r--   0        0        0     5511 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/README.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/__init__.py
+-rw-r--r--   0        0        0    26239 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/bucket.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/client.py
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/cluster.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/const.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/errors.py
+-rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/etl.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/etl_const.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/etl_templates.py
+-rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/job.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/list_object_flag.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/namespace.py
+-rw-r--r--   0        0        0     8204 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/object.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/object_attributes.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/object_iterator.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/object_reader.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/request_client.py
+-rw-r--r--   0        0        0    10465 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/types.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/utils.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/multiobj/__init__.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/multiobj/object_collection.py
+-rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/multiobj/object_group.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/multiobj/object_names.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/multiobj/object_range.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/multiobj/object_template.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aistore-1.2.2/LICENSE
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aistore-1.2.2/.gitignore
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 aistore-1.2.2/README.md
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 aistore-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 aistore-1.2.2/PKG-INFO
```

### Comparing `aistore-1.2.1/aistore/botocore_patch/README.md` & `aistore-1.2.2/aistore/botocore_patch/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/botocore_patch/botocore.py` & `aistore-1.2.2/aistore/botocore_patch/botocore.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/pytorch/README.md` & `aistore-1.2.2/aistore/pytorch/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/pytorch/aisio.py` & `aistore-1.2.2/aistore/pytorch/aisio.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/pytorch/dataset.py` & `aistore-1.2.2/aistore/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/pytorch/utils.py` & `aistore-1.2.2/aistore/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/sdk/README.md` & `aistore-1.2.2/aistore/sdk/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/sdk/bucket.py` & `aistore-1.2.2/aistore/sdk/bucket.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/sdk/client.py` & `aistore-1.2.2/aistore/sdk/client.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/sdk/cluster.py` & `aistore-1.2.2/aistore/sdk/cluster.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/sdk/const.py` & `aistore-1.2.2/aistore/sdk/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # URL Params
 # See api/apc/query.go
 QPARAM_WHAT = "what"
 QPARAM_ETL_NAME = "etl_name"
 QPARAM_PROVIDER = "provider"
 QPARAM_BCK_TO = "bck_to"
-QPARAM_KEEP_REMOTE = "keep_md"
+QPARAM_KEEP_REMOTE = "keep_bck_md"
 QPARAM_ARCHPATH = "archpath"
 QPARAM_FORCE = "frc"
 QPARAM_PRIMARY_READY_REB = "prr"
 QPARAM_NAMESPACE = "namespace"
 
 # URL Param values
 # See api/apc/query.go
```

### Comparing `aistore-1.2.1/aistore/sdk/errors.py` & `aistore-1.2.2/aistore/sdk/errors.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/sdk/etl.py` & `aistore-1.2.2/aistore/sdk/etl.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,14 +102,15 @@
         transform: Callable,
         dependencies: List[str] = None,
         preimported_modules: List[str] = None,
         runtime: str = _get_default_runtime(),
         communication_type: str = DEFAULT_ETL_COMM,
         timeout: str = DEFAULT_ETL_TIMEOUT,
         chunk_size: int = None,
+        transform_url: bool = False,
     ) -> str:
         """
         Initializes ETL based on the provided source code. Returns etl_name.
 
         Args:
             transform (Callable): Transform function of the ETL
             dependencies (list[str]): Python dependencies to install
@@ -119,14 +120,16 @@
                 python3.8v2] Runtime environment of the ETL [choose from: python3.8v2, python3.10v2, python3.11v2]
                 (see ext/etl/runtime/all.go)
             communication_type (str): [optional, default="hpush"] Communication type of the ETL (options: hpull, hrev,
                 hpush, io)
             timeout (str): [optional, default="5m"] Timeout of the ETL job (e.g. 5m for 5 minutes)
             chunk_size (int): Chunk size in bytes if transform function in streaming data.
                 (whole object is read by default)
+            transform_url (optional, bool): If True, the runtime will provide the transform function with the URL to the
+             object on the target rather than the raw bytes read from the object
         Returns:
             Job ID string associated with this ETL
         """
         _validate_comm_type(communication_type, ETL_COMM_CODE)
 
         # code functions to call
         functions = {
@@ -140,14 +143,15 @@
             timeout=timeout,
             dependencies=self._encode_dependencies(dependencies),
             functions=functions,
             code=self._encode_transform(
                 transform, preimported_modules, communication_type
             ),
             chunk_size=chunk_size,
+            transform_url=transform_url,
         ).as_dict()
 
         return self._client.request(
             HTTP_METHOD_PUT,
             path=URL_PATH_ETL,
             json=value,
         ).text
```

### Comparing `aistore-1.2.1/aistore/sdk/etl_const.py` & `aistore-1.2.2/aistore/sdk/etl_const.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/sdk/etl_templates.py` & `aistore-1.2.2/aistore/sdk/etl_templates.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/sdk/job.py` & `aistore-1.2.2/aistore/sdk/job.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/sdk/list_object_flag.py` & `aistore-1.2.2/aistore/sdk/list_object_flag.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/sdk/object.py` & `aistore-1.2.2/aistore/sdk/object.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/sdk/object_attributes.py` & `aistore-1.2.2/aistore/sdk/object_attributes.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/sdk/object_iterator.py` & `aistore-1.2.2/aistore/sdk/object_iterator.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/sdk/object_reader.py` & `aistore-1.2.2/aistore/sdk/object_reader.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/sdk/request_client.py` & `aistore-1.2.2/aistore/sdk/request_client.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/sdk/types.py` & `aistore-1.2.2/aistore/sdk/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,24 +242,26 @@
     """
 
     runtime: str
     dependencies: str
     functions: Dict[str, str]
     code: str
     chunk_size: int = None
+    transform_url: bool = False
 
     def as_dict(self):
         dict_rep = {
             "id": self.etl_name,
             "runtime": self.runtime,
             "communication": f"{self.communication_type}://",
             "timeout": self.timeout,
             "funcs": self.functions,
             "code": self.code,
             "dependencies": self.dependencies,
+            "transform_url": self.transform_url,
         }
         if self.chunk_size:
             dict_rep["chunk_size"] = self.chunk_size
         return dict_rep
 
 
 class PromoteAPIArgs(BaseModel):
```

### Comparing `aistore-1.2.1/aistore/sdk/utils.py` & `aistore-1.2.2/aistore/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/sdk/multiobj/object_collection.py` & `aistore-1.2.2/aistore/sdk/multiobj/object_collection.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/sdk/multiobj/object_group.py` & `aistore-1.2.2/aistore/sdk/multiobj/object_group.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/sdk/multiobj/object_names.py` & `aistore-1.2.2/aistore/sdk/multiobj/object_names.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/sdk/multiobj/object_range.py` & `aistore-1.2.2/aistore/sdk/multiobj/object_range.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/aistore/sdk/multiobj/object_template.py` & `aistore-1.2.2/aistore/sdk/multiobj/object_template.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/LICENSE` & `aistore-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/.gitignore` & `aistore-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/README.md` & `aistore-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.2.1/pyproject.toml` & `aistore-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [tool.pytest.ini_options]
 markers = [
     "etl: marks tests as using etl and therefore requiring k8s cluster",
 ]
 
 [project]
 name = "aistore"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   { name="AIStore Team", email="ais@exchange.nvidia.com" },
 ]
 description = "A (growing) set of client-side APIs to access and utilize clusters, buckets, and objects on AIStore."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT License"}
```

### Comparing `aistore-1.2.1/PKG-INFO` & `aistore-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aistore
-Version: 1.2.1
+Version: 1.2.2
 Summary: A (growing) set of client-side APIs to access and utilize clusters, buckets, and objects on AIStore.
 Project-URL: Homepage, https://aiatscale.org
 Project-URL: Download, https://github.com/NVIDIA/aistore/tags
 Project-URL: Documentation, https://aiatscale.org/docs/
 Project-URL: Release notes, https://github.com/NVIDIA/aistore/releases/
 Project-URL: Source, https://github.com/NVIDIA/aistore/
 Author-email: AIStore Team <ais@exchange.nvidia.com>
```

