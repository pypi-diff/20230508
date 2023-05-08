# Comparing `tmp/alibabacloud_rocketmq20220801-1.0.4.tar.gz` & `tmp/alibabacloud_rocketmq20220801-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_rocketmq20220801-1.0.4.tar", last modified: Wed Feb  8 06:42:34 2023, max compression
+gzip compressed data, was "dist/alibabacloud_rocketmq20220801-1.0.5.tar", last modified: Mon May  8 11:38:20 2023, max compression
```

## Comparing `alibabacloud_rocketmq20220801-1.0.4.tar` & `alibabacloud_rocketmq20220801-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 06:42:34.000000 alibabacloud_rocketmq20220801-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      337 2023-02-08 06:42:34.000000 alibabacloud_rocketmq20220801-1.0.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-02-08 06:42:34.000000 alibabacloud_rocketmq20220801-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-02-08 06:42:34.000000 alibabacloud_rocketmq20220801-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2023-02-08 06:42:34.000000 alibabacloud_rocketmq20220801-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2023-02-08 06:42:34.000000 alibabacloud_rocketmq20220801-1.0.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-02-08 06:42:34.000000 alibabacloud_rocketmq20220801-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 06:42:34.000000 alibabacloud_rocketmq20220801-1.0.4/alibabacloud_rocketmq20220801/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-08 06:42:34.000000 alibabacloud_rocketmq20220801-1.0.4/alibabacloud_rocketmq20220801/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54664 2023-02-08 06:42:34.000000 alibabacloud_rocketmq20220801-1.0.4/alibabacloud_rocketmq20220801/client.py
--rw-r--r--   0 root         (0) root         (0)   131081 2023-02-08 06:42:34.000000 alibabacloud_rocketmq20220801-1.0.4/alibabacloud_rocketmq20220801/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 06:42:34.000000 alibabacloud_rocketmq20220801-1.0.4/alibabacloud_rocketmq20220801.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2023-02-08 06:42:34.000000 alibabacloud_rocketmq20220801-1.0.4/alibabacloud_rocketmq20220801.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2023-02-08 06:42:34.000000 alibabacloud_rocketmq20220801-1.0.4/alibabacloud_rocketmq20220801.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-08 06:42:34.000000 alibabacloud_rocketmq20220801-1.0.4/alibabacloud_rocketmq20220801.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-02-08 06:42:34.000000 alibabacloud_rocketmq20220801-1.0.4/alibabacloud_rocketmq20220801.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-02-08 06:42:34.000000 alibabacloud_rocketmq20220801-1.0.4/alibabacloud_rocketmq20220801.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-08 06:42:34.000000 alibabacloud_rocketmq20220801-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2635 2023-02-08 06:42:34.000000 alibabacloud_rocketmq20220801-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:38:20.000000 alibabacloud_rocketmq20220801-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      412 2023-05-08 11:38:19.000000 alibabacloud_rocketmq20220801-1.0.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-08 11:38:19.000000 alibabacloud_rocketmq20220801-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-08 11:38:19.000000 alibabacloud_rocketmq20220801-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-05-08 11:38:20.000000 alibabacloud_rocketmq20220801-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-05-08 11:38:19.000000 alibabacloud_rocketmq20220801-1.0.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-05-08 11:38:19.000000 alibabacloud_rocketmq20220801-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:38:20.000000 alibabacloud_rocketmq20220801-1.0.5/alibabacloud_rocketmq20220801/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-08 11:38:19.000000 alibabacloud_rocketmq20220801-1.0.5/alibabacloud_rocketmq20220801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54664 2023-05-08 11:38:19.000000 alibabacloud_rocketmq20220801-1.0.5/alibabacloud_rocketmq20220801/client.py
+-rw-r--r--   0 root         (0) root         (0)   133269 2023-05-08 11:38:19.000000 alibabacloud_rocketmq20220801-1.0.5/alibabacloud_rocketmq20220801/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:38:20.000000 alibabacloud_rocketmq20220801-1.0.5/alibabacloud_rocketmq20220801.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-05-08 11:38:20.000000 alibabacloud_rocketmq20220801-1.0.5/alibabacloud_rocketmq20220801.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-05-08 11:38:20.000000 alibabacloud_rocketmq20220801-1.0.5/alibabacloud_rocketmq20220801.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 11:38:20.000000 alibabacloud_rocketmq20220801-1.0.5/alibabacloud_rocketmq20220801.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-08 11:38:20.000000 alibabacloud_rocketmq20220801-1.0.5/alibabacloud_rocketmq20220801.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-08 11:38:20.000000 alibabacloud_rocketmq20220801-1.0.5/alibabacloud_rocketmq20220801.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-08 11:38:20.000000 alibabacloud_rocketmq20220801-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-05-08 11:38:19.000000 alibabacloud_rocketmq20220801-1.0.5/setup.py
```

### Comparing `alibabacloud_rocketmq20220801-1.0.4/LICENSE` & `alibabacloud_rocketmq20220801-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_rocketmq20220801-1.0.4/PKG-INFO` & `alibabacloud_rocketmq20220801-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_rocketmq20220801
-Version: 1.0.4
+Version: 1.0.5
 Summary: Alibaba Cloud RocketMQ (20220801) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rocketmq20220801-1.0.4/README-CN.md` & `alibabacloud_rocketmq20220801-1.0.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rocketmq20220801-1.0.4/README.md` & `alibabacloud_rocketmq20220801-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rocketmq20220801-1.0.4/alibabacloud_rocketmq20220801/client.py` & `alibabacloud_rocketmq20220801-1.0.5/alibabacloud_rocketmq20220801/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rocketmq20220801-1.0.4/alibabacloud_rocketmq20220801/models.py` & `alibabacloud_rocketmq20220801-1.0.5/alibabacloud_rocketmq20220801/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1630,15 +1630,15 @@
 
 
 class GetInstanceResponseBodyDataNetworkInfoEndpoints(TeaModel):
     def __init__(
         self,
         endpoint_type: str = None,
         endpoint_url: str = None,
-        ip_whitelist: str = None,
+        ip_whitelist: List[str] = None,
     ):
         self.endpoint_type = endpoint_type
         self.endpoint_url = endpoint_url
         self.ip_whitelist = ip_whitelist
 
     def validate(self):
         pass
