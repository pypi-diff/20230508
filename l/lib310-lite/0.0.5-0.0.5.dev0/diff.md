# Comparing `tmp/lib310_lite-0.0.5.tar.gz` & `tmp/lib310_lite-0.0.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib310_lite-0.0.5.tar", max compression
+gzip compressed data, was "lib310_lite-0.0.5.dev0.tar", max compression
```

## Comparing `lib310_lite-0.0.5.tar` & `lib310_lite-0.0.5.dev0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0      249 2023-03-08 14:56:22.920616 lib310_lite-0.0.5/lib310_lite/__init__.py
--rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.0.5/lib310_lite/bigquery/_functions.py
--rw-r--r--   0        0        0     7467 2023-03-08 14:56:22.918017 lib310_lite-0.0.5/lib310_lite/bigquery/client.py
--rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.0.5/lib310_lite/bigquery/constants.py
--rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.0.5/lib310_lite/fucntion.py
--rw-r--r--   0        0        0     9952 2023-05-01 20:32:25.307400 lib310_lite-0.0.5/lib310_lite/mldl/mldl.py
--rw-r--r--   0        0        0      769 2023-05-01 20:14:07.640872 lib310_lite-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 lib310_lite-0.0.5/setup.py
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 lib310_lite-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-03-08 14:56:22.920616 lib310_lite-0.0.5.dev0/lib310_lite/__init__.py
+-rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.0.5.dev0/lib310_lite/bigquery/_functions.py
+-rw-r--r--   0        0        0     7467 2023-05-08 08:51:40.656605 lib310_lite-0.0.5.dev0/lib310_lite/bigquery/client.py
+-rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.0.5.dev0/lib310_lite/bigquery/constants.py
+-rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.0.5.dev0/lib310_lite/fucntion.py
+-rw-r--r--   0        0        0     9457 2023-05-08 08:54:28.807696 lib310_lite-0.0.5.dev0/lib310_lite/mldl/mldl.py
+-rw-r--r--   0        0        0      843 2023-05-08 09:08:49.952690 lib310_lite-0.0.5.dev0/lib310_lite/mldl/models/InteractionModel.py
+-rw-r--r--   0        0        0     2102 2023-05-08 09:07:24.596219 lib310_lite-0.0.5.dev0/lib310_lite/mldl/models/SeqLangModel.py
+-rw-r--r--   0        0        0      803 2023-05-08 09:20:53.701182 lib310_lite-0.0.5.dev0/pyproject.toml
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 lib310_lite-0.0.5.dev0/setup.py
+-rw-r--r--   0        0        0      897 1970-01-01 00:00:00.000000 lib310_lite-0.0.5.dev0/PKG-INFO
```

### Comparing `lib310_lite-0.0.5/lib310_lite/bigquery/client.py` & `lib310_lite-0.0.5.dev0/lib310_lite/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.5/lib310_lite/bigquery/constants.py` & `lib310_lite-0.0.5.dev0/lib310_lite/bigquery/constants.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.5/lib310_lite/mldl/mldl.py` & `lib310_lite-0.0.5.dev0/lib310_lite/mldl/mldl.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 import numpy as np
-from pymongo import MongoClient, ASCENDING
 import random
 import time
 import pandas as pd
 from threading import Thread, Event
 from queue import Queue
 import concurrent.futures
 from bounded_pool_executor import BoundedThreadPoolExecutor
 import dask.dataframe as dd
 from ..bigquery.client import Client as BigQueryClient
 from ..bigquery.constants import FileFormat
 
+# PGSQL
+from sqlalchemy import create_engine
+from sqlalchemy.orm import sessionmaker
+from .models.SeqLangModel import SeqLangModel
+from .models.InteractionModel import InteractionModel
+
 
 class MLDL:
 
     __TRAIN = 'TRAIN'
     __TEST = 'TEST'
+    __VAL = 'VAL'
     __MAIN = 'MAIN'
     __INTERACTION = 'INTERACTION'
-    __DB_NAME = 'A310'
-    __TOKEN_NAMES = 'token_names'
-    __PROTEIN_NAMES = 'protein_names'
-    __TAXONOMIES = 'taxonomies'
-    __ORGANISMS = 'organisms'
-    __PARTS = {__INTERACTION: 1, __TOKEN_NAMES: 1, __PROTEIN_NAMES: 1, __TAXONOMIES: 1, __ORGANISMS: 0}
+    __PARTS = {__INTERACTION: 1}
 
