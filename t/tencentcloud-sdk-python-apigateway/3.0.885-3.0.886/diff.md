# Comparing `tmp/tencentcloud-sdk-python-apigateway-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-apigateway-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-apigateway-3.0.885.tar", last modified: Mon May  1 00:24:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-apigateway-3.0.886.tar", last modified: Mon May  8 02:44:05 2023, max compression
```

## Comparing `tencentcloud-sdk-python-apigateway-3.0.885.tar` & `tencentcloud-sdk-python-apigateway-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:24:22.000000 tencentcloud-sdk-python-apigateway-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      758 2023-05-01 00:24:22.000000 tencentcloud-sdk-python-apigateway-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:24:22.000000 tencentcloud-sdk-python-apigateway-3.0.885/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:24:22.000000 tencentcloud-sdk-python-apigateway-3.0.885/tencentcloud/apigateway/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:24:22.000000 tencentcloud-sdk-python-apigateway-3.0.885/tencentcloud/apigateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:24:22.000000 tencentcloud-sdk-python-apigateway-3.0.885/tencentcloud/apigateway/v20180808/
--rw-r--r--   0 root         (0) root         (0)    95979 2023-05-01 00:24:22.000000 tencentcloud-sdk-python-apigateway-3.0.885/tencentcloud/apigateway/v20180808/apigateway_client.py
--rw-r--r--   0 root         (0) root         (0)    20869 2023-05-01 00:24:22.000000 tencentcloud-sdk-python-apigateway-3.0.885/tencentcloud/apigateway/v20180808/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:24:22.000000 tencentcloud-sdk-python-apigateway-3.0.885/tencentcloud/apigateway/v20180808/__init__.py
--rw-r--r--   0 root         (0) root         (0)   394892 2023-05-01 00:24:22.000000 tencentcloud-sdk-python-apigateway-3.0.885/tencentcloud/apigateway/v20180808/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:24:22.000000 tencentcloud-sdk-python-apigateway-3.0.885/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:24:22.000000 tencentcloud-sdk-python-apigateway-3.0.885/tencentcloud_sdk_python_apigateway.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:24:22.000000 tencentcloud-sdk-python-apigateway-3.0.885/tencentcloud_sdk_python_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-05-01 00:24:22.000000 tencentcloud-sdk-python-apigateway-3.0.885/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-05-01 00:24:22.000000 tencentcloud-sdk-python-apigateway-3.0.885/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:24:22.000000 tencentcloud-sdk-python-apigateway-3.0.885/tencentcloud_sdk_python_apigateway.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-05-01 00:24:22.000000 tencentcloud-sdk-python-apigateway-3.0.885/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-05-01 00:24:22.000000 tencentcloud-sdk-python-apigateway-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:24:22.000000 tencentcloud-sdk-python-apigateway-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:44:05.000000 tencentcloud-sdk-python-apigateway-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-05-08 02:44:05.000000 tencentcloud-sdk-python-apigateway-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:44:05.000000 tencentcloud-sdk-python-apigateway-3.0.886/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:44:05.000000 tencentcloud-sdk-python-apigateway-3.0.886/tencentcloud/apigateway/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 02:44:05.000000 tencentcloud-sdk-python-apigateway-3.0.886/tencentcloud/apigateway/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:44:05.000000 tencentcloud-sdk-python-apigateway-3.0.886/tencentcloud/apigateway/v20180808/
+-rw-r--r--   0 root         (0) root         (0)    95979 2023-05-08 02:44:05.000000 tencentcloud-sdk-python-apigateway-3.0.886/tencentcloud/apigateway/v20180808/apigateway_client.py
+-rw-r--r--   0 root         (0) root         (0)    20869 2023-05-08 02:44:05.000000 tencentcloud-sdk-python-apigateway-3.0.886/tencentcloud/apigateway/v20180808/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 02:44:05.000000 tencentcloud-sdk-python-apigateway-3.0.886/tencentcloud/apigateway/v20180808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   394892 2023-05-08 02:44:05.000000 tencentcloud-sdk-python-apigateway-3.0.886/tencentcloud/apigateway/v20180808/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 02:44:05.000000 tencentcloud-sdk-python-apigateway-3.0.886/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:44:05.000000 tencentcloud-sdk-python-apigateway-3.0.886/tencentcloud_sdk_python_apigateway.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 02:44:05.000000 tencentcloud-sdk-python-apigateway-3.0.886/tencentcloud_sdk_python_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-05-08 02:44:05.000000 tencentcloud-sdk-python-apigateway-3.0.886/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-05-08 02:44:05.000000 tencentcloud-sdk-python-apigateway-3.0.886/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 02:44:05.000000 tencentcloud-sdk-python-apigateway-3.0.886/tencentcloud_sdk_python_apigateway.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-05-08 02:44:05.000000 tencentcloud-sdk-python-apigateway-3.0.886/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-05-08 02:44:05.000000 tencentcloud-sdk-python-apigateway-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 02:44:05.000000 tencentcloud-sdk-python-apigateway-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.885/README.rst` & `tencentcloud-sdk-python-apigateway-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.885/tencentcloud/apigateway/v20180808/apigateway_client.py` & `tencentcloud-sdk-python-apigateway-3.0.886/tencentcloud/apigateway/v20180808/apigateway_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.885/tencentcloud/apigateway/v20180808/errorcodes.py` & `tencentcloud-sdk-python-apigateway-3.0.886/tencentcloud/apigateway/v20180808/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.885/tencentcloud/apigateway/v20180808/models.py` & `tencentcloud-sdk-python-apigateway-3.0.886/tencentcloud/apigateway/v20180808/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-apigateway-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-apigateway-3.0.885/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-apigateway-3.0.886/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.885/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO` & `tencentcloud-sdk-python-apigateway-3.0.886/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apigateway
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Apigateway SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-apigateway-3.0.886/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apigateway
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Apigateway SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.885/setup.py` & `tencentcloud-sdk-python-apigateway-3.0.886/setup.py`

 * *Files identical despite different names*