@@ -1846,65 +1846,110 @@
         if m.get('sendReceiveRatio') is not None:
             self.send_receive_ratio = m.get('sendReceiveRatio')
         if m.get('supportAutoScaling') is not None:
             self.support_auto_scaling = m.get('supportAutoScaling')
         return self
 
 
+class GetInstanceResponseBodyDataSoftware(TeaModel):
+    def __init__(
+        self,
+        maintain_time: str = None,
+        software_version: str = None,
+        upgrade_method: str = None,
+    ):
+        self.maintain_time = maintain_time
+        self.software_version = software_version
+        self.upgrade_method = upgrade_method
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.maintain_time is not None:
+            result['maintainTime'] = self.maintain_time
+        if self.software_version is not None:
+            result['softwareVersion'] = self.software_version
+        if self.upgrade_method is not None:
+            result['upgradeMethod'] = self.upgrade_method
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('maintainTime') is not None:
+            self.maintain_time = m.get('maintainTime')
+        if m.get('softwareVersion') is not None:
+            self.software_version = m.get('softwareVersion')
+        if m.get('upgradeMethod') is not None:
+            self.upgrade_method = m.get('upgradeMethod')
+        return self
+
+
 class GetInstanceResponseBodyData(TeaModel):
     def __init__(
         self,
         account_info: GetInstanceResponseBodyDataAccountInfo = None,
         acl_info: GetInstanceResponseBodyDataAclInfo = None,
         bid: str = None,
         commodity_code: str = None,
         create_time: str = None,
         expire_time: str = None,
         ext_config: GetInstanceResponseBodyDataExtConfig = None,
+        group_count: int = None,
         instance_id: str = None,
         instance_name: str = None,
         instance_quotas: List[GetInstanceResponseBodyDataInstanceQuotas] = None,
         network_info: GetInstanceResponseBodyDataNetworkInfo = None,
         payment_type: str = None,
         product_info: GetInstanceResponseBodyDataProductInfo = None,
         region_id: str = None,
         release_time: str = None,
         remark: str = None,
         resource_group_id: str = None,
         series_code: str = None,
         service_code: str = None,
+        software: GetInstanceResponseBodyDataSoftware = None,
         start_time: str = None,
         status: str = None,
         sub_series_code: str = None,
+        topic_count: int = None,
         update_time: str = None,
         user_id: str = None,
     ):
         self.account_info = account_info
         self.acl_info = acl_info
         # BID
         self.bid = bid
         self.commodity_code = commodity_code
         self.create_time = create_time
         self.expire_time = expire_time
         self.ext_config = ext_config
+        self.group_count = group_count
         self.instance_id = instance_id
         self.instance_name = instance_name
         self.instance_quotas = instance_quotas
         self.network_info = network_info
         self.payment_type = payment_type
         self.product_info = product_info
         self.region_id = region_id
         self.release_time = release_time
         self.remark = remark
         self.resource_group_id = resource_group_id
         self.series_code = series_code
         self.service_code = service_code
