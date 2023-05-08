# Comparing `tmp/ODtools-2.1.8.tar.gz` & `tmp/ODtools-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ODtools-2.1.8.tar", last modified: Thu Mar 17 06:32:46 2022, max compression
+gzip compressed data, was "ODtools-2.1.9.tar", last modified: Sat Apr  2 10:29:25 2022, max compression
```

## Comparing `ODtools-2.1.8.tar` & `ODtools-2.1.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 malongfei   (501) staff       (20)        0 2022-03-17 06:32:46.413672 ODtools-2.1.8/
-drwxr-xr-x   0 malongfei   (501) staff       (20)        0 2022-03-17 06:32:46.407284 ODtools-2.1.8/ODtools/
--rw-r--r--   0 malongfei   (501) staff       (20)     1112 2022-03-17 06:32:33.000000 ODtools-2.1.8/ODtools/__init__.py
--rw-r--r--   0 malongfei   (501) staff       (20)     2113 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/bloom_filter_tools.py
--rw-r--r--   0 malongfei   (501) staff       (20)     1195 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/excel_tools.py
--rw-r--r--   0 malongfei   (501) staff       (20)     8011 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/fastdfs_tools.py
-drwxr-xr-x   0 malongfei   (501) staff       (20)        0 2022-03-17 06:32:46.409915 ODtools-2.1.8/ODtools/fdfs_client/
--rw-r--r--   0 malongfei   (501) staff       (20)       88 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/fdfs_client/__init__.py
--rw-r--r--   0 malongfei   (501) staff       (20)    25670 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/fdfs_client/client.py
--rw-r--r--   0 malongfei   (501) staff       (20)     6401 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/fdfs_client/connection.py
--rw-r--r--   0 malongfei   (501) staff       (20)      328 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/fdfs_client/exceptions.py
--rw-r--r--   0 malongfei   (501) staff       (20)     8394 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/fdfs_client/fdfs_protol.py
--rw-r--r--   0 malongfei   (501) staff       (20)    13820 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/fdfs_client/fdfs_test.py
--rw-r--r--   0 malongfei   (501) staff       (20)    27972 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/fdfs_client/storage_client.py
--rw-r--r--   0 malongfei   (501) staff       (20)    22102 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/fdfs_client/tracker_client.py
--rw-r--r--   0 malongfei   (501) staff       (20)     8342 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/fdfs_client/utils.py
-drwxr-xr-x   0 malongfei   (501) staff       (20)        0 2022-03-17 06:32:46.411394 ODtools-2.1.8/ODtools/hbase_client/
--rw-r--r--   0 malongfei   (501) staff       (20)   147396 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/hbase_client/THBaseService.py
--rw-r--r--   0 malongfei   (501) staff       (20)       51 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/hbase_client/__init__.py
--rw-r--r--   0 malongfei   (501) staff       (20)      326 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/hbase_client/constants.py
--rw-r--r--   0 malongfei   (501) staff       (20)    81619 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/hbase_client/ttypes.py
--rw-r--r--   0 malongfei   (501) staff       (20)     8556 2021-03-11 10:06:00.000000 ODtools-2.1.8/ODtools/hbase_tools.py
--rw-r--r--   0 malongfei   (501) staff       (20)     2865 2021-03-08 11:12:38.000000 ODtools-2.1.8/ODtools/kafka_tools.py
--rw-r--r--   0 malongfei   (501) staff       (20)     2858 2021-08-05 08:22:22.000000 ODtools-2.1.8/ODtools/log_tools.py
--rw-r--r--   0 malongfei   (501) staff       (20)    13529 2021-07-29 03:57:20.000000 ODtools-2.1.8/ODtools/monitor_tools.py
--rw-r--r--   0 malongfei   (501) staff       (20)    17102 2022-03-17 06:32:33.000000 ODtools-2.1.8/ODtools/monitor_tools_new.py
--rw-r--r--   0 malongfei   (501) staff       (20)     1383 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/redis_tools.py
--rw-r--r--   0 malongfei   (501) staff       (20)     1581 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/request_headers.py
--rw-r--r--   0 malongfei   (501) staff       (20)    16129 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/save_data_class.py
-drwxr-xr-x   0 malongfei   (501) staff       (20)        0 2022-03-17 06:32:46.413333 ODtools-2.1.8/ODtools/scrapy_redis/
--rw-r--r--   0 malongfei   (501) staff       (20)      193 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/scrapy_redis/__init__.py
--rw-r--r--   0 malongfei   (501) staff       (20)     2482 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/scrapy_redis/connection.py
--rw-r--r--   0 malongfei   (501) staff       (20)      701 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/scrapy_redis/defaults.py
--rw-r--r--   0 malongfei   (501) staff       (20)     3993 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/scrapy_redis/dupefilter.py
--rw-r--r--   0 malongfei   (501) staff       (20)      242 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/scrapy_redis/picklecompat.py
--rw-r--r--   0 malongfei   (501) staff       (20)     2083 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/scrapy_redis/pipelines.py
--rw-r--r--   0 malongfei   (501) staff       (20)     4419 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/scrapy_redis/queue.py
--rw-r--r--   0 malongfei   (501) staff       (20)     6110 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/scrapy_redis/scheduler.py
--rw-r--r--   0 malongfei   (501) staff       (20)     7033 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/scrapy_redis/spiders.py
--rw-r--r--   0 malongfei   (501) staff       (20)      192 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/scrapy_redis/utils.py
--rw-r--r--   0 malongfei   (501) staff       (20)      594 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/singleton_tools.py
--rw-r--r--   0 malongfei   (501) staff       (20)      496 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/time_counter.py
--rw-r--r--   0 malongfei   (501) staff       (20)      767 2021-03-08 09:51:56.000000 ODtools-2.1.8/ODtools/timeit_counter.py
-drwxr-xr-x   0 malongfei   (501) staff       (20)        0 2022-03-17 06:32:46.408005 ODtools-2.1.8/ODtools.egg-info/
--rw-r--r--   0 malongfei   (501) staff       (20)      997 2022-03-17 06:32:46.000000 ODtools-2.1.8/ODtools.egg-info/PKG-INFO
--rw-r--r--   0 malongfei   (501) staff       (20)     1343 2022-03-17 06:32:46.000000 ODtools-2.1.8/ODtools.egg-info/SOURCES.txt
--rw-r--r--   0 malongfei   (501) staff       (20)        1 2022-03-17 06:32:46.000000 ODtools-2.1.8/ODtools.egg-info/dependency_links.txt
--rw-r--r--   0 malongfei   (501) staff       (20)      145 2022-03-17 06:32:46.000000 ODtools-2.1.8/ODtools.egg-info/requires.txt
--rw-r--r--   0 malongfei   (501) staff       (20)        8 2022-03-17 06:32:46.000000 ODtools-2.1.8/ODtools.egg-info/top_level.txt
--rw-r--r--   0 malongfei   (501) staff       (20)        1 2022-03-17 06:32:46.000000 ODtools-2.1.8/ODtools.egg-info/zip-safe
--rw-r--r--   0 malongfei   (501) staff       (20)      997 2022-03-17 06:32:46.413540 ODtools-2.1.8/PKG-INFO
--rw-r--r--   0 malongfei   (501) staff       (20)      132 2021-03-08 09:51:56.000000 ODtools-2.1.8/README.md
--rw-r--r--   0 malongfei   (501) staff       (20)       38 2022-03-17 06:32:46.413718 ODtools-2.1.8/setup.cfg
--rw-r--r--   0 malongfei   (501) staff       (20)     1451 2022-03-17 06:32:33.000000 ODtools-2.1.8/setup.py
+drwxr-xr-x   0 malongfei   (501) staff       (20)        0 2022-04-02 10:29:25.747722 ODtools-2.1.9/
+drwxr-xr-x   0 malongfei   (501) staff       (20)        0 2022-04-02 10:29:25.731792 ODtools-2.1.9/ODtools/
+-rw-r--r--   0 malongfei   (501) staff       (20)     1112 2022-04-02 10:29:20.000000 ODtools-2.1.9/ODtools/__init__.py
+-rw-r--r--   0 malongfei   (501) staff       (20)     2113 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/bloom_filter_tools.py
+-rw-r--r--   0 malongfei   (501) staff       (20)     1195 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/excel_tools.py
+-rw-r--r--   0 malongfei   (501) staff       (20)     8011 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/fastdfs_tools.py
+drwxr-xr-x   0 malongfei   (501) staff       (20)        0 2022-04-02 10:29:25.739307 ODtools-2.1.9/ODtools/fdfs_client/
+-rw-r--r--   0 malongfei   (501) staff       (20)       88 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/fdfs_client/__init__.py
+-rw-r--r--   0 malongfei   (501) staff       (20)    25670 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/fdfs_client/client.py
+-rw-r--r--   0 malongfei   (501) staff       (20)     6401 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/fdfs_client/connection.py
+-rw-r--r--   0 malongfei   (501) staff       (20)      328 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/fdfs_client/exceptions.py
+-rw-r--r--   0 malongfei   (501) staff       (20)     8394 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/fdfs_client/fdfs_protol.py
+-rw-r--r--   0 malongfei   (501) staff       (20)    13820 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/fdfs_client/fdfs_test.py
+-rw-r--r--   0 malongfei   (501) staff       (20)    27972 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/fdfs_client/storage_client.py
+-rw-r--r--   0 malongfei   (501) staff       (20)    22102 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/fdfs_client/tracker_client.py
+-rw-r--r--   0 malongfei   (501) staff       (20)     8342 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/fdfs_client/utils.py
+drwxr-xr-x   0 malongfei   (501) staff       (20)        0 2022-04-02 10:29:25.740751 ODtools-2.1.9/ODtools/hbase_client/
+-rw-r--r--   0 malongfei   (501) staff       (20)   147396 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/hbase_client/THBaseService.py
+-rw-r--r--   0 malongfei   (501) staff       (20)       51 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/hbase_client/__init__.py
+-rw-r--r--   0 malongfei   (501) staff       (20)      326 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/hbase_client/constants.py
+-rw-r--r--   0 malongfei   (501) staff       (20)    81619 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/hbase_client/ttypes.py
+-rw-r--r--   0 malongfei   (501) staff       (20)     8556 2021-03-11 10:06:00.000000 ODtools-2.1.9/ODtools/hbase_tools.py
+-rw-r--r--   0 malongfei   (501) staff       (20)     2865 2021-03-08 11:12:38.000000 ODtools-2.1.9/ODtools/kafka_tools.py
+-rw-r--r--   0 malongfei   (501) staff       (20)     2858 2021-08-05 08:22:22.000000 ODtools-2.1.9/ODtools/log_tools.py
+-rw-r--r--   0 malongfei   (501) staff       (20)    13529 2021-07-29 03:57:20.000000 ODtools-2.1.9/ODtools/monitor_tools.py
+-rw-r--r--   0 malongfei   (501) staff       (20)    17515 2022-04-02 07:56:51.000000 ODtools-2.1.9/ODtools/monitor_tools_new.py
+-rw-r--r--   0 malongfei   (501) staff       (20)     1383 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/redis_tools.py
+-rw-r--r--   0 malongfei   (501) staff       (20)     1581 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/request_headers.py
+-rw-r--r--   0 malongfei   (501) staff       (20)    16129 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/save_data_class.py
+drwxr-xr-x   0 malongfei   (501) staff       (20)        0 2022-04-02 10:29:25.744681 ODtools-2.1.9/ODtools/scrapy_redis/
+-rw-r--r--   0 malongfei   (501) staff       (20)      193 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/scrapy_redis/__init__.py
+-rw-r--r--   0 malongfei   (501) staff       (20)     2482 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/scrapy_redis/connection.py
+-rw-r--r--   0 malongfei   (501) staff       (20)      701 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/scrapy_redis/defaults.py
+-rw-r--r--   0 malongfei   (501) staff       (20)     3993 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/scrapy_redis/dupefilter.py
+-rw-r--r--   0 malongfei   (501) staff       (20)      242 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/scrapy_redis/picklecompat.py
+-rw-r--r--   0 malongfei   (501) staff       (20)     2083 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/scrapy_redis/pipelines.py
+-rw-r--r--   0 malongfei   (501) staff       (20)     4419 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/scrapy_redis/queue.py
+-rw-r--r--   0 malongfei   (501) staff       (20)     6110 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/scrapy_redis/scheduler.py
+-rw-r--r--   0 malongfei   (501) staff       (20)     7033 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/scrapy_redis/spiders.py
+-rw-r--r--   0 malongfei   (501) staff       (20)      192 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/scrapy_redis/utils.py
+-rw-r--r--   0 malongfei   (501) staff       (20)      594 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/singleton_tools.py
+-rw-r--r--   0 malongfei   (501) staff       (20)      496 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/time_counter.py
+-rw-r--r--   0 malongfei   (501) staff       (20)      767 2021-03-08 09:51:56.000000 ODtools-2.1.9/ODtools/timeit_counter.py
+drwxr-xr-x   0 malongfei   (501) staff       (20)        0 2022-04-02 10:29:25.733342 ODtools-2.1.9/ODtools.egg-info/
+-rw-r--r--   0 malongfei   (501) staff       (20)      986 2022-04-02 10:29:25.000000 ODtools-2.1.9/ODtools.egg-info/PKG-INFO
+-rw-r--r--   0 malongfei   (501) staff       (20)     1343 2022-04-02 10:29:25.000000 ODtools-2.1.9/ODtools.egg-info/SOURCES.txt
+-rw-r--r--   0 malongfei   (501) staff       (20)        1 2022-04-02 10:29:25.000000 ODtools-2.1.9/ODtools.egg-info/dependency_links.txt
+-rw-r--r--   0 malongfei   (501) staff       (20)      157 2022-04-02 10:29:25.000000 ODtools-2.1.9/ODtools.egg-info/requires.txt
+-rw-r--r--   0 malongfei   (501) staff       (20)        8 2022-04-02 10:29:25.000000 ODtools-2.1.9/ODtools.egg-info/top_level.txt
+-rw-r--r--   0 malongfei   (501) staff       (20)        1 2022-03-17 06:32:46.000000 ODtools-2.1.9/ODtools.egg-info/zip-safe
+-rw-r--r--   0 malongfei   (501) staff       (20)      986 2022-04-02 10:29:25.747362 ODtools-2.1.9/PKG-INFO
+-rw-r--r--   0 malongfei   (501) staff       (20)      132 2021-03-08 09:51:56.000000 ODtools-2.1.9/README.md
+-rw-r--r--   0 malongfei   (501) staff       (20)       38 2022-04-02 10:29:25.747790 ODtools-2.1.9/setup.cfg
+-rw-r--r--   0 malongfei   (501) staff       (20)     1474 2022-04-02 10:29:20.000000 ODtools-2.1.9/setup.py
```

### Comparing `ODtools-2.1.8/ODtools/__init__.py` & `ODtools-2.1.9/ODtools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ODtools.redis_tools import RedisClient
 from ODtools.request_headers import user_agents, headers
 from ODtools.save_data_class import SaveOriginalData
 from ODtools.singleton_tools import Singleton
 from ODtools.time_counter import time_counter
 from ODtools.timeit_counter import timeit_counter
 
