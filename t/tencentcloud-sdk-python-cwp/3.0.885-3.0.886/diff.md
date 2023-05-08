# Comparing `tmp/tencentcloud-sdk-python-cwp-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-cwp-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cwp-3.0.885.tar", last modified: Mon May  1 00:33:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cwp-3.0.886.tar", last modified: Mon May  8 03:11:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cwp-3.0.885.tar` & `tencentcloud-sdk-python-cwp-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:33:59.000000 tencentcloud-sdk-python-cwp-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-01 00:33:59.000000 tencentcloud-sdk-python-cwp-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:33:59.000000 tencentcloud-sdk-python-cwp-3.0.885/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:33:59.000000 tencentcloud-sdk-python-cwp-3.0.885/tencentcloud/cwp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:33:59.000000 tencentcloud-sdk-python-cwp-3.0.885/tencentcloud/cwp/v20180228/
--rw-r--r--   0 root         (0) root         (0)     3900 2023-05-01 00:33:59.000000 tencentcloud-sdk-python-cwp-3.0.885/tencentcloud/cwp/v20180228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   250541 2023-05-01 00:33:59.000000 tencentcloud-sdk-python-cwp-3.0.885/tencentcloud/cwp/v20180228/cwp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:33:59.000000 tencentcloud-sdk-python-cwp-3.0.885/tencentcloud/cwp/v20180228/__init__.py
--rw-r--r--   0 root         (0) root         (0)   901827 2023-05-01 00:33:59.000000 tencentcloud-sdk-python-cwp-3.0.885/tencentcloud/cwp/v20180228/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:33:59.000000 tencentcloud-sdk-python-cwp-3.0.885/tencentcloud/cwp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:33:59.000000 tencentcloud-sdk-python-cwp-3.0.885/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:33:59.000000 tencentcloud-sdk-python-cwp-3.0.885/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:33:59.000000 tencentcloud-sdk-python-cwp-3.0.885/tencentcloud_sdk_python_cwp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:33:59.000000 tencentcloud-sdk-python-cwp-3.0.885/tencentcloud_sdk_python_cwp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-01 00:33:59.000000 tencentcloud-sdk-python-cwp-3.0.885/tencentcloud_sdk_python_cwp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:33:59.000000 tencentcloud-sdk-python-cwp-3.0.885/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:33:59.000000 tencentcloud-sdk-python-cwp-3.0.885/tencentcloud_sdk_python_cwp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-01 00:33:59.000000 tencentcloud-sdk-python-cwp-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:33:59.000000 tencentcloud-sdk-python-cwp-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:11:54.000000 tencentcloud-sdk-python-cwp-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-08 03:11:54.000000 tencentcloud-sdk-python-cwp-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:11:54.000000 tencentcloud-sdk-python-cwp-3.0.886/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:11:54.000000 tencentcloud-sdk-python-cwp-3.0.886/tencentcloud/cwp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:11:54.000000 tencentcloud-sdk-python-cwp-3.0.886/tencentcloud/cwp/v20180228/
+-rw-r--r--   0 root         (0) root         (0)     3900 2023-05-08 03:11:54.000000 tencentcloud-sdk-python-cwp-3.0.886/tencentcloud/cwp/v20180228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   250541 2023-05-08 03:11:54.000000 tencentcloud-sdk-python-cwp-3.0.886/tencentcloud/cwp/v20180228/cwp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:11:54.000000 tencentcloud-sdk-python-cwp-3.0.886/tencentcloud/cwp/v20180228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   903384 2023-05-08 03:11:54.000000 tencentcloud-sdk-python-cwp-3.0.886/tencentcloud/cwp/v20180228/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:11:54.000000 tencentcloud-sdk-python-cwp-3.0.886/tencentcloud/cwp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 03:11:54.000000 tencentcloud-sdk-python-cwp-3.0.886/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 03:11:54.000000 tencentcloud-sdk-python-cwp-3.0.886/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:11:54.000000 tencentcloud-sdk-python-cwp-3.0.886/tencentcloud_sdk_python_cwp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 03:11:54.000000 tencentcloud-sdk-python-cwp-3.0.886/tencentcloud_sdk_python_cwp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-08 03:11:54.000000 tencentcloud-sdk-python-cwp-3.0.886/tencentcloud_sdk_python_cwp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 03:11:54.000000 tencentcloud-sdk-python-cwp-3.0.886/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 03:11:54.000000 tencentcloud-sdk-python-cwp-3.0.886/tencentcloud_sdk_python_cwp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-08 03:11:54.000000 tencentcloud-sdk-python-cwp-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 03:11:54.000000 tencentcloud-sdk-python-cwp-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.885/README.rst` & `tencentcloud-sdk-python-cwp-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.885/tencentcloud/cwp/v20180228/errorcodes.py` & `tencentcloud-sdk-python-cwp-3.0.886/tencentcloud/cwp/v20180228/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.885/tencentcloud/cwp/v20180228/cwp_client.py` & `tencentcloud-sdk-python-cwp-3.0.886/tencentcloud/cwp/v20180228/cwp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.885/tencentcloud/cwp/v20180228/models.py` & `tencentcloud-sdk-python-cwp-3.0.886/tencentcloud/cwp/v20180228/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -13465,14 +13465,16 @@
         :type CwpVersionLicenseCnt: int
         :param AvailableLHLicenseCnt: 可用惠普版授权数
         :type AvailableLHLicenseCnt: int
         :param AutoRepurchaseSwitch: 自动加购开关, true 开启, false 关闭
         :type AutoRepurchaseSwitch: bool
         :param AutoRepurchaseRenewSwitch: 自动加购订单是否自动续费 ,true 开启, false 关闭
         :type AutoRepurchaseRenewSwitch: bool
