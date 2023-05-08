# Comparing `tmp/tencentcloud-sdk-python-ssa-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-ssa-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ssa-3.0.885.tar", last modified: Mon May  1 00:49:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ssa-3.0.886.tar", last modified: Mon May  8 03:56:04 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ssa-3.0.885.tar` & `tencentcloud-sdk-python-ssa-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:49:22.000000 tencentcloud-sdk-python-ssa-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-01 00:49:22.000000 tencentcloud-sdk-python-ssa-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:49:22.000000 tencentcloud-sdk-python-ssa-3.0.885/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:49:22.000000 tencentcloud-sdk-python-ssa-3.0.885/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:49:22.000000 tencentcloud-sdk-python-ssa-3.0.885/tencentcloud/ssa/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:49:22.000000 tencentcloud-sdk-python-ssa-3.0.885/tencentcloud/ssa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:49:22.000000 tencentcloud-sdk-python-ssa-3.0.885/tencentcloud/ssa/v20180608/
--rw-r--r--   0 root         (0) root         (0)     2265 2023-05-01 00:49:22.000000 tencentcloud-sdk-python-ssa-3.0.885/tencentcloud/ssa/v20180608/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:49:22.000000 tencentcloud-sdk-python-ssa-3.0.885/tencentcloud/ssa/v20180608/__init__.py
--rw-r--r--   0 root         (0) root         (0)   147601 2023-05-01 00:49:22.000000 tencentcloud-sdk-python-ssa-3.0.885/tencentcloud/ssa/v20180608/models.py
--rw-r--r--   0 root         (0) root         (0)    21767 2023-05-01 00:49:22.000000 tencentcloud-sdk-python-ssa-3.0.885/tencentcloud/ssa/v20180608/ssa_client.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:49:22.000000 tencentcloud-sdk-python-ssa-3.0.885/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-01 00:49:22.000000 tencentcloud-sdk-python-ssa-3.0.885/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:49:22.000000 tencentcloud-sdk-python-ssa-3.0.885/tencentcloud_sdk_python_ssa.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:49:22.000000 tencentcloud-sdk-python-ssa-3.0.885/tencentcloud_sdk_python_ssa.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-01 00:49:22.000000 tencentcloud-sdk-python-ssa-3.0.885/tencentcloud_sdk_python_ssa.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:49:22.000000 tencentcloud-sdk-python-ssa-3.0.885/tencentcloud_sdk_python_ssa.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:49:22.000000 tencentcloud-sdk-python-ssa-3.0.885/tencentcloud_sdk_python_ssa.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:49:22.000000 tencentcloud-sdk-python-ssa-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:56:04.000000 tencentcloud-sdk-python-ssa-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-08 03:56:04.000000 tencentcloud-sdk-python-ssa-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:56:04.000000 tencentcloud-sdk-python-ssa-3.0.886/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 03:56:04.000000 tencentcloud-sdk-python-ssa-3.0.886/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:56:04.000000 tencentcloud-sdk-python-ssa-3.0.886/tencentcloud/ssa/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:56:04.000000 tencentcloud-sdk-python-ssa-3.0.886/tencentcloud/ssa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:56:04.000000 tencentcloud-sdk-python-ssa-3.0.886/tencentcloud/ssa/v20180608/
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-05-08 03:56:04.000000 tencentcloud-sdk-python-ssa-3.0.886/tencentcloud/ssa/v20180608/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:56:04.000000 tencentcloud-sdk-python-ssa-3.0.886/tencentcloud/ssa/v20180608/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   158213 2023-05-08 03:56:04.000000 tencentcloud-sdk-python-ssa-3.0.886/tencentcloud/ssa/v20180608/models.py
+-rw-r--r--   0 root         (0) root         (0)    21767 2023-05-08 03:56:04.000000 tencentcloud-sdk-python-ssa-3.0.886/tencentcloud/ssa/v20180608/ssa_client.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 03:56:04.000000 tencentcloud-sdk-python-ssa-3.0.886/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-08 03:56:04.000000 tencentcloud-sdk-python-ssa-3.0.886/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:56:04.000000 tencentcloud-sdk-python-ssa-3.0.886/tencentcloud_sdk_python_ssa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 03:56:04.000000 tencentcloud-sdk-python-ssa-3.0.886/tencentcloud_sdk_python_ssa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-08 03:56:04.000000 tencentcloud-sdk-python-ssa-3.0.886/tencentcloud_sdk_python_ssa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 03:56:04.000000 tencentcloud-sdk-python-ssa-3.0.886/tencentcloud_sdk_python_ssa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 03:56:04.000000 tencentcloud-sdk-python-ssa-3.0.886/tencentcloud_sdk_python_ssa.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 03:56:04.000000 tencentcloud-sdk-python-ssa-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ssa-3.0.885/README.rst` & `tencentcloud-sdk-python-ssa-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssa-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ssa-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ssa-3.0.885/tencentcloud/ssa/v20180608/errorcodes.py` & `tencentcloud-sdk-python-ssa-3.0.886/tencentcloud/ssa/v20180608/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssa-3.0.885/tencentcloud/ssa/v20180608/models.py` & `tencentcloud-sdk-python-ssa-3.0.886/tencentcloud/ssa/v20180608/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,40 +79,77 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class AlertListAggregations(AbstractModel):
+    """空Aggregations结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: 名字
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Name: str
+        :param Value: 值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Value: str
+        """
+        self.Name = None
+        self.Value = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        self.Value = params.get("Value")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class AlertListData(AbstractModel):
     """告警列表响应数据
 
     """
 
     def __init__(self):
         r"""
         :param Total: 总数
 注意：此字段可能返回 null，表示取不到有效值。
         :type Total: int
         :param AlertList: 返回列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type AlertList: list of AlertType
+        :param Aggregations: 聚合参数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Aggregations: :class:`tencentcloud.ssa.v20180608.models.AlertListAggregations`
         """
         self.Total = None
         self.AlertList = None
