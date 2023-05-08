# Comparing `tmp/alibabacloud_cams20200606_py2-1.0.8.tar.gz` & `tmp/alibabacloud_cams20200606_py2-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cams20200606_py2-1.0.8.tar", last modified: Wed May 11 09:36:29 2022, max compression
+gzip compressed data, was "dist/alibabacloud_cams20200606_py2-1.0.9.tar", last modified: Fri Jul 15 02:41:45 2022, max compression
```

## Comparing `alibabacloud_cams20200606_py2-1.0.8.tar` & `alibabacloud_cams20200606_py2-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-11 09:36:29.000000 alibabacloud_cams20200606_py2-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      588 2022-05-11 09:36:29.000000 alibabacloud_cams20200606_py2-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-05-11 09:36:29.000000 alibabacloud_cams20200606_py2-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2478 2022-05-11 09:36:29.000000 alibabacloud_cams20200606_py2-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1036 2022-05-11 09:36:29.000000 alibabacloud_cams20200606_py2-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2022-05-11 09:36:29.000000 alibabacloud_cams20200606_py2-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-11 09:36:29.000000 alibabacloud_cams20200606_py2-1.0.8/alibabacloud_cams20200606/
--rw-r--r--   0 root         (0) root         (0)       21 2022-05-11 09:36:29.000000 alibabacloud_cams20200606_py2-1.0.8/alibabacloud_cams20200606/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11964 2022-05-11 09:36:29.000000 alibabacloud_cams20200606_py2-1.0.8/alibabacloud_cams20200606/client.py
--rw-r--r--   0 root         (0) root         (0)    54292 2022-05-11 09:36:29.000000 alibabacloud_cams20200606_py2-1.0.8/alibabacloud_cams20200606/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-11 09:36:29.000000 alibabacloud_cams20200606_py2-1.0.8/alibabacloud_cams20200606_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2478 2022-05-11 09:36:29.000000 alibabacloud_cams20200606_py2-1.0.8/alibabacloud_cams20200606_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      435 2022-05-11 09:36:29.000000 alibabacloud_cams20200606_py2-1.0.8/alibabacloud_cams20200606_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-11 09:36:29.000000 alibabacloud_cams20200606_py2-1.0.8/alibabacloud_cams20200606_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-05-11 09:36:29.000000 alibabacloud_cams20200606_py2-1.0.8/alibabacloud_cams20200606_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2022-05-11 09:36:29.000000 alibabacloud_cams20200606_py2-1.0.8/alibabacloud_cams20200606_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-05-11 09:36:29.000000 alibabacloud_cams20200606_py2-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2908 2022-05-11 09:36:29.000000 alibabacloud_cams20200606_py2-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 02:41:45.000000 alibabacloud_cams20200606_py2-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)       79 2022-07-15 02:41:44.000000 alibabacloud_cams20200606_py2-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2022-07-15 02:41:44.000000 alibabacloud_cams20200606_py2-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2022-07-15 02:41:44.000000 alibabacloud_cams20200606_py2-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2478 2022-07-15 02:41:45.000000 alibabacloud_cams20200606_py2-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1036 2022-07-15 02:41:44.000000 alibabacloud_cams20200606_py2-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2022-07-15 02:41:44.000000 alibabacloud_cams20200606_py2-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 02:41:45.000000 alibabacloud_cams20200606_py2-1.0.9/alibabacloud_cams20200606/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-07-15 02:41:44.000000 alibabacloud_cams20200606_py2-1.0.9/alibabacloud_cams20200606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12203 2022-07-15 02:41:44.000000 alibabacloud_cams20200606_py2-1.0.9/alibabacloud_cams20200606/client.py
+-rw-r--r--   0 root         (0) root         (0)    55658 2022-07-15 02:41:44.000000 alibabacloud_cams20200606_py2-1.0.9/alibabacloud_cams20200606/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 02:41:45.000000 alibabacloud_cams20200606_py2-1.0.9/alibabacloud_cams20200606_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2478 2022-07-15 02:41:45.000000 alibabacloud_cams20200606_py2-1.0.9/alibabacloud_cams20200606_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      448 2022-07-15 02:41:45.000000 alibabacloud_cams20200606_py2-1.0.9/alibabacloud_cams20200606_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-07-15 02:41:45.000000 alibabacloud_cams20200606_py2-1.0.9/alibabacloud_cams20200606_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2022-07-15 02:41:45.000000 alibabacloud_cams20200606_py2-1.0.9/alibabacloud_cams20200606_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2022-07-15 02:41:45.000000 alibabacloud_cams20200606_py2-1.0.9/alibabacloud_cams20200606_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-07-15 02:41:45.000000 alibabacloud_cams20200606_py2-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2908 2022-07-15 02:41:44.000000 alibabacloud_cams20200606_py2-1.0.9/setup.py
```

### Comparing `alibabacloud_cams20200606_py2-1.0.8/LICENSE` & `alibabacloud_cams20200606_py2-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cams20200606_py2-1.0.8/PKG-INFO` & `alibabacloud_cams20200606_py2-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cams20200606_py2
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud cams (20200606) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cams20200606_py2-1.0.8/README-CN.md` & `alibabacloud_cams20200606_py2-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cams20200606_py2-1.0.8/README.md` & `alibabacloud_cams20200606_py2-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cams20200606_py2-1.0.8/alibabacloud_cams20200606/client.py` & `alibabacloud_cams20200606_py2-1.0.9/alibabacloud_cams20200606/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,14 +230,18 @@
         if not UtilClient.is_unset(request.payload_shrink):
             query['Payload'] = request.payload_shrink
         body = {}
         if not UtilClient.is_unset(request.channel_type):
             body['ChannelType'] = request.channel_type
         if not UtilClient.is_unset(request.cust_waba_id):
             body['CustWabaId'] = request.cust_waba_id
