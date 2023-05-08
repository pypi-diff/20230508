# Comparing `tmp/tencentcloud-sdk-python-teo-3.0.884.tar.gz` & `tmp/tencentcloud-sdk-python-teo-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.884.tar", last modified: Fri Apr 28 02:41:14 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.886.tar", last modified: Mon May  8 04:10:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-teo-3.0.884.tar` & `tencentcloud-sdk-python-teo-3.0.886.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220106/
--rw-r--r--   0 root         (0) root         (0)     2192 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220106/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220106/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24724 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220106/models.py
--rw-r--r--   0 root         (0) root         (0)     5379 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220106/teo_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220901/
--rw-r--r--   0 root         (0) root         (0)    21826 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220901/__init__.py
--rw-r--r--   0 root         (0) root         (0)   512265 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220901/models.py
--rw-r--r--   0 root         (0) root         (0)    84601 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220901/teo_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud_sdk_python_teo.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud_sdk_python_teo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/tencentcloud/teo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/tencentcloud/teo/v20220106/
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/tencentcloud/teo/v20220106/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/tencentcloud/teo/v20220106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24724 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/tencentcloud/teo/v20220106/models.py
+-rw-r--r--   0 root         (0) root         (0)     5379 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/tencentcloud/teo/v20220106/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/tencentcloud/teo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/tencentcloud/teo/v20220901/
+-rw-r--r--   0 root         (0) root         (0)    21992 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/tencentcloud/teo/v20220901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/tencentcloud/teo/v20220901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   512734 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/tencentcloud/teo/v20220901/models.py
+-rw-r--r--   0 root         (0) root         (0)    84601 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/tencentcloud/teo/v20220901/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/tencentcloud_sdk_python_teo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/tencentcloud_sdk_python_teo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 04:10:46.000000 tencentcloud-sdk-python-teo-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-teo-3.0.884/README.rst` & `tencentcloud-sdk-python-teo-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220106/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.886/tencentcloud/teo/v20220106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220106/models.py` & `tencentcloud-sdk-python-teo-3.0.886/tencentcloud/teo/v20220106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220106/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.886/tencentcloud/teo/v20220106/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220901/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.886/tencentcloud/teo/v20220901/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,14 +430,17 @@
 
 # 单位时间内接口请求频率达到限制。
 LIMITEXCEEDED_RATELIMITEXCEEDED = 'LimitExceeded.RateLimitExceeded'
 
 # 操作被拒绝。
 OPERATIONDENIED = 'OperationDenied'
 
+# 请联系商务开启「中国大陆网络优化(国际加速)」功能。
+OPERATIONDENIED_ACCELERATEMAINLANDDISABLE = 'OperationDenied.AccelerateMainlandDisable'
+
 # 有域名在共享cname组内，不可切换接入类型。
 OPERATIONDENIED_DOMAININSHARECNAMEGROUP = 'OperationDenied.DomainInShareCnameGroup'
 
 # 域名被封禁，暂时无法操作。
 OPERATIONDENIED_DOMAINISBLOCKED = 'OperationDenied.DomainIsBlocked'
 
 # 域名尚未备案。
```

### Comparing `tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220901/models.py` & `tencentcloud-sdk-python-teo-3.0.886/tencentcloud/teo/v20220901/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -13529,14 +13529,17 @@
         :type ClientIpCountry: :class:`tencentcloud.teo.v20220901.models.ClientIpCountry`
         :param Grpc: Grpc协议支持配置。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Grpc: :class:`tencentcloud.teo.v20220901.models.Grpc`
         :param ImageOptimize: 图片优化相关配置。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ImageOptimize: :class:`tencentcloud.teo.v20220901.models.ImageOptimize`
+        :param AccelerateMainland: 中国大陆加速优化配置。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AccelerateMainland: :class:`tencentcloud.teo.v20220901.models.AccelerateMainland`
         """
         self.ZoneName = None
         self.Area = None
         self.CacheKey = None
         self.Quic = None
         self.PostMaxSize = None
         self.Compression = None
@@ -13551,14 +13554,15 @@
         self.ClientIpHeader = None
         self.CachePrefresh = None
         self.Ipv6 = None
         self.Https = None
         self.ClientIpCountry = None
         self.Grpc = None
         self.ImageOptimize = None
+        self.AccelerateMainland = None
 
 
     def _deserialize(self, params):
         self.ZoneName = params.get("ZoneName")
         self.Area = params.get("Area")
         if params.get("CacheKey") is not None:
             self.CacheKey = CacheKey()
@@ -13613,14 +13617,17 @@
             self.ClientIpCountry._deserialize(params.get("ClientIpCountry"))
         if params.get("Grpc") is not None:
             self.Grpc = Grpc()
             self.Grpc._deserialize(params.get("Grpc"))
         if params.get("ImageOptimize") is not None:
             self.ImageOptimize = ImageOptimize()
             self.ImageOptimize._deserialize(params.get("ImageOptimize"))
+        if params.get("AccelerateMainland") is not None:
+            self.AccelerateMainland = AccelerateMainland()
+            self.AccelerateMainland._deserialize(params.get("AccelerateMainland"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220901/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.886/tencentcloud/teo/v20220901/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.884/tencentcloud/__init__.py` & `tencentcloud-sdk-python-teo-3.0.886/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.884'
+__version__ = '3.0.886'
```

### Comparing `tencentcloud-sdk-python-teo-3.0.884/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.886/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.884
+Version: 3.0.886
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.884/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-teo-3.0.886/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.884/tencentcloud_sdk_python_teo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.886/tencentcloud_sdk_python_teo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.884
+Version: 3.0.886
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.884/setup.py` & `tencentcloud-sdk-python-teo-3.0.886/setup.py`

 * *Files identical despite different names*

