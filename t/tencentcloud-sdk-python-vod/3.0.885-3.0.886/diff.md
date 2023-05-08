# Comparing `tmp/tencentcloud-sdk-python-vod-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-vod-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.885.tar", last modified: Mon May  1 00:59:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.886.tar", last modified: Mon May  8 04:21:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vod-3.0.885.tar` & `tencentcloud-sdk-python-vod-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:59:02.000000 tencentcloud-sdk-python-vod-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-01 00:59:02.000000 tencentcloud-sdk-python-vod-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:59:02.000000 tencentcloud-sdk-python-vod-3.0.885/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:59:02.000000 tencentcloud-sdk-python-vod-3.0.885/tencentcloud/vod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:59:02.000000 tencentcloud-sdk-python-vod-3.0.885/tencentcloud/vod/v20180717/
--rw-r--r--   0 root         (0) root         (0)   172410 2023-05-01 00:59:02.000000 tencentcloud-sdk-python-vod-3.0.885/tencentcloud/vod/v20180717/vod_client.py
--rw-r--r--   0 root         (0) root         (0)    25111 2023-05-01 00:59:02.000000 tencentcloud-sdk-python-vod-3.0.885/tencentcloud/vod/v20180717/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:59:02.000000 tencentcloud-sdk-python-vod-3.0.885/tencentcloud/vod/v20180717/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1171841 2023-05-01 00:59:02.000000 tencentcloud-sdk-python-vod-3.0.885/tencentcloud/vod/v20180717/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:59:02.000000 tencentcloud-sdk-python-vod-3.0.885/tencentcloud/vod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:59:02.000000 tencentcloud-sdk-python-vod-3.0.885/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:59:02.000000 tencentcloud-sdk-python-vod-3.0.885/tencentcloud_sdk_python_vod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:59:02.000000 tencentcloud-sdk-python-vod-3.0.885/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-01 00:59:02.000000 tencentcloud-sdk-python-vod-3.0.885/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:59:02.000000 tencentcloud-sdk-python-vod-3.0.885/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:59:02.000000 tencentcloud-sdk-python-vod-3.0.885/tencentcloud_sdk_python_vod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:59:02.000000 tencentcloud-sdk-python-vod-3.0.885/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-01 00:59:02.000000 tencentcloud-sdk-python-vod-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:59:02.000000 tencentcloud-sdk-python-vod-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:21:50.000000 tencentcloud-sdk-python-vod-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-08 04:21:50.000000 tencentcloud-sdk-python-vod-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:21:50.000000 tencentcloud-sdk-python-vod-3.0.886/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:21:50.000000 tencentcloud-sdk-python-vod-3.0.886/tencentcloud/vod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:21:50.000000 tencentcloud-sdk-python-vod-3.0.886/tencentcloud/vod/v20180717/
+-rw-r--r--   0 root         (0) root         (0)   172410 2023-05-08 04:21:50.000000 tencentcloud-sdk-python-vod-3.0.886/tencentcloud/vod/v20180717/vod_client.py
+-rw-r--r--   0 root         (0) root         (0)    25111 2023-05-08 04:21:50.000000 tencentcloud-sdk-python-vod-3.0.886/tencentcloud/vod/v20180717/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:21:50.000000 tencentcloud-sdk-python-vod-3.0.886/tencentcloud/vod/v20180717/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1171923 2023-05-08 04:21:50.000000 tencentcloud-sdk-python-vod-3.0.886/tencentcloud/vod/v20180717/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:21:50.000000 tencentcloud-sdk-python-vod-3.0.886/tencentcloud/vod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 04:21:50.000000 tencentcloud-sdk-python-vod-3.0.886/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:21:50.000000 tencentcloud-sdk-python-vod-3.0.886/tencentcloud_sdk_python_vod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 04:21:50.000000 tencentcloud-sdk-python-vod-3.0.886/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-08 04:21:50.000000 tencentcloud-sdk-python-vod-3.0.886/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 04:21:50.000000 tencentcloud-sdk-python-vod-3.0.886/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 04:21:50.000000 tencentcloud-sdk-python-vod-3.0.886/tencentcloud_sdk_python_vod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 04:21:50.000000 tencentcloud-sdk-python-vod-3.0.886/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-08 04:21:50.000000 tencentcloud-sdk-python-vod-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 04:21:50.000000 tencentcloud-sdk-python-vod-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vod-3.0.885/README.rst` & `tencentcloud-sdk-python-vod-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.885/tencentcloud/vod/v20180717/vod_client.py` & `tencentcloud-sdk-python-vod-3.0.886/tencentcloud/vod/v20180717/vod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.885/tencentcloud/vod/v20180717/errorcodes.py` & `tencentcloud-sdk-python-vod-3.0.886/tencentcloud/vod/v20180717/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.885/tencentcloud/vod/v20180717/models.py` & `tencentcloud-sdk-python-vod-3.0.886/tencentcloud/vod/v20180717/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -9428,14 +9428,15 @@
 
     def __init__(self):
         r"""
         :param Metric: 查询指标，取值有：
 <li>Traffic：流量，单位为 Byte。</li>
 <li>Bandwidth：带宽，单位为 Bps。</li>
 <li>Requests：请求数。</li>
+<li>QUICRequests：QUIC 请求数。</li>
         :type Metric: str
         :param StartTime: 起始时间，使用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
         :type StartTime: str
         :param EndTime: 结束时间，使用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
         :type EndTime: str
         :param SubAppId: <b>点播[子应用](/document/product/266/14574) ID。如果要访问子应用中的资源，则将该字段填写为子应用 ID；否则无需填写该字段。</b>
         :type SubAppId: int
@@ -25800,14 +25801,15 @@
         :type Time: str
         :param Value: 数据大小。
 <li>存储空间的数据，单位是字节。</li>
 <li>转码时长的数据，单位是秒。</li>
 <li>流量数据，单位是字节。</li>
 <li>带宽数据，单位是比特每秒。</li>
 <li>直播剪辑数据，单位是秒。</li>
+<li>轮播数据，单位是秒。</li>
         :type Value: int
         """
         self.Time = None
         self.Value = None
 
 
     def _deserialize(self, params):
```

### Comparing `tencentcloud-sdk-python-vod-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vod-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vod-3.0.885/tencentcloud_sdk_python_vod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.886/tencentcloud_sdk_python_vod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.886/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.885/setup.py` & `tencentcloud-sdk-python-vod-3.0.886/setup.py`

 * *Files identical despite different names*

