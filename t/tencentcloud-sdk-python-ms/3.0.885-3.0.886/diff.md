# Comparing `tmp/tencentcloud-sdk-python-ms-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-ms-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ms-3.0.885.tar", last modified: Mon May  1 00:45:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ms-3.0.886.tar", last modified: Mon May  8 03:38:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ms-3.0.885.tar` & `tencentcloud-sdk-python-ms-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:45:44.000000 tencentcloud-sdk-python-ms-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      734 2023-05-01 00:45:44.000000 tencentcloud-sdk-python-ms-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:45:44.000000 tencentcloud-sdk-python-ms-3.0.885/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:45:44.000000 tencentcloud-sdk-python-ms-3.0.885/tencentcloud/ms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:45:44.000000 tencentcloud-sdk-python-ms-3.0.885/tencentcloud/ms/v20180408/
--rw-r--r--   0 root         (0) root         (0)    19521 2023-05-01 00:45:44.000000 tencentcloud-sdk-python-ms-3.0.885/tencentcloud/ms/v20180408/ms_client.py
--rw-r--r--   0 root         (0) root         (0)     3281 2023-05-01 00:45:44.000000 tencentcloud-sdk-python-ms-3.0.885/tencentcloud/ms/v20180408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:45:44.000000 tencentcloud-sdk-python-ms-3.0.885/tencentcloud/ms/v20180408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81482 2023-05-01 00:45:44.000000 tencentcloud-sdk-python-ms-3.0.885/tencentcloud/ms/v20180408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:45:44.000000 tencentcloud-sdk-python-ms-3.0.885/tencentcloud/ms/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:45:44.000000 tencentcloud-sdk-python-ms-3.0.885/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:45:44.000000 tencentcloud-sdk-python-ms-3.0.885/tencentcloud_sdk_python_ms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:45:44.000000 tencentcloud-sdk-python-ms-3.0.885/tencentcloud_sdk_python_ms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-01 00:45:44.000000 tencentcloud-sdk-python-ms-3.0.885/tencentcloud_sdk_python_ms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-05-01 00:45:44.000000 tencentcloud-sdk-python-ms-3.0.885/tencentcloud_sdk_python_ms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:45:44.000000 tencentcloud-sdk-python-ms-3.0.885/tencentcloud_sdk_python_ms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-05-01 00:45:44.000000 tencentcloud-sdk-python-ms-3.0.885/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1004 2023-05-01 00:45:44.000000 tencentcloud-sdk-python-ms-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:45:44.000000 tencentcloud-sdk-python-ms-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:38:42.000000 tencentcloud-sdk-python-ms-3.0.886/
+-rw-r--r--   0 root         (0) root         (0)      734 2023-05-08 03:38:42.000000 tencentcloud-sdk-python-ms-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:38:42.000000 tencentcloud-sdk-python-ms-3.0.886/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:38:42.000000 tencentcloud-sdk-python-ms-3.0.886/tencentcloud/ms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:38:42.000000 tencentcloud-sdk-python-ms-3.0.886/tencentcloud/ms/v20180408/
+-rw-r--r--   0 root         (0) root         (0)    14712 2023-05-08 03:38:42.000000 tencentcloud-sdk-python-ms-3.0.886/tencentcloud/ms/v20180408/ms_client.py
+-rw-r--r--   0 root         (0) root         (0)     3281 2023-05-08 03:38:42.000000 tencentcloud-sdk-python-ms-3.0.886/tencentcloud/ms/v20180408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:38:42.000000 tencentcloud-sdk-python-ms-3.0.886/tencentcloud/ms/v20180408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55731 2023-05-08 03:38:42.000000 tencentcloud-sdk-python-ms-3.0.886/tencentcloud/ms/v20180408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:38:42.000000 tencentcloud-sdk-python-ms-3.0.886/tencentcloud/ms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 03:38:42.000000 tencentcloud-sdk-python-ms-3.0.886/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:38:42.000000 tencentcloud-sdk-python-ms-3.0.886/tencentcloud_sdk_python_ms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 03:38:42.000000 tencentcloud-sdk-python-ms-3.0.886/tencentcloud_sdk_python_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-08 03:38:42.000000 tencentcloud-sdk-python-ms-3.0.886/tencentcloud_sdk_python_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-05-08 03:38:42.000000 tencentcloud-sdk-python-ms-3.0.886/tencentcloud_sdk_python_ms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 03:38:42.000000 tencentcloud-sdk-python-ms-3.0.886/tencentcloud_sdk_python_ms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-05-08 03:38:42.000000 tencentcloud-sdk-python-ms-3.0.886/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-05-08 03:38:42.000000 tencentcloud-sdk-python-ms-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 03:38:42.000000 tencentcloud-sdk-python-ms-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ms-3.0.885/README.rst` & `tencentcloud-sdk-python-ms-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ms-3.0.885/tencentcloud/ms/v20180408/ms_client.py` & `tencentcloud-sdk-python-ms-3.0.886/tencentcloud/ms/v20180408/ms_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -91,39 +91,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def CreateScanInstances(self, request):
-        """由于该产品是线上免费使用产品，无企业版用户，升级迭代成本高及人力安排等原因，安全测评产品不再接入新用户，故下线。
-
-        用户通过该接口批量提交应用进行应用扫描，扫描后需通过DescribeScanResults接口查询扫描结果
-
-        :param request: Request instance for CreateScanInstances.
-        :type request: :class:`tencentcloud.ms.v20180408.models.CreateScanInstancesRequest`
-        :rtype: :class:`tencentcloud.ms.v20180408.models.CreateScanInstancesResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("CreateScanInstances", params, headers=headers)
-            response = json.loads(body)
-            model = models.CreateScanInstancesResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def CreateShieldInstance(self, request):
         """用户通过该接口提交应用进行应用加固，加固后需通过DescribeShieldResult接口查询加固结果。（注意：根据国家互联网用户实名制相关要求，使用该产品前，需先完成实名认证。）
 
         :param request: Request instance for CreateShieldInstance.
         :type request: :class:`tencentcloud.ms.v20180408.models.CreateShieldInstanceRequest`
         :rtype: :class:`tencentcloud.ms.v20180408.models.CreateShieldInstanceResponse`
 
