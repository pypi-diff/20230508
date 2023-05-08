# Comparing `tmp/tencentcloud-sdk-python-monitor-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-monitor-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-monitor-3.0.885.tar", last modified: Mon May  1 00:45:20 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-monitor-3.0.886.tar", last modified: Mon May  8 03:37:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-monitor-3.0.885.tar` & `tencentcloud-sdk-python-monitor-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:45:20.000000 tencentcloud-sdk-python-monitor-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      749 2023-05-01 00:45:20.000000 tencentcloud-sdk-python-monitor-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:45:20.000000 tencentcloud-sdk-python-monitor-3.0.885/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:45:20.000000 tencentcloud-sdk-python-monitor-3.0.885/tencentcloud/monitor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:45:20.000000 tencentcloud-sdk-python-monitor-3.0.885/tencentcloud/monitor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:45:20.000000 tencentcloud-sdk-python-monitor-3.0.885/tencentcloud/monitor/v20180724/
--rw-r--r--   0 root         (0) root         (0)    10348 2023-05-01 00:45:20.000000 tencentcloud-sdk-python-monitor-3.0.885/tencentcloud/monitor/v20180724/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   143620 2023-05-01 00:45:20.000000 tencentcloud-sdk-python-monitor-3.0.885/tencentcloud/monitor/v20180724/monitor_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:45:20.000000 tencentcloud-sdk-python-monitor-3.0.885/tencentcloud/monitor/v20180724/__init__.py
--rw-r--r--   0 root         (0) root         (0)   551751 2023-05-01 00:45:20.000000 tencentcloud-sdk-python-monitor-3.0.885/tencentcloud/monitor/v20180724/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:45:20.000000 tencentcloud-sdk-python-monitor-3.0.885/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-01 00:45:20.000000 tencentcloud-sdk-python-monitor-3.0.885/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:45:20.000000 tencentcloud-sdk-python-monitor-3.0.885/tencentcloud_sdk_python_monitor.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:45:20.000000 tencentcloud-sdk-python-monitor-3.0.885/tencentcloud_sdk_python_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-01 00:45:20.000000 tencentcloud-sdk-python-monitor-3.0.885/tencentcloud_sdk_python_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-01 00:45:20.000000 tencentcloud-sdk-python-monitor-3.0.885/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:45:20.000000 tencentcloud-sdk-python-monitor-3.0.885/tencentcloud_sdk_python_monitor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-01 00:45:20.000000 tencentcloud-sdk-python-monitor-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:45:20.000000 tencentcloud-sdk-python-monitor-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:37:28.000000 tencentcloud-sdk-python-monitor-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-08 03:37:28.000000 tencentcloud-sdk-python-monitor-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:37:28.000000 tencentcloud-sdk-python-monitor-3.0.886/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:37:28.000000 tencentcloud-sdk-python-monitor-3.0.886/tencentcloud/monitor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:37:28.000000 tencentcloud-sdk-python-monitor-3.0.886/tencentcloud/monitor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:37:28.000000 tencentcloud-sdk-python-monitor-3.0.886/tencentcloud/monitor/v20180724/
+-rw-r--r--   0 root         (0) root         (0)    10348 2023-05-08 03:37:28.000000 tencentcloud-sdk-python-monitor-3.0.886/tencentcloud/monitor/v20180724/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   143620 2023-05-08 03:37:28.000000 tencentcloud-sdk-python-monitor-3.0.886/tencentcloud/monitor/v20180724/monitor_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:37:28.000000 tencentcloud-sdk-python-monitor-3.0.886/tencentcloud/monitor/v20180724/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   552386 2023-05-08 03:37:28.000000 tencentcloud-sdk-python-monitor-3.0.886/tencentcloud/monitor/v20180724/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 03:37:28.000000 tencentcloud-sdk-python-monitor-3.0.886/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-08 03:37:28.000000 tencentcloud-sdk-python-monitor-3.0.886/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:37:28.000000 tencentcloud-sdk-python-monitor-3.0.886/tencentcloud_sdk_python_monitor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 03:37:28.000000 tencentcloud-sdk-python-monitor-3.0.886/tencentcloud_sdk_python_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-08 03:37:28.000000 tencentcloud-sdk-python-monitor-3.0.886/tencentcloud_sdk_python_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-08 03:37:28.000000 tencentcloud-sdk-python-monitor-3.0.886/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 03:37:28.000000 tencentcloud-sdk-python-monitor-3.0.886/tencentcloud_sdk_python_monitor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-08 03:37:28.000000 tencentcloud-sdk-python-monitor-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 03:37:28.000000 tencentcloud-sdk-python-monitor-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.885/README.rst` & `tencentcloud-sdk-python-monitor-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.885/tencentcloud/monitor/v20180724/errorcodes.py` & `tencentcloud-sdk-python-monitor-3.0.886/tencentcloud/monitor/v20180724/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.885/tencentcloud/monitor/v20180724/monitor_client.py` & `tencentcloud-sdk-python-monitor-3.0.886/tencentcloud/monitor/v20180724/monitor_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.885/tencentcloud/monitor/v20180724/models.py` & `tencentcloud-sdk-python-monitor-3.0.886/tencentcloud/monitor/v20180724/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10635,26 +10635,34 @@
         :type IsAdvanced: int
         :param IsOpen: 高级指标是否开通。1是 0否
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsOpen: int
         :param ProductId: 集成中心产品ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type ProductId: int
+        :param Operators: 匹配运算符
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Operators: list of Operator
+        :param Periods: 指标触发
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Periods: list of int
         """
         self.Namespace = None
         self.MetricName = None
         self.Description = None
         self.Min = None
         self.Max = None
         self.Dimensions = None
         self.Unit = None
         self.MetricConfig = None
         self.IsAdvanced = None
         self.IsOpen = None
         self.ProductId = None
+        self.Operators = None
+        self.Periods = None
 
 
     def _deserialize(self, params):
         self.Namespace = params.get("Namespace")
         self.MetricName = params.get("MetricName")
         self.Description = params.get("Description")
         self.Min = params.get("Min")
@@ -10663,14 +10671,21 @@
         self.Unit = params.get("Unit")
         if params.get("MetricConfig") is not None:
             self.MetricConfig = MetricConfig()
             self.MetricConfig._deserialize(params.get("MetricConfig"))
         self.IsAdvanced = params.get("IsAdvanced")
         self.IsOpen = params.get("IsOpen")
         self.ProductId = params.get("ProductId")
+        if params.get("Operators") is not None:
+            self.Operators = []
+            for item in params.get("Operators"):
+                obj = Operator()
+                obj._deserialize(item)
+                self.Operators.append(obj)
+        self.Periods = params.get("Periods")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-monitor-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-monitor-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-monitor-3.0.886/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-monitor
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Monitor SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.885/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO` & `tencentcloud-sdk-python-monitor-3.0.886/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-monitor
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Monitor SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.885/setup.py` & `tencentcloud-sdk-python-monitor-3.0.886/setup.py`

 * *Files identical despite different names*

