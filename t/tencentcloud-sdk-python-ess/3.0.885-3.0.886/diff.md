# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.885.tar", last modified: Mon May  1 00:39:53 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.886.tar", last modified: Mon May  8 03:15:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.885.tar` & `tencentcloud-sdk-python-ess-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:39:53.000000 tencentcloud-sdk-python-ess-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-01 00:39:53.000000 tencentcloud-sdk-python-ess-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:39:53.000000 tencentcloud-sdk-python-ess-3.0.885/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:39:53.000000 tencentcloud-sdk-python-ess-3.0.885/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:39:53.000000 tencentcloud-sdk-python-ess-3.0.885/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:39:53.000000 tencentcloud-sdk-python-ess-3.0.885/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:39:53.000000 tencentcloud-sdk-python-ess-3.0.885/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    49606 2023-05-01 00:39:53.000000 tencentcloud-sdk-python-ess-3.0.885/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    23727 2023-05-01 00:39:53.000000 tencentcloud-sdk-python-ess-3.0.885/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:39:53.000000 tencentcloud-sdk-python-ess-3.0.885/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   219543 2023-05-01 00:39:53.000000 tencentcloud-sdk-python-ess-3.0.885/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:39:53.000000 tencentcloud-sdk-python-ess-3.0.885/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:39:53.000000 tencentcloud-sdk-python-ess-3.0.885/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-01 00:39:53.000000 tencentcloud-sdk-python-ess-3.0.885/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:39:53.000000 tencentcloud-sdk-python-ess-3.0.885/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:39:53.000000 tencentcloud-sdk-python-ess-3.0.885/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:39:53.000000 tencentcloud-sdk-python-ess-3.0.885/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-01 00:39:53.000000 tencentcloud-sdk-python-ess-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:39:53.000000 tencentcloud-sdk-python-ess-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:15:21.000000 tencentcloud-sdk-python-ess-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-08 03:15:21.000000 tencentcloud-sdk-python-ess-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:15:21.000000 tencentcloud-sdk-python-ess-3.0.886/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 03:15:21.000000 tencentcloud-sdk-python-ess-3.0.886/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:15:21.000000 tencentcloud-sdk-python-ess-3.0.886/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:15:21.000000 tencentcloud-sdk-python-ess-3.0.886/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:15:21.000000 tencentcloud-sdk-python-ess-3.0.886/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    49606 2023-05-08 03:15:21.000000 tencentcloud-sdk-python-ess-3.0.886/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    23727 2023-05-08 03:15:21.000000 tencentcloud-sdk-python-ess-3.0.886/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:15:21.000000 tencentcloud-sdk-python-ess-3.0.886/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   220367 2023-05-08 03:15:21.000000 tencentcloud-sdk-python-ess-3.0.886/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:15:21.000000 tencentcloud-sdk-python-ess-3.0.886/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 03:15:21.000000 tencentcloud-sdk-python-ess-3.0.886/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-08 03:15:21.000000 tencentcloud-sdk-python-ess-3.0.886/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 03:15:21.000000 tencentcloud-sdk-python-ess-3.0.886/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 03:15:21.000000 tencentcloud-sdk-python-ess-3.0.886/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 03:15:21.000000 tencentcloud-sdk-python-ess-3.0.886/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-08 03:15:21.000000 tencentcloud-sdk-python-ess-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 03:15:21.000000 tencentcloud-sdk-python-ess-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.885/README.rst` & `tencentcloud-sdk-python-ess-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.885/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.886/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.885/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.886/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.885/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.886/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1587,34 +1587,40 @@
         r"""
         :param FlowId: 流程编号
         :type FlowId: str
         :param FlowApproverInfos: 流程签署人，其中ApproverName，ApproverMobile和ApproverType必传，其他可不传，ApproverType目前只支持个人类型的签署人。还需注意签署人只能有手写签名和时间类型的签署控件，其他类型的填写控件和签署控件暂时都未支持。
         :type FlowApproverInfos: list of FlowCreateApprover
         :param Operator: 用户信息，此结构体UserId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param Organization: 机构信息，暂未开放
         :type Organization: :class:`tencentcloud.ess.v20201111.models.OrganizationInfo`
         """
         self.FlowId = None
         self.FlowApproverInfos = None
         self.Operator = None
