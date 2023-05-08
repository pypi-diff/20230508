# Comparing `tmp/tencentcloud-sdk-python-dbbrain-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-dbbrain-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.885.tar", last modified: Mon May  1 00:34:42 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.886.tar", last modified: Mon May  8 03:12:47 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dbbrain-3.0.885.tar` & `tencentcloud-sdk-python-dbbrain-3.0.886.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      749 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/dbbrain/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/dbbrain/v20210527/
--rw-r--r--   0 root         (0) root         (0)    48612 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/dbbrain/v20210527/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/dbbrain/v20210527/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/dbbrain/v20210527/__init__.py
--rw-r--r--   0 root         (0) root         (0)   182325 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/dbbrain/v20210527/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/dbbrain/v20191016/
--rw-r--r--   0 root         (0) root         (0)    27659 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/dbbrain/v20191016/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/dbbrain/v20191016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/dbbrain/v20191016/__init__.py
--rw-r--r--   0 root         (0) root         (0)   111297 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/dbbrain/v20191016/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/dbbrain/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud_sdk_python_dbbrain.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      663 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:34:42.000000 tencentcloud-sdk-python-dbbrain-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/dbbrain/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/dbbrain/v20210527/
+-rw-r--r--   0 root         (0) root         (0)    48612 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/dbbrain/v20210527/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/dbbrain/v20210527/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/dbbrain/v20210527/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   183066 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/dbbrain/v20210527/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/dbbrain/v20191016/
+-rw-r--r--   0 root         (0) root         (0)    27659 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/dbbrain/v20191016/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/dbbrain/v20191016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/dbbrain/v20191016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   111297 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/dbbrain/v20191016/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/dbbrain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud_sdk_python_dbbrain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      663 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 03:12:47.000000 tencentcloud-sdk-python-dbbrain-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.885/README.rst` & `tencentcloud-sdk-python-dbbrain-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/dbbrain/v20210527/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/dbbrain/v20210527/dbbrain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/dbbrain/v20210527/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/dbbrain/v20210527/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/dbbrain/v20210527/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/dbbrain/v20210527/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -994,24 +994,28 @@
         r"""
         :param InstanceId: 实例ID。
         :type InstanceId: str
         :param SessionToken: 通过VerifyUserAccount获取有效期为5分钟的会话token，使用后会自动延长token有效期至五分钟后。
         :type SessionToken: str
         :param FilterIds: 限流任务ID列表。
         :type FilterIds: list of int
+        :param Product: 服务产品类型，支持值："mysql" - 云数据库 MySQL；"cynosdb" - 云数据库 TDSQL-C for MySQL，默认为"mysql"。
+        :type Product: str
         """
         self.InstanceId = None
         self.SessionToken = None
         self.FilterIds = None
+        self.Product = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.SessionToken = params.get("SessionToken")
         self.FilterIds = params.get("FilterIds")
+        self.Product = params.get("Product")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2726,28 +2730,32 @@
         :type FilterIds: list of int
         :param Statuses: 任务状态列表，用于筛选任务列表，取值包括RUNNING - 运行中, FINISHED - 已完成, TERMINATED - 已终止。
         :type Statuses: list of str
         :param Offset: 偏移量，默认为0。
         :type Offset: int
         :param Limit: 返回数量，默认为20，最大值为100。
         :type Limit: int
+        :param Product: 服务产品类型，支持值："mysql" - 云数据库 MySQL；"cynosdb" - 云数据库 TDSQL-C for MySQL，默认为"mysql"。
+        :type Product: str
         """
         self.InstanceId = None
         self.FilterIds = None
         self.Statuses = None
         self.Offset = None
         self.Limit = None
+        self.Product = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.FilterIds = params.get("FilterIds")
         self.Statuses = params.get("Statuses")
         self.Offset = params.get("Offset")
         self.Limit = params.get("Limit")
+        self.Product = params.get("Product")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3772,28 +3780,32 @@
         :type Stage: str
         :param Threads: 需要kill的sql会话ID列表，此参数用于Prepare阶段。
         :type Threads: list of int
         :param SqlExecId: 执行ID，此参数用于Commit阶段。
         :type SqlExecId: str
         :param Product: 服务产品类型，支持值包括： "mysql" - 云数据库 MySQL， "cynosdb" - 云数据库 CynosDB  for MySQL，默认为"mysql"。
         :type Product: str
+        :param RecordHistory: 默认是ture, 记录下kill的记录，为了加快kill，可设置为false。
+        :type RecordHistory: bool
         """
         self.InstanceId = None
         self.Stage = None
         self.Threads = None
         self.SqlExecId = None
         self.Product = None
+        self.RecordHistory = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.Stage = params.get("Stage")
         self.Threads = params.get("Threads")
         self.SqlExecId = params.get("SqlExecId")
         self.Product = params.get("Product")
+        self.RecordHistory = params.get("RecordHistory")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/dbbrain/v20191016/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/dbbrain/v20191016/dbbrain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/dbbrain/v20191016/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/dbbrain/v20191016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/dbbrain/v20191016/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/dbbrain/v20191016/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.885/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.886/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.886/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.885/setup.py` & `tencentcloud-sdk-python-dbbrain-3.0.886/setup.py`

 * *Files identical despite different names*

