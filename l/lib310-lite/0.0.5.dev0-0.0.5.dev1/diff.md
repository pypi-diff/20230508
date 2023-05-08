# Comparing `tmp/lib310_lite-0.0.5.dev0.tar.gz` & `tmp/lib310_lite-0.0.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib310_lite-0.0.5.dev0.tar", max compression
+gzip compressed data, was "lib310_lite-0.0.5.dev1.tar", max compression
```

## Comparing `lib310_lite-0.0.5.dev0.tar` & `lib310_lite-0.0.5.dev1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      249 2023-03-08 14:56:22.920616 lib310_lite-0.0.5.dev0/lib310_lite/__init__.py
--rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.0.5.dev0/lib310_lite/bigquery/_functions.py
--rw-r--r--   0        0        0     7467 2023-05-08 08:51:40.656605 lib310_lite-0.0.5.dev0/lib310_lite/bigquery/client.py
--rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.0.5.dev0/lib310_lite/bigquery/constants.py
--rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.0.5.dev0/lib310_lite/fucntion.py
--rw-r--r--   0        0        0     9457 2023-05-08 08:54:28.807696 lib310_lite-0.0.5.dev0/lib310_lite/mldl/mldl.py
--rw-r--r--   0        0        0      843 2023-05-08 09:08:49.952690 lib310_lite-0.0.5.dev0/lib310_lite/mldl/models/InteractionModel.py
--rw-r--r--   0        0        0     2102 2023-05-08 09:07:24.596219 lib310_lite-0.0.5.dev0/lib310_lite/mldl/models/SeqLangModel.py
--rw-r--r--   0        0        0      803 2023-05-08 09:20:53.701182 lib310_lite-0.0.5.dev0/pyproject.toml
--rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 lib310_lite-0.0.5.dev0/setup.py
--rw-r--r--   0        0        0      897 1970-01-01 00:00:00.000000 lib310_lite-0.0.5.dev0/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-03-08 14:56:22.920616 lib310_lite-0.0.5.dev1/lib310_lite/__init__.py
+-rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.0.5.dev1/lib310_lite/bigquery/_functions.py
+-rw-r--r--   0        0        0     7467 2023-05-08 08:51:40.656605 lib310_lite-0.0.5.dev1/lib310_lite/bigquery/client.py
+-rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.0.5.dev1/lib310_lite/bigquery/constants.py
+-rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.0.5.dev1/lib310_lite/fucntion.py
+-rw-r--r--   0        0        0     9716 2023-05-08 09:35:35.797881 lib310_lite-0.0.5.dev1/lib310_lite/mldl/mldl.py
+-rw-r--r--   0        0        0      843 2023-05-08 09:08:49.952690 lib310_lite-0.0.5.dev1/lib310_lite/mldl/models/InteractionModel.py
+-rw-r--r--   0        0        0     2102 2023-05-08 09:07:24.596219 lib310_lite-0.0.5.dev1/lib310_lite/mldl/models/SeqLangModel.py
+-rw-r--r--   0        0        0      804 2023-05-08 09:38:04.514021 lib310_lite-0.0.5.dev1/pyproject.toml
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 lib310_lite-0.0.5.dev1/setup.py
+-rw-r--r--   0        0        0      897 1970-01-01 00:00:00.000000 lib310_lite-0.0.5.dev1/PKG-INFO
```

### Comparing `lib310_lite-0.0.5.dev0/lib310_lite/bigquery/client.py` & `lib310_lite-0.0.5.dev1/lib310_lite/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.5.dev0/lib310_lite/bigquery/constants.py` & `lib310_lite-0.0.5.dev1/lib310_lite/bigquery/constants.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.5.dev0/lib310_lite/mldl/mldl.py` & `lib310_lite-0.0.5.dev1/lib310_lite/mldl/mldl.py`

 * *Files 7% similar despite different names*

```diff
@@ -134,39 +134,42 @@
             while not self.kill_event.is_set():
                 executor.submit(self.filler_worker, num, stage, parts)
             while not self.queue.empty():
                 self.queue.get()
             executor.shutdown(wait=True)
 
     def filler_worker(self, num: int, stage: str, parts: dict = None):
+        session = self.Session()
         if parts is None:
             parts = MLDL.__PARTS
-        df = self.fetch_sample(num, stage, parts)
+        df = self.fetch_sample(num, stage, session, parts)
         self.queue.put(df)
+        session.close()
         return
 
-    def fetch_sample(self, num: int, stage: str, parts: dict = None):
+    def fetch_sample(self, num: int, stage: str, session, parts: dict = None):
         """
         This function is used to fetch the data from the database
         Run two threads to fetch the data from the database
         :param num: number of samples
         :param stage: TRAIN or TEST
+        :param session: the session that we use to connect to the database
         :param parts: the parts of the data that we want to fetch
         :return: dataframe of the data
         """
         if parts is None:
             parts = MLDL.__PARTS
         try:
             # get random row_id from the pool
             index_list = random.sample(self.sample_cache, min(num, len(self.sample_cache)))
 
             with concurrent.futures.ThreadPoolExecutor() as executor:
-                main_thread = executor.submit(self.fetch_sample_main, index_list, stage, parts)
+                main_thread = executor.submit(self.fetch_sample_main, index_list, stage, session, parts)
                 if parts[MLDL.__INTERACTION] and parts[MLDL.__INTERACTION] == 1:
-                    interaction_thread = executor.submit(self.fetch_sample_interaction, index_list)
+                    interaction_thread = executor.submit(self.fetch_sample_interaction, index_list, session)
 
                 main_df = main_thread.result()
                 interaction_df = pd.DataFrame()
                 if parts[MLDL.__INTERACTION] and parts[MLDL.__INTERACTION] == 1:
                     interaction_df = interaction_thread.result()
 
                 if len(interaction_df) == 0:
@@ -182,52 +185,50 @@
                 time.sleep(1)
             else:
                 time.sleep(self.retry * 10)
             self.retry += 1
             print(f'Cannot fetch data from database, retry number {self.retry} times')
             if self.retry > 7:
                 raise Exception('Cannot fetch data from database')
-            return self.fetch_sample(num, stage, parts)
+            return self.fetch_sample(num, stage, session, parts)
 
-    def fetch_sample_main(self, index_list: list, stage: str, parts: dict = None):
+    def fetch_sample_main(self, index_list: list, stage: str, session, parts: dict = None):
         """
         This function is used to fetch the main data from the database
         :param index_list: list of row_ids
         :param stage: stage of the data
+        :param session: the session that we use to connect to the database
         :param parts: parts of the data
         :return: dataframe of main data
         """
-        session = self.Session()
+        # session = self.Session()
         if parts is None:
             parts = MLDL.__PARTS
         try:
             results = session.query(SeqLangModel).filter(SeqLangModel.row_id.in_(index_list)).all()
             df = pd.DataFrame([r.to_dict() for r in results])
         except Exception as e:
             print(e)
             raise Exception('Cannot fetch data from database <SeqLang>')
-        finally:
-            session.close()
         return df
 
-    def fetch_sample_interaction(self, index_list: list):
+    def fetch_sample_interaction(self, index_list: list, session):
         """
         This function is used to fetch the interaction data from the database
         :param index_list: list of row_ids
+        :param session: the session that we use to connect to the database
         :return: dataframe of interaction data
         """
-        session = self.Session()
+        # session = self.Session()
         try:
             results = session.query(InteractionModel).filter(InteractionModel.row_id.in_(index_list)).all()
             df = pd.DataFrame([r.to_dict() for r in results])
         except Exception as e:
             print(e)
             raise Exception('Cannot fetch data from database <Interaction>')
-        finally:
-            session.close()
         return df
 
     def terminate(self):
         """
         Terminate the filler threads and clear the queue
         """
         # Terminate the filler thread
```

### Comparing `lib310_lite-0.0.5.dev0/lib310_lite/mldl/models/InteractionModel.py` & `lib310_lite-0.0.5.dev1/lib310_lite/mldl/models/InteractionModel.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.5.dev0/lib310_lite/mldl/models/SeqLangModel.py` & `lib310_lite-0.0.5.dev1/lib310_lite/mldl/models/SeqLangModel.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.5.dev0/pyproject.toml` & `lib310_lite-0.0.5.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib310_lite"
-version = "0.0.5.dev"
+version = "0.0.5.dev1"
 description = "lib310 Lite Python Package"
 authors = ["310 <info@310.ai>"]
 maintainers = ["Saman Fekri <saman@310.ai>"]
 keywords = ["biology", "AI", "genomics", "bioinforma", "machine learning", "GAN"]
 packages = [
     { include = "lib310_lite" }
 ]
```

### Comparing `lib310_lite-0.0.5.dev0/setup.py` & `lib310_lite-0.0.5.dev1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'google-cloud-bigquery>=3.2.0',
  'google-cloud>=0.34.0',
  'numpy<1.23.0',
  'psycopg2-binary>=2.9.0']
 
 setup_kwargs = {
     'name': 'lib310-lite',
-    'version': '0.0.5.dev0',
+    'version': '0.0.5.dev1',
     'description': 'lib310 Lite Python Package',
     'long_description': 'None',
     'author': '310',
     'author_email': 'info@310.ai',
     'maintainer': 'Saman Fekri',
     'maintainer_email': 'saman@310.ai',
     'url': 'None',
```

### Comparing `lib310_lite-0.0.5.dev0/PKG-INFO` & `lib310_lite-0.0.5.dev1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib310-lite
-Version: 0.0.5.dev0
+Version: 0.0.5.dev1
 Summary: lib310 Lite Python Package
 Keywords: biology,AI,genomics,bioinforma,machine learning,GAN
 Author: 310
 Author-email: info@310.ai
 Maintainer: Saman Fekri
 Maintainer-email: saman@310.ai
 Requires-Python: >=3.8
```

