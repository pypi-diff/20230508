# Comparing `tmp/tencentcloud-sdk-python-trtc-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-trtc-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.885.tar", last modified: Mon May  1 00:58:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.886.tar", last modified: Mon May  8 04:17:56 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trtc-3.0.885.tar` & `tencentcloud-sdk-python-trtc-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:58:04.000000 tencentcloud-sdk-python-trtc-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-01 00:58:04.000000 tencentcloud-sdk-python-trtc-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:58:04.000000 tencentcloud-sdk-python-trtc-3.0.885/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:58:04.000000 tencentcloud-sdk-python-trtc-3.0.885/tencentcloud/trtc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:58:04.000000 tencentcloud-sdk-python-trtc-3.0.885/tencentcloud/trtc/v20190722/
--rw-r--r--   0 root         (0) root         (0)     9679 2023-05-01 00:58:04.000000 tencentcloud-sdk-python-trtc-3.0.885/tencentcloud/trtc/v20190722/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:58:04.000000 tencentcloud-sdk-python-trtc-3.0.885/tencentcloud/trtc/v20190722/__init__.py
--rw-r--r--   0 root         (0) root         (0)   199055 2023-05-01 00:58:04.000000 tencentcloud-sdk-python-trtc-3.0.885/tencentcloud/trtc/v20190722/models.py
--rw-r--r--   0 root         (0) root         (0)    58535 2023-05-01 00:58:04.000000 tencentcloud-sdk-python-trtc-3.0.885/tencentcloud/trtc/v20190722/trtc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:58:04.000000 tencentcloud-sdk-python-trtc-3.0.885/tencentcloud/trtc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:58:04.000000 tencentcloud-sdk-python-trtc-3.0.885/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:58:04.000000 tencentcloud-sdk-python-trtc-3.0.885/tencentcloud_sdk_python_trtc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:58:04.000000 tencentcloud-sdk-python-trtc-3.0.885/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-01 00:58:04.000000 tencentcloud-sdk-python-trtc-3.0.885/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-01 00:58:04.000000 tencentcloud-sdk-python-trtc-3.0.885/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:58:04.000000 tencentcloud-sdk-python-trtc-3.0.885/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-01 00:58:04.000000 tencentcloud-sdk-python-trtc-3.0.885/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-01 00:58:04.000000 tencentcloud-sdk-python-trtc-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:58:04.000000 tencentcloud-sdk-python-trtc-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:17:56.000000 tencentcloud-sdk-python-trtc-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-08 04:17:56.000000 tencentcloud-sdk-python-trtc-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:17:56.000000 tencentcloud-sdk-python-trtc-3.0.886/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:17:56.000000 tencentcloud-sdk-python-trtc-3.0.886/tencentcloud/trtc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:17:56.000000 tencentcloud-sdk-python-trtc-3.0.886/tencentcloud/trtc/v20190722/
+-rw-r--r--   0 root         (0) root         (0)     9679 2023-05-08 04:17:56.000000 tencentcloud-sdk-python-trtc-3.0.886/tencentcloud/trtc/v20190722/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:17:56.000000 tencentcloud-sdk-python-trtc-3.0.886/tencentcloud/trtc/v20190722/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   199052 2023-05-08 04:17:56.000000 tencentcloud-sdk-python-trtc-3.0.886/tencentcloud/trtc/v20190722/models.py
+-rw-r--r--   0 root         (0) root         (0)    58535 2023-05-08 04:17:56.000000 tencentcloud-sdk-python-trtc-3.0.886/tencentcloud/trtc/v20190722/trtc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:17:56.000000 tencentcloud-sdk-python-trtc-3.0.886/tencentcloud/trtc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 04:17:56.000000 tencentcloud-sdk-python-trtc-3.0.886/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:17:56.000000 tencentcloud-sdk-python-trtc-3.0.886/tencentcloud_sdk_python_trtc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 04:17:56.000000 tencentcloud-sdk-python-trtc-3.0.886/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-08 04:17:56.000000 tencentcloud-sdk-python-trtc-3.0.886/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-08 04:17:56.000000 tencentcloud-sdk-python-trtc-3.0.886/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 04:17:56.000000 tencentcloud-sdk-python-trtc-3.0.886/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-08 04:17:56.000000 tencentcloud-sdk-python-trtc-3.0.886/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-08 04:17:56.000000 tencentcloud-sdk-python-trtc-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 04:17:56.000000 tencentcloud-sdk-python-trtc-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.885/README.rst` & `tencentcloud-sdk-python-trtc-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.885/tencentcloud/trtc/v20190722/errorcodes.py` & `tencentcloud-sdk-python-trtc-3.0.886/tencentcloud/trtc/v20190722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.885/tencentcloud/trtc/v20190722/models.py` & `tencentcloud-sdk-python-trtc-3.0.886/tencentcloud/trtc/v20190722/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1175,15 +1175,15 @@
         r"""
         :param SdkAppId: 用户SdkAppId（如：1400xxxxxx）
         :type SdkAppId: int
         :param StartTime: 查询开始时间，本地unix时间戳，单位为秒（如：1590065777）
 注意：支持查询14天内的数据。
         :type StartTime: int
         :param EndTime: 查询结束时间，本地unix时间戳，单位为秒（如：1590065877），建议与StartTime间隔时间超过24小时。
-注意：按天统计，结束时间小于前一天，否则查询数据为空（如：需查询20号数据，结束时间需晚于20号0点）。
+注意：按天统计，结束时间大于前一天，否则查询数据为空（如：需查询20号数据，结束时间需晚于20号0点）。
         :type EndTime: int
         """
         self.SdkAppId = None
         self.StartTime = None
         self.EndTime = None
 
 
