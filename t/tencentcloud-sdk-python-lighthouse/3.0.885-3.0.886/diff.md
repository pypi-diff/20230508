# Comparing `tmp/tencentcloud-sdk-python-lighthouse-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-lighthouse-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.885.tar", last modified: Mon May  1 00:44:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.886.tar", last modified: Mon May  8 03:36:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lighthouse-3.0.885.tar` & `tencentcloud-sdk-python-lighthouse-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:44:04.000000 tencentcloud-sdk-python-lighthouse-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      758 2023-05-01 00:44:04.000000 tencentcloud-sdk-python-lighthouse-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:44:04.000000 tencentcloud-sdk-python-lighthouse-3.0.885/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:44:04.000000 tencentcloud-sdk-python-lighthouse-3.0.885/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:44:04.000000 tencentcloud-sdk-python-lighthouse-3.0.885/tencentcloud/lighthouse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:44:04.000000 tencentcloud-sdk-python-lighthouse-3.0.885/tencentcloud/lighthouse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:44:04.000000 tencentcloud-sdk-python-lighthouse-3.0.885/tencentcloud/lighthouse/v20200324/
--rw-r--r--   0 root         (0) root         (0)    24692 2023-05-01 00:44:04.000000 tencentcloud-sdk-python-lighthouse-3.0.885/tencentcloud/lighthouse/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    88751 2023-05-01 00:44:04.000000 tencentcloud-sdk-python-lighthouse-3.0.885/tencentcloud/lighthouse/v20200324/lighthouse_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:44:04.000000 tencentcloud-sdk-python-lighthouse-3.0.885/tencentcloud/lighthouse/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)   230902 2023-05-01 00:44:04.000000 tencentcloud-sdk-python-lighthouse-3.0.885/tencentcloud/lighthouse/v20200324/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:44:04.000000 tencentcloud-sdk-python-lighthouse-3.0.885/tencentcloud_sdk_python_lighthouse.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:44:04.000000 tencentcloud-sdk-python-lighthouse-3.0.885/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-05-01 00:44:04.000000 tencentcloud-sdk-python-lighthouse-3.0.885/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-05-01 00:44:04.000000 tencentcloud-sdk-python-lighthouse-3.0.885/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:44:04.000000 tencentcloud-sdk-python-lighthouse-3.0.885/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-05-01 00:44:04.000000 tencentcloud-sdk-python-lighthouse-3.0.885/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-05-01 00:44:04.000000 tencentcloud-sdk-python-lighthouse-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:44:04.000000 tencentcloud-sdk-python-lighthouse-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/lighthouse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/lighthouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/lighthouse/v20200324/
+-rw-r--r--   0 root         (0) root         (0)    24695 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/lighthouse/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    88751 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/lighthouse/v20200324/lighthouse_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/lighthouse/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   231682 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/lighthouse/v20200324/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud_sdk_python_lighthouse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.885/README.rst` & `tencentcloud-sdk-python-lighthouse-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.885'
+__version__ = '3.0.886'
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.885/tencentcloud/lighthouse/v20200324/errorcodes.py` & `tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/lighthouse/v20200324/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,15 +334,15 @@
 
 # 非法的可用区。
 INVALIDPARAMETERVALUE_ZONEINVALID = 'InvalidParameterValue.ZoneInvalid'
 
 # 超过配额限制。
 LIMITEXCEEDED = 'LimitExceeded'
 
-# 实例挂载数据盘配额不足，无法挂载磁盘。
+# 实例挂载数据盘配额不足，无法挂载云硬盘。
 LIMITEXCEEDED_ATTACHDATADISKQUOTALIMITEXCEEDED = 'LimitExceeded.AttachDataDiskQuotaLimitExceeded'
 
 # 配额不足，当前自定义镜像配额不允许创建新的自定义镜像。
 LIMITEXCEEDED_BLUEPRINTQUOTALIMITEXCEEDED = 'LimitExceeded.BlueprintQuotaLimitExceeded'
 
 # 超过磁盘备份点配额限制。
 LIMITEXCEEDED_DISKBACKUPQUOTALIMITEXCEEDED = 'LimitExceeded.DiskBackupQuotaLimitExceeded'
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.885/tencentcloud/lighthouse/v20200324/lighthouse_client.py` & `tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/lighthouse/v20200324/lighthouse_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.885/tencentcloud/lighthouse/v20200324/models.py` & `tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/lighthouse/v20200324/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,19 @@
 
     def __init__(self):
         r"""
         :param DiskIds: 云硬盘ID列表。
         :type DiskIds: list of str
         :param InstanceId: 实例ID。
         :type InstanceId: str
-        :param RenewFlag: 续费标识。
+        :param RenewFlag: 自动续费标识。取值范围：
+
+NOTIFY_AND_AUTO_RENEW：通知过期且自动续费。 NOTIFY_AND_MANUAL_RENEW：通知过期不自动续费，用户需要手动续费。 DISABLE_NOTIFY_AND_AUTO_RENEW：不自动续费，且不通知。
+
+默认取值：NOTIFY_AND_MANUAL_RENEW。若该参数指定为NOTIFY_AND_AUTO_RENEW，在账户余额充足的情况下，云盘到期后将按月自动续费。
         :type RenewFlag: str
         """
         self.DiskIds = None
         self.InstanceId = None
         self.RenewFlag = None
 
 
@@ -3720,15 +3724,21 @@
 
     """
 
     def __init__(self):
         r"""
         :param Period: 新购周期。
         :type Period: int
-        :param RenewFlag: 续费标识。
+        :param RenewFlag: 自动续费标识。取值范围：
+
+NOTIFY_AND_AUTO_RENEW：通知过期且自动续费。
+NOTIFY_AND_MANUAL_RENEW：通知过期不自动续费，用户需要手动续费。
+DISABLE_NOTIFY_AND_AUTO_RENEW：不自动续费，且不通知。
+
+默认取值：NOTIFY_AND_MANUAL_RENEW。若该参数指定为NOTIFY_AND_AUTO_RENEW，在账户余额充足的情况下，云盘到期后将按月自动续费。
         :type RenewFlag: str
         :param TimeUnit: 新购单位. 默认值: "m"。
         :type TimeUnit: str
         """
         self.Period = None
         self.RenewFlag = None
         self.TimeUnit = None
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.885/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.885/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.886/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.885/setup.py` & `tencentcloud-sdk-python-lighthouse-3.0.886/setup.py`

 * *Files identical despite different names*

