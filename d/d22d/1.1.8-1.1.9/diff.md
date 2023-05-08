# Comparing `tmp/d22d-1.1.8.tar.gz` & `tmp/d22d-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/d22d-1.1.8.tar", last modified: Mon Dec 14 08:50:17 2020, max compression
+gzip compressed data, was "d22d-1.1.9.tar", last modified: Fri Oct 15 12:29:26 2021, max compression
```

## Comparing `d22d-1.1.8.tar` & `d22d-1.1.9.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-14 08:50:17.282412 d22d-1.1.8/
--rw-r--r--   0 user      (1000) user      (1000)    34378 2020-11-25 02:42:55.000000 d22d-1.1.8/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)      136 2020-11-25 06:15:17.000000 d22d-1.1.8/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)    10239 2020-12-14 08:50:17.282412 d22d-1.1.8/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     7844 2020-12-11 07:00:18.000000 d22d-1.1.8/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-14 08:50:17.282412 d22d-1.1.8/d22d/
--rw-r--r--   0 user      (1000) user      (1000)      236 2020-12-10 02:40:47.000000 d22d-1.1.8/d22d/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    13790 2020-12-10 03:24:03.000000 d22d-1.1.8/d22d/task.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-14 08:50:17.282412 d22d-1.1.8/d22d/utils/
--rw-r--r--   0 user      (1000) user      (1000)      298 2020-11-25 05:19:55.000000 d22d-1.1.8/d22d/utils/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-14 08:50:17.282412 d22d-1.1.8/d22d/utils/db/
--rw-r--r--   0 user      (1000) user      (1000)    28657 2020-12-14 08:35:02.000000 d22d-1.1.8/d22d/utils/db/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    39048 2020-12-09 01:58:20.000000 d22d-1.1.8/d22d/utils/db/myutils.py
--rw-r--r--   0 user      (1000) user      (1000)    36239 2020-12-14 08:39:15.000000 d22d-1.1.8/d22d/utils/db/sqlfileextra.py
--rw-r--r--   0 user      (1000) user      (1000)      491 2020-11-25 05:15:40.000000 d22d-1.1.8/d22d/utils/exceptions.py
--rw-r--r--   0 user      (1000) user      (1000)    11457 2020-11-25 06:03:33.000000 d22d-1.1.8/d22d/utils/logger.py
--rw-r--r--   0 user      (1000) user      (1000)     1700 2020-11-25 03:58:53.000000 d22d-1.1.8/d22d/utils/req_conflit.py
--rw-r--r--   0 user      (1000) user      (1000)    11340 2020-11-25 06:03:33.000000 d22d-1.1.8/d22d/utils/utils.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-12-14 08:50:17.282412 d22d-1.1.8/d22d.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)    10239 2020-12-14 08:50:17.000000 d22d-1.1.8/d22d.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      420 2020-12-14 08:50:17.000000 d22d-1.1.8/d22d.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2020-12-14 08:50:17.000000 d22d-1.1.8/d22d.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)      891 2020-12-14 08:50:17.000000 d22d-1.1.8/d22d.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        5 2020-12-14 08:50:17.000000 d22d-1.1.8/d22d.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)     1341 2020-12-09 04:29:48.000000 d22d-1.1.8/requirements.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2020-12-14 08:50:17.282412 d22d-1.1.8/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     2466 2020-12-09 02:12:00.000000 d22d-1.1.8/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-10-15 12:29:26.514384 d22d-1.1.9/
+-rwxr-xr-x   0 user      (1000) user      (1000)    34378 2020-11-25 02:42:55.000000 d22d-1.1.9/LICENSE
+-rwxr-xr-x   0 user      (1000) user      (1000)      136 2020-11-25 06:15:17.000000 d22d-1.1.9/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)    10272 2021-10-15 12:29:26.510383 d22d-1.1.9/PKG-INFO
+-rwxr-xr-x   0 user      (1000) user      (1000)     7869 2021-10-15 12:29:09.000000 d22d-1.1.9/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-10-15 12:29:26.510383 d22d-1.1.9/d22d/
+-rwxr-xr-x   0 user      (1000) user      (1000)      268 2021-10-15 12:29:09.000000 d22d-1.1.9/d22d/__init__.py
+-rwxr-xr-x   0 user      (1000) user      (1000)    13952 2021-10-15 12:29:09.000000 d22d-1.1.9/d22d/task.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-10-15 12:29:26.510383 d22d-1.1.9/d22d/utils/
+-rwxr-xr-x   0 user      (1000) user      (1000)      317 2021-10-15 11:36:06.000000 d22d-1.1.9/d22d/utils/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-10-15 12:29:26.510383 d22d-1.1.9/d22d/utils/db/
+-rwxr-xr-x   0 user      (1000) user      (1000)    50911 2021-10-15 12:29:09.000000 d22d-1.1.9/d22d/utils/db/__init__.py
+-rwxr-xr-x   0 user      (1000) user      (1000)    39044 2021-10-15 11:32:21.000000 d22d-1.1.9/d22d/utils/db/myutils.py
+-rwxr-xr-x   0 user      (1000) user      (1000)    36239 2020-12-14 08:39:15.000000 d22d-1.1.9/d22d/utils/db/sqlfileextra.py
+-rw-r--r--   0 user      (1000) user      (1000)    25119 2021-07-28 07:39:48.000000 d22d-1.1.9/d22d/utils/decorators.py
+-rw-r--r--   0 user      (1000) user      (1000)     4934 2021-10-15 11:48:11.000000 d22d-1.1.9/d22d/utils/diskcacheofsqlite.py
+-rwxr-xr-x   0 user      (1000) user      (1000)      491 2020-11-25 05:15:40.000000 d22d-1.1.9/d22d/utils/exceptions.py
+-rwxr-xr-x   0 user      (1000) user      (1000)    11457 2020-11-25 06:03:33.000000 d22d-1.1.9/d22d/utils/logger.py
+-rw-r--r--   0 user      (1000) user      (1000)    14439 2021-10-15 11:40:40.000000 d22d-1.1.9/d22d/utils/logutils.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     1700 2020-11-25 03:58:53.000000 d22d-1.1.9/d22d/utils/req_conflit.py
+-rwxr-xr-x   0 user      (1000) user      (1000)    13464 2021-10-15 12:02:20.000000 d22d-1.1.9/d22d/utils/utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-10-15 12:29:26.510383 d22d-1.1.9/d22d.egg-info/
+-rwxr-xr-x   0 user      (1000) user      (1000)    10272 2021-10-15 12:29:25.000000 d22d-1.1.9/d22d.egg-info/PKG-INFO
+-rwxr-xr-x   0 user      (1000) user      (1000)      500 2021-10-15 12:29:26.000000 d22d-1.1.9/d22d.egg-info/SOURCES.txt
+-rwxr-xr-x   0 user      (1000) user      (1000)        1 2021-10-15 12:29:25.000000 d22d-1.1.9/d22d.egg-info/dependency_links.txt
+-rwxr-xr-x   0 user      (1000) user      (1000)      921 2021-10-15 12:29:25.000000 d22d-1.1.9/d22d.egg-info/requires.txt
+-rwxr-xr-x   0 user      (1000) user      (1000)        5 2021-10-15 12:29:25.000000 d22d-1.1.9/d22d.egg-info/top_level.txt
+-rwxr-xr-x   0 user      (1000) user      (1000)     1362 2021-10-15 12:04:31.000000 d22d-1.1.9/requirements.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2021-10-15 12:29:26.514384 d22d-1.1.9/setup.cfg
+-rwxr-xr-x   0 user      (1000) user      (1000)     2529 2021-10-15 12:04:31.000000 d22d-1.1.9/setup.py
```

### Comparing `d22d-1.1.8/LICENSE` & `d22d-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `d22d-1.1.8/PKG-INFO` & `d22d-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d22d
-Version: 1.1.8
+Version: 1.1.9
 Summary: Migrating form DateBase to DateBase by 2 lines code
 Home-page: https://github.com/DJMIN/D2D
 Author: readerror
 Author-email: readerror@sina.com
 Maintainer: readerror
 Maintainer-email: readerror@sina.com
 License: GPL License
@@ -91,18 +91,19 @@
         1. need python3
         1. create your .py file 
         ```python
         import d22d
         from d22d import (
         ElasticSearchD, MySqlD, CsvD, SqlFileD, JsonListD,
          XlsIbyFileD, XlsxIbyFileD, MongoDBD, 
-         Migration, Migration2DB
+         Migration, Migration2DB, open_log
         )
         
         def test1():