@@ -162,39 +137,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DeleteScanInstances(self, request):
-        """由于该产品是线上免费使用产品，无企业版用户，升级迭代成本高及人力安排等原因，安全测评产品不再接入新用户，故下线。
-
-        删除一个或者多个app扫描信息
-
-        :param request: Request instance for DeleteScanInstances.
-        :type request: :class:`tencentcloud.ms.v20180408.models.DeleteScanInstancesRequest`
-        :rtype: :class:`tencentcloud.ms.v20180408.models.DeleteScanInstancesResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DeleteScanInstances", params, headers=headers)
-            response = json.loads(body)
-            model = models.DeleteScanInstancesResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def DeleteShieldInstances(self, request):
         """删除一个或者多个app加固信息。（注意：根据国家互联网用户实名制相关要求，使用该产品前，需先完成实名认证。）
 
         :param request: Request instance for DeleteShieldInstances.
         :type request: :class:`tencentcloud.ms.v20180408.models.DeleteShieldInstancesRequest`
         :rtype: :class:`tencentcloud.ms.v20180408.models.DeleteShieldInstancesResponse`
 
@@ -254,65 +204,14 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeScanInstances(self, request):
-        """由于该产品是线上免费使用产品，无企业版用户，升级迭代成本高及人力安排等原因，安全测评产品不再接入新用户，故下线。
-
-        本接口用于查看app列表。
-        可以通过指定任务唯一标识ItemId来查询指定app的详细信息，或通过设定过滤器来查询满足过滤条件的app的详细信息。 指定偏移(Offset)和限制(Limit)来选择结果中的一部分，默认返回满足条件的前20个app信息。
-
-        :param request: Request instance for DescribeScanInstances.
-        :type request: :class:`tencentcloud.ms.v20180408.models.DescribeScanInstancesRequest`
-        :rtype: :class:`tencentcloud.ms.v20180408.models.DescribeScanInstancesResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeScanInstances", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeScanInstancesResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeScanResults(self, request):
-        """由于该产品是线上免费使用产品，无企业版用户，升级迭代成本高及人力安排等原因，安全测评产品不再接入新用户，故下线。
-
-        用户通过CreateScanInstances接口提交应用进行风险批量扫描后，用此接口批量获取风险详细信息,包含漏洞信息，广告信息，插件信息和病毒信息
-
-        :param request: Request instance for DescribeScanResults.
-        :type request: :class:`tencentcloud.ms.v20180408.models.DescribeScanResultsRequest`
-        :rtype: :class:`tencentcloud.ms.v20180408.models.DescribeScanResultsResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeScanResults", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeScanResultsResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeShieldInstances(self, request):
         """本接口用于查看app列表。
         可以通过指定任务唯一标识ItemId来查询指定app的详细信息，或通过设定过滤器来查询满足过滤条件的app的详细信息。 指定偏移(Offset)和限制(Limit)来选择结果中的一部分，默认返回满足条件的前20个app信息。（注意：根据国家互联网用户实名制相关要求，使用该产品前，需先完成实名认证。）
 
         :param request: Request instance for DescribeShieldInstances.
```

