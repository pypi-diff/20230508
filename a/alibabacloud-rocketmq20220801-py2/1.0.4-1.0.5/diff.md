# Comparing `tmp/alibabacloud_rocketmq20220801_py2-1.0.4.tar.gz` & `tmp/alibabacloud_rocketmq20220801_py2-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_rocketmq20220801_py2-1.0.4.tar", last modified: Wed Feb  8 06:41:51 2023, max compression
+gzip compressed data, was "dist/alibabacloud_rocketmq20220801_py2-1.0.5.tar", last modified: Mon May  8 11:38:24 2023, max compression
```

## Comparing `alibabacloud_rocketmq20220801_py2-1.0.4.tar` & `alibabacloud_rocketmq20220801_py2-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 06:41:51.000000 alibabacloud_rocketmq20220801_py2-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      337 2023-02-08 06:41:50.000000 alibabacloud_rocketmq20220801_py2-1.0.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-02-08 06:41:50.000000 alibabacloud_rocketmq20220801_py2-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-02-08 06:41:50.000000 alibabacloud_rocketmq20220801_py2-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2502 2023-02-08 06:41:51.000000 alibabacloud_rocketmq20220801_py2-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2023-02-08 06:41:50.000000 alibabacloud_rocketmq20220801_py2-1.0.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2023-02-08 06:41:50.000000 alibabacloud_rocketmq20220801_py2-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 06:41:51.000000 alibabacloud_rocketmq20220801_py2-1.0.4/alibabacloud_rocketmq20220801/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-08 06:41:50.000000 alibabacloud_rocketmq20220801_py2-1.0.4/alibabacloud_rocketmq20220801/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23444 2023-02-08 06:41:50.000000 alibabacloud_rocketmq20220801_py2-1.0.4/alibabacloud_rocketmq20220801/client.py
--rw-r--r--   0 root         (0) root         (0)   131730 2023-02-08 06:41:50.000000 alibabacloud_rocketmq20220801_py2-1.0.4/alibabacloud_rocketmq20220801/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 06:41:51.000000 alibabacloud_rocketmq20220801_py2-1.0.4/alibabacloud_rocketmq20220801_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2502 2023-02-08 06:41:51.000000 alibabacloud_rocketmq20220801_py2-1.0.4/alibabacloud_rocketmq20220801_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2023-02-08 06:41:51.000000 alibabacloud_rocketmq20220801_py2-1.0.4/alibabacloud_rocketmq20220801_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-08 06:41:51.000000 alibabacloud_rocketmq20220801_py2-1.0.4/alibabacloud_rocketmq20220801_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-02-08 06:41:51.000000 alibabacloud_rocketmq20220801_py2-1.0.4/alibabacloud_rocketmq20220801_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-02-08 06:41:51.000000 alibabacloud_rocketmq20220801_py2-1.0.4/alibabacloud_rocketmq20220801_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-08 06:41:51.000000 alibabacloud_rocketmq20220801_py2-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2928 2023-02-08 06:41:50.000000 alibabacloud_rocketmq20220801_py2-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:38:24.000000 alibabacloud_rocketmq20220801_py2-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      412 2023-05-08 11:38:23.000000 alibabacloud_rocketmq20220801_py2-1.0.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-08 11:38:23.000000 alibabacloud_rocketmq20220801_py2-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-08 11:38:23.000000 alibabacloud_rocketmq20220801_py2-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-05-08 11:38:24.000000 alibabacloud_rocketmq20220801_py2-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-05-08 11:38:23.000000 alibabacloud_rocketmq20220801_py2-1.0.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-05-08 11:38:23.000000 alibabacloud_rocketmq20220801_py2-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:38:24.000000 alibabacloud_rocketmq20220801_py2-1.0.5/alibabacloud_rocketmq20220801/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-08 11:38:23.000000 alibabacloud_rocketmq20220801_py2-1.0.5/alibabacloud_rocketmq20220801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23444 2023-05-08 11:38:23.000000 alibabacloud_rocketmq20220801_py2-1.0.5/alibabacloud_rocketmq20220801/client.py
+-rw-r--r--   0 root         (0) root         (0)   133926 2023-05-08 11:38:23.000000 alibabacloud_rocketmq20220801_py2-1.0.5/alibabacloud_rocketmq20220801/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:38:24.000000 alibabacloud_rocketmq20220801_py2-1.0.5/alibabacloud_rocketmq20220801_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-05-08 11:38:23.000000 alibabacloud_rocketmq20220801_py2-1.0.5/alibabacloud_rocketmq20220801_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2023-05-08 11:38:23.000000 alibabacloud_rocketmq20220801_py2-1.0.5/alibabacloud_rocketmq20220801_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 11:38:23.000000 alibabacloud_rocketmq20220801_py2-1.0.5/alibabacloud_rocketmq20220801_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-08 11:38:23.000000 alibabacloud_rocketmq20220801_py2-1.0.5/alibabacloud_rocketmq20220801_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-08 11:38:23.000000 alibabacloud_rocketmq20220801_py2-1.0.5/alibabacloud_rocketmq20220801_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-08 11:38:24.000000 alibabacloud_rocketmq20220801_py2-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-05-08 11:38:23.000000 alibabacloud_rocketmq20220801_py2-1.0.5/setup.py
```

### Comparing `alibabacloud_rocketmq20220801_py2-1.0.4/LICENSE` & `alibabacloud_rocketmq20220801_py2-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_rocketmq20220801_py2-1.0.4/PKG-INFO` & `alibabacloud_rocketmq20220801_py2-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_rocketmq20220801_py2
-Version: 1.0.4
+Version: 1.0.5
 Summary: Alibaba Cloud RocketMQ (20220801) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rocketmq20220801_py2-1.0.4/README-CN.md` & `alibabacloud_rocketmq20220801_py2-1.0.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rocketmq20220801_py2-1.0.4/README.md` & `alibabacloud_rocketmq20220801_py2-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rocketmq20220801_py2-1.0.4/alibabacloud_rocketmq20220801/client.py` & `alibabacloud_rocketmq20220801_py2-1.0.5/alibabacloud_rocketmq20220801/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rocketmq20220801_py2-1.0.4/alibabacloud_rocketmq20220801/models.py` & `alibabacloud_rocketmq20220801_py2-1.0.5/alibabacloud_rocketmq20220801/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1427,15 +1427,15 @@
         return self
 
 
 class GetInstanceResponseBodyDataNetworkInfoEndpoints(TeaModel):
     def __init__(self, endpoint_type=None, endpoint_url=None, ip_whitelist=None):
         self.endpoint_type = endpoint_type  # type: str
         self.endpoint_url = endpoint_url  # type: str
