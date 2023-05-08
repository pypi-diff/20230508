# Comparing `tmp/tencentcloud-sdk-python-ses-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-ses-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ses-3.0.885.tar", last modified: Mon May  1 00:48:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ses-3.0.886.tar", last modified: Mon May  8 03:52:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ses-3.0.885.tar` & `tencentcloud-sdk-python-ses-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:48:18.000000 tencentcloud-sdk-python-ses-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-01 00:48:18.000000 tencentcloud-sdk-python-ses-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:48:18.000000 tencentcloud-sdk-python-ses-3.0.885/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:48:18.000000 tencentcloud-sdk-python-ses-3.0.885/tencentcloud/ses/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:48:18.000000 tencentcloud-sdk-python-ses-3.0.885/tencentcloud/ses/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:48:18.000000 tencentcloud-sdk-python-ses-3.0.885/tencentcloud/ses/v20201002/
--rw-r--r--   0 root         (0) root         (0)    11392 2023-05-01 00:48:18.000000 tencentcloud-sdk-python-ses-3.0.885/tencentcloud/ses/v20201002/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    28299 2023-05-01 00:48:18.000000 tencentcloud-sdk-python-ses-3.0.885/tencentcloud/ses/v20201002/ses_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:48:18.000000 tencentcloud-sdk-python-ses-3.0.885/tencentcloud/ses/v20201002/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71316 2023-05-01 00:48:18.000000 tencentcloud-sdk-python-ses-3.0.885/tencentcloud/ses/v20201002/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:48:18.000000 tencentcloud-sdk-python-ses-3.0.885/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:48:18.000000 tencentcloud-sdk-python-ses-3.0.885/tencentcloud_sdk_python_ses.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:48:18.000000 tencentcloud-sdk-python-ses-3.0.885/tencentcloud_sdk_python_ses.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-01 00:48:18.000000 tencentcloud-sdk-python-ses-3.0.885/tencentcloud_sdk_python_ses.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:48:18.000000 tencentcloud-sdk-python-ses-3.0.885/tencentcloud_sdk_python_ses.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:48:18.000000 tencentcloud-sdk-python-ses-3.0.885/tencentcloud_sdk_python_ses.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:48:18.000000 tencentcloud-sdk-python-ses-3.0.885/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-01 00:48:18.000000 tencentcloud-sdk-python-ses-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:48:18.000000 tencentcloud-sdk-python-ses-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:52:06.000000 tencentcloud-sdk-python-ses-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-08 03:52:06.000000 tencentcloud-sdk-python-ses-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:52:06.000000 tencentcloud-sdk-python-ses-3.0.886/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:52:06.000000 tencentcloud-sdk-python-ses-3.0.886/tencentcloud/ses/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:52:06.000000 tencentcloud-sdk-python-ses-3.0.886/tencentcloud/ses/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:52:06.000000 tencentcloud-sdk-python-ses-3.0.886/tencentcloud/ses/v20201002/
+-rw-r--r--   0 root         (0) root         (0)    11392 2023-05-08 03:52:06.000000 tencentcloud-sdk-python-ses-3.0.886/tencentcloud/ses/v20201002/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    28299 2023-05-08 03:52:06.000000 tencentcloud-sdk-python-ses-3.0.886/tencentcloud/ses/v20201002/ses_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:52:06.000000 tencentcloud-sdk-python-ses-3.0.886/tencentcloud/ses/v20201002/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71414 2023-05-08 03:52:06.000000 tencentcloud-sdk-python-ses-3.0.886/tencentcloud/ses/v20201002/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 03:52:06.000000 tencentcloud-sdk-python-ses-3.0.886/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:52:06.000000 tencentcloud-sdk-python-ses-3.0.886/tencentcloud_sdk_python_ses.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 03:52:06.000000 tencentcloud-sdk-python-ses-3.0.886/tencentcloud_sdk_python_ses.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-08 03:52:06.000000 tencentcloud-sdk-python-ses-3.0.886/tencentcloud_sdk_python_ses.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 03:52:06.000000 tencentcloud-sdk-python-ses-3.0.886/tencentcloud_sdk_python_ses.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 03:52:06.000000 tencentcloud-sdk-python-ses-3.0.886/tencentcloud_sdk_python_ses.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 03:52:06.000000 tencentcloud-sdk-python-ses-3.0.886/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-08 03:52:06.000000 tencentcloud-sdk-python-ses-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 03:52:06.000000 tencentcloud-sdk-python-ses-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ses-3.0.885/README.rst` & `tencentcloud-sdk-python-ses-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ses-3.0.885/tencentcloud/ses/v20201002/errorcodes.py` & `tencentcloud-sdk-python-ses-3.0.886/tencentcloud/ses/v20201002/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ses-3.0.885/tencentcloud/ses/v20201002/ses_client.py` & `tencentcloud-sdk-python-ses-3.0.886/tencentcloud/ses/v20201002/ses_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ses-3.0.885/tencentcloud/ses/v20201002/models.py` & `tencentcloud-sdk-python-ses-3.0.886/tencentcloud/ses/v20201002/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1509,15 +1509,15 @@
         :type ReplyToAddresses: str
         :param Template: 使用模板发送时，填写的模板相关参数。因 Simple 已经废除使用，Template 为必填项
         :type Template: :class:`tencentcloud.ses.v20201002.models.Template`
         :param Simple: 已废弃
         :type Simple: :class:`tencentcloud.ses.v20201002.models.Simple`
         :param Attachments: 需要发送附件时，填写附件相关参数。腾讯云接口请求最大支持 8M 的请求包，附件内容经过 Base64 预期扩大1.5倍，应该控制所有附件的总大小最大在 4M 以内，整体请求超出 8M 时接口会返回错误
         :type Attachments: list of Attachment
-        :param Unsubscribe: 退订选项 1: 加入退订链接 0: 不加入退订链接
+        :param Unsubscribe: 退订链接选项 0: 不加入退订链接 1: 简体中文 2: 英文 3: 繁体中文 4: 西班牙语 5: 法语 6: 德语 7: 日语 8: 韩语 9: 阿拉伯语
         :type Unsubscribe: str
         :param TriggerType: 邮件触发类型 0:非触发类，默认类型，营销类邮件、非即时类邮件等选择此类型  1:触发类，验证码等即时发送类邮件，若邮件超过一定大小，系统会自动选择非触发类型通道
         :type TriggerType: int
         """
         self.FromEmailAddress = None
         self.Destination = None
         self.Subject = None
```

### Comparing `tencentcloud-sdk-python-ses-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ses-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ses-3.0.885/tencentcloud_sdk_python_ses.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ses-3.0.886/tencentcloud_sdk_python_ses.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ses
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Ses SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ses-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-ses-3.0.886/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ses
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Ses SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ses-3.0.885/setup.py` & `tencentcloud-sdk-python-ses-3.0.886/setup.py`

 * *Files identical despite different names*