### Comparing `tencentcloud-sdk-python-ms-3.0.885/tencentcloud/ms/v20180408/errorcodes.py` & `tencentcloud-sdk-python-ms-3.0.886/tencentcloud/ms/v20180408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ms-3.0.885/tencentcloud/ms/v20180408/models.py` & `tencentcloud-sdk-python-ms-3.0.886/tencentcloud/ms/v20180408/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,88 +14,14 @@
 # limitations under the License.
 
 import warnings
 
 from tencentcloud.common.abstract_model import AbstractModel
 
 
-class AdInfo(AbstractModel):
-    """广告信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param Spots: 插播广告列表
-        :type Spots: list of PluginInfo
-        :param BoutiqueRecommands: 精品推荐广告列表
-        :type BoutiqueRecommands: list of PluginInfo
-        :param FloatWindowses: 悬浮窗广告列表
-        :type FloatWindowses: list of PluginInfo
-        :param Banners: banner广告列表
-        :type Banners: list of PluginInfo
-        :param IntegralWalls: 积分墙广告列表
-        :type IntegralWalls: list of PluginInfo
-        :param NotifyBars: 通知栏广告列表
-        :type NotifyBars: list of PluginInfo
-        """
-        self.Spots = None
-        self.BoutiqueRecommands = None
-        self.FloatWindowses = None
-        self.Banners = None
-        self.IntegralWalls = None
-        self.NotifyBars = None
-
-
-    def _deserialize(self, params):
-        if params.get("Spots") is not None:
-            self.Spots = []
-            for item in params.get("Spots"):
-                obj = PluginInfo()
-                obj._deserialize(item)
-                self.Spots.append(obj)
-        if params.get("BoutiqueRecommands") is not None:
-            self.BoutiqueRecommands = []
-            for item in params.get("BoutiqueRecommands"):
-                obj = PluginInfo()
-                obj._deserialize(item)
-                self.BoutiqueRecommands.append(obj)
-        if params.get("FloatWindowses") is not None:
-            self.FloatWindowses = []
-            for item in params.get("FloatWindowses"):
-                obj = PluginInfo()
-                obj._deserialize(item)
-                self.FloatWindowses.append(obj)
-        if params.get("Banners") is not None:
-            self.Banners = []
-            for item in params.get("Banners"):
-                obj = PluginInfo()
-                obj._deserialize(item)
-                self.Banners.append(obj)
-        if params.get("IntegralWalls") is not None:
-            self.IntegralWalls = []
-            for item in params.get("IntegralWalls"):
-                obj = PluginInfo()
-                obj._deserialize(item)
-                self.IntegralWalls.append(obj)
-        if params.get("NotifyBars") is not None:
-            self.NotifyBars = []
-            for item in params.get("NotifyBars"):
-                obj = PluginInfo()
-                obj._deserialize(item)
-                self.NotifyBars.append(obj)
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class AppDetailInfo(AbstractModel):
     """app的详细基础信息
 
     """
 
     def __init__(self):
         r"""
@@ -188,86 +114,14 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class AppScanSet(AbstractModel):
-    """扫描后app的信息，包含基本信息和扫描状态信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param ItemId: 任务唯一标识
-        :type ItemId: str
-        :param AppName: app的名称
-        :type AppName: str
-        :param AppPkgName: app的包名
-        :type AppPkgName: str
-        :param AppVersion: app的版本号
-        :type AppVersion: str
-        :param AppMd5: app的md5
-        :type AppMd5: str
-        :param AppSize: app的大小
-        :type AppSize: int
-        :param ScanCode: 扫描结果返回码
-        :type ScanCode: int
-        :param TaskStatus: 任务状态: 1-已完成,2-处理中,3-处理出错,4-处理超时
-        :type TaskStatus: int
-        :param TaskTime: 提交扫描时间
-        :type TaskTime: int
-        :param AppIconUrl: app的图标url
-        :type AppIconUrl: str
-        :param AppSid: 标识唯一该app，主要用于删除
-        :type AppSid: str
-        :param SafeType: 安全类型:1-安全软件，2-风险软件，3病毒软件
-        :type SafeType: int
-        :param VulCount: 漏洞个数
-        :type VulCount: int
-        """
-        self.ItemId = None
-        self.AppName = None
-        self.AppPkgName = None
-        self.AppVersion = None
-        self.AppMd5 = None
-        self.AppSize = None
-        self.ScanCode = None
-        self.TaskStatus = None
-        self.TaskTime = None
-        self.AppIconUrl = None
-        self.AppSid = None
-        self.SafeType = None
-        self.VulCount = None
-
-
-    def _deserialize(self, params):
-        self.ItemId = params.get("ItemId")
-        self.AppName = params.get("AppName")
-        self.AppPkgName = params.get("AppPkgName")
-        self.AppVersion = params.get("AppVersion")
-        self.AppMd5 = params.get("AppMd5")
-        self.AppSize = params.get("AppSize")
-        self.ScanCode = params.get("ScanCode")
-        self.TaskStatus = params.get("TaskStatus")
-        self.TaskTime = params.get("TaskTime")
-        self.AppIconUrl = params.get("AppIconUrl")
-        self.AppSid = params.get("AppSid")
-        self.SafeType = params.get("SafeType")
-        self.VulCount = params.get("VulCount")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class AppSetInfo(AbstractModel):
     """加固后app的信息，包含基本信息和加固信息
 
     """
 
     def __init__(self):
         r"""
