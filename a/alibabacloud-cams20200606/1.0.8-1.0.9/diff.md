# Comparing `tmp/alibabacloud_cams20200606-1.0.8.tar.gz` & `tmp/alibabacloud_cams20200606-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cams20200606-1.0.8.tar", last modified: Thu May 26 03:49:24 2022, max compression
+gzip compressed data, was "dist/alibabacloud_cams20200606-1.0.9.tar", last modified: Fri Jul 15 02:42:12 2022, max compression
```

## Comparing `alibabacloud_cams20200606-1.0.8.tar` & `alibabacloud_cams20200606-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 03:49:24.000000 alibabacloud_cams20200606-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      350 2022-05-26 03:49:23.000000 alibabacloud_cams20200606-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-05-26 03:49:23.000000 alibabacloud_cams20200606-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-05-26 03:49:23.000000 alibabacloud_cams20200606-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2334 2022-05-26 03:49:24.000000 alibabacloud_cams20200606-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2022-05-26 03:49:23.000000 alibabacloud_cams20200606-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1110 2022-05-26 03:49:23.000000 alibabacloud_cams20200606-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 03:49:24.000000 alibabacloud_cams20200606-1.0.8/alibabacloud_cams20200606/
--rw-r--r--   0 root         (0) root         (0)       21 2022-05-26 03:49:23.000000 alibabacloud_cams20200606-1.0.8/alibabacloud_cams20200606/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26426 2022-05-26 03:49:23.000000 alibabacloud_cams20200606-1.0.8/alibabacloud_cams20200606/client.py
--rw-r--r--   0 root         (0) root         (0)    54011 2022-05-26 03:49:23.000000 alibabacloud_cams20200606-1.0.8/alibabacloud_cams20200606/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 03:49:24.000000 alibabacloud_cams20200606-1.0.8/alibabacloud_cams20200606.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2334 2022-05-26 03:49:23.000000 alibabacloud_cams20200606-1.0.8/alibabacloud_cams20200606.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2022-05-26 03:49:23.000000 alibabacloud_cams20200606-1.0.8/alibabacloud_cams20200606.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-26 03:49:23.000000 alibabacloud_cams20200606-1.0.8/alibabacloud_cams20200606.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-05-26 03:49:23.000000 alibabacloud_cams20200606-1.0.8/alibabacloud_cams20200606.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2022-05-26 03:49:23.000000 alibabacloud_cams20200606-1.0.8/alibabacloud_cams20200606.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-05-26 03:49:24.000000 alibabacloud_cams20200606-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2615 2022-05-26 03:49:23.000000 alibabacloud_cams20200606-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 02:42:12.000000 alibabacloud_cams20200606-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      397 2022-07-15 02:42:11.000000 alibabacloud_cams20200606-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-07-15 02:42:11.000000 alibabacloud_cams20200606-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-07-15 02:42:11.000000 alibabacloud_cams20200606-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2334 2022-07-15 02:42:12.000000 alibabacloud_cams20200606-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2022-07-15 02:42:11.000000 alibabacloud_cams20200606-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1110 2022-07-15 02:42:11.000000 alibabacloud_cams20200606-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 02:42:12.000000 alibabacloud_cams20200606-1.0.9/alibabacloud_cams20200606/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-07-15 02:42:11.000000 alibabacloud_cams20200606-1.0.9/alibabacloud_cams20200606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26904 2022-07-15 02:42:11.000000 alibabacloud_cams20200606-1.0.9/alibabacloud_cams20200606/client.py
+-rw-r--r--   0 root         (0) root         (0)    55351 2022-07-15 02:42:11.000000 alibabacloud_cams20200606-1.0.9/alibabacloud_cams20200606/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 02:42:12.000000 alibabacloud_cams20200606-1.0.9/alibabacloud_cams20200606.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2334 2022-07-15 02:42:11.000000 alibabacloud_cams20200606-1.0.9/alibabacloud_cams20200606.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2022-07-15 02:42:11.000000 alibabacloud_cams20200606-1.0.9/alibabacloud_cams20200606.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-07-15 02:42:11.000000 alibabacloud_cams20200606-1.0.9/alibabacloud_cams20200606.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-07-15 02:42:11.000000 alibabacloud_cams20200606-1.0.9/alibabacloud_cams20200606.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2022-07-15 02:42:11.000000 alibabacloud_cams20200606-1.0.9/alibabacloud_cams20200606.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-07-15 02:42:12.000000 alibabacloud_cams20200606-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2615 2022-07-15 02:42:11.000000 alibabacloud_cams20200606-1.0.9/setup.py
```

### Comparing `alibabacloud_cams20200606-1.0.8/LICENSE` & `alibabacloud_cams20200606-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cams20200606-1.0.8/PKG-INFO` & `alibabacloud_cams20200606-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cams20200606
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud cams (20200606) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cams20200606-1.0.8/README-CN.md` & `alibabacloud_cams20200606-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cams20200606-1.0.8/README.md` & `alibabacloud_cams20200606-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cams20200606-1.0.8/alibabacloud_cams20200606/client.py` & `alibabacloud_cams20200606-1.0.9/alibabacloud_cams20200606/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,14 +501,18 @@
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
@@ -557,14 +561,18 @@
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

