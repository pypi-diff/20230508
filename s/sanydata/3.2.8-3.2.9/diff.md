# Comparing `tmp/sanydata-3.2.8.tar.gz` & `tmp/sanydata-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanydata-3.2.8.tar", last modified: Tue Feb 28 03:41:46 2023, max compression
+gzip compressed data, was "sanydata-3.2.9.tar", last modified: Mon May  8 11:33:13 2023, max compression
```

## Comparing `sanydata-3.2.8.tar` & `sanydata-3.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-02-28 03:41:46.014167 sanydata-3.2.8/
--rw-r--r--   0 thao       (501) staff       (20)      302 2023-02-28 03:41:46.013876 sanydata-3.2.8/PKG-INFO
-drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-02-28 03:41:46.009398 sanydata-3.2.8/sanydata/
--rw-r--r--   0 thao       (501) staff       (20)      103 2022-04-09 07:48:22.000000 sanydata-3.2.8/sanydata/__init__.py
--rw-r--r--   0 thao       (501) staff       (20)   114403 2023-02-28 02:55:21.000000 sanydata-3.2.8/sanydata/datatools.py
--rw-r--r--   0 thao       (501) staff       (20)    20291 2022-08-29 10:08:03.000000 sanydata-3.2.8/sanydata/model_data_message_pb2.py
--rw-r--r--   0 thao       (501) staff       (20)    20370 2022-08-29 10:08:03.000000 sanydata-3.2.8/sanydata/model_data_message_pb2_grpc.py
-drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-02-28 03:41:46.011013 sanydata-3.2.8/sanydata.egg-info/
--rw-r--r--   0 thao       (501) staff       (20)      302 2023-02-28 03:41:45.000000 sanydata-3.2.8/sanydata.egg-info/PKG-INFO
--rw-r--r--   0 thao       (501) staff       (20)      371 2023-02-28 03:41:45.000000 sanydata-3.2.8/sanydata.egg-info/SOURCES.txt
--rw-r--r--   0 thao       (501) staff       (20)        1 2023-02-28 03:41:45.000000 sanydata-3.2.8/sanydata.egg-info/dependency_links.txt
--rw-r--r--   0 thao       (501) staff       (20)      130 2023-02-28 03:41:45.000000 sanydata-3.2.8/sanydata.egg-info/requires.txt
--rw-r--r--   0 thao       (501) staff       (20)       15 2023-02-28 03:41:45.000000 sanydata-3.2.8/sanydata.egg-info/top_level.txt
--rw-r--r--   0 thao       (501) staff       (20)       38 2023-02-28 03:41:46.014284 sanydata-3.2.8/setup.cfg
--rw-r--r--   0 thao       (501) staff       (20)      999 2023-02-28 02:55:30.000000 sanydata-3.2.8/setup.py
-drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-02-28 03:41:46.013276 sanydata-3.2.8/utils/
--rw-r--r--   0 thao       (501) staff       (20)      103 2022-04-09 07:48:22.000000 sanydata-3.2.8/utils/__init__.py
--rw-r--r--   0 thao       (501) staff       (20)     1328 2022-04-14 01:33:04.000000 sanydata-3.2.8/utils/cos_handler.py
--rw-r--r--   0 thao       (501) staff       (20)     1080 2022-04-13 10:48:13.000000 sanydata-3.2.8/utils/file_operation.py
--rw-r--r--   0 thao       (501) staff       (20)      667 2022-04-14 01:24:56.000000 sanydata-3.2.8/utils/local_handler.py
+drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-05-08 11:33:13.902794 sanydata-3.2.9/
+-rw-r--r--   0 thao       (501) staff       (20)      302 2023-05-08 11:33:13.902558 sanydata-3.2.9/PKG-INFO
+drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-05-08 11:33:13.898800 sanydata-3.2.9/sanydata/
+-rw-r--r--   0 thao       (501) staff       (20)      103 2022-04-09 07:48:22.000000 sanydata-3.2.9/sanydata/__init__.py
+-rw-r--r--   0 thao       (501) staff       (20)   114403 2023-05-08 11:32:13.000000 sanydata-3.2.9/sanydata/datatools.py
+-rw-r--r--   0 thao       (501) staff       (20)    20291 2022-08-29 10:08:03.000000 sanydata-3.2.9/sanydata/model_data_message_pb2.py
+-rw-r--r--   0 thao       (501) staff       (20)    20370 2022-08-29 10:08:03.000000 sanydata-3.2.9/sanydata/model_data_message_pb2_grpc.py
+drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-05-08 11:33:13.900299 sanydata-3.2.9/sanydata.egg-info/
+-rw-r--r--   0 thao       (501) staff       (20)      302 2023-05-08 11:33:13.000000 sanydata-3.2.9/sanydata.egg-info/PKG-INFO
+-rw-r--r--   0 thao       (501) staff       (20)      371 2023-05-08 11:33:13.000000 sanydata-3.2.9/sanydata.egg-info/SOURCES.txt
+-rw-r--r--   0 thao       (501) staff       (20)        1 2023-05-08 11:33:13.000000 sanydata-3.2.9/sanydata.egg-info/dependency_links.txt
+-rw-r--r--   0 thao       (501) staff       (20)      130 2023-05-08 11:33:13.000000 sanydata-3.2.9/sanydata.egg-info/requires.txt
+-rw-r--r--   0 thao       (501) staff       (20)       15 2023-05-08 11:33:13.000000 sanydata-3.2.9/sanydata.egg-info/top_level.txt
+-rw-r--r--   0 thao       (501) staff       (20)       38 2023-05-08 11:33:13.902897 sanydata-3.2.9/setup.cfg
+-rw-r--r--   0 thao       (501) staff       (20)      999 2023-05-08 11:31:50.000000 sanydata-3.2.9/setup.py
+drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-05-08 11:33:13.901966 sanydata-3.2.9/utils/
+-rw-r--r--   0 thao       (501) staff       (20)      103 2022-04-09 07:48:22.000000 sanydata-3.2.9/utils/__init__.py
+-rw-r--r--   0 thao       (501) staff       (20)     1328 2022-04-14 01:33:04.000000 sanydata-3.2.9/utils/cos_handler.py
+-rw-r--r--   0 thao       (501) staff       (20)     1080 2022-04-13 10:48:13.000000 sanydata-3.2.9/utils/file_operation.py
+-rw-r--r--   0 thao       (501) staff       (20)      667 2022-04-14 01:24:56.000000 sanydata-3.2.9/utils/local_handler.py
```

### Comparing `sanydata-3.2.8/sanydata/datatools.py` & `sanydata-3.2.9/sanydata/datatools.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
 
     return wrapper
 
 
 class DataTools(object):
     # This programme is to get data.
     PROGRAMME = 'DataTools'
