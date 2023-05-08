# Comparing `tmp/tencentcloud-sdk-python-tsf-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-tsf-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tsf-3.0.885.tar", last modified: Mon May  1 00:58:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tsf-3.0.886.tar", last modified: Mon May  8 04:21:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tsf-3.0.885.tar` & `tencentcloud-sdk-python-tsf-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:58:18.000000 tencentcloud-sdk-python-tsf-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-01 00:58:18.000000 tencentcloud-sdk-python-tsf-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:58:18.000000 tencentcloud-sdk-python-tsf-3.0.885/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:58:18.000000 tencentcloud-sdk-python-tsf-3.0.885/tencentcloud/tsf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:58:18.000000 tencentcloud-sdk-python-tsf-3.0.885/tencentcloud/tsf/v20180326/
--rw-r--r--   0 root         (0) root         (0)    49509 2023-05-01 00:58:18.000000 tencentcloud-sdk-python-tsf-3.0.885/tencentcloud/tsf/v20180326/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   193599 2023-05-01 00:58:18.000000 tencentcloud-sdk-python-tsf-3.0.885/tencentcloud/tsf/v20180326/tsf_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:58:18.000000 tencentcloud-sdk-python-tsf-3.0.885/tencentcloud/tsf/v20180326/__init__.py
--rw-r--r--   0 root         (0) root         (0)   798817 2023-05-01 00:58:18.000000 tencentcloud-sdk-python-tsf-3.0.885/tencentcloud/tsf/v20180326/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:58:18.000000 tencentcloud-sdk-python-tsf-3.0.885/tencentcloud/tsf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:58:18.000000 tencentcloud-sdk-python-tsf-3.0.885/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:58:18.000000 tencentcloud-sdk-python-tsf-3.0.885/tencentcloud_sdk_python_tsf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:58:18.000000 tencentcloud-sdk-python-tsf-3.0.885/tencentcloud_sdk_python_tsf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-01 00:58:18.000000 tencentcloud-sdk-python-tsf-3.0.885/tencentcloud_sdk_python_tsf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:58:18.000000 tencentcloud-sdk-python-tsf-3.0.885/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:58:18.000000 tencentcloud-sdk-python-tsf-3.0.885/tencentcloud_sdk_python_tsf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:58:18.000000 tencentcloud-sdk-python-tsf-3.0.885/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-01 00:58:18.000000 tencentcloud-sdk-python-tsf-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:58:18.000000 tencentcloud-sdk-python-tsf-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:21:07.000000 tencentcloud-sdk-python-tsf-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-08 04:21:07.000000 tencentcloud-sdk-python-tsf-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:21:07.000000 tencentcloud-sdk-python-tsf-3.0.886/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:21:07.000000 tencentcloud-sdk-python-tsf-3.0.886/tencentcloud/tsf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:21:07.000000 tencentcloud-sdk-python-tsf-3.0.886/tencentcloud/tsf/v20180326/
+-rw-r--r--   0 root         (0) root         (0)    49713 2023-05-08 04:21:07.000000 tencentcloud-sdk-python-tsf-3.0.886/tencentcloud/tsf/v20180326/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   193599 2023-05-08 04:21:07.000000 tencentcloud-sdk-python-tsf-3.0.886/tencentcloud/tsf/v20180326/tsf_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:21:07.000000 tencentcloud-sdk-python-tsf-3.0.886/tencentcloud/tsf/v20180326/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   798817 2023-05-08 04:21:07.000000 tencentcloud-sdk-python-tsf-3.0.886/tencentcloud/tsf/v20180326/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:21:07.000000 tencentcloud-sdk-python-tsf-3.0.886/tencentcloud/tsf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 04:21:07.000000 tencentcloud-sdk-python-tsf-3.0.886/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:21:07.000000 tencentcloud-sdk-python-tsf-3.0.886/tencentcloud_sdk_python_tsf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 04:21:07.000000 tencentcloud-sdk-python-tsf-3.0.886/tencentcloud_sdk_python_tsf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-08 04:21:07.000000 tencentcloud-sdk-python-tsf-3.0.886/tencentcloud_sdk_python_tsf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 04:21:07.000000 tencentcloud-sdk-python-tsf-3.0.886/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 04:21:07.000000 tencentcloud-sdk-python-tsf-3.0.886/tencentcloud_sdk_python_tsf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 04:21:07.000000 tencentcloud-sdk-python-tsf-3.0.886/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-08 04:21:07.000000 tencentcloud-sdk-python-tsf-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 04:21:07.000000 tencentcloud-sdk-python-tsf-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.885/README.rst` & `tencentcloud-sdk-python-tsf-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.885/tencentcloud/tsf/v20180326/errorcodes.py` & `tencentcloud-sdk-python-tsf-3.0.886/tencentcloud/tsf/v20180326/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -925,14 +925,17 @@
 
 # 服务不存在或权限不足。
 INVALIDPARAMETERVALUE_SERVICENOTEXISTSORPERMISSIONDENIED = 'InvalidParameterValue.ServiceNotExistsOrPermissionDenied'
 
 # 无效请求参数。
 INVALIDPARAMETERVALUE_TASKPARAMETERINVALID = 'InvalidParameterValue.TaskParameterInvalid'
 
+# TSF应用性能管理业务日志搜索解析时间格式错误。
+INVALIDPARAMETERVALUE_TSFAPMBUSILOGSEARCHPARSERSPDATEFORMATERROR = 'InvalidParameterValue.TsfApmBusiLogSearchParseRspDateFormatError'
+
 # 仅有停止状态下的部署组才可以不启动。
 INVALIDPARAMETERVALUE_WRONGDONTSTARTVALUE = 'InvalidParameterValue.WrongDontStartValue'
 
 # 命名空间数达到上限。
 LIMITEXCEEDED_ERRNAMESPACEMAXLIMIT = 'LimitExceeded.ErrNamespaceMaxLimit'
 
 # 仓库达到上限。
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.885/tencentcloud/tsf/v20180326/tsf_client.py` & `tencentcloud-sdk-python-tsf-3.0.886/tencentcloud/tsf/v20180326/tsf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.885/tencentcloud/tsf/v20180326/models.py` & `tencentcloud-sdk-python-tsf-3.0.886/tencentcloud/tsf/v20180326/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tsf-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tsf-3.0.885/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tsf-3.0.886/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsf
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Tsf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-tsf-3.0.886/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsf
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Tsf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.885/setup.py` & `tencentcloud-sdk-python-tsf-3.0.886/setup.py`

 * *Files identical despite different names*

