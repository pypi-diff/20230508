# Comparing `tmp/dtsdk-1.1.0.tar.gz` & `tmp/dtsdk-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dtsdk-1.1.0.tar", last modified: Fri Dec 30 18:06:25 2022, max compression
+gzip compressed data, was "/Users/vivi/SourceCode/datatower.ai-python/dist/.tmp-6a_fwd1a/dtsdk-2.0.0.tar", last modified: Mon May  8 09:50:54 2023, max compression
```

## Comparing `dtsdk-1.1.0.tar` & `dtsdk-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 vivi       (501) staff       (20)        0 2022-12-30 18:06:25.000000 dtsdk-1.1.0/
--rw-r--r--   0 vivi       (501) staff       (20)      558 2022-12-30 17:48:24.000000 dtsdk-1.1.0/LICENSE
--rw-r--r--   0 vivi       (501) staff       (20)      116 2022-12-30 17:48:24.000000 dtsdk-1.1.0/MANIFEST.in
--rw-r--r--   0 vivi       (501) staff       (20)     1223 2022-12-30 18:06:25.000000 dtsdk-1.1.0/PKG-INFO
--rw-r--r--   0 vivi       (501) staff       (20)      618 2022-12-30 17:49:10.000000 dtsdk-1.1.0/README.md
-drwxr-xr-x   0 vivi       (501) staff       (20)        0 2022-12-30 18:06:25.000000 dtsdk-1.1.0/dtsdk/
--rw-r--r--   0 vivi       (501) staff       (20)      201 2022-12-30 17:48:24.000000 dtsdk-1.1.0/dtsdk/__init__.py
--rw-r--r--   0 vivi       (501) staff       (20)    23991 2022-12-30 17:49:10.000000 dtsdk-1.1.0/dtsdk/sdk.py
-drwxr-xr-x   0 vivi       (501) staff       (20)        0 2022-12-30 18:06:25.000000 dtsdk-1.1.0/dtsdk.egg-info/
--rw-r--r--   0 vivi       (501) staff       (20)     1223 2022-12-30 18:06:24.000000 dtsdk-1.1.0/dtsdk.egg-info/PKG-INFO
--rw-r--r--   0 vivi       (501) staff       (20)      223 2022-12-30 18:06:24.000000 dtsdk-1.1.0/dtsdk.egg-info/SOURCES.txt
--rw-r--r--   0 vivi       (501) staff       (20)        1 2022-12-30 18:06:24.000000 dtsdk-1.1.0/dtsdk.egg-info/dependency_links.txt
--rw-r--r--   0 vivi       (501) staff       (20)        9 2022-12-30 18:06:24.000000 dtsdk-1.1.0/dtsdk.egg-info/requires.txt
--rw-r--r--   0 vivi       (501) staff       (20)       14 2022-12-30 18:06:24.000000 dtsdk-1.1.0/dtsdk.egg-info/top_level.txt
--rw-r--r--   0 vivi       (501) staff       (20)       78 2022-12-30 18:06:25.000000 dtsdk-1.1.0/setup.cfg
--rw-r--r--   0 vivi       (501) staff       (20)     1274 2022-12-30 17:48:24.000000 dtsdk-1.1.0/setup.py
+drwxr-xr-x   0 vivi       (501) staff       (20)        0 2023-05-08 09:50:54.000000 dtsdk-2.0.0/
+-rw-r--r--   0 vivi       (501) staff       (20)      558 2023-05-08 09:47:41.000000 dtsdk-2.0.0/LICENSE
+-rw-r--r--   0 vivi       (501) staff       (20)      116 2023-05-08 09:47:41.000000 dtsdk-2.0.0/MANIFEST.in
+-rw-r--r--   0 vivi       (501) staff       (20)     1223 2023-05-08 09:50:54.000000 dtsdk-2.0.0/PKG-INFO
+-rw-r--r--   0 vivi       (501) staff       (20)      618 2023-05-08 09:47:41.000000 dtsdk-2.0.0/README.md
+drwxr-xr-x   0 vivi       (501) staff       (20)        0 2023-05-08 09:50:54.000000 dtsdk-2.0.0/dtsdk/
+-rw-r--r--   0 vivi       (501) staff       (20)      201 2023-05-08 09:47:41.000000 dtsdk-2.0.0/dtsdk/__init__.py
+-rw-r--r--   0 vivi       (501) staff       (20)    27043 2023-05-08 09:47:41.000000 dtsdk-2.0.0/dtsdk/sdk.py
+drwxr-xr-x   0 vivi       (501) staff       (20)        0 2023-05-08 09:50:54.000000 dtsdk-2.0.0/dtsdk.egg-info/
+-rw-r--r--   0 vivi       (501) staff       (20)     1223 2023-05-08 09:50:54.000000 dtsdk-2.0.0/dtsdk.egg-info/PKG-INFO
+-rw-r--r--   0 vivi       (501) staff       (20)      259 2023-05-08 09:50:54.000000 dtsdk-2.0.0/dtsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 vivi       (501) staff       (20)        1 2023-05-08 09:50:54.000000 dtsdk-2.0.0/dtsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 vivi       (501) staff       (20)        9 2023-05-08 09:50:54.000000 dtsdk-2.0.0/dtsdk.egg-info/requires.txt
+-rw-r--r--   0 vivi       (501) staff       (20)       19 2023-05-08 09:50:54.000000 dtsdk-2.0.0/dtsdk.egg-info/top_level.txt
+-rw-r--r--   0 vivi       (501) staff       (20)       78 2023-05-08 09:50:54.000000 dtsdk-2.0.0/setup.cfg
+-rw-r--r--   0 vivi       (501) staff       (20)     1274 2023-05-08 09:47:41.000000 dtsdk-2.0.0/setup.py
+drwxr-xr-x   0 vivi       (501) staff       (20)        0 2023-05-08 09:50:54.000000 dtsdk-2.0.0/test/
+-rw-r--r--   0 vivi       (501) staff       (20)       65 2023-05-08 09:47:41.000000 dtsdk-2.0.0/test/__init__.py
+-rw-r--r--   0 vivi       (501) staff       (20)     3301 2023-05-08 09:47:41.000000 dtsdk-2.0.0/test/test_dtsdk.py
```

### Comparing `dtsdk-1.1.0/LICENSE` & `dtsdk-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dtsdk-1.1.0/PKG-INFO` & `dtsdk-2.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtsdk
-Version: 1.1.0
+Version: 2.0.0
 Summary: DataTower.ai SDK for Python
 Home-page: https://github.com/lovinjoy/datatower.ai-python
 Author: DataTower.ai, Inc.
 Author-email: contact@lovinjoy.com
 License: Apache
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dtsdk-1.1.0/README.md` & `dtsdk-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dtsdk-1.1.0/dtsdk/sdk.py` & `dtsdk-2.0.0/dtsdk/sdk.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # encoding:utf-8
 
 from __future__ import unicode_literals
