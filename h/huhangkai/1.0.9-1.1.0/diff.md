# Comparing `tmp/huhangkai-1.0.9.tar.gz` & `tmp/huhangkai-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhangkai-1.0.9.tar", last modified: Sun Apr 23 09:22:57 2023, max compression
+gzip compressed data, was "huhangkai-1.1.0.tar", last modified: Mon May  8 06:01:24 2023, max compression
```

## Comparing `huhangkai-1.0.9.tar` & `huhangkai-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 09:22:57.717679 huhangkai-1.0.9/
--rw-rw-rw-   0        0        0      228 2023-04-23 09:22:57.716681 huhangkai-1.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-23 09:22:57.701691 huhangkai-1.0.9/commen/
--rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.0.9/commen/__init__.py
--rw-rw-rw-   0        0        0    32340 2023-02-22 03:30:12.000000 huhangkai-1.0.9/commen/init_project.py
--rw-rw-rw-   0        0        0     4508 2022-11-09 07:51:47.000000 huhangkai-1.0.9/commen/unit_dict.py
--rw-rw-rw-   0        0        0    20151 2023-04-23 09:21:46.000000 huhangkai-1.0.9/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2022-11-09 07:51:47.000000 huhangkai-1.0.9/commen/unit_logger.py
--rw-rw-rw-   0        0        0     6122 2023-02-15 10:10:32.000000 huhangkai-1.0.9/commen/unit_request.py
-drwxrwxrwx   0        0        0        0 2023-04-23 09:22:57.714684 huhangkai-1.0.9/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      228 2023-04-23 09:22:57.000000 huhangkai-1.0.9/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-04-23 09:22:57.000000 huhangkai-1.0.9/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 09:22:57.000000 huhangkai-1.0.9/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-23 09:22:57.000000 huhangkai-1.0.9/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-23 09:22:57.000000 huhangkai-1.0.9/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 09:22:57.717679 huhangkai-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      495 2023-04-23 09:22:51.000000 huhangkai-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 06:01:24.218857 huhangkai-1.1.0/
+-rw-rw-rw-   0        0        0      228 2023-05-08 06:01:24.217859 huhangkai-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-08 06:01:24.203899 huhangkai-1.1.0/commen/
+-rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.1.0/commen/__init__.py
+-rw-rw-rw-   0        0        0    32340 2023-04-23 09:30:51.000000 huhangkai-1.1.0/commen/init_project.py
+-rw-rw-rw-   0        0        0     4508 2023-04-23 09:30:51.000000 huhangkai-1.1.0/commen/unit_dict.py
+-rw-rw-rw-   0        0        0    20377 2023-05-08 03:19:39.000000 huhangkai-1.1.0/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-04-23 09:30:51.000000 huhangkai-1.1.0/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     6122 2023-04-23 09:30:51.000000 huhangkai-1.1.0/commen/unit_request.py
+drwxrwxrwx   0        0        0        0 2023-05-08 06:01:24.215866 huhangkai-1.1.0/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-05-08 06:01:24.000000 huhangkai-1.1.0/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-05-08 06:01:24.000000 huhangkai-1.1.0/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 06:01:24.000000 huhangkai-1.1.0/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-08 06:01:24.000000 huhangkai-1.1.0/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-08 06:01:24.000000 huhangkai-1.1.0/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 06:01:24.218857 huhangkai-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      495 2023-05-08 06:01:11.000000 huhangkai-1.1.0/setup.py
```

### Comparing `huhangkai-1.0.9/commen/__init__.py` & `huhangkai-1.1.0/commen/__init__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.0.9/commen/init_project.py` & `huhangkai-1.1.0/commen/init_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.0.9/commen/unit_dict.py` & `huhangkai-1.1.0/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.0.9/commen/unit_fun.py` & `huhangkai-1.1.0/commen/unit_fun.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 import random
 import time
 import requests
+import datetime
 # import pymysql
 
 from typing import List
 from faker import Faker
 from commen.unit_logger import logger
 
 
@@ -114,14 +115,16 @@
     def time_hms(self, string=None, fmt="%Y-%m-%d %H:%M:%S"):
         return self.time(string=string, fmt=fmt) * 1000
 
     def time_ms(self, string=None, fmt="%Y-%m-%d"):
         time_array = self.time(string=string, fmt=fmt)
         return time_array * 1000
 
+    def data_str(self):
+        return datetime.datetime.now().strftime("%Y-%m-%d")
     # # 根据sql语句执行sql
     # def run_mysql(self, sql_str="", host="", user="", password="", database=""):
     #     sql_str = sql_str or self.sql_str
     #     if self._db.get(host+database):
     #         cursor = self._db.get(host+database)
     #     else:
     #         try:
@@ -454,14 +457,16 @@
             # 写入到第一个sheet
             if data and isinstance(data[0], list):
                 h = data[0]
                 data1 = []
                 for i in data[1:]:
                     data1.append({x[0]: str(x[1]) for x in zip(h, i)})
                 data = data1
+            elif data and isinstance(data[0], dict):
+                data = [{k: str(v) for k, v in i.items()} for i in data]
             DataFrame(data).to_excel(writer,
                               sheet_name="sheet1",
                               index=False,
                               engine="openpyxl"
                               )
```

### Comparing `huhangkai-1.0.9/commen/unit_logger.py` & `huhangkai-1.1.0/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.0.9/commen/unit_request.py` & `huhangkai-1.1.0/commen/unit_request.py`

 * *Files identical despite different names*