-__version__ = "2.1.8"
+__version__ = "2.1.9"
 VERSION = tuple(map(int, __version__.split('.')))
 
 __all__ = [
     "fastdfs_tools", "hbase_tools", "redis_tools",
     "SimpleHash", "BloomFilter", "read_excel", "write_excel",
     "HBaseClient", "KafkaProducerClient", "KafkaConsumerClient",
     "FastDfsClient", "base_logger", "RedisClient", "user_agents",
```

### Comparing `ODtools-2.1.8/ODtools/bloom_filter_tools.py` & `ODtools-2.1.9/ODtools/bloom_filter_tools.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/excel_tools.py` & `ODtools-2.1.9/ODtools/excel_tools.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/fastdfs_tools.py` & `ODtools-2.1.9/ODtools/fastdfs_tools.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/fdfs_client/client.py` & `ODtools-2.1.9/ODtools/fdfs_client/client.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/fdfs_client/connection.py` & `ODtools-2.1.9/ODtools/fdfs_client/connection.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/fdfs_client/fdfs_protol.py` & `ODtools-2.1.9/ODtools/fdfs_client/fdfs_protol.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/fdfs_client/fdfs_test.py` & `ODtools-2.1.9/ODtools/fdfs_client/fdfs_test.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/fdfs_client/storage_client.py` & `ODtools-2.1.9/ODtools/fdfs_client/storage_client.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/fdfs_client/tracker_client.py` & `ODtools-2.1.9/ODtools/fdfs_client/tracker_client.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/fdfs_client/utils.py` & `ODtools-2.1.9/ODtools/fdfs_client/utils.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/hbase_client/THBaseService.py` & `ODtools-2.1.9/ODtools/hbase_client/THBaseService.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/hbase_client/ttypes.py` & `ODtools-2.1.9/ODtools/hbase_client/ttypes.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/hbase_tools.py` & `ODtools-2.1.9/ODtools/hbase_tools.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/kafka_tools.py` & `ODtools-2.1.9/ODtools/kafka_tools.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/log_tools.py` & `ODtools-2.1.9/ODtools/log_tools.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/monitor_tools.py` & `ODtools-2.1.9/ODtools/monitor_tools.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/monitor_tools_new.py` & `ODtools-2.1.9/ODtools/monitor_tools_new.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,25 +104,27 @@
 
 class Source(Enum):
     """项目数据源"""
     WEIBO = 'Weibo'
     WECHAT = 'Wechat'
     DOUYIN = 'Douyin'
     NEWS = 'News'
+    SD = 'SD'
     TIEBA = 'Tieba'
     APP = 'App'
     HOTLIST = 'HotList'
     TOUTIAO = 'Toutiao'
     BAIDU_BAIJIAHAO = 'baidu_baijihao'
     OTHER = 'OtherSource'
 
 
 class Response(Enum):
     """错误的数据链接请求"""
     status_code = 500
+    status = 500
     headers = {}
 
 
 class Task(object):
     """
     任务调度分发类,主要分为定时分发任务、循环分发任务、单次分发任务
     """
@@ -286,37 +288,42 @@
                 try:
                     async with session.get(url, **kwargs) as response:
                         if response.status == 200:
                             if self.statistic: record_dict['record_info'] = '{}_request_success'.format(component_name)
                         else:
                             if self.statistic: record_dict['record_info'] = '{}_request_fail'.format(component_name)
                         if self.statistic: spider_record(self.db_client, record_dict, step, False)
+                        if self.statistic: record_dict['record_info'] = '{}_request_content_length'.format(
+                            component_name)
+                        content_length = eval(response.headers.get("Content-Length", "0"))
+                        res_content = await response.read()
+                        if self.statistic: spider_record(self.db_client, record_dict,
+                                                         content_length if content_length else len(res_content),
+                                                         False)
                         if response_model == 'json':
                             return await response.json(), str(response.url), response
                         elif response_model == 'bytes':
                             return await response.read(), str(response.url), response
                         elif response_model == 'html':
                             return await response.text(), str(response.url), response
                         else:
                             return await response, str(response.url), response
                 except Exception as e:
                     if self.statistic:
                         record_dict['record_info'] = '{}_request_fail'.format(component_name)
                         spider_record(self.db_client, record_dict, step, False)
                     import traceback
                     print(traceback.format_exc(), url)
-                    return '', url, Response
-                finally:
-                    """增加返回值，结果结果统计，按照bytes为单位统计"""
                     if self.statistic: record_dict['record_info'] = '{}_request_content_length'.format(component_name)
-                    content_length = eval(response.headers.get("Content-Length", "0"))
-                    res_content = await response.read()
+                    content_length = 0
+                    res_content = ""
                     if self.statistic: spider_record(self.db_client, record_dict,
                                                      content_length if content_length else len(res_content),
                                                      False)
+                    return '', url, Response
 
         tasks = [asyncio.ensure_future(async_request(i, cookies=cookies, **kwargs)) for i in urls]
         loop = asyncio.get_event_loop()
         loop.run_until_complete(asyncio.wait(tasks))
         del loop
         return [i.result() for i in tasks]
```

### Comparing `ODtools-2.1.8/ODtools/redis_tools.py` & `ODtools-2.1.9/ODtools/redis_tools.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/request_headers.py` & `ODtools-2.1.9/ODtools/request_headers.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/save_data_class.py` & `ODtools-2.1.9/ODtools/save_data_class.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/scrapy_redis/connection.py` & `ODtools-2.1.9/ODtools/scrapy_redis/connection.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/scrapy_redis/defaults.py` & `ODtools-2.1.9/ODtools/scrapy_redis/defaults.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/scrapy_redis/dupefilter.py` & `ODtools-2.1.9/ODtools/scrapy_redis/dupefilter.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/scrapy_redis/pipelines.py` & `ODtools-2.1.9/ODtools/scrapy_redis/pipelines.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/scrapy_redis/queue.py` & `ODtools-2.1.9/ODtools/scrapy_redis/queue.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/scrapy_redis/scheduler.py` & `ODtools-2.1.9/ODtools/scrapy_redis/scheduler.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/scrapy_redis/spiders.py` & `ODtools-2.1.9/ODtools/scrapy_redis/spiders.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/singleton_tools.py` & `ODtools-2.1.9/ODtools/singleton_tools.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools/timeit_counter.py` & `ODtools-2.1.9/ODtools/timeit_counter.py`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/ODtools.egg-info/PKG-INFO` & `ODtools-2.1.9/ODtools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: ODtools
-Version: 2.1.8
+Version: 2.1.9
 Summary: zkrTools
 Home-page: https://github.com/zkr-origin-data-dpt/ODtools
 Author: zkrPython
 Author-email: 178031608@qq.com
 License: Apache License
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: Indexing
 Classifier: Topic :: Utilities
 Classifier: Topic :: Internet
@@ -20,7 +19,10 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+
+UNKNOWN
+
```

### Comparing `ODtools-2.1.8/ODtools.egg-info/SOURCES.txt` & `ODtools-2.1.9/ODtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ODtools-2.1.8/PKG-INFO` & `ODtools-2.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: ODtools
-Version: 2.1.8
+Version: 2.1.9
 Summary: zkrTools
 Home-page: https://github.com/zkr-origin-data-dpt/ODtools
 Author: zkrPython
 Author-email: 178031608@qq.com
 License: Apache License
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: Indexing
 Classifier: Topic :: Utilities
 Classifier: Topic :: Internet
@@ -20,7 +19,10 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+
+UNKNOWN
+
```

### Comparing `ODtools-2.1.8/setup.py` & `ODtools-2.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ODtools",
-    version="2.1.8",
+    version="2.1.9",
     author="zkrPython",
     author_email="178031608@qq.com",
     description="zkrTools",
     long_description="",
     license="Apache License",
     url="https://github.com/zkr-origin-data-dpt/ODtools",
     packages=find_packages(),
@@ -21,14 +21,15 @@
         "kafka-python",
         "redis-py-cluster==1.3.6",
         "pymysql",
         "loguru",
         "colorlog",
         "aiohttp==3.1.3",
         "aiosocksy==0.1.2",
+        "apscheduler",
     ],
     classifiers=[
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Topic :: Text Processing :: Indexing",
         "Topic :: Utilities",
```