-    def __init__(self, mongo_url: str, cache_size: int = 50, num_threads: int = 10, random_seed: int = time.time()):
+    def __init__(self, db_url: str, cache_size: int = 50, num_threads: int = 10, random_seed: int = time.time()):
         random.seed(random_seed)
-        self.client = MongoClient(mongo_url)
+        self.engine = create_engine(db_url)
+        self.Session = sessionmaker(bind=self.engine)
+
         self.bq_client = BigQueryClient()
-        self.db = self.client[MLDL.__DB_NAME]
 
-        self.collections = {
-            MLDL.__TRAIN: {
-                MLDL.__MAIN: self.db['seq_lang5_copy'],
-                MLDL.__INTERACTION: self.db['interactions_lang5_train'],
-            },
-            MLDL.__TEST: {
-                MLDL.__MAIN: self.db['seq_lang5_copy'],
-                MLDL.__INTERACTION: self.db['interactions_lang5_test'],
-            }
-        }
+        # self.collections = {
+        #     MLDL.__TRAIN: {
+        #         MLDL.__MAIN: self.db['seq_lang5_copy'],
+        #         MLDL.__INTERACTION: self.db['interactions_lang5_train'],
+        #     },
+        #     MLDL.__TEST: {
+        #         MLDL.__MAIN: self.db['seq_lang5_copy'],
+        #         MLDL.__INTERACTION: self.db['interactions_lang5_test'],
+        #     }
+        # }
 
         # this is the pool of samples row_id
         self.sample_cache = []
         # this is the maximum number of requests we fetch sooner from the database
         self.max_queue_size = cache_size
         # this is the number of threads we use to fetch data from the database
         self.num_threads = num_threads
@@ -69,38 +71,38 @@
         :param max_length: maximum length of the sequence
         :param min_num_feature: minimum number of features
         :param stage: TRAIN or TEST
         :param parts: the parts of the data that we want to fetch
         :return: a pandas dataframe
         """
         stage = stage.upper()
-        if stage == MLDL.__TRAIN:
-            col = self.collections[MLDL.__TRAIN]
-        elif stage == MLDL.__TEST:
-            col = self.collections[MLDL.__TEST]
-        else:
-            raise ValueError('Stage must be either TRAIN or TEST')
+        # if stage == MLDL.__TRAIN:
+        #     col = self.collections[MLDL.__TRAIN]
+        # elif stage == MLDL.__TEST:
+        #     col = self.collections[MLDL.__TEST]
+        # else:
+        #     raise ValueError('Stage must be either TRAIN or TEST')
 
         if parts is None:
             parts = MLDL.__PARTS
 
         hit = self.queue_key == f'{num}_{max_length}_{min_num_feature}_{stage}'
         if hit:
             # HIT
             return pd.DataFrame(self.queue.get())
 
         # MISS
-        table = '1_uniprot.mongo_lang5'
+        table = '1_uniprot.pg_lang5'
         
         if len(self.sample_cache) == 0 or not self.pool_key or self.pool_key != f'{max_length}_{min_num_feature}_{stage}':
             self.pool_key = f'{max_length}_{min_num_feature}_{stage}'
             res = self.bq_client.cache_query(
                 query=f"SELECT row_id FROM `{table}` WHERE len <= {max_length} and token_size >= {min_num_feature} and stage = '{stage}'",
                 name=f'{max_length}_{min_num_feature}_{stage}',
-                destination_format=FileFormat.CSV,
+                destination_format=FileFormat.CSV
             )
             ddf = dd.read_csv(res['uri'])
             df = ddf.compute()
             self.sample_cache = df['row_id'].tolist()
 
         # killing the previous thread
         if self.filler_thread is not None:
@@ -110,61 +112,61 @@
             self.kill_event.clear()
             self.queue = Queue(self.max_queue_size)
 
         # generate new key
         self.queue_key = f'{num}_{max_length}_{min_num_feature}_{stage}'
 
         # start new thread
-        self.filler_thread = Thread(target=self.filler, args=(num, col, stage, parts))
+        self.filler_thread = Thread(target=self.filler, args=(num, stage, parts))
         self.filler_thread.start()
         time.sleep(3)
-        return self.fetch_sample(num, col, stage, parts)
+        return self.fetch_sample(num, stage, parts)
 
-    def filler(self, num: int, col, stage: str, parts: dict = None):
+    def filler(self, num: int, stage: str, parts: dict = None):
         """
         This function is used to fill the queue with data then get batch read data from the queue
         :param num: number of samples
