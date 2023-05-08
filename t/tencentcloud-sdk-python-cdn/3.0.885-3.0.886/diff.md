# Comparing `tmp/tencentcloud-sdk-python-cdn-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-cdn-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.885.tar", last modified: Mon May  1 00:31:09 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.886.tar", last modified: Mon May  8 02:58:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdn-3.0.885.tar` & `tencentcloud-sdk-python-cdn-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:31:09.000000 tencentcloud-sdk-python-cdn-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-01 00:31:09.000000 tencentcloud-sdk-python-cdn-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:31:09.000000 tencentcloud-sdk-python-cdn-3.0.885/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:31:09.000000 tencentcloud-sdk-python-cdn-3.0.885/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:31:09.000000 tencentcloud-sdk-python-cdn-3.0.885/tencentcloud/cdn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:31:09.000000 tencentcloud-sdk-python-cdn-3.0.885/tencentcloud/cdn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:31:09.000000 tencentcloud-sdk-python-cdn-3.0.885/tencentcloud/cdn/v20180606/
--rw-r--r--   0 root         (0) root         (0)    21844 2023-05-01 00:31:09.000000 tencentcloud-sdk-python-cdn-3.0.885/tencentcloud/cdn/v20180606/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    80657 2023-05-01 00:31:09.000000 tencentcloud-sdk-python-cdn-3.0.885/tencentcloud/cdn/v20180606/cdn_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:31:09.000000 tencentcloud-sdk-python-cdn-3.0.885/tencentcloud/cdn/v20180606/__init__.py
--rw-r--r--   0 root         (0) root         (0)   568491 2023-05-01 00:31:09.000000 tencentcloud-sdk-python-cdn-3.0.885/tencentcloud/cdn/v20180606/models.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:31:09.000000 tencentcloud-sdk-python-cdn-3.0.885/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:31:09.000000 tencentcloud-sdk-python-cdn-3.0.885/tencentcloud_sdk_python_cdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:31:09.000000 tencentcloud-sdk-python-cdn-3.0.885/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-01 00:31:09.000000 tencentcloud-sdk-python-cdn-3.0.885/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:31:09.000000 tencentcloud-sdk-python-cdn-3.0.885/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:31:09.000000 tencentcloud-sdk-python-cdn-3.0.885/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-01 00:31:09.000000 tencentcloud-sdk-python-cdn-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:31:09.000000 tencentcloud-sdk-python-cdn-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:58:07.000000 tencentcloud-sdk-python-cdn-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-08 02:58:07.000000 tencentcloud-sdk-python-cdn-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:58:07.000000 tencentcloud-sdk-python-cdn-3.0.886/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 02:58:07.000000 tencentcloud-sdk-python-cdn-3.0.886/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:58:07.000000 tencentcloud-sdk-python-cdn-3.0.886/tencentcloud/cdn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 02:58:07.000000 tencentcloud-sdk-python-cdn-3.0.886/tencentcloud/cdn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:58:07.000000 tencentcloud-sdk-python-cdn-3.0.886/tencentcloud/cdn/v20180606/
+-rw-r--r--   0 root         (0) root         (0)    21844 2023-05-08 02:58:07.000000 tencentcloud-sdk-python-cdn-3.0.886/tencentcloud/cdn/v20180606/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    80657 2023-05-08 02:58:07.000000 tencentcloud-sdk-python-cdn-3.0.886/tencentcloud/cdn/v20180606/cdn_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 02:58:07.000000 tencentcloud-sdk-python-cdn-3.0.886/tencentcloud/cdn/v20180606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   568745 2023-05-08 02:58:07.000000 tencentcloud-sdk-python-cdn-3.0.886/tencentcloud/cdn/v20180606/models.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 02:58:07.000000 tencentcloud-sdk-python-cdn-3.0.886/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:58:07.000000 tencentcloud-sdk-python-cdn-3.0.886/tencentcloud_sdk_python_cdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 02:58:07.000000 tencentcloud-sdk-python-cdn-3.0.886/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-08 02:58:07.000000 tencentcloud-sdk-python-cdn-3.0.886/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 02:58:07.000000 tencentcloud-sdk-python-cdn-3.0.886/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 02:58:07.000000 tencentcloud-sdk-python-cdn-3.0.886/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-08 02:58:07.000000 tencentcloud-sdk-python-cdn-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 02:58:07.000000 tencentcloud-sdk-python-cdn-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.885/README.rst` & `tencentcloud-sdk-python-cdn-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdn-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdn-3.0.885/tencentcloud/cdn/v20180606/errorcodes.py` & `tencentcloud-sdk-python-cdn-3.0.886/tencentcloud/cdn/v20180606/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.885/tencentcloud/cdn/v20180606/cdn_client.py` & `tencentcloud-sdk-python-cdn-3.0.886/tencentcloud/cdn/v20180606/cdn_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.885/tencentcloud/cdn/v20180606/models.py` & `tencentcloud-sdk-python-cdn-3.0.886/tencentcloud/cdn/v20180606/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8861,14 +8861,17 @@
         :type ExtensionAvailable: bool
         :param ExtensionMode: HTTPS请求包当前续订模式
 0：未续订
 1：到期续订
 2：用完续订
 3：到期或用完续订
         :type ExtensionMode: int
+        :param AutoExtension: HTTPS请求包是否自动续订
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AutoExtension: bool
         """
         self.Id = None
         self.Type = None
         self.Size = None
         self.SizeUsed = None
         self.Status = None
         self.CreateTime = None
@@ -8880,14 +8883,15 @@
         self.ConfigId = None
         self.TrueEnableTime = None
         self.TrueExpireTime = None
         self.Area = None
         self.ContractExtension = None
         self.ExtensionAvailable = None
         self.ExtensionMode = None
+        self.AutoExtension = None
 
 
     def _deserialize(self, params):
         self.Id = params.get("Id")
         self.Type = params.get("Type")
         self.Size = params.get("Size")
         self.SizeUsed = params.get("SizeUsed")
@@ -8901,14 +8905,15 @@
         self.ConfigId = params.get("ConfigId")
         self.TrueEnableTime = params.get("TrueEnableTime")
         self.TrueExpireTime = params.get("TrueExpireTime")
         self.Area = params.get("Area")
         self.ContractExtension = params.get("ContractExtension")
         self.ExtensionAvailable = params.get("ExtensionAvailable")
         self.ExtensionMode = params.get("ExtensionMode")
+        self.AutoExtension = params.get("AutoExtension")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.886/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.885/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.886/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.885/setup.py` & `tencentcloud-sdk-python-cdn-3.0.886/setup.py`

 * *Files identical despite different names*