@@ -563,86 +417,14 @@
 
 
     def _deserialize(self, params):
         self.ResourceSet = params.get("ResourceSet")
         self.RequestId = params.get("RequestId")
 
 
-class CreateScanInstancesRequest(AbstractModel):
-    """CreateScanInstances请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param AppInfos: 待扫描的app信息列表，一次最多提交20个
-        :type AppInfos: list of AppInfo
-        :param ScanInfo: 扫描信息
-        :type ScanInfo: :class:`tencentcloud.ms.v20180408.models.ScanInfo`
-        """
-        self.AppInfos = None
-        self.ScanInfo = None
-
-
-    def _deserialize(self, params):
-        if params.get("AppInfos") is not None:
-            self.AppInfos = []
-            for item in params.get("AppInfos"):
-                obj = AppInfo()
-                obj._deserialize(item)
-                self.AppInfos.append(obj)
-        if params.get("ScanInfo") is not None:
-            self.ScanInfo = ScanInfo()
-            self.ScanInfo._deserialize(params.get("ScanInfo"))
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class CreateScanInstancesResponse(AbstractModel):
-    """CreateScanInstances返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param ItemId: 任务唯一标识
-        :type ItemId: str
-        :param Progress: 任务状态: 1-已完成,2-处理中,3-处理出错,4-处理超时
-        :type Progress: int
-        :param AppMd5s: 提交成功的app的md5集合
-        :type AppMd5s: list of str
-        :param LimitCount: 剩余可用次数
-        :type LimitCount: int
-        :param LimitTime: 到期时间
-        :type LimitTime: int
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.ItemId = None
-        self.Progress = None
-        self.AppMd5s = None
-        self.LimitCount = None
-        self.LimitTime = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.ItemId = params.get("ItemId")
-        self.Progress = params.get("Progress")
-        self.AppMd5s = params.get("AppMd5s")
-        self.LimitCount = params.get("LimitCount")
-        self.LimitTime = params.get("LimitTime")
-        self.RequestId = params.get("RequestId")
-
-
 class CreateShieldInstanceRequest(AbstractModel):
     """CreateShieldInstance请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -751,59 +533,14 @@
 
     def _deserialize(self, params):
         self.PlanId = params.get("PlanId")
         self.Progress = params.get("Progress")
         self.RequestId = params.get("RequestId")
 
 
