# Comparing `tmp/tencentcloud-sdk-python-waf-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-waf-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.885.tar", last modified: Mon May  1 00:59:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.886.tar", last modified: Mon May  8 04:22:15 2023, max compression
```

## Comparing `tencentcloud-sdk-python-waf-3.0.885.tar` & `tencentcloud-sdk-python-waf-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:59:25.000000 tencentcloud-sdk-python-waf-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-01 00:59:25.000000 tencentcloud-sdk-python-waf-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:59:25.000000 tencentcloud-sdk-python-waf-3.0.885/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:59:25.000000 tencentcloud-sdk-python-waf-3.0.885/tencentcloud/waf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:59:25.000000 tencentcloud-sdk-python-waf-3.0.885/tencentcloud/waf/v20180125/
--rw-r--r--   0 root         (0) root         (0)    46564 2023-05-01 00:59:25.000000 tencentcloud-sdk-python-waf-3.0.885/tencentcloud/waf/v20180125/waf_client.py
--rw-r--r--   0 root         (0) root         (0)     2419 2023-05-01 00:59:25.000000 tencentcloud-sdk-python-waf-3.0.885/tencentcloud/waf/v20180125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:59:25.000000 tencentcloud-sdk-python-waf-3.0.885/tencentcloud/waf/v20180125/__init__.py
--rw-r--r--   0 root         (0) root         (0)   180081 2023-05-01 00:59:25.000000 tencentcloud-sdk-python-waf-3.0.885/tencentcloud/waf/v20180125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:59:25.000000 tencentcloud-sdk-python-waf-3.0.885/tencentcloud/waf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:59:25.000000 tencentcloud-sdk-python-waf-3.0.885/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:59:25.000000 tencentcloud-sdk-python-waf-3.0.885/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-01 00:59:25.000000 tencentcloud-sdk-python-waf-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:59:25.000000 tencentcloud-sdk-python-waf-3.0.885/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:59:25.000000 tencentcloud-sdk-python-waf-3.0.885/tencentcloud_sdk_python_waf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:59:25.000000 tencentcloud-sdk-python-waf-3.0.885/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-01 00:59:25.000000 tencentcloud-sdk-python-waf-3.0.885/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:59:25.000000 tencentcloud-sdk-python-waf-3.0.885/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:59:25.000000 tencentcloud-sdk-python-waf-3.0.885/tencentcloud_sdk_python_waf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:22:15.000000 tencentcloud-sdk-python-waf-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-08 04:22:15.000000 tencentcloud-sdk-python-waf-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:22:15.000000 tencentcloud-sdk-python-waf-3.0.886/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:22:15.000000 tencentcloud-sdk-python-waf-3.0.886/tencentcloud/waf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:22:15.000000 tencentcloud-sdk-python-waf-3.0.886/tencentcloud/waf/v20180125/
+-rw-r--r--   0 root         (0) root         (0)    46563 2023-05-08 04:22:15.000000 tencentcloud-sdk-python-waf-3.0.886/tencentcloud/waf/v20180125/waf_client.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-05-08 04:22:15.000000 tencentcloud-sdk-python-waf-3.0.886/tencentcloud/waf/v20180125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:22:15.000000 tencentcloud-sdk-python-waf-3.0.886/tencentcloud/waf/v20180125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   180125 2023-05-08 04:22:15.000000 tencentcloud-sdk-python-waf-3.0.886/tencentcloud/waf/v20180125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:22:15.000000 tencentcloud-sdk-python-waf-3.0.886/tencentcloud/waf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 04:22:15.000000 tencentcloud-sdk-python-waf-3.0.886/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 04:22:15.000000 tencentcloud-sdk-python-waf-3.0.886/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-08 04:22:15.000000 tencentcloud-sdk-python-waf-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 04:22:15.000000 tencentcloud-sdk-python-waf-3.0.886/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:22:15.000000 tencentcloud-sdk-python-waf-3.0.886/tencentcloud_sdk_python_waf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 04:22:15.000000 tencentcloud-sdk-python-waf-3.0.886/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-08 04:22:15.000000 tencentcloud-sdk-python-waf-3.0.886/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 04:22:15.000000 tencentcloud-sdk-python-waf-3.0.886/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 04:22:15.000000 tencentcloud-sdk-python-waf-3.0.886/tencentcloud_sdk_python_waf.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-waf-3.0.885/README.rst` & `tencentcloud-sdk-python-waf-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.885/tencentcloud/waf/v20180125/waf_client.py` & `tencentcloud-sdk-python-waf-3.0.886/tencentcloud/waf/v20180125/waf_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,14 @@
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DeleteDomainWhiteRules(self, request):
         """删除域名规则白名单
 
-
         :param request: Request instance for DeleteDomainWhiteRules.
         :type request: :class:`tencentcloud.waf.v20180125.models.DeleteDomainWhiteRulesRequest`
         :rtype: :class:`tencentcloud.waf.v20180125.models.DeleteDomainWhiteRulesResponse`
 
         """
         try:
             params = request._serialize()
```

### Comparing `tencentcloud-sdk-python-waf-3.0.885/tencentcloud/waf/v20180125/errorcodes.py` & `tencentcloud-sdk-python-waf-3.0.886/tencentcloud/waf/v20180125/errorcodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,7 +81,10 @@
 UNAUTHORIZEDOPERATION = 'UnauthorizedOperation'
 
 # 未知参数错误。
 UNKNOWNPARAMETER = 'UnknownParameter'
 
 # 操作不支持。
 UNSUPPORTEDOPERATION = 'UnsupportedOperation'
+
+# InvalidRequest
+UNSUPPORTEDOPERATION_INVALIDREQUEST = 'UnsupportedOperation.InvalidRequest'
```

### Comparing `tencentcloud-sdk-python-waf-3.0.885/tencentcloud/waf/v20180125/models.py` & `tencentcloud-sdk-python-waf-3.0.886/tencentcloud/waf/v20180125/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4383,15 +4383,15 @@
         :type Id: int
         :param Rules: 规则的id列表
         :type Rules: list of int non-negative
         :param Url: 规则匹配路径
         :type Url: str
         :param Function: 规则匹配方法
         :type Function: str
-        :param Status: 规则的开关状态
+        :param Status: 规则的开关状态，0表示关闭开关，1表示打开开关
         :type Status: int
         """
         self.Domain = None
         self.Id = None
         self.Rules = None
         self.Url = None
         self.Function = None
```

### Comparing `tencentcloud-sdk-python-waf-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-waf-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-waf-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.886/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.885/setup.py` & `tencentcloud-sdk-python-waf-3.0.886/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.885/tencentcloud_sdk_python_waf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.886/tencentcloud_sdk_python_waf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