-    VERSION = '3.2.8'
+    VERSION = '3.2.9'
 
     def __init__(self, stub=None, es_hosts='http://es.sanywind.net:9200/'):
         self.es = Elasticsearch(hosts=es_hosts)
 
         if stub:
             with grpc.insecure_channel(stub, options=options) as channel:
                 stub = model_data_message_pb2_grpc.ModelDataMessageStub(channel)
@@ -640,17 +640,17 @@
                         df = self.map_data(df, check_result, map_fc, map_v)
                         df_all.append(df)
                     else:
                         turbine_num = file_name.split('_')[1]
                         if 'cmsadaptor' in file_list[0].split('/'):
                             header = None
                             names = ['振动幅值']
-                        df = self.pd_read_csv(file_data, columns, header, names, map_fc, map_v, check_result, turbine_num)
                         if use_filename:
                             df['sanydata_file_name'] = file_name
+                        df = self.pd_read_csv(file_data, columns, header, names, map_fc, map_v, check_result, turbine_num)
                         df_all.append(df)
                 except Exception as e:
                     print(file_name)
                     print(e)
         if len(df_all) > 0:
             df_all = pd.concat(df_all)
             df_all = df_all.reset_index(drop=True)
```

### Comparing `sanydata-3.2.8/sanydata/model_data_message_pb2.py` & `sanydata-3.2.9/sanydata/model_data_message_pb2.py`

 * *Files identical despite different names*

### Comparing `sanydata-3.2.8/sanydata/model_data_message_pb2_grpc.py` & `sanydata-3.2.9/sanydata/model_data_message_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sanydata-3.2.8/setup.py` & `sanydata-3.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import sys
 import importlib
 
 importlib.reload(sys)
 
 setup(
     name="sanydata",
-    version="3.2.8",
+    version="3.2.9",
     keywords=["pip", "sanydata", "thao"],
     description="get data and get wind farm information",
     long_description="get data and get wind farm information",
     license="MIT Licence",
 
     url="http://gitlab.sanywind.net/sanydata/sanydata",
     author="thao",
```

### Comparing `sanydata-3.2.8/utils/cos_handler.py` & `sanydata-3.2.9/utils/cos_handler.py`

 * *Files identical despite different names*

### Comparing `sanydata-3.2.8/utils/file_operation.py` & `sanydata-3.2.9/utils/file_operation.py`

 * *Files identical despite different names*

### Comparing `sanydata-3.2.8/utils/local_handler.py` & `sanydata-3.2.9/utils/local_handler.py`

 * *Files identical despite different names*

