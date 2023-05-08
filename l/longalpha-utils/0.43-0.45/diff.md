# Comparing `tmp/longalpha_utils-0.43.tar.gz` & `tmp/longalpha_utils-0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.43.tar", last modified: Tue May  2 00:58:42 2023, max compression
+gzip compressed data, was "longalpha_utils-0.45.tar", last modified: Mon May  8 03:02:43 2023, max compression
```

## Comparing `longalpha_utils-0.43.tar` & `longalpha_utils-0.45.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:42.043999 longalpha_utils-0.43/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-02 00:58:42.043999 longalpha_utils-0.43/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:42.039999 longalpha_utils-0.43/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 00:58:30.000000 longalpha_utils-0.43/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 00:58:30.000000 longalpha_utils-0.43/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-02 00:58:30.000000 longalpha_utils-0.43/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-05-02 00:58:30.000000 longalpha_utils-0.43/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-02 00:58:30.000000 longalpha_utils-0.43/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-02 00:58:30.000000 longalpha_utils-0.43/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:42.043999 longalpha_utils-0.43/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-02 00:58:42.000000 longalpha_utils-0.43/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-02 00:58:42.000000 longalpha_utils-0.43/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:58:42.000000 longalpha_utils-0.43/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-02 00:58:42.000000 longalpha_utils-0.43/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 00:58:42.000000 longalpha_utils-0.43/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 00:58:42.043999 longalpha_utils-0.43/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-02 00:58:30.000000 longalpha_utils-0.43/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:02:43.010789 longalpha_utils-0.45/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-08 03:02:43.010789 longalpha_utils-0.45/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:02:43.010789 longalpha_utils-0.45/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-08 03:02:28.000000 longalpha_utils-0.45/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-08 03:02:28.000000 longalpha_utils-0.45/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-08 03:02:28.000000 longalpha_utils-0.45/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-05-08 03:02:28.000000 longalpha_utils-0.45/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-08 03:02:28.000000 longalpha_utils-0.45/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-08 03:02:28.000000 longalpha_utils-0.45/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:02:43.010789 longalpha_utils-0.45/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-08 03:02:42.000000 longalpha_utils-0.45/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-08 03:02:43.000000 longalpha_utils-0.45/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 03:02:42.000000 longalpha_utils-0.45/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-08 03:02:42.000000 longalpha_utils-0.45/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 03:02:42.000000 longalpha_utils-0.45/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 03:02:43.010789 longalpha_utils-0.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-08 03:02:28.000000 longalpha_utils-0.45/setup.py
```

### Comparing `longalpha_utils-0.43/longalpha_utils/messenger.py` & `longalpha_utils-0.45/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.43/longalpha_utils/transfers.py` & `longalpha_utils-0.45/longalpha_utils/transfers.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 import pandas as pd
 from minio import Minio
 from pyspark.conf import SparkConf
 from pyspark.sql import SparkSession, DataFrame
 from sqlalchemy import Engine
 from sqlalchemy import create_engine
 from sqlalchemy import text
-
 from minio.error import S3Error
