# Comparing `tmp/tencentcloud-sdk-python-iotexplorer-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-iotexplorer-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iotexplorer-3.0.885.tar", last modified: Mon May  1 00:42:42 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iotexplorer-3.0.886.tar", last modified: Mon May  8 03:30:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iotexplorer-3.0.885.tar` & `tencentcloud-sdk-python-iotexplorer-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:42:42.000000 tencentcloud-sdk-python-iotexplorer-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      761 2023-05-01 00:42:42.000000 tencentcloud-sdk-python-iotexplorer-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:42:42.000000 tencentcloud-sdk-python-iotexplorer-3.0.885/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:42:42.000000 tencentcloud-sdk-python-iotexplorer-3.0.885/tencentcloud/iotexplorer/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:42:42.000000 tencentcloud-sdk-python-iotexplorer-3.0.885/tencentcloud/iotexplorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:42:42.000000 tencentcloud-sdk-python-iotexplorer-3.0.885/tencentcloud/iotexplorer/v20190423/
--rw-r--r--   0 root         (0) root         (0)    20510 2023-05-01 00:42:42.000000 tencentcloud-sdk-python-iotexplorer-3.0.885/tencentcloud/iotexplorer/v20190423/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:42:42.000000 tencentcloud-sdk-python-iotexplorer-3.0.885/tencentcloud/iotexplorer/v20190423/__init__.py
--rw-r--r--   0 root         (0) root         (0)   224364 2023-05-01 00:42:42.000000 tencentcloud-sdk-python-iotexplorer-3.0.885/tencentcloud/iotexplorer/v20190423/models.py
--rw-r--r--   0 root         (0) root         (0)    82835 2023-05-01 00:42:42.000000 tencentcloud-sdk-python-iotexplorer-3.0.885/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:42:42.000000 tencentcloud-sdk-python-iotexplorer-3.0.885/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1699 2023-05-01 00:42:42.000000 tencentcloud-sdk-python-iotexplorer-3.0.885/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:42:42.000000 tencentcloud-sdk-python-iotexplorer-3.0.885/tencentcloud_sdk_python_iotexplorer.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:42:42.000000 tencentcloud-sdk-python-iotexplorer-3.0.885/tencentcloud_sdk_python_iotexplorer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      525 2023-05-01 00:42:42.000000 tencentcloud-sdk-python-iotexplorer-3.0.885/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1699 2023-05-01 00:42:42.000000 tencentcloud-sdk-python-iotexplorer-3.0.885/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:42:42.000000 tencentcloud-sdk-python-iotexplorer-3.0.885/tencentcloud_sdk_python_iotexplorer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1022 2023-05-01 00:42:42.000000 tencentcloud-sdk-python-iotexplorer-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:42:42.000000 tencentcloud-sdk-python-iotexplorer-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:30:44.000000 tencentcloud-sdk-python-iotexplorer-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      761 2023-05-08 03:30:43.000000 tencentcloud-sdk-python-iotexplorer-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:30:44.000000 tencentcloud-sdk-python-iotexplorer-3.0.886/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:30:44.000000 tencentcloud-sdk-python-iotexplorer-3.0.886/tencentcloud/iotexplorer/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:30:43.000000 tencentcloud-sdk-python-iotexplorer-3.0.886/tencentcloud/iotexplorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:30:44.000000 tencentcloud-sdk-python-iotexplorer-3.0.886/tencentcloud/iotexplorer/v20190423/
+-rw-r--r--   0 root         (0) root         (0)    20510 2023-05-08 03:30:43.000000 tencentcloud-sdk-python-iotexplorer-3.0.886/tencentcloud/iotexplorer/v20190423/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:30:43.000000 tencentcloud-sdk-python-iotexplorer-3.0.886/tencentcloud/iotexplorer/v20190423/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   224834 2023-05-08 03:30:43.000000 tencentcloud-sdk-python-iotexplorer-3.0.886/tencentcloud/iotexplorer/v20190423/models.py
+-rw-r--r--   0 root         (0) root         (0)    82835 2023-05-08 03:30:43.000000 tencentcloud-sdk-python-iotexplorer-3.0.886/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 03:30:43.000000 tencentcloud-sdk-python-iotexplorer-3.0.886/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-05-08 03:30:44.000000 tencentcloud-sdk-python-iotexplorer-3.0.886/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:30:44.000000 tencentcloud-sdk-python-iotexplorer-3.0.886/tencentcloud_sdk_python_iotexplorer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 03:30:44.000000 tencentcloud-sdk-python-iotexplorer-3.0.886/tencentcloud_sdk_python_iotexplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      525 2023-05-08 03:30:44.000000 tencentcloud-sdk-python-iotexplorer-3.0.886/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-05-08 03:30:44.000000 tencentcloud-sdk-python-iotexplorer-3.0.886/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 03:30:44.000000 tencentcloud-sdk-python-iotexplorer-3.0.886/tencentcloud_sdk_python_iotexplorer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-05-08 03:30:43.000000 tencentcloud-sdk-python-iotexplorer-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 03:30:44.000000 tencentcloud-sdk-python-iotexplorer-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.885/README.rst` & `tencentcloud-sdk-python-iotexplorer-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.885/tencentcloud/iotexplorer/v20190423/errorcodes.py` & `tencentcloud-sdk-python-iotexplorer-3.0.886/tencentcloud/iotexplorer/v20190423/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.885/tencentcloud/iotexplorer/v20190423/models.py` & `tencentcloud-sdk-python-iotexplorer-3.0.886/tencentcloud/iotexplorer/v20190423/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3386,22 +3386,32 @@
 
     def __init__(self):
         r"""
         :param UserId: 用户ID
         :type UserId: str
         :param Role: 用户角色 1所有者，0：其他分享者
         :type Role: int
+        :param FamilyId: 家庭ID，所有者带该参数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FamilyId: str
+        :param FamilyName: 家庭名称，所有者带该参数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FamilyName: str
         """
         self.UserId = None
         self.Role = None
+        self.FamilyId = None
+        self.FamilyName = None
 
 
     def _deserialize(self, params):
         self.UserId = params.get("UserId")
         self.Role = params.get("Role")
+        self.FamilyId = params.get("FamilyId")
+        self.FamilyName = params.get("FamilyName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.885/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py` & `tencentcloud-sdk-python-iotexplorer-3.0.886/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iotexplorer-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-iotexplorer-3.0.886/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotexplorer
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Iotexplorer SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.885/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-iotexplorer-3.0.886/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.885/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iotexplorer-3.0.886/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotexplorer
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Iotexplorer SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.885/setup.py` & `tencentcloud-sdk-python-iotexplorer-3.0.886/setup.py`

 * *Files identical despite different names*

