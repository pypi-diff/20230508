# Comparing `tmp/klp-commons-0.0.8.tar.gz` & `tmp/klp-commons-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klp-commons-0.0.8.tar", last modified: Thu Mar 16 16:24:20 2023, max compression
+gzip compressed data, was "klp-commons-0.0.9.tar", last modified: Thu Mar 16 18:07:10 2023, max compression
```

## Comparing `klp-commons-0.0.8.tar` & `klp-commons-0.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1082 2023-03-11 16:29:59.052345 klp-commons-0.0.8/LICENSE
--rw-r--r--   0        0        0     4840 2023-03-11 17:02:05.306612 klp-commons-0.0.8/README.md
--rw-r--r--   0        0        0    10244 2023-03-15 02:52:05.661685 klp-commons-0.0.8/klp_commons/.DS_Store
--rw-r--r--   0        0        0      624 2023-03-16 16:21:06.924909 klp-commons-0.0.8/klp_commons/__init__.py
--rw-r--r--   0        0        0     6148 2023-03-11 14:55:21.254936 klp-commons-0.0.8/klp_commons/controllers/.DS_Store
--rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp-commons-0.0.8/klp_commons/controllers/__init__.py
--rw-r--r--   0        0        0    31510 2023-03-13 05:25:25.017217 klp-commons-0.0.8/klp_commons/controllers/controller_dynamodb.py
--rw-r--r--   0        0        0      260 2023-02-16 19:52:02.340344 klp-commons-0.0.8/klp_commons/controllers/controller_mlflow.py
--rw-r--r--   0        0        0     6591 2023-03-14 16:59:36.965113 klp-commons-0.0.8/klp_commons/controllers/controller_mongodb.py
--rw-r--r--   0        0        0    49187 2023-03-12 05:47:13.143660 klp-commons-0.0.8/klp_commons/controllers/controller_postgresdb.py
--rw-r--r--   0        0        0    34377 2023-03-16 14:33:58.035158 klp-commons-0.0.8/klp_commons/controllers/controller_redshift.py
--rw-r--r--   0        0        0     6148 2023-03-11 14:55:23.888578 klp-commons-0.0.8/klp_commons/cryptools/.DS_Store
--rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp-commons-0.0.8/klp_commons/cryptools/__init__.py
--rw-r--r--   0        0        0      795 2022-11-14 19:44:11.325419 klp-commons-0.0.8/klp_commons/cryptools/cryptology.py
--rw-r--r--   0        0        0     6148 2023-03-11 14:55:26.531304 klp-commons-0.0.8/klp_commons/datadict/.DS_Store
--rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp-commons-0.0.8/klp_commons/datadict/__init__.py
--rw-r--r--   0        0        0    24123 2023-03-14 04:27:56.957869 klp-commons-0.0.8/klp_commons/datadict/struct_dicts.py
--rw-r--r--   0        0        0    18932 2023-03-12 05:47:05.332172 klp-commons-0.0.8/klp_commons/datefinder/__init__.py
--rw-r--r--   0        0        0     8208 2023-01-03 03:53:19.224934 klp-commons-0.0.8/klp_commons/datefinder/constants.py
--rw-r--r--   0        0        0      628 2023-01-03 03:53:19.225149 klp-commons-0.0.8/klp_commons/datefinder/date_fragment.py
--rw-r--r--   0        0        0     6148 2023-03-11 14:55:29.092392 klp-commons-0.0.8/klp_commons/log/.DS_Store
--rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp-commons-0.0.8/klp_commons/log/__init__.py
--rw-r--r--   0        0        0     2384 2023-02-16 19:52:02.267127 klp-commons-0.0.8/klp_commons/log/log.py
--rw-r--r--   0        0        0      350 2022-12-28 18:14:36.139801 klp-commons-0.0.8/klp_commons/log/structuredMessage.py
--rw-r--r--   0        0        0        0 2023-01-03 03:53:19.226945 klp-commons-0.0.8/klp_commons/places/__init__.py
--rw-r--r--   0        0        0      396 2023-01-03 03:53:19.263289 klp-commons-0.0.8/klp_commons/places/apis.py
--rw-r--r--   0        0        0     6148 2023-03-11 14:55:31.869752 klp-commons-0.0.8/klp_commons/scripts/.DS_Store
--rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp-commons-0.0.8/klp_commons/scripts/__init__.py
--rw-r--r--   0        0        0    14823 2023-02-21 13:40:03.843358 klp-commons-0.0.8/klp_commons/scripts/detect_recurrency.py
--rw-r--r--   0        0        0     6173 2023-02-21 13:40:03.843531 klp-commons-0.0.8/klp_commons/scripts/get_send_kw_group.py
--rw-r--r--   0        0        0    22232 2023-03-16 16:11:46.946090 klp-commons-0.0.8/klp_commons/scripts/ingest_dwh.py
--rw-r--r--   0        0        0    30962 2023-03-14 14:00:46.771225 klp-commons-0.0.8/klp_commons/scripts/summary.py
--rw-r--r--   0        0        0     6148 2023-03-11 14:55:36.942806 klp-commons-0.0.8/klp_commons/streaming/.DS_Store
--rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp-commons-0.0.8/klp_commons/streaming/__init__.py
--rw-r--r--   0        0        0     3747 2023-02-21 13:40:03.842168 klp-commons-0.0.8/klp_commons/streaming/consumer.py
--rw-r--r--   0        0        0      959 2023-03-12 06:38:51.960204 klp-commons-0.0.8/klp_commons/streaming/producer.py
--rw-r--r--   0        0        0     6148 2023-03-11 15:04:19.230154 klp-commons-0.0.8/klp_commons/utils/.DS_Store
--rw-r--r--   0        0        0        0 2023-01-03 03:53:19.227104 klp-commons-0.0.8/klp_commons/utils/__init__.py
--rw-r--r--   0        0        0      408 2023-02-16 19:52:02.303071 klp-commons-0.0.8/klp_commons/utils/utils.py
--rw-r--r--   0        0        0      470 2023-03-12 05:35:00.941176 klp-commons-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5221 1970-01-01 00:00:00.000000 klp-commons-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-03-11 16:29:59.052345 klp-commons-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4840 2023-03-11 17:02:05.306612 klp-commons-0.0.9/README.md
+-rw-r--r--   0        0        0    10244 2023-03-15 02:52:05.661685 klp-commons-0.0.9/klp_commons/.DS_Store
+-rw-r--r--   0        0        0      624 2023-03-16 18:05:31.245053 klp-commons-0.0.9/klp_commons/__init__.py
+-rw-r--r--   0        0        0     6148 2023-03-11 14:55:21.254936 klp-commons-0.0.9/klp_commons/controllers/.DS_Store
+-rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp-commons-0.0.9/klp_commons/controllers/__init__.py
+-rw-r--r--   0        0        0    31510 2023-03-13 05:25:25.017217 klp-commons-0.0.9/klp_commons/controllers/controller_dynamodb.py
+-rw-r--r--   0        0        0      260 2023-02-16 19:52:02.340344 klp-commons-0.0.9/klp_commons/controllers/controller_mlflow.py
+-rw-r--r--   0        0        0     6591 2023-03-14 16:59:36.965113 klp-commons-0.0.9/klp_commons/controllers/controller_mongodb.py
+-rw-r--r--   0        0        0    49187 2023-03-12 05:47:13.143660 klp-commons-0.0.9/klp_commons/controllers/controller_postgresdb.py
+-rw-r--r--   0        0        0    34378 2023-03-16 17:06:01.490903 klp-commons-0.0.9/klp_commons/controllers/controller_redshift.py
+-rw-r--r--   0        0        0     6148 2023-03-11 14:55:23.888578 klp-commons-0.0.9/klp_commons/cryptools/.DS_Store
+-rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp-commons-0.0.9/klp_commons/cryptools/__init__.py
+-rw-r--r--   0        0        0      795 2022-11-14 19:44:11.325419 klp-commons-0.0.9/klp_commons/cryptools/cryptology.py
+-rw-r--r--   0        0        0     6148 2023-03-11 14:55:26.531304 klp-commons-0.0.9/klp_commons/datadict/.DS_Store
+-rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp-commons-0.0.9/klp_commons/datadict/__init__.py
+-rw-r--r--   0        0        0    24123 2023-03-14 04:27:56.957869 klp-commons-0.0.9/klp_commons/datadict/struct_dicts.py
+-rw-r--r--   0        0        0    18932 2023-03-12 05:47:05.332172 klp-commons-0.0.9/klp_commons/datefinder/__init__.py
+-rw-r--r--   0        0        0     8208 2023-01-03 03:53:19.224934 klp-commons-0.0.9/klp_commons/datefinder/constants.py
+-rw-r--r--   0        0        0      628 2023-01-03 03:53:19.225149 klp-commons-0.0.9/klp_commons/datefinder/date_fragment.py
+-rw-r--r--   0        0        0     6148 2023-03-11 14:55:29.092392 klp-commons-0.0.9/klp_commons/log/.DS_Store
+-rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp-commons-0.0.9/klp_commons/log/__init__.py
+-rw-r--r--   0        0        0     2384 2023-02-16 19:52:02.267127 klp-commons-0.0.9/klp_commons/log/log.py
+-rw-r--r--   0        0        0      350 2022-12-28 18:14:36.139801 klp-commons-0.0.9/klp_commons/log/structuredMessage.py
+-rw-r--r--   0        0        0        0 2023-01-03 03:53:19.226945 klp-commons-0.0.9/klp_commons/places/__init__.py
+-rw-r--r--   0        0        0      396 2023-01-03 03:53:19.263289 klp-commons-0.0.9/klp_commons/places/apis.py
+-rw-r--r--   0        0        0     6148 2023-03-11 14:55:31.869752 klp-commons-0.0.9/klp_commons/scripts/.DS_Store
+-rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp-commons-0.0.9/klp_commons/scripts/__init__.py
+-rw-r--r--   0        0        0    14823 2023-02-21 13:40:03.843358 klp-commons-0.0.9/klp_commons/scripts/detect_recurrency.py
+-rw-r--r--   0        0        0     6173 2023-02-21 13:40:03.843531 klp-commons-0.0.9/klp_commons/scripts/get_send_kw_group.py
+-rw-r--r--   0        0        0    22232 2023-03-16 16:11:46.946090 klp-commons-0.0.9/klp_commons/scripts/ingest_dwh.py
+-rw-r--r--   0        0        0    30962 2023-03-14 14:00:46.771225 klp-commons-0.0.9/klp_commons/scripts/summary.py
+-rw-r--r--   0        0        0     6148 2023-03-11 14:55:36.942806 klp-commons-0.0.9/klp_commons/streaming/.DS_Store
+-rw-r--r--   0        0        0        0 2022-08-16 00:46:28.548105 klp-commons-0.0.9/klp_commons/streaming/__init__.py
+-rw-r--r--   0        0        0     3747 2023-02-21 13:40:03.842168 klp-commons-0.0.9/klp_commons/streaming/consumer.py
+-rw-r--r--   0        0        0      959 2023-03-12 06:38:51.960204 klp-commons-0.0.9/klp_commons/streaming/producer.py
+-rw-r--r--   0        0        0     6148 2023-03-11 15:04:19.230154 klp-commons-0.0.9/klp_commons/utils/.DS_Store
+-rw-r--r--   0        0        0        0 2023-01-03 03:53:19.227104 klp-commons-0.0.9/klp_commons/utils/__init__.py
+-rw-r--r--   0        0        0      408 2023-02-16 19:52:02.303071 klp-commons-0.0.9/klp_commons/utils/utils.py
+-rw-r--r--   0        0        0      470 2023-03-12 05:35:00.941176 klp-commons-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5221 1970-01-01 00:00:00.000000 klp-commons-0.0.9/PKG-INFO
```

### Comparing `klp-commons-0.0.8/LICENSE` & `klp-commons-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/README.md` & `klp-commons-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/.DS_Store` & `klp-commons-0.0.9/klp_commons/.DS_Store`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/__init__.py` & `klp-commons-0.0.9/klp_commons/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,10 +13,10 @@
     from importlib.metadata import PackageNotFoundError, version  # pragma: no cover
 else:
     from importlib_metadata import PackageNotFoundError, version  # pragma: no cover
 
 try:
     __version__ = version(__name__)
 except PackageNotFoundError:  # pragma: no cover
-    __version__ = "0.0.8"
+    __version__ = "0.0.9"
 
     log = logging.getLogger(__name__)
```