@@ -2139,15 +2139,15 @@
         :type PresetLayoutConfig: list of PresetLayoutConfig
         :param PlaceHolderMode: 自定义模板中有效，设置为1时代表启用占位图功能，0时代表不启用占位图功能，默认为0。启用占位图功能时，在预设位置的用户没有上行视频时可显示对应的占位图。
         :type PlaceHolderMode: int
         :param PureAudioHoldPlaceMode: 悬浮模板、九宫格、屏幕分享模板生效，用于控制纯音频上行是否占用画面布局位置。设置为0是代表后台默认处理方式，悬浮小画面占布局位置，九宫格画面占布局位置、屏幕分享小画面不占布局位置；设置为1时代表纯音频上行占布局位置；设置为2时代表纯音频上行不占布局位置。默认为0。
         :type PureAudioHoldPlaceMode: int
         :param WaterMarkParams: 水印参数。
         :type WaterMarkParams: :class:`tencentcloud.trtc.v20190722.models.WaterMarkParams`
-        :param RenderMode: 屏幕分享模板、悬浮模板、九宫格模板、画中画模版有效，画面在输出时的显示模式：0为裁剪，1为缩放，2为缩放并显示黑底，不填采用后台的默认渲染方式（屏幕分享大画面为缩放，其他为裁剪）。若此参数不生效，请请提交工单寻求帮助。
+        :param RenderMode: 屏幕分享模板、悬浮模板、九宫格模板、画中画模版有效，画面在输出时的显示模式：0为裁剪，1为缩放，2为缩放并显示黑底，不填采用后台的默认渲染方式（屏幕分享大画面为缩放，其他为裁剪）。若此参数不生效，请提交工单寻求帮助。
         :type RenderMode: int
         """
         self.Template = None
         self.MainVideoUserId = None
         self.MainVideoStreamType = None
         self.SmallVideoLayoutParams = None
         self.MainVideoRightAlign = None
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.885/tencentcloud/trtc/v20190722/trtc_client.py` & `tencentcloud-sdk-python-trtc-3.0.886/tencentcloud/trtc/v20190722/trtc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trtc-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trtc-3.0.885/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.886/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.886/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.885/setup.py` & `tencentcloud-sdk-python-trtc-3.0.886/setup.py`

 * *Files identical despite different names*