-        self.ip_whitelist = ip_whitelist  # type: str
+        self.ip_whitelist = ip_whitelist  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetInstanceResponseBodyDataNetworkInfoEndpoints, self).to_map()
         if _map is not None:
@@ -1618,43 +1618,80 @@
         if m.get('sendReceiveRatio') is not None:
             self.send_receive_ratio = m.get('sendReceiveRatio')
         if m.get('supportAutoScaling') is not None:
             self.support_auto_scaling = m.get('supportAutoScaling')
         return self
 
 
+class GetInstanceResponseBodyDataSoftware(TeaModel):
+    def __init__(self, maintain_time=None, software_version=None, upgrade_method=None):
+        self.maintain_time = maintain_time  # type: str
+        self.software_version = software_version  # type: str
+        self.upgrade_method = upgrade_method  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetInstanceResponseBodyDataSoftware, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, account_info=None, acl_info=None, bid=None, commodity_code=None, create_time=None,
-                 expire_time=None, ext_config=None, instance_id=None, instance_name=None, instance_quotas=None,
-                 network_info=None, payment_type=None, product_info=None, region_id=None, release_time=None, remark=None,
-                 resource_group_id=None, series_code=None, service_code=None, start_time=None, status=None, sub_series_code=None,
-                 update_time=None, user_id=None):
+                 expire_time=None, ext_config=None, group_count=None, instance_id=None, instance_name=None,
+                 instance_quotas=None, network_info=None, payment_type=None, product_info=None, region_id=None, release_time=None,
+                 remark=None, resource_group_id=None, series_code=None, service_code=None, software=None, start_time=None,
+                 status=None, sub_series_code=None, topic_count=None, update_time=None, user_id=None):
         self.account_info = account_info  # type: GetInstanceResponseBodyDataAccountInfo
         self.acl_info = acl_info  # type: GetInstanceResponseBodyDataAclInfo
         # BID
         self.bid = bid  # type: str
         self.commodity_code = commodity_code  # type: str
         self.create_time = create_time  # type: str
         self.expire_time = expire_time  # type: str
         self.ext_config = ext_config  # type: GetInstanceResponseBodyDataExtConfig
+        self.group_count = group_count  # type: long
         self.instance_id = instance_id  # type: str
         self.instance_name = instance_name  # type: str
         self.instance_quotas = instance_quotas  # type: list[GetInstanceResponseBodyDataInstanceQuotas]
         self.network_info = network_info  # type: GetInstanceResponseBodyDataNetworkInfo
         self.payment_type = payment_type  # type: str
         self.product_info = product_info  # type: GetInstanceResponseBodyDataProductInfo
         self.region_id = region_id  # type: str
         self.release_time = release_time  # type: str
         self.remark = remark  # type: str
         self.resource_group_id = resource_group_id  # type: str
         self.series_code = series_code  # type: str
         self.service_code = service_code  # type: str
+        self.software = software  # type: GetInstanceResponseBodyDataSoftware
         self.start_time = start_time  # type: str
         self.status = status  # type: str
         self.sub_series_code = sub_series_code  # type: str
+        self.topic_count = topic_count  # type: long
         self.update_time = update_time  # type: str
         self.user_id = user_id  # type: str
 
     def validate(self):
         if self.account_info:
             self.account_info.validate()
         if self.acl_info:
@@ -1665,14 +1702,16 @@
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
         _map = super(GetInstanceResponseBodyData, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -1686,14 +1725,16 @@
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
@@ -1712,20 +1753,24 @@
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
 
     def from_map(self, m=None):
@@ -1743,14 +1788,16 @@
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
@@ -1772,20 +1819,25 @@
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

### Comparing `alibabacloud_rocketmq20220801_py2-1.0.4/alibabacloud_rocketmq20220801_py2.egg-info/PKG-INFO` & `alibabacloud_rocketmq20220801_py2-1.0.5/alibabacloud_rocketmq20220801_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-rocketmq20220801-py2
-Version: 1.0.4
+Version: 1.0.5
 Summary: Alibaba Cloud RocketMQ (20220801) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rocketmq20220801_py2-1.0.4/setup.py` & `alibabacloud_rocketmq20220801_py2-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_rocketmq20220801_py2.
 
-Created on 08/02/2023
+Created on 08/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_rocketmq20220801"
 NAME = "alibabacloud_rocketmq20220801_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud RocketMQ (20220801) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.7, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
```