+            open_log()
             t = Migration(
                 database_from=MySqlD(host='localhost', port=3306, database='test',
                                         user='root', passwd='root'),
                 database_to=MySqlD(host='192.168.0.100', port=3306, database='test',
                                         user='root', passwd='root'),
                 table_from='user',
                 table_to='user'
```

### Comparing `d22d-1.1.8/README.md` & `d22d-1.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -81,18 +81,19 @@
 1. need python3
 1. create your .py file 
 ```python
 import d22d
 from d22d import (
 ElasticSearchD, MySqlD, CsvD, SqlFileD, JsonListD,
  XlsIbyFileD, XlsxIbyFileD, MongoDBD, 
- Migration, Migration2DB
+ Migration, Migration2DB, open_log
 )
 
 def test1():
+    open_log()
     t = Migration(
         database_from=MySqlD(host='localhost', port=3306, database='test',
                                 user='root', passwd='root'),
         database_to=MySqlD(host='192.168.0.100', port=3306, database='test',
                                 user='root', passwd='root'),
         table_from='user',
         table_to='user'
```

### Comparing `d22d-1.1.8/d22d/task.py` & `d22d-1.1.9/d22d/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,23 @@
 import sys
 import json
 import time
 import datetime
 import logging
 from . import utils
 
+if '-debug' in sys.argv:
+    logger = utils.logger.get_logger('d22d')
+else:
+    logger = logging.getLogger('d22d')
 
-logger = utils.logger.get_logger('d22d')
+
+def open_log():
+    global logger
+    logger = utils.logger.get_logger('d22d')
 
 
 def format_value(data):
     if isinstance(data, float) and data % 1 == 0.0:
         data = int(data)
     elif isinstance(data, str):
         data = data.strip()
@@ -90,17 +97,17 @@
                 #     table_to = {'index':table_from_raw}
 
                 self.run_one(table_from_raw, table_from_raw, self.pkd.get(table_from_raw, 'id'))
         del self.database_from
         del self.database_to
 
     def run_one(self, table_from, table_to, pks):
-        count = self.count_from or self.database_from.get_count(table_from)
         gkws = {}
         gkws.update(self.get_data_kwargs)
+        count = self.count_from or self.database_from.get_count(table_from, **gkws)
         table = self.database_from.get_data(table_from, **gkws)
         action = []
         time_start = time.time()
         first = False
 
         idx = 0
         for idx, d in enumerate(table):
```

### Comparing `d22d-1.1.8/d22d/utils/db/myutils.py` & `d22d-1.1.9/d22d/utils/db/myutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import time
 import datetime
 import json
 import hashlib
 import elasticsearch
 import elasticsearch.helpers
 from six import itervalues
-from werkzeug.utils import text_type
+# from werkzeug.utils import text_type
 import psycopg2 as d_b_c
 import psycopg2
 
 INSERT_NORMAL = 0
 INSERT_REPLACE = 1
 INSERT_IGNORE = 2
 import mysql.connector as d_b_c
@@ -136,15 +136,15 @@
 class T:
     def __init__(self, **kwargs):
         for k, v in kwargs.items():
             setattr(self, k, v)
 
 
 def secure_filename(filename):
-    if isinstance(filename, text_type):
+    if isinstance(filename, str):
         from unicodedata import normalize
         filename = normalize('NFKD', filename).encode('utf-8', 'ignore')  # 转码
         if not PY2:
             filename = filename.decode('utf-8')  # 解码
     for sep in os.path.sep, os.path.altsep:
         if sep:
             filename = filename.replace(sep, ' ')
@@ -539,16 +539,16 @@
         实现了"加强"连接。具体指当数据库连接关闭、丢失或使用频率超出限制时，将自动重新获取连接。
 
         典型的应用场景如下：在某个维持了某些数据库连接的程序运行时重启了数据库，
         或在某个防火墙隔离的网络中访问远程数据库时重启了防火墙。
         """
 
         import pymysql
-        from DBUtils import SteadyDB
-        self.dbc = SteadyDB.connect(
+        from dbutils.steady_db import connect
+        self.dbc = connect(
             creator=pymysql,
             host=host, user=user,
             passwd=passwd,
             database=database if database else None,
             port=port,
             charset='utf8mb4',
             use_unicode=True,
```

### Comparing `d22d-1.1.8/d22d/utils/db/sqlfileextra.py` & `d22d-1.1.9/d22d/utils/db/sqlfileextra.py`

 * *Files identical despite different names*

### Comparing `d22d-1.1.8/d22d/utils/logger.py` & `d22d-1.1.9/d22d/utils/logger.py`

 * *Files identical despite different names*

### Comparing `d22d-1.1.8/d22d/utils/req_conflit.py` & `d22d-1.1.9/d22d/utils/req_conflit.py`

 * *Files identical despite different names*

### Comparing `d22d-1.1.8/d22d/utils/utils.py` & `d22d-1.1.9/d22d/utils/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import random
+import string
 import time
 import logging
 import wrapt
+import traceback
 import datetime
 import asyncio.exceptions
 from json import JSONEncoder, dumps
 from asyncio import sleep
 from base64 import b64encode
 from async_timeout import timeout as a_timeout
 
-
 logger = logging.getLogger('d22d.task')
 
 
 def dump_json(obj):
     if (not obj) or isinstance(obj, type(None)):
         return ''
 
@@ -82,15 +84,16 @@
             ex_msg = error_d[ex.__class__]
             if ex_msg is not None:
                 logger.error(f'[RetryS:{retry:04d}:{time.time() - time_start:.2f}s] {func_info} {ex_msg}')
             if ex.__class__ in raise_e:
                 raise ex
         except tuple({Exception: ""}.keys()) as ex:
             error = ex
-            logger.error(f'[RetryS:{retry:04d}:{time.time() - time_start:.2f}s]  {func_info}', ex)
+            logger.error(f'[RetryS:{retry:04d}:{time.time() - time_start:.2f}s]  {func_info}'
+                         f' {type(ex)} {str(ex)[:250]:250s}\n{traceback.format_exc()}')
             if ex.__class__ in raise_e:
                 raise ex
         if (
                 (max_retry and retry > max_retry) or
                 (timeout and ((time.time() - time_start) > timeout))
         ):
             raise error
@@ -154,18 +157,19 @@
                 ex_msg = error_d[ex.__class__]
                 if ex_msg is not None:
                     logger.error(f'[RetryS:{retry:04d}:{time.time() - time_start:.2f}s] {func_info} {ex_msg}')
                 if ex.__class__ in raise_e:
                     raise ex
             except tuple({Exception: ""}.keys()) as ex:
                 error = ex
-                logger.error(f'[RetryS:{retry:04d}:{time.time() - time_start:.2f}s]  {func_info}'
-                              f' {type(ex)} {str(ex)[:250]:250s}',
-                              # f' {args} {kwargs}',
-                              )
+                logger.error(
+                    f'[RetryS:{retry:04d}:{time.time() - time_start:.2f}s]  {func_info}'
+                    f' {type(ex)} {str(ex)[:250]:250s}\n{traceback.format_exc()}',
+                    # f' {args} {kwargs}',
+                )
                 if ex.__class__ in raise_e:
                     raise ex
             if (
                     (max_retry and retry > max_retry) or
                     (timeout and ((time.time() - time_start) > timeout))
             ):
                 raise error
@@ -269,18 +273,18 @@
                     logger.error(f'[RetryS:{retry:04d}:{time.time() - time_start:.2f}s] {func_info} {ex_msg}')
                     if (raise_e is True) or (ex.__class__ in raise_e):
                         raise ex
             except tuple({Exception: ""}.keys()) as ex:
                 error = ex
                 import traceback
                 logger.error(f'[RetryS:{retry:04d}:{time.time() - time_start:.2f}s]  {func_info}'
-                              f' {type(ex)} {str(ex)[:150]}'
-                              f'\n{traceback.format_exc()}',
-                              # f' {args} {kwargs}',
-                              )
+                             f' {type(ex)} {str(ex)[:150]}'
+                             f'\n{traceback.format_exc()}',
+                             # f' {args} {kwargs}',
+                             )
                 if (raise_e is True) or (ex.__class__ in raise_e):
                     raise ex
             finally:
                 if finally_callback is not None:
                     finally_callback(*args, **kwargs)
             if (
                     (max_retry and retry > max_retry) or
@@ -322,10 +326,60 @@
                 if hasattr(obj, '__str__'):
                     return str(obj)
                 elif hasattr(obj, '__repr__'):
                     return obj.__repr__()
                 else:
                     raise ex
 
+def format_error(ex):
+    return '[{}] {}\n{}'.format(type(ex), ex, traceback.format_exc())
+
+
+def with_cur_lock():
+    @wrapt.decorator
+    def wrapper(func, instance, args, kwargs):
+        lock = instance.cur_lock
+        if lock.locked():
+            raise IOError(f'{args[0:]} cur locked')
+        lock.acquire()
+        try:
+            res = func(instance.cur, *args, **kwargs)
+            return res
+        except Exception as ex:
+            raise ex
+        finally:
+            lock.release()
+
+    return wrapper
+
+
+def gen_pass(val_type='all', val_len=8):
+    src_digits = string.digits  # string_数字  '0123456789'
+    src_uppercase = string.ascii_uppercase  # string_大写字母 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
+    src_lowercase = string.ascii_lowercase  # string_小写字母 'abcdefghijklmnopqrstuvwxyz'
+    src_special = string.punctuation  # string_特殊字符 '!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~'
+
+    if val_type.lower().find('int') == -1:
+        # sample从序列中选择n个随机独立的元素，返回列表
+        num = random.sample(src_digits, 1)  # 随机取1位数字
+        lower = random.sample(src_uppercase, 1)  # 随机取1位小写字母
+        upper = random.sample(src_lowercase, 1)  # 随机取1位大写字母
+        special = random.sample(src_special, 1)  # 随机取1位大写字母特殊字符
+        other = random.sample(string.ascii_letters + string.digits + string.punctuation, val_len - 4)
+        # 生成字符串
+        # print(num, lower, upper, special, other)
+        pwd_list = num + lower + upper + special + other
+        # shuffle将一个序列中的元素随机打乱，打乱字符串
+        random.shuffle(pwd_list)
+        # 列表转字符串
+        password_str = ''.join(pwd_list)
+        # print(password_str)
+    else:
+        pwd_list = random.sample(string.digits, val_len)
+        random.shuffle(pwd_list)
+        # 列表转字符串
+        password_str = int(''.join(pwd_list))
+
+    return password_str
 
 if __name__ == '__main__':
     run_task_auto_retry(run_task_auto_retry)
```

### Comparing `d22d-1.1.8/d22d.egg-info/PKG-INFO` & `d22d-1.1.9/d22d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d22d
-Version: 1.1.8
+Version: 1.1.9
 Summary: Migrating form DateBase to DateBase by 2 lines code
 Home-page: https://github.com/DJMIN/D2D
 Author: readerror
 Author-email: readerror@sina.com
 Maintainer: readerror
 Maintainer-email: readerror@sina.com
 License: GPL License
@@ -91,18 +91,19 @@
         1. need python3
         1. create your .py file 
         ```python
         import d22d
         from d22d import (
         ElasticSearchD, MySqlD, CsvD, SqlFileD, JsonListD,
          XlsIbyFileD, XlsxIbyFileD, MongoDBD, 
-         Migration, Migration2DB
+         Migration, Migration2DB, open_log
         )
         
         def test1():
+            open_log()
             t = Migration(
                 database_from=MySqlD(host='localhost', port=3306, database='test',
                                         user='root', passwd='root'),
                 database_to=MySqlD(host='192.168.0.100', port=3306, database='test',
                                         user='root', passwd='root'),
                 table_from='user',
                 table_to='user'
```

### Comparing `d22d-1.1.8/d22d.egg-info/requires.txt` & `d22d-1.1.9/d22d.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -68,16 +68,19 @@
 flask_mongoengine
 celery
 flask_sqlalchemy
 setuptools
 pycryptodome
 wrapt
 twine
+sqlparse
 six
 requests>=2.22.0
 elasticsearch_dsl>=6.1
-PyMySQL==0.9.3
-telethon==1.11.3
+PyMySQL>=0.9.3
 mysql-connector-python>=8.0.6
 redis>=3.2.1
-DBUtils==1.3
+DBUtils>=2.0
 elasticsearch>=6.1.1
+diskcache
+tomorrow3
+clickhouse_driver
```

### Comparing `d22d-1.1.8/requirements.txt` & `d22d-1.1.9/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -71,22 +71,24 @@
 setuptools
 pycryptodome
 wrapt
 twine
 six
 requests>=2.22.0
 elasticsearch_dsl>=6.1
-PyMySQL==0.9.3
-telethon==1.11.3
+PyMySQL>=1.0.2
 mysql-connector-python>=8.0.6
 redis>=3.2.1
-DBUtils==1.3
+DBUtils>=2.0
 elasticsearch>=6.1.1
 wheel
 sqlparse
+diskcache
+tomorrow3
+clickhouse_driver
 # supervisor
 # flask_mongoengine install error need 3 pkg
 # mysql
 # pymongo==3.2  # pymongo.errors.ConfigurationError: Server at 127.0.0.1:27017 reports wire version 0, but this version of PyMongo requires at least 2 (MongoDB 2.6).
 # blob utf8 decode error
 # sasl
 # gevent
```

### Comparing `d22d-1.1.8/setup.py` & `d22d-1.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,18 +91,21 @@
         "flask_mongoengine",
         "celery",
         "flask_sqlalchemy",
         "setuptools",
         "pycryptodome",
         "wrapt",
         "twine",
+        "sqlparse",
         "six",
         "requests>=2.22.0",
         "elasticsearch_dsl>=6.1",
-        "PyMySQL==0.9.3",
-        "telethon==1.11.3",
+        "PyMySQL>=0.9.3",
         "mysql-connector-python>=8.0.6",
         "redis>=3.2.1",
-        "DBUtils==1.3",
+        "DBUtils>=2.0",
         "elasticsearch>=6.1.1",
+        "diskcache",
+        "tomorrow3",
+        "clickhouse_driver",
     ],
 )
```

