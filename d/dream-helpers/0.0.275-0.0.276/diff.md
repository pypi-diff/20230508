# Comparing `tmp/dream_helpers-0.0.275.tar.gz` & `tmp/dream_helpers-0.0.276.tar.gz`

## Comparing `dream_helpers-0.0.275.tar` & `dream_helpers-0.0.276.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dream_helpers-0.0.275/.bumpversion.cfg
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 dream_helpers-0.0.275/Makefile
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dream_helpers-0.0.275/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dream_helpers-0.0.275/src/dream_helpers/__init__.py
--rw-r--r--   0        0        0    11961 2020-02-02 00:00:00.000000 dream_helpers-0.0.275/src/dream_helpers/datahub_helper.py
--rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 dream_helpers-0.0.275/src/dream_helpers/kubeflow_helper.py
--rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 dream_helpers-0.0.275/src/dream_helpers/minio_helper.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 dream_helpers-0.0.275/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dream_helpers-0.0.275/LICENSE
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dream_helpers-0.0.275/README.md
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 dream_helpers-0.0.275/pyproject.toml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dream_helpers-0.0.275/PKG-INFO
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dream_helpers-0.0.276/.bumpversion.cfg
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 dream_helpers-0.0.276/Makefile
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dream_helpers-0.0.276/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dream_helpers-0.0.276/src/dream_helpers/__init__.py
+-rw-r--r--   0        0        0    11932 2020-02-02 00:00:00.000000 dream_helpers-0.0.276/src/dream_helpers/datahub_helper.py
+-rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 dream_helpers-0.0.276/src/dream_helpers/kubeflow_helper.py
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 dream_helpers-0.0.276/src/dream_helpers/minio_helper.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 dream_helpers-0.0.276/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dream_helpers-0.0.276/LICENSE
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dream_helpers-0.0.276/README.md
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 dream_helpers-0.0.276/pyproject.toml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dream_helpers-0.0.276/PKG-INFO
```

### Comparing `dream_helpers-0.0.275/src/dream_helpers/datahub_helper.py` & `dream_helpers-0.0.276/src/dream_helpers/datahub_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,20 +67,21 @@
             version=0
         ).customProperties['table_path']
     
 def get_dataset_properties(endpoint: str, dataset_urn: str) -> str:
     with get_client(endpoint=endpoint) as client:
         return client.get_dataset_properties(
             entity_urn=dataset_urn
-            #make_dataset_urn(platform="s3", name=dataset_name, env="PROD")
         )
     
-def load_csv_dataset_as_pandas_dataframe(dataset:str, 
-                                         minio_endpoint:str, 
-                                         datahub_endpoint:str) -> pd.DataFrame:
+
+def load_csv_dataset_as_pandas_dataframe(
+    dataset:str, 
+    minio_endpoint:str="http://minio-service.kubeflow.svc.cluster.local:9000", 
+    datahub_endpoint:str="http://datahub-datahub-gms.datahub.svc.cluster.local:8080") -> pd.DataFrame:
     dataset_source_url = get_dataset_source_url(
         endpoint=datahub_endpoint,
         dataset_name=dataset
     )
     dataset_source_url = "s3://%s" % dataset_source_url
     #dataset_source_url = "s3://sources/get-sources-example/new%20zealand%20business%20demography%20statistics"    
     logger.info("Dataset source url -> %s" % dataset_source_url)
```

### Comparing `dream_helpers-0.0.275/src/dream_helpers/kubeflow_helper.py` & `dream_helpers-0.0.276/src/dream_helpers/kubeflow_helper.py`

 * *Files identical despite different names*

### Comparing `dream_helpers-0.0.275/src/dream_helpers/minio_helper.py` & `dream_helpers-0.0.276/src/dream_helpers/minio_helper.py`

 * *Files identical despite different names*

### Comparing `dream_helpers-0.0.275/.gitignore` & `dream_helpers-0.0.276/.gitignore`

 * *Files identical despite different names*

