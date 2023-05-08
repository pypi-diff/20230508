# Comparing `tmp/tencentcloud-sdk-python-asr-3.0.884.tar.gz` & `tmp/tencentcloud-sdk-python-asr-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.884.tar", last modified: Fri Apr 28 02:04:33 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.886.tar", last modified: Mon May  8 02:46:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-asr-3.0.884.tar` & `tencentcloud-sdk-python-asr-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:04:33.000000 tencentcloud-sdk-python-asr-3.0.884/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-28 02:04:33.000000 tencentcloud-sdk-python-asr-3.0.884/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:04:33.000000 tencentcloud-sdk-python-asr-3.0.884/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:04:33.000000 tencentcloud-sdk-python-asr-3.0.884/tencentcloud/asr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:04:33.000000 tencentcloud-sdk-python-asr-3.0.884/tencentcloud/asr/v20190614/
--rw-r--r--   0 root         (0) root         (0)    23847 2023-04-28 02:04:33.000000 tencentcloud-sdk-python-asr-3.0.884/tencentcloud/asr/v20190614/asr_client.py
--rw-r--r--   0 root         (0) root         (0)     6428 2023-04-28 02:04:33.000000 tencentcloud-sdk-python-asr-3.0.884/tencentcloud/asr/v20190614/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:04:33.000000 tencentcloud-sdk-python-asr-3.0.884/tencentcloud/asr/v20190614/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62142 2023-04-28 02:04:33.000000 tencentcloud-sdk-python-asr-3.0.884/tencentcloud/asr/v20190614/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:04:33.000000 tencentcloud-sdk-python-asr-3.0.884/tencentcloud/asr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:04:33.000000 tencentcloud-sdk-python-asr-3.0.884/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:04:33.000000 tencentcloud-sdk-python-asr-3.0.884/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-28 02:04:33.000000 tencentcloud-sdk-python-asr-3.0.884/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:04:33.000000 tencentcloud-sdk-python-asr-3.0.884/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:04:33.000000 tencentcloud-sdk-python-asr-3.0.884/tencentcloud_sdk_python_asr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:04:33.000000 tencentcloud-sdk-python-asr-3.0.884/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-28 02:04:33.000000 tencentcloud-sdk-python-asr-3.0.884/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:04:33.000000 tencentcloud-sdk-python-asr-3.0.884/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:04:33.000000 tencentcloud-sdk-python-asr-3.0.884/tencentcloud_sdk_python_asr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:46:29.000000 tencentcloud-sdk-python-asr-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-08 02:46:29.000000 tencentcloud-sdk-python-asr-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:46:29.000000 tencentcloud-sdk-python-asr-3.0.886/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:46:29.000000 tencentcloud-sdk-python-asr-3.0.886/tencentcloud/asr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:46:29.000000 tencentcloud-sdk-python-asr-3.0.886/tencentcloud/asr/v20190614/
+-rw-r--r--   0 root         (0) root         (0)    24720 2023-05-08 02:46:29.000000 tencentcloud-sdk-python-asr-3.0.886/tencentcloud/asr/v20190614/asr_client.py
+-rw-r--r--   0 root         (0) root         (0)     6428 2023-05-08 02:46:29.000000 tencentcloud-sdk-python-asr-3.0.886/tencentcloud/asr/v20190614/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 02:46:29.000000 tencentcloud-sdk-python-asr-3.0.886/tencentcloud/asr/v20190614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63416 2023-05-08 02:46:29.000000 tencentcloud-sdk-python-asr-3.0.886/tencentcloud/asr/v20190614/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 02:46:29.000000 tencentcloud-sdk-python-asr-3.0.886/tencentcloud/asr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 02:46:29.000000 tencentcloud-sdk-python-asr-3.0.886/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 02:46:29.000000 tencentcloud-sdk-python-asr-3.0.886/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-08 02:46:29.000000 tencentcloud-sdk-python-asr-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 02:46:29.000000 tencentcloud-sdk-python-asr-3.0.886/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:46:29.000000 tencentcloud-sdk-python-asr-3.0.886/tencentcloud_sdk_python_asr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 02:46:29.000000 tencentcloud-sdk-python-asr-3.0.886/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-08 02:46:29.000000 tencentcloud-sdk-python-asr-3.0.886/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 02:46:29.000000 tencentcloud-sdk-python-asr-3.0.886/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 02:46:29.000000 tencentcloud-sdk-python-asr-3.0.886/tencentcloud_sdk_python_asr.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-asr-3.0.884/README.rst` & `tencentcloud-sdk-python-asr-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.884/tencentcloud/asr/v20190614/asr_client.py` & `tencentcloud-sdk-python-asr-3.0.886/tencentcloud/asr/v20190614/asr_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,14 +370,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def GetModelInfo(self, request):
+        """通过自学习模型id获取自学习模型详细信息
+
+        :param request: Request instance for GetModelInfo.
+        :type request: :class:`tencentcloud.asr.v20190614.models.GetModelInfoRequest`
+        :rtype: :class:`tencentcloud.asr.v20190614.models.GetModelInfoResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("GetModelInfo", params, headers=headers)
+            response = json.loads(body)
+            model = models.GetModelInfoResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ModifyCustomization(self, request):
         """用户通过该接口可以更新自学习模型，如模型名称、模型类型、模型语料。
 
         :param request: Request instance for ModifyCustomization.
         :type request: :class:`tencentcloud.asr.v20190614.models.ModifyCustomizationRequest`
         :rtype: :class:`tencentcloud.asr.v20190614.models.ModifyCustomizationResponse`
```

### Comparing `tencentcloud-sdk-python-asr-3.0.884/tencentcloud/asr/v20190614/errorcodes.py` & `tencentcloud-sdk-python-asr-3.0.886/tencentcloud/asr/v20190614/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.884/tencentcloud/asr/v20190614/models.py` & `tencentcloud-sdk-python-asr-3.0.886/tencentcloud/asr/v20190614/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -928,14 +928,61 @@
                 obj = Model()
                 obj._deserialize(item)
                 self.Data.append(obj)
         self.TotalCount = params.get("TotalCount")
         self.RequestId = params.get("RequestId")
 
 
+class GetModelInfoRequest(AbstractModel):
+    """GetModelInfo请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ModelId: 模型id
+        :type ModelId: str
+        """
+        self.ModelId = None
+
+
+    def _deserialize(self, params):
+        self.ModelId = params.get("ModelId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class GetModelInfoResponse(AbstractModel):
+    """GetModelInfo返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Data: 模型信息
+        :type Data: :class:`tencentcloud.asr.v20190614.models.Model`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Data = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self.Data = Model()
+            self.Data._deserialize(params.get("Data"))
+        self.RequestId = params.get("RequestId")
+
+
 class HotWord(AbstractModel):
     """热词的词和权重
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-asr-3.0.884/tencentcloud/__init__.py` & `tencentcloud-sdk-python-asr-3.0.886/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.884'
+__version__ = '3.0.886'
```

### Comparing `tencentcloud-sdk-python-asr-3.0.884/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.886/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.884
+Version: 3.0.886
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.884/setup.py` & `tencentcloud-sdk-python-asr-3.0.886/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.884/tencentcloud_sdk_python_asr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.886/tencentcloud_sdk_python_asr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.884
+Version: 3.0.886
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

