# Comparing `tmp/proteus_cli-0.2.25.tar.gz` & `tmp/proteus_cli-0.2.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteus_cli-0.2.25.tar", max compression
+gzip compressed data, was "proteus_cli-0.2.26.tar", max compression
```

## Comparing `proteus_cli-0.2.25.tar` & `proteus_cli-0.2.26.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1330 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/__init__.py
--rw-r--r--   0        0        0      384 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/api/__init__.py
--rw-r--r--   0        0        0     1784 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/api/decorators.py
--rw-r--r--   0        0        0      849 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/api/hooks.py
--rw-r--r--   0        0        0        0 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/buckets/__init__.py
--rw-r--r--   0        0        0     1092 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/buckets/commands.py
--rw-r--r--   0        0        0     2621 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/config.py
--rw-r--r--   0        0        0        0 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/__init__.py
--rw-r--r--   0        0        0     1332 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/commands.py
--rw-r--r--   0        0        0        0 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/__init__.py
--rw-r--r--   0        0        0      939 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/__init__.py
--rw-r--r--   0        0        0      323 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/case/__init__.py
--rw-r--r--   0        0        0      851 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/case/cnn_pca.py
--rw-r--r--   0        0        0     3447 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/case/hm.py
--rw-r--r--   0        0        0     3054 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/case/well_model.py
--rw-r--r--   0        0        0      446 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/common/__init__.py
--rw-r--r--   0        0        0     3238 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/common/cnn_pca.py
--rw-r--r--   0        0        0     2009 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/common/hm.py
--rw-r--r--   0        0        0     1542 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/common/well_model.py
--rw-r--r--   0        0        0     2665 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/default.py
--rw-r--r--   0        0        0      418 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/step/__init__.py
--rw-r--r--   0        0        0      125 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/step/cnn_pca.py
--rw-r--r--   0        0        0     2415 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/step/hm.py
--rw-r--r--   0        0        0      128 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/step/well_model.py
--rw-r--r--   0        0        0      673 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/init_keywords.json
--rw-r--r--   0        0        0    13633 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/preprocess_functions.py
--rw-r--r--   0        0        0     4446 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/process_step.py
--rw-r--r--   0        0        0     8185 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/utils.py
--rw-r--r--   0        0        0      411 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/well_init_keywords.json
--rw-r--r--   0        0        0        0 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/sources/__init__.py
--rw-r--r--   0        0        0     4737 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/sources/az.py
--rw-r--r--   0        0        0      824 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/sources/common.py
--rw-r--r--   0        0        0     2366 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/sources/local.py
--rw-r--r--   0        0        0     1783 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/sources/s3.py
--rw-r--r--   0        0        0     9008 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/upload.py
--rw-r--r--   0        0        0        0 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/debugger/__init__.py
--rw-r--r--   0        0        0     2265 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/debugger/commands.py
--rw-r--r--   0        0        0     3926 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/debugger/init_keyword_check.py
--rw-r--r--   0        0        0        0 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/debugger/restart_keyword_check.py
--rw-r--r--   0        0        0        0 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/cli/jobs/__init__.py
--rw-r--r--   0        0        0     1283 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/cli/jobs/commands.py
--rw-r--r--   0        0        0     3026 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/cli/jobs/list.py
--rw-r--r--   0        0        0      100 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/cli/runtime.py
--rw-r--r--   0        0        0        0 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/cli/simulations/__init__.py
--rw-r--r--   0        0        0     2460 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/cli/simulations/commands.py
--rw-r--r--   0        0        0     7603 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/cli/simulations/create.py
--rw-r--r--   0        0        0     4119 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/cli/simulations/dependencySolver.py
--rw-r--r--   0        0        0     5190 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/cli/simulations/opm.py
--rw-r--r--   0        0        0      449 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/logging.ini
--rw-r--r--   0        0        0     1533 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/pyproject.toml
--rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 proteus_cli-0.2.25/PKG-INFO
+-rw-r--r--   0        0        0     1330 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/__init__.py
+-rw-r--r--   0        0        0      384 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/api/__init__.py
+-rw-r--r--   0        0        0     1784 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/api/decorators.py
+-rw-r--r--   0        0        0      849 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/api/hooks.py
+-rw-r--r--   0        0        0        0 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/buckets/__init__.py
+-rw-r--r--   0        0        0     1092 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/buckets/commands.py
+-rw-r--r--   0        0        0     2621 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/config.py
+-rw-r--r--   0        0        0        0 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/__init__.py
+-rw-r--r--   0        0        0     1332 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/commands.py
+-rw-r--r--   0        0        0        0 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/preprocessor/__init__.py
+-rw-r--r--   0        0        0      939 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/preprocessor/config/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/preprocessor/config/case/__init__.py
+-rw-r--r--   0        0        0      851 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/preprocessor/config/case/cnn_pca.py
+-rw-r--r--   0        0        0     3447 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/preprocessor/config/case/hm.py
+-rw-r--r--   0        0        0     3054 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/preprocessor/config/case/well_model.py
+-rw-r--r--   0        0        0      446 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/preprocessor/config/common/__init__.py
+-rw-r--r--   0        0        0     3238 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/preprocessor/config/common/cnn_pca.py
+-rw-r--r--   0        0        0     2009 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/preprocessor/config/common/hm.py
+-rw-r--r--   0        0        0     1542 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/preprocessor/config/common/well_model.py
+-rw-r--r--   0        0        0     2665 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/preprocessor/config/default.py
+-rw-r--r--   0        0        0      418 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/preprocessor/config/step/__init__.py
+-rw-r--r--   0        0        0      125 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/preprocessor/config/step/cnn_pca.py
+-rw-r--r--   0        0        0     2415 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/preprocessor/config/step/hm.py
+-rw-r--r--   0        0        0      128 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/preprocessor/config/step/well_model.py
+-rw-r--r--   0        0        0      673 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/preprocessor/init_keywords.json
+-rw-r--r--   0        0        0    13633 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/preprocessor/preprocess_functions.py
+-rw-r--r--   0        0        0     4446 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/preprocessor/process_step.py
+-rw-r--r--   0        0        0     8185 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/preprocessor/utils.py
+-rw-r--r--   0        0        0      411 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/preprocessor/well_init_keywords.json
+-rw-r--r--   0        0        0        0 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/sources/__init__.py
+-rw-r--r--   0        0        0     5316 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/sources/az.py
+-rw-r--r--   0        0        0      824 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/sources/common.py
+-rw-r--r--   0        0        0     2366 2023-05-08 10:38:21.027882 proteus_cli-0.2.26/cli/datasets/sources/local.py
+-rw-r--r--   0        0        0     1783 2023-05-08 10:38:21.031882 proteus_cli-0.2.26/cli/datasets/sources/s3.py
+-rw-r--r--   0        0        0     9008 2023-05-08 10:38:21.031882 proteus_cli-0.2.26/cli/datasets/upload.py
+-rw-r--r--   0        0        0        0 2023-05-08 10:38:21.031882 proteus_cli-0.2.26/cli/debugger/__init__.py
+-rw-r--r--   0        0        0     2265 2023-05-08 10:38:21.031882 proteus_cli-0.2.26/cli/debugger/commands.py
+-rw-r--r--   0        0        0     3926 2023-05-08 10:38:21.031882 proteus_cli-0.2.26/cli/debugger/init_keyword_check.py
+-rw-r--r--   0        0        0        0 2023-05-08 10:38:21.031882 proteus_cli-0.2.26/cli/debugger/restart_keyword_check.py
+-rw-r--r--   0        0        0        0 2023-05-08 10:38:21.031882 proteus_cli-0.2.26/cli/jobs/__init__.py
+-rw-r--r--   0        0        0     1283 2023-05-08 10:38:21.031882 proteus_cli-0.2.26/cli/jobs/commands.py
+-rw-r--r--   0        0        0     3026 2023-05-08 10:38:21.031882 proteus_cli-0.2.26/cli/jobs/list.py
+-rw-r--r--   0        0        0      100 2023-05-08 10:38:21.031882 proteus_cli-0.2.26/cli/runtime.py
+-rw-r--r--   0        0        0        0 2023-05-08 10:38:21.031882 proteus_cli-0.2.26/cli/simulations/__init__.py
+-rw-r--r--   0        0        0     2460 2023-05-08 10:38:21.031882 proteus_cli-0.2.26/cli/simulations/commands.py
+-rw-r--r--   0        0        0     7603 2023-05-08 10:38:21.031882 proteus_cli-0.2.26/cli/simulations/create.py
+-rw-r--r--   0        0        0     4119 2023-05-08 10:38:21.031882 proteus_cli-0.2.26/cli/simulations/dependencySolver.py
+-rw-r--r--   0        0        0     5190 2023-05-08 10:38:21.031882 proteus_cli-0.2.26/cli/simulations/opm.py
+-rw-r--r--   0        0        0      449 2023-05-08 10:38:21.031882 proteus_cli-0.2.26/logging.ini
+-rw-r--r--   0        0        0     1533 2023-05-08 10:38:21.031882 proteus_cli-0.2.26/pyproject.toml
+-rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 proteus_cli-0.2.26/PKG-INFO
```

### Comparing `proteus_cli-0.2.25/cli/__init__.py` & `proteus_cli-0.2.26/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/api/decorators.py` & `proteus_cli-0.2.26/cli/api/decorators.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/api/hooks.py` & `proteus_cli-0.2.26/cli/api/hooks.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/buckets/commands.py` & `proteus_cli-0.2.26/cli/buckets/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/config.py` & `proteus_cli-0.2.26/cli/config.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/datasets/commands.py` & `proteus_cli-0.2.26/cli/datasets/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/datasets/preprocessor/config/__init__.py` & `proteus_cli-0.2.26/cli/datasets/preprocessor/config/__init__.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/datasets/preprocessor/config/case/cnn_pca.py` & `proteus_cli-0.2.26/cli/datasets/preprocessor/config/case/cnn_pca.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/datasets/preprocessor/config/case/hm.py` & `proteus_cli-0.2.26/cli/datasets/preprocessor/config/case/hm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/datasets/preprocessor/config/case/well_model.py` & `proteus_cli-0.2.26/cli/datasets/preprocessor/config/case/well_model.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/datasets/preprocessor/config/common/cnn_pca.py` & `proteus_cli-0.2.26/cli/datasets/preprocessor/config/common/cnn_pca.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/datasets/preprocessor/config/common/hm.py` & `proteus_cli-0.2.26/cli/datasets/preprocessor/config/common/hm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/datasets/preprocessor/config/common/well_model.py` & `proteus_cli-0.2.26/cli/datasets/preprocessor/config/common/well_model.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/datasets/preprocessor/config/default.py` & `proteus_cli-0.2.26/cli/datasets/preprocessor/config/default.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/datasets/preprocessor/config/step/hm.py` & `proteus_cli-0.2.26/cli/datasets/preprocessor/config/step/hm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/datasets/preprocessor/init_keywords.json` & `proteus_cli-0.2.26/cli/datasets/preprocessor/init_keywords.json`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/datasets/preprocessor/preprocess_functions.py` & `proteus_cli-0.2.26/cli/datasets/preprocessor/preprocess_functions.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/datasets/preprocessor/process_step.py` & `proteus_cli-0.2.26/cli/datasets/preprocessor/process_step.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/datasets/preprocessor/utils.py` & `proteus_cli-0.2.26/cli/datasets/preprocessor/utils.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/datasets/sources/az.py` & `proteus_cli-0.2.26/cli/datasets/sources/az.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import re
 
 # from azure.storage.blob._models import BlobProperties as AzureBlobProperties
 from io import BytesIO
 
 from azure.storage.blob import ContainerClient
 from azure.core.credentials import AzureSasCredential
+from azure.core.exceptions import HttpResponseError
+from azure.identity import DefaultAzureCredential
 
 from .common import Source, SourcedItem
 from ... import proteus
 from cli.config import config
 
 AZURE_SAS_TOKEN = config.AZURE_SAS_TOKEN
 
@@ -22,31 +24,44 @@
 
     def __init__(self, uri):
         super().__init__(uri)
         match = self.URI_re.match(uri.rstrip("/"))
         assert match is not None, f"{uri} must be an s3 URI"
         container_name = match.groupdict()["container_name"]
         storage_url = f'https://{match.groupdict()["bucket_name"]}'
+
+        if AZURE_SAS_TOKEN:
+            credential = AzureSasCredential(AZURE_SAS_TOKEN)
+        else:
+            credential = DefaultAzureCredential(exclude_managed_identity_credential=True)
+
         self.container_client = ContainerClient(
             storage_url,
-            credential=AzureSasCredential(AZURE_SAS_TOKEN),
+            credential=credential,
             container_name=container_name,
         )
 
     @proteus.may_insist_up_to(5, 1)
     def list_contents(self, starts_with="", ends_with=None):
         bucket_uri = self.uri
         match = self.URI_re.match(bucket_uri.rstrip("/"))
         assert match is not None, f"{bucket_uri} must be an s3 URI"
         prefix = match.groupdict()["prefix"]
-        for item in self.container_client.list_blobs(name_starts_with=prefix + starts_with):
-            item_name = f'/{item["name"]}'
-            assert item_name.startswith("/" + prefix + starts_with)
-            if ends_with is None or item_name.endswith(ends_with):
-                yield SourcedItem(item, item_name, self, item.size)
+        try:
+            for item in self.container_client.list_blobs(name_starts_with=prefix + starts_with):
+                item_name = f'/{item["name"]}'
+                assert item_name.startswith("/" + prefix + starts_with)
+                if ends_with is None or item_name.endswith(ends_with):
+                    yield SourcedItem(item, item_name, self, item.size)
+        except HttpResponseError as e:
+            proteus.logger.error(
+                "Missing Azure credentials to perform this operation, please "
+                "provide a SAS token or provide another authentication method on Azure"
+            )
+            raise e
 
     def open(self, reference):
         reference_path = reference.get("name")
         file_size = reference["size"]
         modified = reference["last_modified"]
 
         stream = BytesIO()
```