-class DeleteScanInstancesRequest(AbstractModel):
-    """DeleteScanInstances请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param AppSids: 删除一个或多个扫描的app，最大支持20个
-        :type AppSids: list of str
-        """
-        self.AppSids = None
-
-
-    def _deserialize(self, params):
-        self.AppSids = params.get("AppSids")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DeleteScanInstancesResponse(AbstractModel):
-    """DeleteScanInstances返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param Progress: 任务状态: 1-已完成,2-处理中,3-处理出错,4-处理超时
-        :type Progress: int
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.Progress = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.Progress = params.get("Progress")
-        self.RequestId = params.get("RequestId")
-
-
 class DeleteShieldInstancesRequest(AbstractModel):
     """DeleteShieldInstances请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -982,151 +719,14 @@
             for item in params.get("ResourceSet"):
                 obj = ResourceInfo()
                 obj._deserialize(item)
                 self.ResourceSet.append(obj)
         self.RequestId = params.get("RequestId")
 
 
-class DescribeScanInstancesRequest(AbstractModel):
-    """DescribeScanInstances请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param Filters: 支持通过app名称，app包名进行筛选
-        :type Filters: list of Filter
-        :param Offset: 偏移量，默认为0
-        :type Offset: int
-        :param Limit: 数量限制，默认为20，最大值为100。
-        :type Limit: int
-        :param ItemIds: 可以提供ItemId数组来查询一个或者多个结果。注意不可以同时指定ItemIds和Filters。
-        :type ItemIds: list of str
-        :param OrderField: 按某个字段排序，目前仅支持TaskTime排序。
-        :type OrderField: str
-        :param OrderDirection: 升序（asc）还是降序（desc），默认：desc。
-        :type OrderDirection: str
-        """
-        self.Filters = None
-        self.Offset = None
-        self.Limit = None
-        self.ItemIds = None
-        self.OrderField = None
-        self.OrderDirection = None
-
-
-    def _deserialize(self, params):
-        if params.get("Filters") is not None:
-            self.Filters = []
-            for item in params.get("Filters"):
-                obj = Filter()
-                obj._deserialize(item)
-                self.Filters.append(obj)
-        self.Offset = params.get("Offset")
-        self.Limit = params.get("Limit")
-        self.ItemIds = params.get("ItemIds")
-        self.OrderField = params.get("OrderField")
-        self.OrderDirection = params.get("OrderDirection")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeScanInstancesResponse(AbstractModel):
-    """DescribeScanInstances返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param TotalCount: 符合要求的app数量
-        :type TotalCount: int
-        :param ScanSet: 一个关于app详细信息的结构体，主要包括app的基本信息和扫描状态信息。
-        :type ScanSet: list of AppScanSet
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.TotalCount = None
-        self.ScanSet = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.TotalCount = params.get("TotalCount")
-        if params.get("ScanSet") is not None:
-            self.ScanSet = []
-            for item in params.get("ScanSet"):
-                obj = AppScanSet()
-                obj._deserialize(item)
-                self.ScanSet.append(obj)
-        self.RequestId = params.get("RequestId")
-
-
-class DescribeScanResultsRequest(AbstractModel):
-    """DescribeScanResults请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param ItemId: 任务唯一标识
-        :type ItemId: str
-        :param AppMd5s: 批量查询一个或者多个app的扫描结果，如果不传表示查询该任务下所提交的所有app
-        :type AppMd5s: list of str
-        """
-        self.ItemId = None
-        self.AppMd5s = None
-
-
-    def _deserialize(self, params):
-        self.ItemId = params.get("ItemId")
-        self.AppMd5s = params.get("AppMd5s")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeScanResultsResponse(AbstractModel):
-    """DescribeScanResults返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param ScanSet: 批量扫描的app结果集
-        :type ScanSet: list of ScanSetInfo
-        :param TotalCount: 批量扫描结果的个数
-        :type TotalCount: int
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.ScanSet = None
-        self.TotalCount = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        if params.get("ScanSet") is not None:
-            self.ScanSet = []
-            for item in params.get("ScanSet"):
-                obj = ScanSetInfo()
-                obj._deserialize(item)
-                self.ScanSet.append(obj)
-        self.TotalCount = params.get("TotalCount")
-        self.RequestId = params.get("RequestId")
-
-
 class DescribeShieldInstancesRequest(AbstractModel):
     """DescribeShieldInstances请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1651,46 +1251,14 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class PluginInfo(AbstractModel):
-    """插件信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param PluginType: 插件类型，分别为 1-通知栏广告，2-积分墙广告，3-banner广告，4- 悬浮窗图标广告，5-精品推荐列表广告, 6-插播广告
-        :type PluginType: int
-        :param PluginName: 插件名称
-        :type PluginName: str
-        :param PluginDesc: 插件描述
-        :type PluginDesc: str
-        """
-        self.PluginType = None
-        self.PluginName = None
-        self.PluginDesc = None
-
-
-    def _deserialize(self, params):
-        self.PluginType = params.get("PluginType")
-        self.PluginName = params.get("PluginName")
-        self.PluginDesc = params.get("PluginDesc")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class PluginListItem(AbstractModel):
     """APK检测服务：广告插件结果结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1921,232 +1489,14 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class ScanInfo(AbstractModel):
