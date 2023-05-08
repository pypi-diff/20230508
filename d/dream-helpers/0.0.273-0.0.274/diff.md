# Comparing `tmp/dream_helpers-0.0.273.tar.gz` & `tmp/dream_helpers-0.0.274.tar.gz`

## Comparing `dream_helpers-0.0.273.tar` & `dream_helpers-0.0.274.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/.bumpversion.cfg
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/Makefile
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/src/dream_helpers/__init__.py
--rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/src/dream_helpers/datahub_helper.py
--rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/src/dream_helpers/kubeflow_helper.py
--rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/src/dream_helpers/minio_helper.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/LICENSE
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/README.md
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/pyproject.toml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dream_helpers-0.0.273/PKG-INFO
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dream_helpers-0.0.274/.bumpversion.cfg
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 dream_helpers-0.0.274/Makefile
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dream_helpers-0.0.274/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dream_helpers-0.0.274/src/dream_helpers/__init__.py
+-rw-r--r--   0        0        0    11960 2020-02-02 00:00:00.000000 dream_helpers-0.0.274/src/dream_helpers/datahub_helper.py
+-rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 dream_helpers-0.0.274/src/dream_helpers/kubeflow_helper.py
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 dream_helpers-0.0.274/src/dream_helpers/minio_helper.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 dream_helpers-0.0.274/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dream_helpers-0.0.274/LICENSE
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dream_helpers-0.0.274/README.md
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 dream_helpers-0.0.274/pyproject.toml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dream_helpers-0.0.274/PKG-INFO
```

### Comparing `dream_helpers-0.0.273/src/dream_helpers/datahub_helper.py` & `dream_helpers-0.0.274/src/dream_helpers/datahub_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
         max_threads=5,
         disable_ssl_verification=True
     )
     return DataHubGraph(config)
 
 def get_dataset_source_url(endpoint: str, dataset_name: str) -> str:
     dataset_urn = make_dataset_urn(platform="s3", name=dataset_name, env="PROD")
-
     with get_client(endpoint=endpoint) as client:
         return client.get_aspect(
             entity_urn=dataset_urn,
             aspect_type=DatasetPropertiesClass,
             version=0
         ).customProperties['table_path']
     
@@ -78,15 +77,16 @@
 def load_csv_dataset_as_pandas_dataframe(dataset:str, 
                                          minio_endpoint:str, 
                                          datahub_endpoint:str) -> pd.DataFrame:
     dataset_source_url = get_dataset_source_url(
         endpoint=datahub_endpoint,
         dataset_name=dataset
     )
-    dataset_source_url = "s3://%s" % dataset_source_url    
+    dataset_source_url = "s3://%s" % dataset_source_url
+    dataset_source_url = "s3://sources/get-sources-example/new%20zealand%20business%20demography%20statistics"    
     logger.info("Dataset source url -> %s" % dataset_source_url)
     return pd.read_csv(
         dataset_source_url,
         storage_options={
             "client_kwargs": {
                 "endpoint_url": minio_endpoint,
                 "aws_access_key_id": "minio",
```

### Comparing `dream_helpers-0.0.273/src/dream_helpers/kubeflow_helper.py` & `dream_helpers-0.0.274/src/dream_helpers/kubeflow_helper.py`

 * *Files identical despite different names*

### Comparing `dream_helpers-0.0.273/src/dream_helpers/minio_helper.py` & `dream_helpers-0.0.274/src/dream_helpers/minio_helper.py`

 * *Files identical despite different names*

### Comparing `dream_helpers-0.0.273/.gitignore` & `dream_helpers-0.0.274/.gitignore`

 * *Files identical despite different names*