+        :param DestroyOrderNum: 已销毁订单数
+        :type DestroyOrderNum: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.LicenseCnt = None
         self.AvailableLicenseCnt = None
         self.AvailableProVersionLicenseCnt = None
         self.AvailableFlagshipVersionLicenseCnt = None
@@ -13485,14 +13487,15 @@
         self.NotExpiredLicenseCnt = None
         self.FlagshipVersionLicenseCnt = None
         self.ProVersionLicenseCnt = None
         self.CwpVersionLicenseCnt = None
         self.AvailableLHLicenseCnt = None
         self.AutoRepurchaseSwitch = None
         self.AutoRepurchaseRenewSwitch = None
+        self.DestroyOrderNum = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.LicenseCnt = params.get("LicenseCnt")
         self.AvailableLicenseCnt = params.get("AvailableLicenseCnt")
         self.AvailableProVersionLicenseCnt = params.get("AvailableProVersionLicenseCnt")
@@ -13506,14 +13509,15 @@
         self.NotExpiredLicenseCnt = params.get("NotExpiredLicenseCnt")
         self.FlagshipVersionLicenseCnt = params.get("FlagshipVersionLicenseCnt")
         self.ProVersionLicenseCnt = params.get("ProVersionLicenseCnt")
         self.CwpVersionLicenseCnt = params.get("CwpVersionLicenseCnt")
         self.AvailableLHLicenseCnt = params.get("AvailableLHLicenseCnt")
         self.AutoRepurchaseSwitch = params.get("AutoRepurchaseSwitch")
         self.AutoRepurchaseRenewSwitch = params.get("AutoRepurchaseRenewSwitch")
+        self.DestroyOrderNum = params.get("DestroyOrderNum")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeLicenseListRequest(AbstractModel):
     """DescribeLicenseList请求参数结构体
 
     """
@@ -21470,14 +21474,16 @@
         :type Id: int
         :param CreateTime: 创建时间
         :type CreateTime: str
         :param ModifyTime: 最近修改时间
         :type ModifyTime: str
         :param Uuid: 服务器Uuid
         :type Uuid: str