+import copy
 import datetime
 import gzip
 import json
 import os
 import re
 import threading
 import time
 import random
 import requests
 from requests import ConnectionError
+import logging
+
+logger = logging.getLogger(__name__)
 
 default_server_url = "https://s2s.roiquery.com/sync"
-__version__ = '1.1.0'
+__version__ = '2.0.0'
 is_print = False
 
 __NAME_PATTERN = re.compile(r"^[#$a-zA-Z][a-zA-Z0-9_]{0,63}$", re.I)
 _STR_LD = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789'
 
 try:
     import queue
@@ -73,31 +77,43 @@
                 raise DTIllegalDataException(
                     "Event_name=[%s] property key must be a valid variable name. [key=%s]" % (event_name, str(key)))
 
             if '#user_add' == event_name.lower() and not isNumber(value):
                 raise DTIllegalDataException('User_add properties must be number type')
 
 
-def log(msg=None):
-    if (msg is not None and is_print):
-        print('[DataTower.ai-Python SDK V%s]-%s' % (__version__, msg))
+def log(msg=None, level=logging.INFO):
+    if msg is not None and is_print:
+        prefix = '[DataTower.ai-Python SDK V%s]' % __version__
+        if level <= logging.INFO:
+            logger.info("{}-{}".format(prefix, msg))
+        elif level <= logging.WARNING:
+            logger.warning("{}-{}".format(prefix, msg))
+        else:
+            logger.error("{}-{}".format(prefix, msg))
 
 
 class DTException(Exception):
     pass
 
 
 class DTIllegalDataException(DTException):
     """
     数据格式异常
     在发送的数据格式有误时，SDK 会抛出此异常，用户应当捕获并处理.
     """
     pass
 
 
