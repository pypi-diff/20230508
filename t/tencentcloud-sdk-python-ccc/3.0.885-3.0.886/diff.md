# Comparing `tmp/tencentcloud-sdk-python-ccc-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-ccc-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ccc-3.0.885.tar", last modified: Mon May  1 00:30:48 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ccc-3.0.886.tar", last modified: Mon May  8 02:57:43 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ccc-3.0.885.tar` & `tencentcloud-sdk-python-ccc-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:30:48.000000 tencentcloud-sdk-python-ccc-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-01 00:30:48.000000 tencentcloud-sdk-python-ccc-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:30:48.000000 tencentcloud-sdk-python-ccc-3.0.885/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:30:48.000000 tencentcloud-sdk-python-ccc-3.0.885/tencentcloud/ccc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:30:48.000000 tencentcloud-sdk-python-ccc-3.0.885/tencentcloud/ccc/v20200210/
--rw-r--r--   0 root         (0) root         (0)    36406 2023-05-01 00:30:48.000000 tencentcloud-sdk-python-ccc-3.0.885/tencentcloud/ccc/v20200210/ccc_client.py
--rw-r--r--   0 root         (0) root         (0)     4155 2023-05-01 00:30:48.000000 tencentcloud-sdk-python-ccc-3.0.885/tencentcloud/ccc/v20200210/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:30:48.000000 tencentcloud-sdk-python-ccc-3.0.885/tencentcloud/ccc/v20200210/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140284 2023-05-01 00:30:48.000000 tencentcloud-sdk-python-ccc-3.0.885/tencentcloud/ccc/v20200210/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:30:48.000000 tencentcloud-sdk-python-ccc-3.0.885/tencentcloud/ccc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:30:48.000000 tencentcloud-sdk-python-ccc-3.0.885/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:30:48.000000 tencentcloud-sdk-python-ccc-3.0.885/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:30:48.000000 tencentcloud-sdk-python-ccc-3.0.885/tencentcloud_sdk_python_ccc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:30:48.000000 tencentcloud-sdk-python-ccc-3.0.885/tencentcloud_sdk_python_ccc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-01 00:30:48.000000 tencentcloud-sdk-python-ccc-3.0.885/tencentcloud_sdk_python_ccc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:30:48.000000 tencentcloud-sdk-python-ccc-3.0.885/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:30:48.000000 tencentcloud-sdk-python-ccc-3.0.885/tencentcloud_sdk_python_ccc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-01 00:30:48.000000 tencentcloud-sdk-python-ccc-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:30:48.000000 tencentcloud-sdk-python-ccc-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:57:43.000000 tencentcloud-sdk-python-ccc-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-08 02:57:43.000000 tencentcloud-sdk-python-ccc-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:57:43.000000 tencentcloud-sdk-python-ccc-3.0.886/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:57:43.000000 tencentcloud-sdk-python-ccc-3.0.886/tencentcloud/ccc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:57:43.000000 tencentcloud-sdk-python-ccc-3.0.886/tencentcloud/ccc/v20200210/
+-rw-r--r--   0 root         (0) root         (0)    36406 2023-05-08 02:57:43.000000 tencentcloud-sdk-python-ccc-3.0.886/tencentcloud/ccc/v20200210/ccc_client.py
+-rw-r--r--   0 root         (0) root         (0)     4155 2023-05-08 02:57:43.000000 tencentcloud-sdk-python-ccc-3.0.886/tencentcloud/ccc/v20200210/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 02:57:43.000000 tencentcloud-sdk-python-ccc-3.0.886/tencentcloud/ccc/v20200210/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140571 2023-05-08 02:57:43.000000 tencentcloud-sdk-python-ccc-3.0.886/tencentcloud/ccc/v20200210/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 02:57:43.000000 tencentcloud-sdk-python-ccc-3.0.886/tencentcloud/ccc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 02:57:43.000000 tencentcloud-sdk-python-ccc-3.0.886/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 02:57:43.000000 tencentcloud-sdk-python-ccc-3.0.886/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:57:43.000000 tencentcloud-sdk-python-ccc-3.0.886/tencentcloud_sdk_python_ccc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 02:57:43.000000 tencentcloud-sdk-python-ccc-3.0.886/tencentcloud_sdk_python_ccc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-08 02:57:43.000000 tencentcloud-sdk-python-ccc-3.0.886/tencentcloud_sdk_python_ccc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 02:57:43.000000 tencentcloud-sdk-python-ccc-3.0.886/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 02:57:43.000000 tencentcloud-sdk-python-ccc-3.0.886/tencentcloud_sdk_python_ccc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-08 02:57:43.000000 tencentcloud-sdk-python-ccc-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 02:57:43.000000 tencentcloud-sdk-python-ccc-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.885/README.rst` & `tencentcloud-sdk-python-ccc-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.885/tencentcloud/ccc/v20200210/ccc_client.py` & `tencentcloud-sdk-python-ccc-3.0.886/tencentcloud/ccc/v20200210/ccc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.885/tencentcloud/ccc/v20200210/errorcodes.py` & `tencentcloud-sdk-python-ccc-3.0.886/tencentcloud/ccc/v20200210/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.885/tencentcloud/ccc/v20200210/models.py` & `tencentcloud-sdk-python-ccc-3.0.886/tencentcloud/ccc/v20200210/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3361,14 +3361,17 @@
         :type RecordId: str
         :param Type: 参与者类型，"staffSeat", "outboundSeat", "staffPhoneSeat"
 注意：此字段可能返回 null，表示取不到有效值。
         :type Type: str
         :param TransferFrom: 转接来源坐席信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type TransferFrom: str
+        :param TransferFromType: 转接来源参与者类型，取值与 Type 一致
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TransferFromType: str
         :param TransferTo: 转接去向坐席信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type TransferTo: str
         :param TransferToType: 转接去向参与者类型，取值与 Type 一致
 注意：此字段可能返回 null，表示取不到有效值。
         :type TransferToType: str
         :param SkillGroupId: 技能组 ID
@@ -3397,14 +3400,15 @@
         self.Phone = None
         self.RingTimestamp = None
         self.AcceptTimestamp = None
         self.EndedTimestamp = None
         self.RecordId = None
         self.Type = None
         self.TransferFrom = None
+        self.TransferFromType = None
         self.TransferTo = None
         self.TransferToType = None
         self.SkillGroupId = None
         self.EndStatusString = None
         self.RecordURL = None
         self.Sequence = None
         self.StartTimestamp = None
@@ -3417,14 +3421,15 @@
         self.Phone = params.get("Phone")
         self.RingTimestamp = params.get("RingTimestamp")
         self.AcceptTimestamp = params.get("AcceptTimestamp")
         self.EndedTimestamp = params.get("EndedTimestamp")
         self.RecordId = params.get("RecordId")
         self.Type = params.get("Type")
         self.TransferFrom = params.get("TransferFrom")
+        self.TransferFromType = params.get("TransferFromType")
         self.TransferTo = params.get("TransferTo")
         self.TransferToType = params.get("TransferToType")
         self.SkillGroupId = params.get("SkillGroupId")
         self.EndStatusString = params.get("EndStatusString")
         self.RecordURL = params.get("RecordURL")
         self.Sequence = params.get("Sequence")
         self.StartTimestamp = params.get("StartTimestamp")
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ccc-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ccc-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-ccc-3.0.886/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ccc
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Ccc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.885/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ccc-3.0.886/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ccc
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Ccc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.885/setup.py` & `tencentcloud-sdk-python-ccc-3.0.886/setup.py`

 * *Files identical despite different names*