+        self.Agent = None
         self.Organization = None
 
 
     def _deserialize(self, params):
         self.FlowId = params.get("FlowId")
         if params.get("FlowApproverInfos") is not None:
             self.FlowApproverInfos = []
             for item in params.get("FlowApproverInfos"):
                 obj = FlowCreateApprover()
                 obj._deserialize(item)
                 self.FlowApproverInfos.append(obj)
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
+        if params.get("Agent") is not None:
+            self.Agent = Agent()
+            self.Agent._deserialize(params.get("Agent"))
         if params.get("Organization") is not None:
             self.Organization = OrganizationInfo()
             self.Organization._deserialize(params.get("Organization"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
@@ -3979,38 +3985,43 @@
 class FlowApproverUrlInfo(AbstractModel):
     """签署链接信息
 
     """
 
     def __init__(self):
         r"""
-        :param SignUrl: 签署链接，注意该链接有效期为30分钟，同时需要注意保密，不要外泄给无关用户。
+        :param SignUrl: 签署链接。注意该链接有效期为30分钟，同时需要注意保密，不要外泄给无关用户。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SignUrl: str
-        :param ApproverMobile: 签署人手机号
+        :param ApproverType: 签署人类型 1-个人
 注意：此字段可能返回 null，表示取不到有效值。
-        :type ApproverMobile: str
+        :type ApproverType: int
         :param ApproverName: 签署人姓名
 注意：此字段可能返回 null，表示取不到有效值。
         :type ApproverName: str
-        :param ApproverType: 签署人类型 1-个人
+        :param ApproverMobile: 签署人手机号
 注意：此字段可能返回 null，表示取不到有效值。
-        :type ApproverType: int
+        :type ApproverMobile: str
+        :param LongUrl: 签署长链接。注意该链接有效期为30分钟，同时需要注意保密，不要外泄给无关用户。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LongUrl: str
         """
         self.SignUrl = None
-        self.ApproverMobile = None
-        self.ApproverName = None
         self.ApproverType = None
+        self.ApproverName = None
+        self.ApproverMobile = None
+        self.LongUrl = None
 
 
     def _deserialize(self, params):
         self.SignUrl = params.get("SignUrl")
-        self.ApproverMobile = params.get("ApproverMobile")
-        self.ApproverName = params.get("ApproverName")
         self.ApproverType = params.get("ApproverType")
+        self.ApproverName = params.get("ApproverName")
+        self.ApproverMobile = params.get("ApproverMobile")
+        self.LongUrl = params.get("LongUrl")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4127,14 +4138,16 @@
         :type ApproverSource: str
         :param CustomApproverTag: 客户自定义签署人标识，64位长度，保证唯一。非企微场景不使用此字段
         :type CustomApproverTag: str
         :param RegisterInfo: 快速注册相关信息，目前暂未开放！
         :type RegisterInfo: :class:`tencentcloud.ess.v20201111.models.RegisterInfo`
         :param ApproverOption: 签署人个性化能力值
         :type ApproverOption: :class:`tencentcloud.ess.v20201111.models.ApproverOption`
+        :param JumpUrl: 签署完前端跳转的url，暂未使用
+        :type JumpUrl: str
         """
         self.ApproverType = None
         self.OrganizationName = None
         self.ApproverName = None
         self.ApproverMobile = None
         self.ApproverIdCardType = None
         self.ApproverIdCardNumber = None
@@ -4145,14 +4158,15 @@
         self.PreReadTime = None
         self.UserId = None
         self.Required = None
         self.ApproverSource = None
         self.CustomApproverTag = None
         self.RegisterInfo = None
         self.ApproverOption = None
+        self.JumpUrl = None
 
 
     def _deserialize(self, params):
         self.ApproverType = params.get("ApproverType")
         self.OrganizationName = params.get("OrganizationName")
         self.ApproverName = params.get("ApproverName")
         self.ApproverMobile = params.get("ApproverMobile")
@@ -4169,14 +4183,15 @@
         self.CustomApproverTag = params.get("CustomApproverTag")
         if params.get("RegisterInfo") is not None:
             self.RegisterInfo = RegisterInfo()
             self.RegisterInfo._deserialize(params.get("RegisterInfo"))
         if params.get("ApproverOption") is not None:
             self.ApproverOption = ApproverOption()
             self.ApproverOption._deserialize(params.get("ApproverOption"))
+        self.JumpUrl = params.get("JumpUrl")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ess-3.0.885/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.886/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.886/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.885/setup.py` & `tencentcloud-sdk-python-ess-3.0.886/setup.py`

 * *Files identical despite different names*