+class DTMetaDataException(DTException):
+    """
+    dt_id, acid, event_name, event_time 等元数据出错异常
+    """
+
+
 class DTNetworkException(DTException):
     """
     网络异常
     在因为网络或者不可预知的问题导致数据无法发送时，SDK会抛出此异常，用户应当捕获并处理.
     """
     pass
 
@@ -203,19 +219,53 @@
 
         当您要上传数值型的属性时，您可以调用 user_add 来对该属性进行累加操作. 如果该属性还未被设置，则会赋值0后再进行计算.
         可传入负值，等同于相减操作.
 
         Args:
             dt_id: 访客 ID
             acid: 账户 ID
-            properties: 数值类型的用户属性
+            properties: Dict[str, int|float|double]
         """
         self.__add(dt_id=dt_id, acid=acid, event_name='#user_add', send_type='user',
                    properties_add=properties)
 
+    def user_append(self, dt_id=None, acid=None, properties=None):
+        """
+        对指定的**列表**类型的用户属性进行追加操作，列表内的元素都会转成字符串类型。
+
+        Args:
+            dt_id: 访客 ID
+            acid: 账户 ID
+            properties:  Dict[str, list]
+        """
+        for key, value in properties.items():
+            if not isinstance(value, list):
+                raise DTIllegalDataException('#user_append properties must be list type')
+            properties[key] = [str(i) for i in value]
+
+        self.__add(dt_id=dt_id, acid=acid, event_name='#user_append', send_type='user',
+                   properties_add=properties)
+
+    def user_uniq_append(self, dt_id=None, acid=None, properties=None):
+        """
+        对指定的**列表**类型的用户属性进行追加操作，列表内的元素都会转成字符串类型，并对该属性的数组进行去重
+
+        Args:
+            dt_id: 访客 ID
+            acid: 账户 ID
+            properties: Dict[str, list]
+        """
+        for key, value in properties.items():
+            if not isinstance(value, list):
+                raise DTIllegalDataException('#user_uniq_append properties must be list type')
+            properties[key] = [str(i) for i in value]
+
+        self.__add(dt_id=dt_id, acid=acid, event_name='#user_uniq_append', send_type='user',
+                   properties_add=properties)
+
     def track(self, dt_id=None, acid=None, event_name=None, properties=None):
         """
         发送事件数据
 
         您可以调用 track 来上传事件，建议您根据先前梳理的文档来设置事件的属性以及发送信息的条件. 事件的名称只能以字母开头，可包含数字，字母和下划线“_”，
         长度最大为 50 个字符，对字母大小写不敏感. 事件的属性是一个 dict 对象，其中每个元素代表一个属性.
 