### Comparing `klp-commons-0.0.8/klp_commons/controllers/.DS_Store` & `klp-commons-0.0.9/klp_commons/controllers/.DS_Store`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/controllers/controller_dynamodb.py` & `klp-commons-0.0.9/klp_commons/controllers/controller_dynamodb.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/controllers/controller_mongodb.py` & `klp-commons-0.0.9/klp_commons/controllers/controller_mongodb.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/controllers/controller_postgresdb.py` & `klp-commons-0.0.9/klp_commons/controllers/controller_postgresdb.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/controllers/controller_redshift.py` & `klp-commons-0.0.9/klp_commons/controllers/controller_redshift.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
                         dict_values['month_name'],
                         dict_values['year'],
                         dict_values['week_of_month'],
                         dict_values['quarter_of_year']
                                 )
             cur.execute(redshift_insert_query, record_to_insert)
             
-    def date_decomposition(self,transaction_date):
+    def date_descomposition(self,transaction_date):
         
         transaction_date = datetime.strptime(transaction_date, self.date_format).date()
         year = transaction_date.year
         month = transaction_date.month
         month_name = transaction_date.strftime('%b')
         day = transaction_date.day
         week_of_month = self.week_of_month(transaction_date)
```

### Comparing `klp-commons-0.0.8/klp_commons/cryptools/.DS_Store` & `klp-commons-0.0.9/klp_commons/cryptools/.DS_Store`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/cryptools/cryptology.py` & `klp-commons-0.0.9/klp_commons/cryptools/cryptology.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/datadict/.DS_Store` & `klp-commons-0.0.9/klp_commons/datadict/.DS_Store`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/datadict/struct_dicts.py` & `klp-commons-0.0.9/klp_commons/datadict/struct_dicts.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/datefinder/__init__.py` & `klp-commons-0.0.9/klp_commons/datefinder/__init__.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/datefinder/constants.py` & `klp-commons-0.0.9/klp_commons/datefinder/constants.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/datefinder/date_fragment.py` & `klp-commons-0.0.9/klp_commons/datefinder/date_fragment.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/log/.DS_Store` & `klp-commons-0.0.9/klp_commons/log/.DS_Store`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/log/log.py` & `klp-commons-0.0.9/klp_commons/log/log.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/scripts/.DS_Store` & `klp-commons-0.0.9/klp_commons/scripts/.DS_Store`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/scripts/detect_recurrency.py` & `klp-commons-0.0.9/klp_commons/scripts/detect_recurrency.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/scripts/get_send_kw_group.py` & `klp-commons-0.0.9/klp_commons/scripts/get_send_kw_group.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/scripts/ingest_dwh.py` & `klp-commons-0.0.9/klp_commons/scripts/ingest_dwh.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/scripts/summary.py` & `klp-commons-0.0.9/klp_commons/scripts/summary.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/streaming/.DS_Store` & `klp-commons-0.0.9/klp_commons/streaming/.DS_Store`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/streaming/consumer.py` & `klp-commons-0.0.9/klp_commons/streaming/consumer.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/streaming/producer.py` & `klp-commons-0.0.9/klp_commons/streaming/producer.py`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/klp_commons/utils/.DS_Store` & `klp-commons-0.0.9/klp_commons/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `klp-commons-0.0.8/PKG-INFO` & `klp-commons-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klp-commons
-Version: 0.0.8
+Version: 0.0.9
 Summary: Modulo Commons del ecosistema Kloop. Contiene los modulos de uso común para los paquetes 
 Author-email: Omar Santa Cruz <omar.castellanos@kolpp.mx>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://gitlab.com/klopp1/backend/microservices/commons
 
 ## Commons
```