-        :param col: collections of the data
         :param stage: TRAIN or TEST
         :param parts: the parts of the data that we want to fetch
         """
         if parts is None:
             parts = MLDL.__PARTS
         with BoundedThreadPoolExecutor(max_workers=self.num_threads) as executor:
             while not self.kill_event.is_set():
-                executor.submit(self.filler_worker, num, col, stage, parts)
+                executor.submit(self.filler_worker, num, stage, parts)
             while not self.queue.empty():
                 self.queue.get()
             executor.shutdown(wait=True)
 
-    def filler_worker(self, num: int, col, stage: str, parts: dict = None):
+    def filler_worker(self, num: int, stage: str, parts: dict = None):
         if parts is None:
             parts = MLDL.__PARTS
-        df = self.fetch_sample(num, col, stage, parts)
+        df = self.fetch_sample(num, stage, parts)
         self.queue.put(df)
         return
 
-    def fetch_sample(self, num: int, collections, stage: str, parts: dict = None):
+    def fetch_sample(self, num: int, stage: str, parts: dict = None):
         """
         This function is used to fetch the data from the database
         Run two threads to fetch the data from the database
         :param num: number of samples
-        :param collections: collections of the data
         :param stage: TRAIN or TEST
         :param parts: the parts of the data that we want to fetch
         :return: dataframe of the data
         """
         if parts is None:
             parts = MLDL.__PARTS
         try:
+            # get random row_id from the pool
             index_list = random.sample(self.sample_cache, min(num, len(self.sample_cache)))
+
             with concurrent.futures.ThreadPoolExecutor() as executor:
-                main_thread = executor.submit(self.fetch_sample_main, index_list, collections[MLDL.__MAIN], stage, parts)
+                main_thread = executor.submit(self.fetch_sample_main, index_list, stage, parts)
                 if parts[MLDL.__INTERACTION] and parts[MLDL.__INTERACTION] == 1:
-                    interaction_thread = executor.submit(self.fetch_sample_interaction, index_list, collections[MLDL.__INTERACTION])
+                    interaction_thread = executor.submit(self.fetch_sample_interaction, index_list)
 
                 main_df = main_thread.result()
                 interaction_df = pd.DataFrame()
                 if parts[MLDL.__INTERACTION] and parts[MLDL.__INTERACTION] == 1:
                     interaction_df = interaction_thread.result()
 
                 if len(interaction_df) == 0:
@@ -180,52 +182,53 @@
                 time.sleep(1)
             else:
                 time.sleep(self.retry * 10)
             self.retry += 1
             print(f'Cannot fetch data from database, retry number {self.retry} times')
             if self.retry > 7:
                 raise Exception('Cannot fetch data from database')
-            return self.fetch_sample(num, collections, stage, parts)
+            return self.fetch_sample(num, stage, parts)
 
-    def fetch_sample_main(self, index_list: list, col, stage: str, parts: dict = None):
+    def fetch_sample_main(self, index_list: list, stage: str, parts: dict = None):
         """
         This function is used to fetch the main data from the database
         :param index_list: list of row_ids
-        :param col: main collection
         :param stage: stage of the data
         :param parts: parts of the data
         :return: dataframe of main data
         """
+        session = self.Session()
         if parts is None:
             parts = MLDL.__PARTS
-        token_names = 0
-        if not parts[MLDL.__TOKEN_NAMES] or parts[MLDL.__TOKEN_NAMES] == 1:
-            token_names = 1
-        protein_names = 0
-        if not parts[MLDL.__PROTEIN_NAMES] or parts[MLDL.__PROTEIN_NAMES] == 1:
-            protein_names = 1
-        taxonomies = 0
-        if not parts[MLDL.__TAXONOMIES] or parts[MLDL.__TAXONOMIES] == 1:
-            taxonomies = 1
-        organisms = 0
-        if not parts[MLDL.__ORGANISMS] or parts[MLDL.__ORGANISMS] == 1:
-            organisms = 1
-        cursor = col.find({'row_id': {'$in': index_list}, 'stage': stage}, {'_id': 0, 'row_id': 1, 'sequence': 1,
-                                                                            'token_ids': 1, 'token_names': token_names, 'protein_names': protein_names, 'taxonomies': taxonomies, 'organisms': organisms})
-        return pd.DataFrame(list(cursor))
+        try:
+            results = session.query(SeqLangModel).filter(SeqLangModel.row_id.in_(index_list)).all()
+            df = pd.DataFrame([r.to_dict() for r in results])
+        except Exception as e:
+            print(e)
+            raise Exception('Cannot fetch data from database <SeqLang>')
+        finally:
+            session.close()
+        return df
 
-    def fetch_sample_interaction(self, index_list: list, col):
+    def fetch_sample_interaction(self, index_list: list):
         """
         This function is used to fetch the interaction data from the database
         :param index_list: list of row_ids