+
+
 class MinioWrapper:
     def __init__(self, minio_url, minio_access_key, minio_secret_key):
         self.minio_client = Minio(
             endpoint=minio_url,
             access_key=minio_access_key,
             secret_key=minio_secret_key,
             secure=False,
@@ -32,103 +33,94 @@
         """
         try:
             self.minio_client.stat_object(bucket_name, object_name)
             return True
         except S3Error as e:
             if e.code == "NoSuchKey":
                 return False
+
     def fput(
         self,
         file_path,
         bucket_name: str,
         object_name: str,
-    )-> None:
+    ) -> None:
         """
         put a file to s3
         Args:
             file_path: path to the file
             bucket_name: Minio bucket_name
             object_name: object name in the minio bucket
 
         Returns:
 
         """
         self.minio_client.fput_object(bucket_name=bucket_name, object_name=object_name, file_path=file_path)
 
-    def put(self, dataframe: pd.DataFrame, bucket_name: str, object_name: str, file_format: str, index=False) -> None:
+    def put(self, dataframe: pd.DataFrame, bucket_name: str, object_name: str, index=False) -> None:
         """
         put a pandas frame to parquet in s3
 
         Args:
             dataframe: a pandas dataframe
             bucket_name: Minio bucket_name
             object_name: object name in the minio bucket
-            file_format: parquet or pickle
             index: whether to save the index of the dataframe, only used for parquet
 
 
         Returns:
 
         """
         with tempfile.TemporaryDirectory() as temp_dir:
-            if file_format == "parquet":
-                path = os.path.join(temp_dir, "file.parquet")
-                dataframe.to_parquet(path, index=index)
-            elif file_format == "pickle":
-                path = os.path.join(temp_dir, "file.pkl")
-                dataframe.to_pickle(path)
-            else:
-                raise ValueError("Incorrect file format")
+            path = os.path.join(temp_dir, "file.parquet")
+            dataframe.to_parquet(path, index=index)
+
             self.fput(file_path=path, bucket_name=bucket_name, object_name=object_name)
 
     def fget(self, file_path: str, bucket_name: str, object_name: str):
         self.minio_client.fget_object(bucket_name=bucket_name, object_name=object_name, file_path=file_path)
 
     def get(
         self,
         bucket_name: str,
         object_name: str,
-        file_format: str,
     ) -> pd.DataFrame:
         """
         get a parquet from s3 and read it into pandas dataframe
         Args:
             bucket_name: Minio bucket_name
             object_name: path + file_name
-            file_format: parquet or pickle
 
         Returns: A pandas dataframe
 
         """
         file = self.minio_client.get_object(
             bucket_name,
             object_name,
         )
-        read_file = {"parquet": pd.read_parquet, "pickle": pd.read_pickle}
-        res = read_file[file_format](BytesIO(file.data))
+        res = pd.read_parquet(BytesIO(file.data))
         file.close()
         file.release_conn()
         return res
 
-    def get_latest(self, bucket_name: str, file_format: str) -> pd.DataFrame:
+    def get_latest(self, bucket_name: str) -> pd.DataFrame:
         """
         get the latest parquet file and read it into pandas. Note that this does not include files in the
         sub-folders of the bucket. To do this, we need to recursively list all the files in the bucket.
         Args:
             bucket_name: bucket_name: Minio bucket_name
-            file_format: parquet or pickle
 
         Returns: A pandas dataframe
 
         """
         objects = [i for i in self.minio_client.list_objects(bucket_name)]
         time_obj = {obj.last_modified: obj for obj in objects}
         latest_time = max([key for key in time_obj.keys() if key is not None])
         latest_obj = time_obj[latest_time]
-        return self.get(bucket_name=bucket_name, object_name=latest_obj.object_name, file_format=file_format)
+        return self.get(bucket_name=bucket_name, object_name=latest_obj.object_name)
 
     def list(self, bucket_name: str) -> List[str]:
         return [i.object_name for i in self.minio_client.list_objects(bucket_name)]
 
 
 def init_spark(
     spark_executor_memory: str = "30g",
@@ -148,15 +140,14 @@
 
     Args:
         minio_endpoint: minio_endpoint
         minio_access_key:  minio_access_key
         minio_secret_key:  minio_secret_key
         spark_executor_memory: size of spark_executor_memory
         spark_driver_memory: size of spark_driver_memory
-        connect_psql: whether to connect to psql
     Returns:
 
     """
     jars = [
         "org.postgresql:postgresql:42.5.2",
         "org.apache.hadoop:hadoop-aws:3.3.2",
         "com.amazonaws:aws-java-sdk-bundle:1.12.405",
@@ -230,16 +221,14 @@
     Args:
         df: pandas dataframe
         table_name: table name to write to psql
         index: whether to write index to psql
         dtype: data type of column. If a dictionary is used, the keys should be the column names and the values
         should be the SQLAlchemy types or strings for the sqlite3 legacy mode
         if_exists: {‘fail’, ‘replace’, ‘append’}, default ‘append’. How to behave if the table already exists.
-        fail: Raise a ValueError. replace: Drop the table before inserting new values append: Insert new values to
-        the existing table.
         engine: sqlalchemy engine. If not None, then we will use this engine to write to psql.
         user_name: username of psql
         password: password of psql
         host_with_port: host_with_port of psql
         db_name: database name of psql to write to
         kwargs: additional keyword argument passed to DataFrame.to_sql
```

### Comparing `longalpha_utils-0.43/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.45/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.43/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.45/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.43/setup.py` & `longalpha_utils-0.45/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.43",
+    version="0.45",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

