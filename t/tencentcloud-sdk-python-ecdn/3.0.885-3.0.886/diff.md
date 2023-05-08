# Comparing `tmp/tencentcloud-sdk-python-ecdn-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-ecdn-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ecdn-3.0.885.tar", last modified: Mon May  1 00:36:14 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ecdn-3.0.886.tar", last modified: Mon May  8 03:14:22 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ecdn-3.0.885.tar` & `tencentcloud-sdk-python-ecdn-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:36:14.000000 tencentcloud-sdk-python-ecdn-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-01 00:36:14.000000 tencentcloud-sdk-python-ecdn-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:36:14.000000 tencentcloud-sdk-python-ecdn-3.0.885/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:36:14.000000 tencentcloud-sdk-python-ecdn-3.0.885/tencentcloud/ecdn/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:36:14.000000 tencentcloud-sdk-python-ecdn-3.0.885/tencentcloud/ecdn/v20191012/
--rw-r--r--   0 root         (0) root         (0)    20189 2023-05-01 00:36:14.000000 tencentcloud-sdk-python-ecdn-3.0.885/tencentcloud/ecdn/v20191012/ecdn_client.py
--rw-r--r--   0 root         (0) root         (0)     9084 2023-05-01 00:36:14.000000 tencentcloud-sdk-python-ecdn-3.0.885/tencentcloud/ecdn/v20191012/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:36:14.000000 tencentcloud-sdk-python-ecdn-3.0.885/tencentcloud/ecdn/v20191012/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80852 2023-05-01 00:36:14.000000 tencentcloud-sdk-python-ecdn-3.0.885/tencentcloud/ecdn/v20191012/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:36:14.000000 tencentcloud-sdk-python-ecdn-3.0.885/tencentcloud/ecdn/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:36:14.000000 tencentcloud-sdk-python-ecdn-3.0.885/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-01 00:36:14.000000 tencentcloud-sdk-python-ecdn-3.0.885/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-01 00:36:14.000000 tencentcloud-sdk-python-ecdn-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:36:14.000000 tencentcloud-sdk-python-ecdn-3.0.885/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:36:14.000000 tencentcloud-sdk-python-ecdn-3.0.885/tencentcloud_sdk_python_ecdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:36:14.000000 tencentcloud-sdk-python-ecdn-3.0.885/tencentcloud_sdk_python_ecdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-01 00:36:14.000000 tencentcloud-sdk-python-ecdn-3.0.885/tencentcloud_sdk_python_ecdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-01 00:36:14.000000 tencentcloud-sdk-python-ecdn-3.0.885/tencentcloud_sdk_python_ecdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:36:14.000000 tencentcloud-sdk-python-ecdn-3.0.885/tencentcloud_sdk_python_ecdn.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:14:22.000000 tencentcloud-sdk-python-ecdn-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-08 03:14:21.000000 tencentcloud-sdk-python-ecdn-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:14:22.000000 tencentcloud-sdk-python-ecdn-3.0.886/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:14:22.000000 tencentcloud-sdk-python-ecdn-3.0.886/tencentcloud/ecdn/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:14:22.000000 tencentcloud-sdk-python-ecdn-3.0.886/tencentcloud/ecdn/v20191012/
+-rw-r--r--   0 root         (0) root         (0)    20260 2023-05-08 03:14:21.000000 tencentcloud-sdk-python-ecdn-3.0.886/tencentcloud/ecdn/v20191012/ecdn_client.py
+-rw-r--r--   0 root         (0) root         (0)     9084 2023-05-08 03:14:21.000000 tencentcloud-sdk-python-ecdn-3.0.886/tencentcloud/ecdn/v20191012/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:14:21.000000 tencentcloud-sdk-python-ecdn-3.0.886/tencentcloud/ecdn/v20191012/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80852 2023-05-08 03:14:21.000000 tencentcloud-sdk-python-ecdn-3.0.886/tencentcloud/ecdn/v20191012/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:14:21.000000 tencentcloud-sdk-python-ecdn-3.0.886/tencentcloud/ecdn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 03:14:21.000000 tencentcloud-sdk-python-ecdn-3.0.886/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-08 03:14:22.000000 tencentcloud-sdk-python-ecdn-3.0.886/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-08 03:14:21.000000 tencentcloud-sdk-python-ecdn-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 03:14:22.000000 tencentcloud-sdk-python-ecdn-3.0.886/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:14:22.000000 tencentcloud-sdk-python-ecdn-3.0.886/tencentcloud_sdk_python_ecdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 03:14:22.000000 tencentcloud-sdk-python-ecdn-3.0.886/tencentcloud_sdk_python_ecdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-08 03:14:22.000000 tencentcloud-sdk-python-ecdn-3.0.886/tencentcloud_sdk_python_ecdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-08 03:14:22.000000 tencentcloud-sdk-python-ecdn-3.0.886/tencentcloud_sdk_python_ecdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 03:14:22.000000 tencentcloud-sdk-python-ecdn-3.0.886/tencentcloud_sdk_python_ecdn.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-ecdn-3.0.885/README.rst` & `tencentcloud-sdk-python-ecdn-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecdn-3.0.885/tencentcloud/ecdn/v20191012/ecdn_client.py` & `tencentcloud-sdk-python-ecdn-3.0.886/tencentcloud/ecdn/v20191012/ecdn_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,15 +258,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribePurgeQuota(self, request):
-        """查询刷新接口的用量配额。
+        """ECDN融合CDN后，接口都用CDN的，此接口已经废弃
+
+        查询刷新接口的用量配额。
 
         >?  若您的业务已迁移至 CDN 控制台，请参考<a href="https://cloud.tencent.com/document/api/228/41956"> CDN 接口文档</a>，使用  CDN 相关API 进行操作。
 
         :param request: Request instance for DescribePurgeQuota.
         :type request: :class:`tencentcloud.ecdn.v20191012.models.DescribePurgeQuotaRequest`
         :rtype: :class:`tencentcloud.ecdn.v20191012.models.DescribePurgeQuotaResponse`
```

### Comparing `tencentcloud-sdk-python-ecdn-3.0.885/tencentcloud/ecdn/v20191012/errorcodes.py` & `tencentcloud-sdk-python-ecdn-3.0.886/tencentcloud/ecdn/v20191012/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecdn-3.0.885/tencentcloud/ecdn/v20191012/models.py` & `tencentcloud-sdk-python-ecdn-3.0.886/tencentcloud/ecdn/v20191012/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecdn-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ecdn-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ecdn-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-ecdn-3.0.886/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ecdn
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Ecdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ecdn-3.0.885/setup.py` & `tencentcloud-sdk-python-ecdn-3.0.886/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecdn-3.0.885/tencentcloud_sdk_python_ecdn.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ecdn-3.0.886/tencentcloud_sdk_python_ecdn.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ecdn
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Ecdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