-        :param col: interaction collection
         :return: dataframe of interaction data
         """
-        cursor = col.find({'row_id': {'$in': index_list}}, {'_id': 0, 'row_id': 1, 'interactions': 1})
-        return pd.DataFrame(list(cursor))
+        session = self.Session()
+        try:
+            results = session.query(InteractionModel).filter(InteractionModel.row_id.in_(index_list)).all()
+            df = pd.DataFrame([r.to_dict() for r in results])
+        except Exception as e:
+            print(e)
+            raise Exception('Cannot fetch data from database <Interaction>')
+        finally:
+            session.close()
+        return df
 
     def terminate(self):
         """
         Terminate the filler threads and clear the queue
         """
         # Terminate the filler thread
         if self.filler_thread is not None:
```

### Comparing `lib310_lite-0.0.5/pyproject.toml` & `lib310_lite-0.0.5.dev0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tool.poetry]
 name = "lib310_lite"
-version = "0.0.5"
+version = "0.0.5.dev"
 description = "lib310 Lite Python Package"
 authors = ["310 <info@310.ai>"]
 maintainers = ["Saman Fekri <saman@310.ai>"]
 keywords = ["biology", "AI", "genomics", "bioinforma", "machine learning", "GAN"]
 packages = [
     { include = "lib310_lite" }
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 google-cloud = ">=0.34.0"
 google-cloud-bigquery = ">=3.2.0"
 db-dtypes = ">=1.0.0"
-pymongo = ">=4.0.0"
 numpy = "<1.23.0"
 bounded_pool_executor = ">=0.0.0"
 dask = ">=2022.11.0"
 distributed = ">=2022.11.0"
 dask-sql = ">=2022.11.0"
 gcsfs = ">=2022.11.0"
+SQLAlchemy = ">=2.0.0"
+psycopg2-binary= ">=2.9.0"
 
 
 [tool.poetry.dev-dependencies]
 pytest = ">7.1.2"
 python-dotenv = ">=0.19.0"
```

### Comparing `lib310_lite-0.0.5/setup.py` & `lib310_lite-0.0.5.dev0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['lib310_lite', 'lib310_lite.bigquery', 'lib310_lite.mldl']
+['lib310_lite',
+ 'lib310_lite.bigquery',
+ 'lib310_lite.mldl',
+ 'lib310_lite.mldl.models']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['bounded_pool_executor>=0.0.0',
+['SQLAlchemy>=2.0.0',
+ 'bounded_pool_executor>=0.0.0',
  'dask-sql>=2022.11.0',
  'dask>=2022.11.0',
  'db-dtypes>=1.0.0',
  'distributed>=2022.11.0',
  'gcsfs>=2022.11.0',
  'google-cloud-bigquery>=3.2.0',
  'google-cloud>=0.34.0',
  'numpy<1.23.0',
- 'pymongo>=4.0.0']
+ 'psycopg2-binary>=2.9.0']
 
 setup_kwargs = {
     'name': 'lib310-lite',
-    'version': '0.0.5',
+    'version': '0.0.5.dev0',
     'description': 'lib310 Lite Python Package',
     'long_description': 'None',
     'author': '310',
     'author_email': 'info@310.ai',
     'maintainer': 'Saman Fekri',
     'maintainer_email': 'saman@310.ai',
     'url': 'None',
```

### Comparing `lib310_lite-0.0.5/PKG-INFO` & `lib310_lite-0.0.5.dev0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: lib310-lite
-Version: 0.0.5
+Version: 0.0.5.dev0
 Summary: lib310 Lite Python Package
 Keywords: biology,AI,genomics,bioinforma,machine learning,GAN
 Author: 310
 Author-email: info@310.ai
 Maintainer: Saman Fekri
 Maintainer-email: saman@310.ai
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: SQLAlchemy (>=2.0.0)
 Requires-Dist: bounded_pool_executor (>=0.0.0)
 Requires-Dist: dask (>=2022.11.0)
 Requires-Dist: dask-sql (>=2022.11.0)
 Requires-Dist: db-dtypes (>=1.0.0)
 Requires-Dist: distributed (>=2022.11.0)
 Requires-Dist: gcsfs (>=2022.11.0)
 Requires-Dist: google-cloud (>=0.34.0)
 Requires-Dist: google-cloud-bigquery (>=3.2.0)
 Requires-Dist: numpy (<1.23.0)
-Requires-Dist: pymongo (>=4.0.0)
+Requires-Dist: psycopg2-binary (>=2.9.0)
```