-    """需要扫描的应用的服务信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param CallbackUrl: 任务处理完成后的反向通知回调地址,批量提交app每扫描完成一个会通知一次,通知为POST请求，post信息{ItemId:
-        :type CallbackUrl: str
-        :param ScanTypes: VULSCAN-漏洞扫描信息，VIRUSSCAN-返回病毒扫描信息， ADSCAN-广告扫描信息，PLUGINSCAN-插件扫描信息，PERMISSION-系统权限信息，SENSITIVE-敏感词信息，可以自由组合
-        :type ScanTypes: list of str
-        """
-        self.CallbackUrl = None
-        self.ScanTypes = None
-
-
-    def _deserialize(self, params):
-        self.CallbackUrl = params.get("CallbackUrl")
-        self.ScanTypes = params.get("ScanTypes")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class ScanPermissionInfo(AbstractModel):
-    """安全扫描系统权限信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param Permission: 系统权限
-        :type Permission: str
-        """
-        self.Permission = None
-
-
-    def _deserialize(self, params):
-        self.Permission = params.get("Permission")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class ScanPermissionList(AbstractModel):
-    """安全扫描系统权限信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param PermissionList: 系统权限信息
-        :type PermissionList: list of ScanPermissionInfo
-        """
-        self.PermissionList = None
-
-
-    def _deserialize(self, params):
-        if params.get("PermissionList") is not None:
-            self.PermissionList = []
-            for item in params.get("PermissionList"):
-                obj = ScanPermissionInfo()
-                obj._deserialize(item)
-                self.PermissionList.append(obj)
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class ScanSensitiveInfo(AbstractModel):
-    """安全扫描敏感词
-
-    """
-
-    def __init__(self):
-        r"""
-        :param WordList: 敏感词
-        :type WordList: list of str
-        :param FilePath: 敏感词对应的文件信息
-        :type FilePath: str
-        :param FileSha: 文件sha1值
-        :type FileSha: str
-        """
-        self.WordList = None
-        self.FilePath = None
-        self.FileSha = None
-
-
-    def _deserialize(self, params):
-        self.WordList = params.get("WordList")
-        self.FilePath = params.get("FilePath")
-        self.FileSha = params.get("FileSha")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class ScanSensitiveList(AbstractModel):
-    """安全扫描敏感词列表
-
-    """
-
-    def __init__(self):
-        r"""
-        :param SensitiveList: 敏感词列表
-        :type SensitiveList: list of ScanSensitiveInfo
-        """
-        self.SensitiveList = None
-
-
-    def _deserialize(self, params):
-        if params.get("SensitiveList") is not None:
-            self.SensitiveList = []
-            for item in params.get("SensitiveList"):
-                obj = ScanSensitiveInfo()
-                obj._deserialize(item)
-                self.SensitiveList.append(obj)
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class ScanSetInfo(AbstractModel):
-    """app扫描结果集
-
-    """
-
-    def __init__(self):
-        r"""
-        :param TaskStatus: 任务状态: 1-已完成,2-处理中,3-处理出错,4-处理超时
-        :type TaskStatus: int
-        :param AppDetailInfo: app信息
-        :type AppDetailInfo: :class:`tencentcloud.ms.v20180408.models.AppDetailInfo`
-        :param VirusInfo: 病毒信息
-        :type VirusInfo: :class:`tencentcloud.ms.v20180408.models.VirusInfo`
-        :param VulInfo: 漏洞信息
-        :type VulInfo: :class:`tencentcloud.ms.v20180408.models.VulInfo`
-        :param AdInfo: 广告插件信息
-        :type AdInfo: :class:`tencentcloud.ms.v20180408.models.AdInfo`
-        :param TaskTime: 提交扫描的时间
-        :type TaskTime: int
-        :param StatusCode: 状态码，成功返回0，失败返回错误码
-        :type StatusCode: int
-        :param StatusDesc: 状态描述
-        :type StatusDesc: str
-        :param StatusRef: 状态操作指引
-        :type StatusRef: str
-        :param PermissionInfo: 系统权限信息
-        :type PermissionInfo: :class:`tencentcloud.ms.v20180408.models.ScanPermissionList`
-        :param SensitiveInfo: 敏感词列表
-        :type SensitiveInfo: :class:`tencentcloud.ms.v20180408.models.ScanSensitiveList`
-        """
-        self.TaskStatus = None
-        self.AppDetailInfo = None
-        self.VirusInfo = None
-        self.VulInfo = None
-        self.AdInfo = None
-        self.TaskTime = None
-        self.StatusCode = None
-        self.StatusDesc = None
-        self.StatusRef = None
-        self.PermissionInfo = None
-        self.SensitiveInfo = None
-
-
-    def _deserialize(self, params):
-        self.TaskStatus = params.get("TaskStatus")
-        if params.get("AppDetailInfo") is not None:
-            self.AppDetailInfo = AppDetailInfo()
-            self.AppDetailInfo._deserialize(params.get("AppDetailInfo"))
-        if params.get("VirusInfo") is not None:
-            self.VirusInfo = VirusInfo()
-            self.VirusInfo._deserialize(params.get("VirusInfo"))
-        if params.get("VulInfo") is not None:
-            self.VulInfo = VulInfo()
-            self.VulInfo._deserialize(params.get("VulInfo"))
-        if params.get("AdInfo") is not None:
-            self.AdInfo = AdInfo()
-            self.AdInfo._deserialize(params.get("AdInfo"))
-        self.TaskTime = params.get("TaskTime")
-        self.StatusCode = params.get("StatusCode")
-        self.StatusDesc = params.get("StatusDesc")
-        self.StatusRef = params.get("StatusRef")
-        if params.get("PermissionInfo") is not None:
-            self.PermissionInfo = ScanPermissionList()
-            self.PermissionInfo._deserialize(params.get("PermissionInfo"))
-        if params.get("SensitiveInfo") is not None:
-            self.SensitiveInfo = ScanSensitiveList()
-            self.SensitiveInfo._deserialize(params.get("SensitiveInfo"))
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class ServiceInfo(AbstractModel):
     """提交app加固的服务信息
 
     """
 
     def __init__(self):
         r"""
@@ -2277,125 +1627,8 @@
         self.SoFileNames = params.get("SoFileNames")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class VirusInfo(AbstractModel):
-    """病毒信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param SafeType: 软件安全类型，分别为0-未知、 1-安全软件、2-风险软件、3-病毒软件
-        :type SafeType: int
-        :param VirusName: 病毒名称， utf8编码，非病毒时值为空
-        :type VirusName: str
-        :param VirusDesc: 病毒描述，utf8编码，非病毒时值为空
-        :type VirusDesc: str
-        """
-        self.SafeType = None
-        self.VirusName = None
-        self.VirusDesc = None
-
-
-    def _deserialize(self, params):
-        self.SafeType = params.get("SafeType")
-        self.VirusName = params.get("VirusName")
-        self.VirusDesc = params.get("VirusDesc")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class VulInfo(AbstractModel):
-    """漏洞信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param VulList: 漏洞列表
-        :type VulList: list of VulList
-        :param VulFileScore: 漏洞文件评分
-        :type VulFileScore: int
-        """
-        self.VulList = None
-        self.VulFileScore = None
-
-
-    def _deserialize(self, params):
-        if params.get("VulList") is not None:
-            self.VulList = []
-            for item in params.get("VulList"):
-                obj = VulList()
-                obj._deserialize(item)
-                self.VulList.append(obj)
-        self.VulFileScore = params.get("VulFileScore")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class VulList(AbstractModel):
-    """漏洞信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param VulId: 漏洞id
-        :type VulId: str
-        :param VulName: 漏洞名称
-        :type VulName: str
-        :param VulCode: 漏洞代码
-        :type VulCode: str
-        :param VulDesc: 漏洞描述
-        :type VulDesc: str
-        :param VulSolution: 漏洞解决方案
-        :type VulSolution: str
-        :param VulSrcType: 漏洞来源类别，0默认自身，1第三方插件
-        :type VulSrcType: int
-        :param VulFilepath: 漏洞位置
-        :type VulFilepath: str
-        :param RiskLevel: 风险级别：1 低风险 ；2中等风险；3 高风险
-        :type RiskLevel: int
-        """
-        self.VulId = None
-        self.VulName = None
-        self.VulCode = None
-        self.VulDesc = None
-        self.VulSolution = None
-        self.VulSrcType = None
-        self.VulFilepath = None
-        self.RiskLevel = None
-
-
-    def _deserialize(self, params):
-        self.VulId = params.get("VulId")
-        self.VulName = params.get("VulName")
-        self.VulCode = params.get("VulCode")
-        self.VulDesc = params.get("VulDesc")
-        self.VulSolution = params.get("VulSolution")
-        self.VulSrcType = params.get("VulSrcType")
-        self.VulFilepath = params.get("VulFilepath")
-        self.RiskLevel = params.get("RiskLevel")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ms-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ms-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ms-3.0.885/tencentcloud_sdk_python_ms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ms-3.0.886/tencentcloud_sdk_python_ms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ms
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Ms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ms-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-ms-3.0.886/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ms
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Ms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ms-3.0.885/setup.py` & `tencentcloud-sdk-python-ms-3.0.886/setup.py`

 * *Files identical despite different names*