@@ -262,45 +312,44 @@
 
         请在退出前调用本接口，以避免缓存内的数据丢失
         """
         self.__consumer.close()
 
     def _public_track_add(self, event_name, properties):
         if not is_str(event_name):
-            raise DTIllegalDataException('a string type event_name is required for track')
+            raise DTMetaDataException('a string type event_name is required for track')
 
         all_properties = self.__preset_properties.copy()
         all_properties.update(self.__super_properties)
         if self.__dynamic_super_properties_tracker:
             all_properties.update(self.__dynamic_super_properties_tracker.get_dynamic_super_properties())
         if properties:
             all_properties.update(properties)
         return all_properties
-        pass
 
     def __add(self, dt_id, acid, send_type, event_name=None, properties_add=None):
         if dt_id is None and acid is None:
-            raise DTException("dt_id and acid must be set at least one")
+            raise DTMetaDataException("dt_id and acid must be set at least one")
         if (dt_id is not None and not is_str(dt_id)) or (acid is not None and not is_str(acid)):
-            raise DTException("dt_id and acid must be string type")
+            raise DTMetaDataException("dt_id and acid must be string type")
 
         assert_properties(event_name, properties_add)
 
         data = {'#event_type': send_type}
         if properties_add:
-            properties = properties_add.copy()
+            properties = copy.deepcopy(properties_add)
         else:
             properties = {}
 
         self.__movePresetProperties(['#app_id', '#debug', '#event_time', '#event_syn'], data, properties)
 
         if '#event_time' not in data:
             self.__buildData(data, '#event_time', int(time.time() * 1000))
         if not is_int(data.get('#event_time')) or len(str(data.get('#event_time'))) != 13:
-            raise DTException("event_time must be timestamp (ms)")
+            raise DTMetaDataException("event_time must be timestamp (ms)")
 
         if '#event_syn' not in data:
             self.__buildData(data, '#event_syn', random_str(16))
 
         if dt_id is None:
             self.__buildData(data, '#dt_id', '0000000000000000000000000000000000000000')
         else:
@@ -309,17 +358,22 @@
         if self.debug:
             self.__buildData(data, '#debug', 'true')
 
         self.__buildData(data, '#app_id', self.__app_id)
         self.__buildData(data, '#event_name', event_name)
         self.__buildData(data, '#acid', acid)
         data['properties'] = properties
-        content = json.dumps(data, separators=(',', ':'), cls=DTDateTimeSerializer)
-        log('collect data={}'.format(content))
-        self.__consumer.add(content)
+        try:
+            content = json.dumps(data, separators=(',', ':'), cls=DTDateTimeSerializer, allow_nan=False)
+            log('collect data={}'.format(data))
+            self.__consumer.add(content)
+        except TypeError as e:
+            raise DTIllegalDataException(e)
+        except ValueError:
+            raise DTIllegalDataException("Nan or Inf data are not allowed")
 
     def __buildData(self, data, key, value):
         if value is not None:
             data[key] = value
 
     def __movePresetProperties(self, keys, data, properties):
         for key in keys:
@@ -409,15 +463,32 @@
         _lock(self._file_handler)
         return self
 
     def __exit__(self, t, v, tb):
         _unlock(self._file_handler)
 
 
-class BatchConsumer(object):
+class AbstractConsumer(object):
+    """
+        Consumer抽象类
+    """
+    def get_app_id(self):
+        raise NotImplementedError
+
+    def add(self, msg):
+        raise NotImplementedError
+
+    def flush(self):
+        raise NotImplementedError
+
+    def close(self):
+        raise NotImplementedError
+
+
+class BatchConsumer(AbstractConsumer):
     """
     同步、批量地向 DT 服务器传输数据
 
     通过HTTPS协议，同步地向 DT 服务器传输数据.
     但是存在网络不稳定等原因造成数据丢失的可能，因此不建议在生产环境中使用.
 
     触发上报的时机为以下条件满足其中之一的时候:
@@ -462,15 +533,16 @@
                 or len(self.__cache_buffer) > 0:
             self.flush_once()
 
     def flush(self, throw_exception=True):
         while len(self.__cache_buffer) > 0 or len(self.__message_channel) > 0:
             try:
                 self.flush_once(throw_exception)
-            except DTIllegalDataException:
+            except DTIllegalDataException as e:
+                log(e, level=logging.WARNING)
                 continue
 
     def flush_once(self, throw_exception=True):
         if len(self.__message_channel) == 0 and len(self.__cache_buffer) == 0:
             return
 
         self._cachelock.acquire()
@@ -499,25 +571,39 @@
             if len(self.__cache_buffer) > self.__max_cache_size:
                 self.__cache_buffer = self.__cache_buffer[1:]
             self._cachelock.release()
 
     def close(self):
         self.flush()
 
-    pass
 
+class DebugConsumer(AbstractConsumer):
+    def __init__(self, app_id, token, server_url=default_server_url, timeout=30000):
 
-class DebugConsumer(BatchConsumer):
-    def __init__(self, app_id, token, server_url=default_server_url, timeout=30000, interval=3, compress=True,
-                 max_cache_size=50):
-        super(DebugConsumer, self).__init__(app_id=app_id, token=token, server_url=server_url, batch=1, timeout=timeout,
-                                            interval=interval, compress=compress, max_cache_size=max_cache_size)
+        self.__message_channel = []
+        self.__cache_buffer = []
+        self.__last_flush = time.time()
+        self.__http_service = _HttpServices((urlparse(server_url)).geturl(), app_id, token, timeout, compress=False)
+        self.__app_id = app_id
+        DTAnalytics.enable_log(True)
+
+    def get_app_id(self):
+        return self.__app_id
 
