# Comparing `tmp/tencentcloud-sdk-python-cls-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-cls-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.885.tar", last modified: Mon May  1 00:33:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.886.tar", last modified: Mon May  8 03:07:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cls-3.0.885.tar` & `tencentcloud-sdk-python-cls-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:33:00.000000 tencentcloud-sdk-python-cls-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-01 00:33:00.000000 tencentcloud-sdk-python-cls-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:33:00.000000 tencentcloud-sdk-python-cls-3.0.885/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:33:00.000000 tencentcloud-sdk-python-cls-3.0.885/tencentcloud/cls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:33:00.000000 tencentcloud-sdk-python-cls-3.0.885/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)     8559 2023-05-01 00:33:00.000000 tencentcloud-sdk-python-cls-3.0.885/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:33:00.000000 tencentcloud-sdk-python-cls-3.0.885/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)   251498 2023-05-01 00:33:00.000000 tencentcloud-sdk-python-cls-3.0.885/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)    67922 2023-05-01 00:33:00.000000 tencentcloud-sdk-python-cls-3.0.885/tencentcloud/cls/v20201016/cls_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:33:00.000000 tencentcloud-sdk-python-cls-3.0.885/tencentcloud/cls/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:33:00.000000 tencentcloud-sdk-python-cls-3.0.885/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:33:00.000000 tencentcloud-sdk-python-cls-3.0.885/tencentcloud_sdk_python_cls.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:33:00.000000 tencentcloud-sdk-python-cls-3.0.885/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-01 00:33:00.000000 tencentcloud-sdk-python-cls-3.0.885/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:33:00.000000 tencentcloud-sdk-python-cls-3.0.885/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:33:00.000000 tencentcloud-sdk-python-cls-3.0.885/tencentcloud_sdk_python_cls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:33:00.000000 tencentcloud-sdk-python-cls-3.0.885/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-01 00:33:00.000000 tencentcloud-sdk-python-cls-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:33:00.000000 tencentcloud-sdk-python-cls-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:07:57.000000 tencentcloud-sdk-python-cls-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-08 03:07:57.000000 tencentcloud-sdk-python-cls-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:07:57.000000 tencentcloud-sdk-python-cls-3.0.886/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:07:57.000000 tencentcloud-sdk-python-cls-3.0.886/tencentcloud/cls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:07:57.000000 tencentcloud-sdk-python-cls-3.0.886/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)     8559 2023-05-08 03:07:57.000000 tencentcloud-sdk-python-cls-3.0.886/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:07:57.000000 tencentcloud-sdk-python-cls-3.0.886/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   252909 2023-05-08 03:07:57.000000 tencentcloud-sdk-python-cls-3.0.886/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)    67925 2023-05-08 03:07:57.000000 tencentcloud-sdk-python-cls-3.0.886/tencentcloud/cls/v20201016/cls_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:07:57.000000 tencentcloud-sdk-python-cls-3.0.886/tencentcloud/cls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 03:07:57.000000 tencentcloud-sdk-python-cls-3.0.886/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:07:57.000000 tencentcloud-sdk-python-cls-3.0.886/tencentcloud_sdk_python_cls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 03:07:57.000000 tencentcloud-sdk-python-cls-3.0.886/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-08 03:07:57.000000 tencentcloud-sdk-python-cls-3.0.886/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 03:07:57.000000 tencentcloud-sdk-python-cls-3.0.886/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 03:07:57.000000 tencentcloud-sdk-python-cls-3.0.886/tencentcloud_sdk_python_cls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 03:07:57.000000 tencentcloud-sdk-python-cls-3.0.886/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-08 03:07:57.000000 tencentcloud-sdk-python-cls-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 03:07:57.000000 tencentcloud-sdk-python-cls-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cls-3.0.885/README.rst` & `tencentcloud-sdk-python-cls-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.885/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-cls-3.0.886/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.885/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-cls-3.0.886/tencentcloud/cls/v20201016/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6800,14 +6800,34 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type Content: :class:`tencentcloud.cls.v20201016.models.ContentInfo`
         :param CreateTime: 投递日志的创建时间
         :type CreateTime: str
         :param FilenameMode: 投递文件命名配置，0：随机数命名，1：投递时间命名，默认0（随机数命名）
 注意：此字段可能返回 null，表示取不到有效值。
         :type FilenameMode: int
+        :param StartTime: 投递数据范围的开始时间点
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StartTime: int
+        :param EndTime: 投递数据范围的结束时间点
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EndTime: int
+        :param Progress: 历史数据投递的进度（仅当用户选择的数据内中历史数据时才有效）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Progress: float
+        :param RemainTime: 历史数据全部投递完成剩余的时间（仅当用户选择的数据中有历史数据时才有效）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RemainTime: int
+        :param HistoryStatus: 历史任务状态：
+0：实时任务
+1：任务准备中
+2：任务运行中
+3：任务运行异常
+4：任务运行结束
+注意：此字段可能返回 null，表示取不到有效值。
+        :type HistoryStatus: int
         """
         self.ShipperId = None
         self.TopicId = None
         self.Bucket = None
         self.Prefix = None
         self.ShipperName = None
         self.Interval = None
@@ -6815,14 +6835,19 @@
         self.Status = None
         self.FilterRules = None
         self.Partition = None
         self.Compress = None
         self.Content = None
         self.CreateTime = None
         self.FilenameMode = None
+        self.StartTime = None
+        self.EndTime = None
+        self.Progress = None
+        self.RemainTime = None
+        self.HistoryStatus = None
 
 
     def _deserialize(self, params):
         self.ShipperId = params.get("ShipperId")
         self.TopicId = params.get("TopicId")
         self.Bucket = params.get("Bucket")
         self.Prefix = params.get("Prefix")
@@ -6841,14 +6866,19 @@
             self.Compress = CompressInfo()
             self.Compress._deserialize(params.get("Compress"))
         if params.get("Content") is not None:
             self.Content = ContentInfo()
             self.Content._deserialize(params.get("Content"))
         self.CreateTime = params.get("CreateTime")
         self.FilenameMode = params.get("FilenameMode")
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.Progress = params.get("Progress")
+        self.RemainTime = params.get("RemainTime")
+        self.HistoryStatus = params.get("HistoryStatus")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cls-3.0.885/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-cls-3.0.886/tencentcloud/cls/v20201016/cls_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1523,15 +1523,15 @@
 
     def UploadLog(self, request, body):
         """## 提示
         为了保障您日志数据的可靠性以及更高效地使用日志服务，建议您使用CLS优化后的接口[上传结构化日志](https://cloud.tencent.com/document/product/614/16873)上传日志。
 
         同时我们给此接口专门优化定制了多个语言版本的SDK供您选择，SDK提供统一的异步发送、资源控制、自动重试、优雅关闭、感知上报等功能，使上报日志功能更完善，详情请参考[SDK采集](https://cloud.tencent.com/document/product/614/67157)。
 
-        同时云API上传日志接口也支持同步上传日志数据，如果您选继续使用此接口请参考下文。
+        同时云API上传日志接口也支持同步上传日志数据，如果您选择继续使用此接口请参考下文。
 
         ## 功能描述
 
         本接口用于将日志写入到指定的日志主题。
 
         日志服务提供以下两种模式：
```

### Comparing `tencentcloud-sdk-python-cls-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cls-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cls-3.0.885/tencentcloud_sdk_python_cls.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.886/tencentcloud_sdk_python_cls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.886/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.885/setup.py` & `tencentcloud-sdk-python-cls-3.0.886/setup.py`

 * *Files identical despite different names*