+        :param Locations: 登陆地
+        :type Locations: str
         """
         self.Places = None
         self.UserName = None
         self.SrcIp = None
         self.Locale = None
         self.Remark = None
         self.StartTime = None
@@ -21485,14 +21491,15 @@
         self.IsGlobal = None
         self.Name = None
         self.Desc = None
         self.Id = None
         self.CreateTime = None
         self.ModifyTime = None
         self.Uuid = None
+        self.Locations = None
 
 
     def _deserialize(self, params):
         if params.get("Places") is not None:
             self.Places = []
             for item in params.get("Places"):
                 obj = Place()
@@ -21507,14 +21514,15 @@
         self.IsGlobal = params.get("IsGlobal")
         self.Name = params.get("Name")
         self.Desc = params.get("Desc")
         self.Id = params.get("Id")
         self.CreateTime = params.get("CreateTime")
         self.ModifyTime = params.get("ModifyTime")
         self.Uuid = params.get("Uuid")
+        self.Locations = params.get("Locations")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -23652,36 +23660,56 @@
         :type Id: str
         :param ProtectStatus: 防护状态
         :type ProtectStatus: int
         :param ProtectException: 防护异常
         :type ProtectException: int
         :param AutoRestoreSwitchStatus: 自动恢复开关 (Filters 过滤Quuid 时 返回) 默认0
         :type AutoRestoreSwitchStatus: int
+        :param FirstProtectTime: 首次开启防护时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FirstProtectTime: str
+        :param LatestProtectTime: 最近开启防护时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LatestProtectTime: str
+        :param ProtectFileType: 防护文件类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProtectFileType: str
+        :param ProtectFilesCount: 防护文件总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProtectFilesCount: int
         """
         self.DirName = None
         self.DirPath = None
         self.RelatedServerNum = None
         self.ProtectServerNum = None
         self.NoProtectServerNum = None
         self.Id = None
         self.ProtectStatus = None
         self.ProtectException = None
         self.AutoRestoreSwitchStatus = None
+        self.FirstProtectTime = None
+        self.LatestProtectTime = None
+        self.ProtectFileType = None
+        self.ProtectFilesCount = None
 
 
     def _deserialize(self, params):
         self.DirName = params.get("DirName")
         self.DirPath = params.get("DirPath")
         self.RelatedServerNum = params.get("RelatedServerNum")
         self.ProtectServerNum = params.get("ProtectServerNum")
         self.NoProtectServerNum = params.get("NoProtectServerNum")
         self.Id = params.get("Id")
         self.ProtectStatus = params.get("ProtectStatus")
         self.ProtectException = params.get("ProtectException")
         self.AutoRestoreSwitchStatus = params.get("AutoRestoreSwitchStatus")
+        self.FirstProtectTime = params.get("FirstProtectTime")
+        self.LatestProtectTime = params.get("LatestProtectTime")
+        self.ProtectFileType = params.get("ProtectFileType")
+        self.ProtectFilesCount = params.get("ProtectFilesCount")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -23790,25 +23818,29 @@
         :param Id: 唯一ID
         :type Id: int
         :param FileType: 文件类型 0-常规文件；1-目录；2-软链
         :type FileType: int
         :param MachineExtraInfo: 主机额外信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type MachineExtraInfo: :class:`tencentcloud.cwp.v20180228.models.MachineExtraInfo`
+        :param Quuid: 机器实例uuid
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Quuid: str
         """
         self.HostName = None
         self.HostIp = None
         self.EventDir = None
         self.EventType = None
         self.EventStatus = None
         self.CreateTime = None
         self.RestoreTime = None
         self.Id = None
         self.FileType = None
         self.MachineExtraInfo = None
+        self.Quuid = None
 
 
     def _deserialize(self, params):
         self.HostName = params.get("HostName")
         self.HostIp = params.get("HostIp")
         self.EventDir = params.get("EventDir")
         self.EventType = params.get("EventType")
@@ -23816,14 +23848,15 @@
         self.CreateTime = params.get("CreateTime")
         self.RestoreTime = params.get("RestoreTime")
         self.Id = params.get("Id")
         self.FileType = params.get("FileType")
         if params.get("MachineExtraInfo") is not None:
             self.MachineExtraInfo = MachineExtraInfo()
             self.MachineExtraInfo._deserialize(params.get("MachineExtraInfo"))
+        self.Quuid = params.get("Quuid")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cwp-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cwp-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-cwp-3.0.886/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cwp
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Cwp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.885/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cwp-3.0.886/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cwp
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Cwp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.885/setup.py` & `tencentcloud-sdk-python-cwp-3.0.886/setup.py`

 * *Files identical despite different names*

