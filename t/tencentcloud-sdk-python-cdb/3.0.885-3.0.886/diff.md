# Comparing `tmp/tencentcloud-sdk-python-cdb-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-cdb-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.885.tar", last modified: Mon May  1 00:30:55 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.886.tar", last modified: Mon May  8 02:57:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdb-3.0.885.tar` & `tencentcloud-sdk-python-cdb-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:30:55.000000 tencentcloud-sdk-python-cdb-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-01 00:30:55.000000 tencentcloud-sdk-python-cdb-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:30:55.000000 tencentcloud-sdk-python-cdb-3.0.885/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:30:55.000000 tencentcloud-sdk-python-cdb-3.0.885/tencentcloud/cdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:30:55.000000 tencentcloud-sdk-python-cdb-3.0.885/tencentcloud/cdb/v20170320/
--rw-r--r--   0 root         (0) root         (0)   150803 2023-05-01 00:30:55.000000 tencentcloud-sdk-python-cdb-3.0.885/tencentcloud/cdb/v20170320/cdb_client.py
--rw-r--r--   0 root         (0) root         (0)    18943 2023-05-01 00:30:55.000000 tencentcloud-sdk-python-cdb-3.0.885/tencentcloud/cdb/v20170320/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:30:55.000000 tencentcloud-sdk-python-cdb-3.0.885/tencentcloud/cdb/v20170320/__init__.py
--rw-r--r--   0 root         (0) root         (0)   526389 2023-05-01 00:30:55.000000 tencentcloud-sdk-python-cdb-3.0.885/tencentcloud/cdb/v20170320/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:30:55.000000 tencentcloud-sdk-python-cdb-3.0.885/tencentcloud/cdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:30:55.000000 tencentcloud-sdk-python-cdb-3.0.885/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:30:55.000000 tencentcloud-sdk-python-cdb-3.0.885/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:30:55.000000 tencentcloud-sdk-python-cdb-3.0.885/tencentcloud_sdk_python_cdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:30:55.000000 tencentcloud-sdk-python-cdb-3.0.885/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-01 00:30:55.000000 tencentcloud-sdk-python-cdb-3.0.885/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:30:55.000000 tencentcloud-sdk-python-cdb-3.0.885/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:30:55.000000 tencentcloud-sdk-python-cdb-3.0.885/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-01 00:30:55.000000 tencentcloud-sdk-python-cdb-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:30:55.000000 tencentcloud-sdk-python-cdb-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:57:50.000000 tencentcloud-sdk-python-cdb-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-08 02:57:50.000000 tencentcloud-sdk-python-cdb-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:57:50.000000 tencentcloud-sdk-python-cdb-3.0.886/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:57:50.000000 tencentcloud-sdk-python-cdb-3.0.886/tencentcloud/cdb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:57:50.000000 tencentcloud-sdk-python-cdb-3.0.886/tencentcloud/cdb/v20170320/
+-rw-r--r--   0 root         (0) root         (0)   150803 2023-05-08 02:57:50.000000 tencentcloud-sdk-python-cdb-3.0.886/tencentcloud/cdb/v20170320/cdb_client.py
+-rw-r--r--   0 root         (0) root         (0)    18943 2023-05-08 02:57:50.000000 tencentcloud-sdk-python-cdb-3.0.886/tencentcloud/cdb/v20170320/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 02:57:50.000000 tencentcloud-sdk-python-cdb-3.0.886/tencentcloud/cdb/v20170320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   526653 2023-05-08 02:57:50.000000 tencentcloud-sdk-python-cdb-3.0.886/tencentcloud/cdb/v20170320/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 02:57:50.000000 tencentcloud-sdk-python-cdb-3.0.886/tencentcloud/cdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 02:57:50.000000 tencentcloud-sdk-python-cdb-3.0.886/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 02:57:50.000000 tencentcloud-sdk-python-cdb-3.0.886/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:57:50.000000 tencentcloud-sdk-python-cdb-3.0.886/tencentcloud_sdk_python_cdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 02:57:50.000000 tencentcloud-sdk-python-cdb-3.0.886/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-08 02:57:50.000000 tencentcloud-sdk-python-cdb-3.0.886/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 02:57:50.000000 tencentcloud-sdk-python-cdb-3.0.886/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 02:57:50.000000 tencentcloud-sdk-python-cdb-3.0.886/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-08 02:57:50.000000 tencentcloud-sdk-python-cdb-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 02:57:50.000000 tencentcloud-sdk-python-cdb-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.885/README.rst` & `tencentcloud-sdk-python-cdb-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.885/tencentcloud/cdb/v20170320/cdb_client.py` & `tencentcloud-sdk-python-cdb-3.0.886/tencentcloud/cdb/v20170320/cdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.885/tencentcloud/cdb/v20170320/errorcodes.py` & `tencentcloud-sdk-python-cdb-3.0.886/tencentcloud/cdb/v20170320/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.885/tencentcloud/cdb/v20170320/models.py` & `tencentcloud-sdk-python-cdb-3.0.886/tencentcloud/cdb/v20170320/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -11308,40 +11308,45 @@
         :type Min: int
         :param EnumValue: 参数的可选枚举值。如果为非枚举参数，则为空
         :type EnumValue: list of str
         :param MaxFunc: 参数是公式类型时，该字段有效，表示公式类型最大值
         :type MaxFunc: str
         :param MinFunc: 参数是公式类型时，该字段有效，表示公式类型最小值
         :type MinFunc: str
+        :param IsNotSupportEdit: 参数是否不支持修改
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsNotSupportEdit: bool
         """
         self.Name = None
         self.ParamType = None
         self.Default = None
         self.Description = None
         self.CurrentValue = None
         self.NeedReboot = None
         self.Max = None
         self.Min = None
         self.EnumValue = None
         self.MaxFunc = None
         self.MinFunc = None
+        self.IsNotSupportEdit = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.ParamType = params.get("ParamType")
         self.Default = params.get("Default")
         self.Description = params.get("Description")
         self.CurrentValue = params.get("CurrentValue")
         self.NeedReboot = params.get("NeedReboot")
         self.Max = params.get("Max")
         self.Min = params.get("Min")
         self.EnumValue = params.get("EnumValue")
         self.MaxFunc = params.get("MaxFunc")
         self.MinFunc = params.get("MinFunc")
+        self.IsNotSupportEdit = params.get("IsNotSupportEdit")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdb-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdb-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.886/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.885/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.886/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.885/setup.py` & `tencentcloud-sdk-python-cdb-3.0.886/setup.py`

 * *Files identical despite different names*