+    def add(self, msg):
+        self.__http_service.send('[' + msg + ']', str(len(msg)))
 
-class AsyncBatchConsumer(object):
+    def flush(self):
+        pass
+
+    def close(self):
+        pass
+
+
+class AsyncBatchConsumer(AbstractConsumer):
     """
     异步、批量地向 DT 服务器发送数据
 
     AsyncBatchConsumer 使用独立的线程进行数据发送，当满足以下两个条件之一时触发数据上报:
     1. 数据条数大于预定义的最大值, 默认为 20 条
     2. 数据发送间隔超过预定义的最大时间, 默认为 3 秒
     """
@@ -582,18 +668,22 @@
                 break
 
         if len(flush_buffer) > 0:
             for i in range(3):  # 网络异常情况下重试 3 次
                 try:
                     self.__http_service.send('[' + ','.join(flush_buffer) + ']', str(len(flush_buffer)))
                     return True
-                except DTNetworkException:
-                    pass
-                except DTIllegalDataException:
+                except DTNetworkException as e:
+                    log("{}: {}".format(e, flush_buffer), level=logging.WARNING)
+                    continue
+                except DTIllegalDataException as e:
+                    log("{}: {}".format(e, flush_buffer), level=logging.WARNING)
                     break
+            log("{}: {}".format("Data translate failed 3 times", flush_buffer), level=logging.ERROR)
+
 
     class _AsyncFlushThread(threading.Thread):
         def __init__(self, consumer, interval):
             threading.Thread.__init__(self)
             self._consumer = consumer
             self._interval = interval
 
@@ -643,20 +733,20 @@
 class _HttpServices(object):
     """
     内部类，用于发送网络请求
 
     指定接收端地址和项目 APP ID, 实现向接收端上传数据的接口. 发送前将数据默认使用 Gzip 压缩,
     """
 
-    def __init__(self, server_uri, app_id, token, timeout=30000):
+    def __init__(self, server_uri, app_id, token, timeout=30000, compress=True):
         self.url = server_uri
         self.app_id = app_id
         self.token = token
         self.timeout = timeout
-        self.compress = True
+        self.compress = compress
 
     def send(self, data, length):
         """使用 Requests 发送数据给服务器
 
         Args:
             data: 待发送的数据
             length
@@ -671,22 +761,22 @@
             compress_type = 'gzip'
             if self.compress:
                 data = _gzip_string(data.encode("utf-8"))
             else:
                 compress_type = 'none'
                 data = data.encode("utf-8")
             headers['compress'] = compress_type
-            # print(self.url,data,headers)
             response = requests.post(self.url, data=data, headers=headers, timeout=self.timeout)
             if response.status_code == 200:
-                responseData = json.loads(response.text)
-                log('response={}'.format(responseData))
-                if responseData["code"] == 0:
+                response_data = json.loads(response.text)
+                log('response={}'.format(response_data))
+                if response_data["code"] == 0:
                     return True
                 else:
-                    raise DTIllegalDataException("Unexpected result code: " + str(responseData["code"]))
+                    raise DTIllegalDataException("Unexpected result code: " + str(response_data["code"]) \
+                                                 + " reason: " + response_data["msg"])
             else:
                 log('response={}'.format(response.status_code))
                 raise DTNetworkException("Unexpected Http status code " + str(response.status_code))
         except ConnectionError as e:
             time.sleep(0.5)
             raise DTNetworkException("Data transmission failed due to " + repr(e))
```

### Comparing `dtsdk-1.1.0/dtsdk.egg-info/PKG-INFO` & `dtsdk-2.0.0/dtsdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtsdk
-Version: 1.1.0
+Version: 2.0.0
 Summary: DataTower.ai SDK for Python
 Home-page: https://github.com/lovinjoy/datatower.ai-python
 Author: DataTower.ai, Inc.
 Author-email: contact@lovinjoy.com
 License: Apache
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dtsdk-1.1.0/setup.py` & `dtsdk-2.0.0/setup.py`

 * *Files identical despite different names*

