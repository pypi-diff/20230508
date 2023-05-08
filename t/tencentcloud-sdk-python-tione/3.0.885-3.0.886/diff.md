# Comparing `tmp/tencentcloud-sdk-python-tione-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-tione-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.885.tar", last modified: Mon May  1 00:56:53 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.886.tar", last modified: Mon May  8 04:11:39 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tione-3.0.885.tar` & `tencentcloud-sdk-python-tione-3.0.886.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/tencentcloud/tione/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/tencentcloud/tione/v20211111/
--rw-r--r--   0 root         (0) root         (0)    51024 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/tencentcloud/tione/v20211111/tione_client.py
--rw-r--r--   0 root         (0) root         (0)    10734 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   331524 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/tencentcloud/tione/v20211111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/tencentcloud/tione/v20191022/
--rw-r--r--   0 root         (0) root         (0)    22010 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/tencentcloud/tione/v20191022/tione_client.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/tencentcloud/tione/v20191022/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/tencentcloud/tione/v20191022/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91250 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/tencentcloud/tione/v20191022/models.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/tencentcloud_sdk_python_tione.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:56:53.000000 tencentcloud-sdk-python-tione-3.0.885/tencentcloud_sdk_python_tione.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20211111/
+-rw-r--r--   0 root         (0) root         (0)    51024 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20211111/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)    10734 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   333554 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20211111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20191022/
+-rw-r--r--   0 root         (0) root         (0)    22010 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20191022/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20191022/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20191022/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91250 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20191022/models.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud_sdk_python_tione.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      633 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud_sdk_python_tione.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tione-3.0.885/README.rst` & `tencentcloud-sdk-python-tione-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tione-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tione-3.0.885/tencentcloud/tione/v20211111/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20211111/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.885/tencentcloud/tione/v20211111/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.885/tencentcloud/tione/v20211111/models.py` & `tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20211111/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1443,15 +1443,16 @@
 
     """
 
     def __init__(self):
         r"""
         :param Name: 训练任务名称，不超过60个字符，仅支持中英文、数字、下划线"_"、短横"-"，只能以中英文、数字开头
         :type Name: str
-        :param ChargeType: 计费模式，eg：PREPAID预付费，即包年包月；POSTPAID_BY_HOUR按小时后付费
+        :param ChargeType: 计费模式，eg：PREPAID 包年包月（资源组）;
+POSTPAID_BY_HOUR 按量计费
         :type ChargeType: str
         :param ResourceConfigInfos: 资源配置，需填写对应算力规格ID和节点数量，算力规格ID查询接口为DescribeBillingSpecsPrice，eg：[{"Role":"WORKER", "InstanceType": "TI.S.MEDIUM.POST", "InstanceNum": 1}]
         :type ResourceConfigInfos: list of ResourceConfigInfo
         :param CodePackagePath: COS代码包路径
         :type CodePackagePath: :class:`tencentcloud.tione.v20211111.models.CosPathInfo`
         :param TrainingMode: 训练模式，通过DescribeTrainingFrameworks接口查询，eg：PS_WORKER、DDP、MPI、HOROVOD
         :type TrainingMode: str
@@ -1792,21 +1793,25 @@
         :type COSSource: :class:`tencentcloud.tione.v20211111.models.CosPathInfo`
         :param CFSSource: 来自CFS的数据
 注意：此字段可能返回 null，表示取不到有效值。
         :type CFSSource: :class:`tencentcloud.tione.v20211111.models.CFSConfig`
         :param HDFSSource: 来自HDFS的数据
 注意：此字段可能返回 null，表示取不到有效值。
         :type HDFSSource: :class:`tencentcloud.tione.v20211111.models.HDFSConfig`
+        :param GooseFSSource: 配饰GooseFS的数据
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GooseFSSource: :class:`tencentcloud.tione.v20211111.models.GooseFS`
         """
         self.MappingPath = None
         self.DataSourceType = None
         self.DataSetSource = None
         self.COSSource = None
         self.CFSSource = None
         self.HDFSSource = None
+        self.GooseFSSource = None
 
 
     def _deserialize(self, params):
         self.MappingPath = params.get("MappingPath")
         self.DataSourceType = params.get("DataSourceType")
         if params.get("DataSetSource") is not None:
             self.DataSetSource = DataSetConfig()
@@ -1816,14 +1821,17 @@
             self.COSSource._deserialize(params.get("COSSource"))
         if params.get("CFSSource") is not None:
             self.CFSSource = CFSConfig()
             self.CFSSource._deserialize(params.get("CFSSource"))
         if params.get("HDFSSource") is not None:
             self.HDFSSource = HDFSConfig()
             self.HDFSSource._deserialize(params.get("HDFSSource"))
+        if params.get("GooseFSSource") is not None:
+            self.GooseFSSource = GooseFS()
+            self.GooseFSSource._deserialize(params.get("GooseFSSource"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4944,14 +4952,39 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class GooseFS(AbstractModel):
+    """配置GooseFS参数
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Id: goosefs实例id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Id: str
+        """
+        self.Id = None
+
+
+    def _deserialize(self, params):
+        self.Id = params.get("Id")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class GpuDetail(AbstractModel):
     """gpu 详情
 
     """
 
     def __init__(self):
         r"""
@@ -6340,14 +6373,39 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class RDMAConfig(AbstractModel):
+    """RDMA配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Enable: 是否开启RDMA
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Enable: bool
+        """
+        self.Enable = None
+
+
+    def _deserialize(self, params):
+        self.Enable = params.get("Enable")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ResourceConfigInfo(AbstractModel):
     """资源配置
 
     """
 
     def __init__(self):
         r"""
@@ -6397,34 +6455,41 @@
 8C80G V100*2 
 32C160G V100*4
 72C320G V100*8
 32C128G T4*1 
 40C160G T4*2 
 80C32
         :type InstanceTypeAlias: str
+        :param RDMAConfig: RDMA配置
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RDMAConfig: :class:`tencentcloud.tione.v20211111.models.RDMAConfig`
         """
         self.Role = None
         self.Cpu = None
         self.Memory = None
         self.GpuType = None
         self.Gpu = None
         self.InstanceType = None
         self.InstanceNum = None
         self.InstanceTypeAlias = None
+        self.RDMAConfig = None
 
 
     def _deserialize(self, params):
         self.Role = params.get("Role")
         self.Cpu = params.get("Cpu")
         self.Memory = params.get("Memory")
         self.GpuType = params.get("GpuType")
         self.Gpu = params.get("Gpu")
         self.InstanceType = params.get("InstanceType")
         self.InstanceNum = params.get("InstanceNum")
         self.InstanceTypeAlias = params.get("InstanceTypeAlias")
+        if params.get("RDMAConfig") is not None:
+            self.RDMAConfig = RDMAConfig()
+            self.RDMAConfig._deserialize(params.get("RDMAConfig"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tione-3.0.885/tencentcloud/tione/v20191022/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20191022/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.885/tencentcloud/tione/v20191022/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20191022/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.885/tencentcloud/tione/v20191022/models.py` & `tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20191022/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.886/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tione-3.0.885/setup.py` & `tencentcloud-sdk-python-tione-3.0.886/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.885/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tione-3.0.886/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.885/tencentcloud_sdk_python_tione.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.886/tencentcloud_sdk_python_tione.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

