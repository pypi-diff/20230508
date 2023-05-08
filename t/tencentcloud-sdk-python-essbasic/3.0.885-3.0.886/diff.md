# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.885.tar", last modified: Mon May  1 00:40:01 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.886.tar", last modified: Mon May  8 03:15:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.885.tar` & `tencentcloud-sdk-python-essbasic-3.0.886.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    15673 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    50524 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   229707 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:40:01.000000 tencentcloud-sdk-python-essbasic-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    15673 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    50524 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   230011 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 03:15:28.000000 tencentcloud-sdk-python-essbasic-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.885/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3871,34 +3871,39 @@
 class FlowApproverUrlInfo(AbstractModel):
     """签署人签署链接信息
 
     """
 
     def __init__(self):
         r"""
-        :param SignUrl: 签署链接，注意该链接有效期为30分钟，同时需要注意保密，不要外泄给无关用户。
+        :param SignUrl: 签署链接。注意该链接有效期为30分钟，同时需要注意保密，不要外泄给无关用户。
         :type SignUrl: str
-        :param Mobile: 签署人手机号
-        :type Mobile: str
-        :param Name: 签署人姓名
-        :type Name: str
         :param ApproverType: 签署人类型 PERSON-个人
         :type ApproverType: str
+        :param Name: 签署人姓名
+        :type Name: str
+        :param Mobile: 签署人手机号
+        :type Mobile: str
+        :param LongUrl: 签署长链接。注意该链接有效期为30分钟，同时需要注意保密，不要外泄给无关用户。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LongUrl: str
         """
         self.SignUrl = None
-        self.Mobile = None
-        self.Name = None
         self.ApproverType = None
+        self.Name = None
+        self.Mobile = None
+        self.LongUrl = None
 
 
     def _deserialize(self, params):
         self.SignUrl = params.get("SignUrl")
-        self.Mobile = params.get("Mobile")
-        self.Name = params.get("Name")
         self.ApproverType = params.get("ApproverType")
+        self.Name = params.get("Name")
+        self.Mobile = params.get("Mobile")
+        self.LongUrl = params.get("LongUrl")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.885/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.886/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.886/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.885/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.886/setup.py`

 * *Files identical despite different names*