+        self.software = software
         self.start_time = start_time
         self.status = status
         self.sub_series_code = sub_series_code
+        self.topic_count = topic_count
         self.update_time = update_time
         self.user_id = user_id
 
     def validate(self):
         if self.account_info:
             self.account_info.validate()
         if self.acl_info:
@@ -1915,14 +1960,16 @@
             for k in self.instance_quotas:
                 if k:
                     k.validate()
         if self.network_info:
             self.network_info.validate()
         if self.product_info:
             self.product_info.validate()
+        if self.software:
+            self.software.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -1936,14 +1983,16 @@
             result['commodityCode'] = self.commodity_code
         if self.create_time is not None:
             result['createTime'] = self.create_time
         if self.expire_time is not None:
             result['expireTime'] = self.expire_time
         if self.ext_config is not None:
             result['extConfig'] = self.ext_config.to_map()
+        if self.group_count is not None:
+            result['groupCount'] = self.group_count
         if self.instance_id is not None:
             result['instanceId'] = self.instance_id
         if self.instance_name is not None:
             result['instanceName'] = self.instance_name
         result['instanceQuotas'] = []
         if self.instance_quotas is not None:
             for k in self.instance_quotas:
@@ -1962,20 +2011,24 @@
             result['remark'] = self.remark
         if self.resource_group_id is not None:
             result['resourceGroupId'] = self.resource_group_id
         if self.series_code is not None:
             result['seriesCode'] = self.series_code
         if self.service_code is not None:
             result['serviceCode'] = self.service_code
+        if self.software is not None:
+            result['software'] = self.software.to_map()
         if self.start_time is not None:
             result['startTime'] = self.start_time
         if self.status is not None:
             result['status'] = self.status
         if self.sub_series_code is not None:
             result['subSeriesCode'] = self.sub_series_code
+        if self.topic_count is not None:
+            result['topicCount'] = self.topic_count
         if self.update_time is not None:
             result['updateTime'] = self.update_time
         if self.user_id is not None:
             result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
@@ -1993,14 +2046,16 @@
         if m.get('createTime') is not None:
             self.create_time = m.get('createTime')
         if m.get('expireTime') is not None:
             self.expire_time = m.get('expireTime')
         if m.get('extConfig') is not None:
             temp_model = GetInstanceResponseBodyDataExtConfig()
             self.ext_config = temp_model.from_map(m['extConfig'])
+        if m.get('groupCount') is not None:
+            self.group_count = m.get('groupCount')
         if m.get('instanceId') is not None:
             self.instance_id = m.get('instanceId')
         if m.get('instanceName') is not None:
             self.instance_name = m.get('instanceName')
         self.instance_quotas = []
         if m.get('instanceQuotas') is not None:
             for k in m.get('instanceQuotas'):
@@ -2022,20 +2077,25 @@
             self.remark = m.get('remark')
         if m.get('resourceGroupId') is not None:
             self.resource_group_id = m.get('resourceGroupId')
         if m.get('seriesCode') is not None:
             self.series_code = m.get('seriesCode')
         if m.get('serviceCode') is not None:
             self.service_code = m.get('serviceCode')
+        if m.get('software') is not None:
+            temp_model = GetInstanceResponseBodyDataSoftware()
+            self.software = temp_model.from_map(m['software'])
         if m.get('startTime') is not None:
             self.start_time = m.get('startTime')
         if m.get('status') is not None:
             self.status = m.get('status')
         if m.get('subSeriesCode') is not None:
             self.sub_series_code = m.get('subSeriesCode')
+        if m.get('topicCount') is not None:
+            self.topic_count = m.get('topicCount')
         if m.get('updateTime') is not None:
             self.update_time = m.get('updateTime')
         if m.get('userId') is not None:
             self.user_id = m.get('userId')
         return self
```

### Comparing `alibabacloud_rocketmq20220801-1.0.4/alibabacloud_rocketmq20220801.egg-info/PKG-INFO` & `alibabacloud_rocketmq20220801-1.0.5/alibabacloud_rocketmq20220801.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-rocketmq20220801
-Version: 1.0.4
+Version: 1.0.5
 Summary: Alibaba Cloud RocketMQ (20220801) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rocketmq20220801-1.0.4/setup.py` & `alibabacloud_rocketmq20220801-1.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_rocketmq20220801.
 
-Created on 08/02/2023
+Created on 08/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_rocketmq20220801"
 NAME = "alibabacloud_rocketmq20220801" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud RocketMQ (20220801) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.8, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.7, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