+        if not UtilClient.is_unset(request.fall_back_content):
+            body['FallBackContent'] = request.fall_back_content
+        if not UtilClient.is_unset(request.fall_back_id):
+            body['FallBackId'] = request.fall_back_id
         if not UtilClient.is_unset(request.from_):
             body['From'] = request.from_
         if not UtilClient.is_unset(request.language):
             body['Language'] = request.language
         if not UtilClient.is_unset(request.message_type):
             body['MessageType'] = request.message_type
         if not UtilClient.is_unset(request.template_code):
```

### Comparing `alibabacloud_cams20200606_py2-1.0.8/alibabacloud_cams20200606/models.py` & `alibabacloud_cams20200606_py2-1.0.9/alibabacloud_cams20200606/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1256,22 +1256,27 @@
         if m.get('body') is not None:
             temp_model = ListChatappTemplateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SendChatappMessageRequest(TeaModel):
-    def __init__(self, channel_type=None, content=None, cust_waba_id=None, from_=None, language=None,
-                 message_type=None, payload=None, template_code=None, template_params=None, to=None, type=None):
+    def __init__(self, channel_type=None, content=None, cust_waba_id=None, fall_back_content=None,
+                 fall_back_id=None, from_=None, language=None, message_type=None, payload=None, template_code=None,
+                 template_params=None, to=None, type=None):
         # 通道类型 whatsapp/viber/line
         self.channel_type = channel_type  # type: str
         # 消息内容
         self.content = content  # type: str
         # ISV客户wabaId
         self.cust_waba_id = cust_waba_id  # type: str
+        # 回落消息内容
+        self.fall_back_content = fall_back_content  # type: str
+        # 回落策略ID，可在控制台创建策略并查看
+        self.fall_back_id = fall_back_id  # type: str
         # 发送方
         self.from_ = from_  # type: str
         # 语言
         self.language = language  # type: str
         # 消息类型
         self.message_type = message_type  # type: str
         self.payload = payload  # type: list[str]
@@ -1296,14 +1301,18 @@
         result = dict()
         if self.channel_type is not None:
             result['ChannelType'] = self.channel_type
         if self.content is not None:
             result['Content'] = self.content
         if self.cust_waba_id is not None:
             result['CustWabaId'] = self.cust_waba_id
+        if self.fall_back_content is not None:
+            result['FallBackContent'] = self.fall_back_content
+        if self.fall_back_id is not None:
+            result['FallBackId'] = self.fall_back_id
         if self.from_ is not None:
             result['From'] = self.from_
         if self.language is not None:
             result['Language'] = self.language
         if self.message_type is not None:
             result['MessageType'] = self.message_type
         if self.payload is not None:
@@ -1322,14 +1331,18 @@
         m = m or dict()
         if m.get('ChannelType') is not None:
             self.channel_type = m.get('ChannelType')
         if m.get('Content') is not None:
             self.content = m.get('Content')
         if m.get('CustWabaId') is not None:
             self.cust_waba_id = m.get('CustWabaId')
+        if m.get('FallBackContent') is not None:
+            self.fall_back_content = m.get('FallBackContent')
+        if m.get('FallBackId') is not None:
+            self.fall_back_id = m.get('FallBackId')
         if m.get('From') is not None:
             self.from_ = m.get('From')
         if m.get('Language') is not None:
             self.language = m.get('Language')
         if m.get('MessageType') is not None:
             self.message_type = m.get('MessageType')
         if m.get('Payload') is not None:
@@ -1342,22 +1355,27 @@
             self.to = m.get('To')
         if m.get('Type') is not None:
             self.type = m.get('Type')
         return self
 
 
 class SendChatappMessageShrinkRequest(TeaModel):
-    def __init__(self, channel_type=None, content=None, cust_waba_id=None, from_=None, language=None,
-                 message_type=None, payload_shrink=None, template_code=None, template_params_shrink=None, to=None, type=None):
+    def __init__(self, channel_type=None, content=None, cust_waba_id=None, fall_back_content=None,
+                 fall_back_id=None, from_=None, language=None, message_type=None, payload_shrink=None, template_code=None,
+                 template_params_shrink=None, to=None, type=None):
         # 通道类型 whatsapp/viber/line
         self.channel_type = channel_type  # type: str
         # 消息内容
         self.content = content  # type: str
         # ISV客户wabaId
         self.cust_waba_id = cust_waba_id  # type: str
+        # 回落消息内容
+        self.fall_back_content = fall_back_content  # type: str
+        # 回落策略ID，可在控制台创建策略并查看
+        self.fall_back_id = fall_back_id  # type: str
         # 发送方
         self.from_ = from_  # type: str
         # 语言
         self.language = language  # type: str
         # 消息类型
         self.message_type = message_type  # type: str
         self.payload_shrink = payload_shrink  # type: str
@@ -1382,14 +1400,18 @@
         result = dict()
         if self.channel_type is not None:
             result['ChannelType'] = self.channel_type
         if self.content is not None:
             result['Content'] = self.content
         if self.cust_waba_id is not None:
             result['CustWabaId'] = self.cust_waba_id
+        if self.fall_back_content is not None:
+            result['FallBackContent'] = self.fall_back_content
+        if self.fall_back_id is not None:
+            result['FallBackId'] = self.fall_back_id
         if self.from_ is not None:
             result['From'] = self.from_
         if self.language is not None:
             result['Language'] = self.language
         if self.message_type is not None:
             result['MessageType'] = self.message_type
         if self.payload_shrink is not None:
@@ -1408,14 +1430,18 @@
         m = m or dict()
         if m.get('ChannelType') is not None:
             self.channel_type = m.get('ChannelType')
         if m.get('Content') is not None:
             self.content = m.get('Content')
         if m.get('CustWabaId') is not None:
             self.cust_waba_id = m.get('CustWabaId')
+        if m.get('FallBackContent') is not None:
+            self.fall_back_content = m.get('FallBackContent')
+        if m.get('FallBackId') is not None:
+            self.fall_back_id = m.get('FallBackId')
         if m.get('From') is not None:
             self.from_ = m.get('From')
         if m.get('Language') is not None:
             self.language = m.get('Language')
         if m.get('MessageType') is not None:
             self.message_type = m.get('MessageType')
         if m.get('Payload') is not None:
```

### Comparing `alibabacloud_cams20200606_py2-1.0.8/alibabacloud_cams20200606_py2.egg-info/PKG-INFO` & `alibabacloud_cams20200606_py2-1.0.9/alibabacloud_cams20200606_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cams20200606-py2
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud cams (20200606) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cams20200606_py2-1.0.8/setup.py` & `alibabacloud_cams20200606_py2-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cams20200606_py2.
 
-Created on 11/05/2022
+Created on 15/07/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cams20200606"
 NAME = "alibabacloud_cams20200606_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud cams (20200606) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.5, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.1, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.6, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.3, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
```