### Comparing `alibabacloud_cams20200606-1.0.8/alibabacloud_cams20200606/models.py` & `alibabacloud_cams20200606-1.0.9/alibabacloud_cams20200606/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1426,14 +1426,16 @@
 
 class SendChatappMessageRequest(TeaModel):
     def __init__(
         self,
         channel_type: str = None,
         content: str = None,
         cust_waba_id: str = None,
+        fall_back_content: str = None,
+        fall_back_id: str = None,
         from_: str = None,
         language: str = None,
         message_type: str = None,
         payload: List[str] = None,
         template_code: str = None,
         template_params: Dict[str, str] = None,
         to: str = None,
@@ -1441,14 +1443,18 @@
     ):
         # 通道类型 whatsapp/viber/line
         self.channel_type = channel_type
         # 消息内容
         self.content = content
         # ISV客户wabaId
         self.cust_waba_id = cust_waba_id
+        # 回落消息内容
+        self.fall_back_content = fall_back_content
+        # 回落策略ID，可在控制台创建策略并查看
+        self.fall_back_id = fall_back_id
         # 发送方
         self.from_ = from_
         # 语言
         self.language = language
         # 消息类型
         self.message_type = message_type
         self.payload = payload
@@ -1473,14 +1479,18 @@
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
@@ -1499,14 +1509,18 @@
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
@@ -1524,14 +1538,16 @@
 
 class SendChatappMessageShrinkRequest(TeaModel):
     def __init__(
         self,
         channel_type: str = None,
         content: str = None,
         cust_waba_id: str = None,
+        fall_back_content: str = None,
+        fall_back_id: str = None,
         from_: str = None,
         language: str = None,
         message_type: str = None,
         payload_shrink: str = None,
         template_code: str = None,
         template_params_shrink: str = None,
         to: str = None,
@@ -1539,14 +1555,18 @@
     ):
         # 通道类型 whatsapp/viber/line
         self.channel_type = channel_type
         # 消息内容
         self.content = content
         # ISV客户wabaId
         self.cust_waba_id = cust_waba_id
+        # 回落消息内容
+        self.fall_back_content = fall_back_content
+        # 回落策略ID，可在控制台创建策略并查看
+        self.fall_back_id = fall_back_id
         # 发送方
         self.from_ = from_
         # 语言
         self.language = language
         # 消息类型
         self.message_type = message_type
         self.payload_shrink = payload_shrink
@@ -1571,14 +1591,18 @@
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
@@ -1597,14 +1621,18 @@
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

### Comparing `alibabacloud_cams20200606-1.0.8/alibabacloud_cams20200606.egg-info/PKG-INFO` & `alibabacloud_cams20200606-1.0.9/alibabacloud_cams20200606.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cams20200606
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud cams (20200606) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cams20200606-1.0.8/setup.py` & `alibabacloud_cams20200606-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cams20200606.
 
-Created on 26/05/2022
+Created on 15/07/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cams20200606"
 NAME = "alibabacloud_cams20200606" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud cams (20200606) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.1, <1.0.0",
+    "alibabacloud_tea_util>=0.3.6, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
     "alibabacloud_openapi_util>=0.1.6, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