### Comparing `proteus_cli-0.2.25/cli/datasets/sources/common.py` & `proteus_cli-0.2.26/cli/datasets/sources/common.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/datasets/sources/local.py` & `proteus_cli-0.2.26/cli/datasets/sources/local.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/datasets/sources/s3.py` & `proteus_cli-0.2.26/cli/datasets/sources/s3.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/datasets/upload.py` & `proteus_cli-0.2.26/cli/datasets/upload.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/debugger/commands.py` & `proteus_cli-0.2.26/cli/debugger/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/debugger/init_keyword_check.py` & `proteus_cli-0.2.26/cli/debugger/init_keyword_check.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/jobs/commands.py` & `proteus_cli-0.2.26/cli/jobs/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/jobs/list.py` & `proteus_cli-0.2.26/cli/jobs/list.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/simulations/commands.py` & `proteus_cli-0.2.26/cli/simulations/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/simulations/create.py` & `proteus_cli-0.2.26/cli/simulations/create.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/simulations/dependencySolver.py` & `proteus_cli-0.2.26/cli/simulations/dependencySolver.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/cli/simulations/opm.py` & `proteus_cli-0.2.26/cli/simulations/opm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.25/pyproject.toml` & `proteus_cli-0.2.26/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proteus-cli"
-version = "0.2.25"
+version = "0.2.26"
 description = ""
 authors = []
 packages = [
     {include="cli"},
     {include="logging.ini"}
 ]
```

### Comparing `proteus_cli-0.2.25/PKG-INFO` & `proteus_cli-0.2.26/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteus-cli
-Version: 0.2.25
+Version: 0.2.26
 Summary: 
 Requires-Python: >=3.8,<3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: azure-identity (>=1.12.0,<2.0.0)
 Requires-Dist: azure-storage-blob (>=12.8.1,<13.0.0)
 Requires-Dist: boto3 (>=1.17.79,<2.0.0)
```