+        self.Aggregations = None
 
 
     def _deserialize(self, params):
         self.Total = params.get("Total")
         if params.get("AlertList") is not None:
             self.AlertList = []
             for item in params.get("AlertList"):
                 obj = AlertType()
                 obj._deserialize(item)
                 self.AlertList.append(obj)
+        if params.get("Aggregations") is not None:
+            self.Aggregations = AlertListAggregations()
+            self.Aggregations._deserialize(params.get("Aggregations"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -196,14 +233,35 @@
         :type AssetPublicIp: list of str
         :param AttackTactic: 攻击战术名称
 注意：此字段可能返回 null，表示取不到有效值。
         :type AttackTactic: str
         :param VictimAssetSub: 资产子网
 注意：此字段可能返回 null，表示取不到有效值。
         :type VictimAssetSub: str
+        :param VictimAssetVpc: 资产vpc
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VictimAssetVpc: str
+        :param Timestamp: 时间戳
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Timestamp: str
+        :param AssetGroupName: 资产组名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetGroupName: list of str
+        :param AssetProjectName: 资产项目名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetProjectName: str
+        :param VictimAssetContent: 失陷资产内容
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VictimAssetContent: list of str
+        :param WrongReportStatus: 错误报告状态
+注意：此字段可能返回 null，表示取不到有效值。
+        :type WrongReportStatus: int
+        :param WrongReportConditionId: 错误报告Id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type WrongReportConditionId: int
         """
         self.AlertTime = None
         self.AlertId = None
         self.AssetId = None
         self.AssetPrivateIp = None
         self.AlertName = None
         self.Level = None
@@ -222,14 +280,21 @@
         self.ConcernVictimCount = None
         self.VictimAssetType = None
         self.SubType = None
         self.AttackName = None
         self.AssetPublicIp = None
         self.AttackTactic = None
         self.VictimAssetSub = None
+        self.VictimAssetVpc = None
+        self.Timestamp = None
+        self.AssetGroupName = None
+        self.AssetProjectName = None
+        self.VictimAssetContent = None
+        self.WrongReportStatus = None
+        self.WrongReportConditionId = None
 
 
     def _deserialize(self, params):
         self.AlertTime = params.get("AlertTime")
         self.AlertId = params.get("AlertId")
         self.AssetId = params.get("AssetId")
         self.AssetPrivateIp = params.get("AssetPrivateIp")
@@ -255,14 +320,21 @@
         self.ConcernVictimCount = params.get("ConcernVictimCount")
         self.VictimAssetType = params.get("VictimAssetType")
         self.SubType = params.get("SubType")
         self.AttackName = params.get("AttackName")
         self.AssetPublicIp = params.get("AssetPublicIp")
         self.AttackTactic = params.get("AttackTactic")
         self.VictimAssetSub = params.get("VictimAssetSub")
+        self.VictimAssetVpc = params.get("VictimAssetVpc")
+        self.Timestamp = params.get("Timestamp")
+        self.AssetGroupName = params.get("AssetGroupName")
+        self.AssetProjectName = params.get("AssetProjectName")
+        self.VictimAssetContent = params.get("VictimAssetContent")
+        self.WrongReportStatus = params.get("WrongReportStatus")
+        self.WrongReportConditionId = params.get("WrongReportConditionId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -557,14 +629,32 @@
         :type RDPRisk: str
         :param EventRisk: 安全事件风险
 注意：此字段可能返回 null，表示取不到有效值。
         :type EventRisk: str
         :param AssetVulNum: 漏洞数量
 注意：此字段可能返回 null，表示取不到有效值。
         :type AssetVulNum: int
+        :param AssetEventNum: 资产事件
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetEventNum: int
+        :param AssetCspmRiskNum: cspm风险
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetCspmRiskNum: int
+        :param SsaAssetDeleteTime: 资产删除时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SsaAssetDeleteTime: str
+        :param ChargeType: 费用类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ChargeType: str
+        :param AssetRegionName: 地域
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetRegionName: str
+        :param AssetVpcid: vpc信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetVpcid: str
         """
         self.AssetType = None
         self.Name = None
         self.Region = None
         self.VpcId = None
         self.InstanceType = None
         self.InstanceState = None
@@ -603,14 +693,20 @@
         self.AssetCreateTime = None
         self.LoadBalancerType = None
         self.AssetIpv6 = None
         self.SSHRisk = None
         self.RDPRisk = None
         self.EventRisk = None
         self.AssetVulNum = None
+        self.AssetEventNum = None
+        self.AssetCspmRiskNum = None
+        self.SsaAssetDeleteTime = None
+        self.ChargeType = None
+        self.AssetRegionName = None
+        self.AssetVpcid = None
 
 
     def _deserialize(self, params):
         self.AssetType = params.get("AssetType")
         self.Name = params.get("Name")
         self.Region = params.get("Region")
         self.VpcId = params.get("VpcId")
@@ -656,14 +752,20 @@
         self.AssetCreateTime = params.get("AssetCreateTime")
         self.LoadBalancerType = params.get("LoadBalancerType")
         self.AssetIpv6 = params.get("AssetIpv6")
         self.SSHRisk = params.get("SSHRisk")
         self.RDPRisk = params.get("RDPRisk")
         self.EventRisk = params.get("EventRisk")
         self.AssetVulNum = params.get("AssetVulNum")
+        self.AssetEventNum = params.get("AssetEventNum")
+        self.AssetCspmRiskNum = params.get("AssetCspmRiskNum")
+        self.SsaAssetDeleteTime = params.get("SsaAssetDeleteTime")
+        self.ChargeType = params.get("ChargeType")
+        self.AssetRegionName = params.get("AssetRegionName")
+        self.AssetVpcid = params.get("AssetVpcid")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1076,14 +1178,92 @@
         :type EntityType: int
         :param Concern: 关注点
 注意：此字段可能返回 null，表示取不到有效值。
         :type Concern: str
         :param StatisticsCount: 最近数量
 注意：此字段可能返回 null，表示取不到有效值。
         :type StatisticsCount: int
+        :param IpCountry: IP国家
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IpCountry: str
+        :param IpProvince: IP省份
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IpProvince: str
+        :param Result: 结果
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Result: str
+        :param Confidence: 置信度
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Confidence: int
+        :param IpIsp: 服务商
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IpIsp: str
+        :param IpInfrastructure: 是否基础设施
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IpInfrastructure: str
+        :param ThreatType: 威胁类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ThreatType: list of str
+        :param Groups: 威胁团伙
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Groups: list of str
+        :param Status: 状态威胁情报接口
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Status: str
+        :param Tags: 恶意标签
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Tags: list of str
+        :param VictimAssetType: 资产类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VictimAssetType: str
+        :param VictimAssetName: 资产名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VictimAssetName: str
+        :param DomainRegistrant: 注册者
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DomainRegistrant: str
+        :param DomainRegisteredInstitution: 注册机构
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DomainRegisteredInstitution: str
+        :param DomainRegistrationTime: 注册时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DomainRegistrationTime: str
+        :param FileName: 文件名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FileName: str
+        :param FileMd5: MD5
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FileMd5: str
+        :param VirusName: 病毒名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VirusName: str
+        :param FilePath: 文件路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FilePath: str
+        :param FileSize: 文件大小
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FileSize: str
+        :param ProcName: 进程名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProcName: str
+        :param Pid: 进程ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Pid: str
+        :param ProcPath: 进程路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProcPath: str
+        :param ProcUser: 用户名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProcUser: str
+        :param DefendedCount: 已防御
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DefendedCount: int
+        :param DetectedCount: 仅检测
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DetectedCount: int
         :param SearchData: 可疑关注点字段
 注意：此字段可能返回 null，表示取不到有效值。
         :type SearchData: str
         :param IpCountryIso: 可疑关注点字段
 注意：此字段可能返回 null，表示取不到有效值。
         :type IpCountryIso: str
         :param IpProvinceIso: 可疑关注点字段
@@ -1096,26 +1276,78 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type EventSubType: str
         """
         self.ConcernType = None
         self.EntityType = None
         self.Concern = None
         self.StatisticsCount = None
+        self.IpCountry = None
+        self.IpProvince = None
+        self.Result = None
+        self.Confidence = None
+        self.IpIsp = None
+        self.IpInfrastructure = None
+        self.ThreatType = None
+        self.Groups = None
+        self.Status = None
+        self.Tags = None
+        self.VictimAssetType = None
+        self.VictimAssetName = None
+        self.DomainRegistrant = None
+        self.DomainRegisteredInstitution = None
+        self.DomainRegistrationTime = None
+        self.FileName = None
+        self.FileMd5 = None
+        self.VirusName = None
+        self.FilePath = None
+        self.FileSize = None
+        self.ProcName = None
+        self.Pid = None
+        self.ProcPath = None
+        self.ProcUser = None
+        self.DefendedCount = None
+        self.DetectedCount = None
         self.SearchData = None
         self.IpCountryIso = None
         self.IpProvinceIso = None
         self.IpCity = None
         self.EventSubType = None
 
 
     def _deserialize(self, params):
         self.ConcernType = params.get("ConcernType")
         self.EntityType = params.get("EntityType")
         self.Concern = params.get("Concern")
         self.StatisticsCount = params.get("StatisticsCount")
+        self.IpCountry = params.get("IpCountry")
+        self.IpProvince = params.get("IpProvince")
+        self.Result = params.get("Result")
+        self.Confidence = params.get("Confidence")
+        self.IpIsp = params.get("IpIsp")
+        self.IpInfrastructure = params.get("IpInfrastructure")
+        self.ThreatType = params.get("ThreatType")
+        self.Groups = params.get("Groups")
+        self.Status = params.get("Status")
+        self.Tags = params.get("Tags")
+        self.VictimAssetType = params.get("VictimAssetType")
+        self.VictimAssetName = params.get("VictimAssetName")
+        self.DomainRegistrant = params.get("DomainRegistrant")
+        self.DomainRegisteredInstitution = params.get("DomainRegisteredInstitution")
+        self.DomainRegistrationTime = params.get("DomainRegistrationTime")
+        self.FileName = params.get("FileName")
+        self.FileMd5 = params.get("FileMd5")
+        self.VirusName = params.get("VirusName")
+        self.FilePath = params.get("FilePath")
+        self.FileSize = params.get("FileSize")
+        self.ProcName = params.get("ProcName")
+        self.Pid = params.get("Pid")
+        self.ProcPath = params.get("ProcPath")
+        self.ProcUser = params.get("ProcUser")
+        self.DefendedCount = params.get("DefendedCount")
+        self.DetectedCount = params.get("DetectedCount")
         self.SearchData = params.get("SearchData")
         self.IpCountryIso = params.get("IpCountryIso")
         self.IpProvinceIso = params.get("IpProvinceIso")
         self.IpCity = params.get("IpCity")
         self.EventSubType = params.get("EventSubType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
@@ -3251,14 +3483,20 @@
         :type MappingStatus: int
         :param Region: 区域
 注意：此字段可能返回 null，表示取不到有效值。
         :type Region: str
         :param SecurityStatus: 安全防护状态
 注意：此字段可能返回 null，表示取不到有效值。
         :type SecurityStatus: list of SecurityStatus
+        :param DisposalRecommendation: 处置建议
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DisposalRecommendation: int
+        :param MappingType: 测绘类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MappingType: str
         """
         self.AssetName = None
         self.AssetIp = None
         self.PrivateIp = None
         self.AssetId = None
         self.Protocol = None
         self.Port = None
@@ -3270,14 +3508,16 @@
         self.DisposalRecommendations = None
         self.DisposalRecommendationDetails = None
         self.AssetType = None
         self.Domain = None
         self.MappingStatus = None
         self.Region = None
         self.SecurityStatus = None
+        self.DisposalRecommendation = None
+        self.MappingType = None
 
 
     def _deserialize(self, params):
         self.AssetName = params.get("AssetName")
         self.AssetIp = params.get("AssetIp")
         self.PrivateIp = params.get("PrivateIp")
         self.AssetId = params.get("AssetId")
@@ -3296,14 +3536,16 @@
         self.Region = params.get("Region")
         if params.get("SecurityStatus") is not None:
             self.SecurityStatus = []
             for item in params.get("SecurityStatus"):
                 obj = SecurityStatus()
                 obj._deserialize(item)
                 self.SecurityStatus.append(obj)
+        self.DisposalRecommendation = params.get("DisposalRecommendation")
+        self.MappingType = params.get("MappingType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4048,15 +4290,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param Fid: 数据库标识
         :type Fid: int
-        :param Fname: 标签名称
+        :param Fname: 标签名称字段
         :type Fname: str
         """
         self.Fid = None
         self.Fname = None
 
 
     def _deserialize(self, params):
```

### Comparing `tencentcloud-sdk-python-ssa-3.0.885/tencentcloud/ssa/v20180608/ssa_client.py` & `tencentcloud-sdk-python-ssa-3.0.886/tencentcloud/ssa/v20180608/ssa_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssa-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-ssa-3.0.886/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssa
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Ssa SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssa-3.0.885/setup.py` & `tencentcloud-sdk-python-ssa-3.0.886/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssa-3.0.885/tencentcloud_sdk_python_ssa.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ssa-3.0.886/tencentcloud_sdk_python_ssa.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssa
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Ssa SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

