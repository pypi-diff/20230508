# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.885.tar", last modified: Mon May  1 00:46:29 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.886.tar", last modified: Mon May  8 03:39:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.885.tar` & `tencentcloud-sdk-python-ocr-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:46:29.000000 tencentcloud-sdk-python-ocr-3.0.885/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:46:29.000000 tencentcloud-sdk-python-ocr-3.0.885/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:46:29.000000 tencentcloud-sdk-python-ocr-3.0.885/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-01 00:46:29.000000 tencentcloud-sdk-python-ocr-3.0.885/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:46:29.000000 tencentcloud-sdk-python-ocr-3.0.885/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:46:29.000000 tencentcloud-sdk-python-ocr-3.0.885/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-01 00:46:29.000000 tencentcloud-sdk-python-ocr-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:46:29.000000 tencentcloud-sdk-python-ocr-3.0.885/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:46:29.000000 tencentcloud-sdk-python-ocr-3.0.885/tencentcloud/ocr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:46:29.000000 tencentcloud-sdk-python-ocr-3.0.885/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)   107569 2023-05-01 00:46:29.000000 tencentcloud-sdk-python-ocr-3.0.885/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)     5764 2023-05-01 00:46:29.000000 tencentcloud-sdk-python-ocr-3.0.885/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:46:29.000000 tencentcloud-sdk-python-ocr-3.0.885/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)   415162 2023-05-01 00:46:29.000000 tencentcloud-sdk-python-ocr-3.0.885/tencentcloud/ocr/v20181119/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:46:29.000000 tencentcloud-sdk-python-ocr-3.0.885/tencentcloud/ocr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:46:29.000000 tencentcloud-sdk-python-ocr-3.0.885/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:46:29.000000 tencentcloud-sdk-python-ocr-3.0.885/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-01 00:46:29.000000 tencentcloud-sdk-python-ocr-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:46:29.000000 tencentcloud-sdk-python-ocr-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/ocr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)   108933 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   505378 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/ocr/v20181119/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/ocr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.885/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.886/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.885/README.rst` & `tencentcloud-sdk-python-ocr-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.885/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1427,14 +1427,39 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def RecognizeGeneralInvoice(self, request):
+        """本接口支持 单张、多张、多类型 票据的混合识别，同时支持自选需要识别的票据类型，已支持票种包括：增值税发票（专票、普票、卷票）、全电发票、非税发票、定额发票、通用机打发票、购车发票、火车票、出租车发票、机票行程单、汽车票、轮船票、过路过桥费发票共14种标准报销发票，并支持其他类发票的识别。
+
+        默认接口请求频率限制：5次/秒。
+
+        :param request: Request instance for RecognizeGeneralInvoice.
+        :type request: :class:`tencentcloud.ocr.v20181119.models.RecognizeGeneralInvoiceRequest`
+        :rtype: :class:`tencentcloud.ocr.v20181119.models.RecognizeGeneralInvoiceResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RecognizeGeneralInvoice", params, headers=headers)
+            response = json.loads(body)
+            model = models.RecognizeGeneralInvoiceResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def RecognizeHealthCodeOCR(self, request):
         """本接口支持北京、上海、广东、江苏、吉林、黑龙江、天津、辽宁、浙江、河南、四川、贵州、山东、安徽、福建、江西、湖北、湖南等省份健康码的识别，包括持码人姓名、持码人身份证号、健康码更新时间、健康码颜色、核酸检测结果、核酸检测间隔时长、核酸检测时间，疫苗接种信息，八个字段的识别结果输出。不同省市健康码显示的字段信息有所不同，上述字段的识别结果可能为空，以图片上具体展示的信息为准。
 
         默认接口请求频率限制：10次/秒。
 
         :param request: Request instance for RecognizeHealthCodeOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.RecognizeHealthCodeOCRRequest`
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.885/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.885/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/ocr/v20181119/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -114,14 +114,135 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class AirTransport(AbstractModel):
+    """机票行程单
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Title: 发票名称
+        :type Title: str
+        :param Number: 电子客票号码
+        :type Number: str
+        :param CheckCode: 校验码
+        :type CheckCode: str
+        :param SerialNumber: 印刷序号
+        :type SerialNumber: str
+        :param Date: 开票日期
+        :type Date: str
+        :param AgentCode: 销售单位代号
+        :type AgentCode: str
+        :param AgentCodeFirst: 销售单位代号第一行
+        :type AgentCodeFirst: str
+        :param AgentCodeSecond: 销售单位代号第二行
+        :type AgentCodeSecond: str
+        :param UserName: 姓名
+        :type UserName: str
+        :param UserID: 身份证号
+        :type UserID: str
+        :param Issuer: 填开单位
+        :type Issuer: str
+        :param Fare: 票价
+        :type Fare: str
+        :param Tax: 合计税额
+        :type Tax: str
+        :param FuelSurcharge: 燃油附加费
+        :type FuelSurcharge: str
+        :param AirDevelopmentFund: 民航发展基金
+        :type AirDevelopmentFund: str
+        :param Insurance: 保险费
+        :type Insurance: str
+        :param Total: 合计金额（小写）
+        :type Total: str
+        :param Kind: 发票消费类型
+        :type Kind: str
+        :param DomesticInternationalTag: 国内国际标签
+        :type DomesticInternationalTag: str
+        :param DateStart: 客票生效日期
+        :type DateStart: str
+        :param DateEnd: 有效截至日期
+        :type DateEnd: str
+        :param Endorsement: 签注
+        :type Endorsement: str
+        :param QRCodeMark: 是否存在二维码（1：有，0：无）
+        :type QRCodeMark: int
+        :param FlightItems: 条目
+        :type FlightItems: list of FlightItem
+        """
+        self.Title = None
+        self.Number = None
+        self.CheckCode = None
+        self.SerialNumber = None
+        self.Date = None
+        self.AgentCode = None
+        self.AgentCodeFirst = None
+        self.AgentCodeSecond = None
+        self.UserName = None
+        self.UserID = None
+        self.Issuer = None
+        self.Fare = None
+        self.Tax = None
+        self.FuelSurcharge = None
+        self.AirDevelopmentFund = None
+        self.Insurance = None
+        self.Total = None
+        self.Kind = None
+        self.DomesticInternationalTag = None
+        self.DateStart = None
+        self.DateEnd = None
+        self.Endorsement = None
+        self.QRCodeMark = None
+        self.FlightItems = None
+
+
+    def _deserialize(self, params):
+        self.Title = params.get("Title")
+        self.Number = params.get("Number")
+        self.CheckCode = params.get("CheckCode")
+        self.SerialNumber = params.get("SerialNumber")
+        self.Date = params.get("Date")
+        self.AgentCode = params.get("AgentCode")
+        self.AgentCodeFirst = params.get("AgentCodeFirst")
+        self.AgentCodeSecond = params.get("AgentCodeSecond")
+        self.UserName = params.get("UserName")
+        self.UserID = params.get("UserID")
+        self.Issuer = params.get("Issuer")
+        self.Fare = params.get("Fare")
+        self.Tax = params.get("Tax")
+        self.FuelSurcharge = params.get("FuelSurcharge")
+        self.AirDevelopmentFund = params.get("AirDevelopmentFund")
+        self.Insurance = params.get("Insurance")
+        self.Total = params.get("Total")
+        self.Kind = params.get("Kind")
+        self.DomesticInternationalTag = params.get("DomesticInternationalTag")
+        self.DateStart = params.get("DateStart")
+        self.DateEnd = params.get("DateEnd")
+        self.Endorsement = params.get("Endorsement")
+        self.QRCodeMark = params.get("QRCodeMark")
+        if params.get("FlightItems") is not None:
+            self.FlightItems = []
+            for item in params.get("FlightItems"):
+                obj = FlightItem()
+                obj._deserialize(item)
+                self.FlightItems.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ArithmeticOCRRequest(AbstractModel):
     """ArithmeticOCR请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -566,14 +687,118 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class BusInvoice(AbstractModel):
+    """汽车票
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Title: 发票名称
+        :type Title: str
+        :param QRCodeMark: 是否存在二维码（1：有，0：无）
+        :type QRCodeMark: int
+        :param Number: 发票号码
+        :type Number: str
+        :param Code: 发票代码
+        :type Code: str
+        :param Date: 开票日期
+        :type Date: str
+        :param TimeGetOn: 乘车时间
+        :type TimeGetOn: str
+        :param DateGetOn: 乘车日期
+        :type DateGetOn: str
+        :param StationGetOn: 出发车站
+        :type StationGetOn: str
+        :param StationGetOff: 到达车站
+        :type StationGetOff: str
+        :param Total: 票价
+        :type Total: str
+        :param UserName: 姓名
+        :type UserName: str
+        :param Kind: 消费类型
+        :type Kind: str
+        :param UserID: 身份证号
+        :type UserID: str
+        :param Province: 省
+        :type Province: str
+        :param City: 市
+        :type City: str
+        :param PlaceGetOn: 乘车地点
+        :type PlaceGetOn: str
+        :param GateNumber: 检票口
+        :type GateNumber: str
+        :param TicketType: 客票类型
+        :type TicketType: str
+        :param VehicleType: 车型
+        :type VehicleType: str
+        :param SeatNumber: 座位号
+        :type SeatNumber: str
+        :param TrainNumber: 车次
+        :type TrainNumber: str
+        """
+        self.Title = None
+        self.QRCodeMark = None
+        self.Number = None
+        self.Code = None
+        self.Date = None
+        self.TimeGetOn = None
+        self.DateGetOn = None
+        self.StationGetOn = None
+        self.StationGetOff = None
+        self.Total = None
+        self.UserName = None
+        self.Kind = None
+        self.UserID = None
+        self.Province = None
+        self.City = None
+        self.PlaceGetOn = None
+        self.GateNumber = None
+        self.TicketType = None
+        self.VehicleType = None
+        self.SeatNumber = None
+        self.TrainNumber = None
+
+
+    def _deserialize(self, params):
+        self.Title = params.get("Title")
+        self.QRCodeMark = params.get("QRCodeMark")
+        self.Number = params.get("Number")
+        self.Code = params.get("Code")
+        self.Date = params.get("Date")
+        self.TimeGetOn = params.get("TimeGetOn")
+        self.DateGetOn = params.get("DateGetOn")
+        self.StationGetOn = params.get("StationGetOn")
+        self.StationGetOff = params.get("StationGetOff")
+        self.Total = params.get("Total")
+        self.UserName = params.get("UserName")
+        self.Kind = params.get("Kind")
+        self.UserID = params.get("UserID")
+        self.Province = params.get("Province")
+        self.City = params.get("City")
+        self.PlaceGetOn = params.get("PlaceGetOn")
+        self.GateNumber = params.get("GateNumber")
+        self.TicketType = params.get("TicketType")
+        self.VehicleType = params.get("VehicleType")
+        self.SeatNumber = params.get("SeatNumber")
+        self.TrainNumber = params.get("TrainNumber")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class BusInvoiceInfo(AbstractModel):
     """汽车票字段信息
 
     """
 
     def __init__(self):
         r"""
@@ -2138,14 +2363,78 @@
             for item in params.get("FlightInvoiceInfos"):
                 obj = FlightInvoiceInfo()
                 obj._deserialize(item)
                 self.FlightInvoiceInfos.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class FlightItem(AbstractModel):
+    """机票行程卡条目
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TerminalGetOn: 出发航站楼
+        :type TerminalGetOn: str
+        :param TerminalGetOff: 到达航站楼
+        :type TerminalGetOff: str
+        :param Carrier: 承运人
+        :type Carrier: str
+        :param FlightNumber: 航班号
+        :type FlightNumber: str
+        :param Seat: 座位等级
+        :type Seat: str
+        :param DateGetOn: 乘机日期
+        :type DateGetOn: str
+        :param TimeGetOn: 乘机时间
+        :type TimeGetOn: str
+        :param StationGetOn: 出发站
+        :type StationGetOn: str
+        :param StationGetOff: 到达站
+        :type StationGetOff: str
+        :param Allow: 免费行李
+        :type Allow: str
+        :param FareBasis: 客票级别/客票类别
+        :type FareBasis: str
+        """
+        self.TerminalGetOn = None
+        self.TerminalGetOff = None
+        self.Carrier = None
+        self.FlightNumber = None
+        self.Seat = None
+        self.DateGetOn = None
+        self.TimeGetOn = None
+        self.StationGetOn = None
+        self.StationGetOff = None
+        self.Allow = None
+        self.FareBasis = None
+
+
+    def _deserialize(self, params):
+        self.TerminalGetOn = params.get("TerminalGetOn")
+        self.TerminalGetOff = params.get("TerminalGetOff")
+        self.Carrier = params.get("Carrier")
+        self.FlightNumber = params.get("FlightNumber")
+        self.Seat = params.get("Seat")
+        self.DateGetOn = params.get("DateGetOn")
+        self.TimeGetOn = params.get("TimeGetOn")
+        self.StationGetOn = params.get("StationGetOn")
+        self.StationGetOff = params.get("StationGetOff")
+        self.Allow = params.get("Allow")
+        self.FareBasis = params.get("FareBasis")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class FormulaOCRRequest(AbstractModel):
     """FormulaOCR请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2619,14 +2908,66 @@
                 obj = TextGeneralHandwriting()
                 obj._deserialize(item)
                 self.TextDetections.append(obj)
         self.Angel = params.get("Angel")
         self.RequestId = params.get("RequestId")
 
 
+class GeneralMachineItem(AbstractModel):
+    """通用机打发票条目
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: 项目名称
+        :type Name: str
+        :param Specification: 规格型号
+        :type Specification: str
+        :param Unit: 单位
+        :type Unit: str
+        :param Quantity: 数量
+        :type Quantity: str
+        :param Price: 单价
+        :type Price: str
+        :param Total: 金额
+        :type Total: str
+        :param TaxRate: 税率
+        :type TaxRate: str
+        :param Tax: 税额
+        :type Tax: str
+        """
+        self.Name = None
+        self.Specification = None
+        self.Unit = None
+        self.Quantity = None
+        self.Price = None
+        self.Total = None
+        self.TaxRate = None
+        self.Tax = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        self.Specification = params.get("Specification")
+        self.Unit = params.get("Unit")
+        self.Quantity = params.get("Quantity")
+        self.Price = params.get("Price")
+        self.Total = params.get("Total")
+        self.TaxRate = params.get("TaxRate")
+        self.Tax = params.get("Tax")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class GetTaskStateRequest(AbstractModel):
     """GetTaskState请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -3460,14 +3801,95 @@
                 obj = InvoiceGeneralInfo()
                 obj._deserialize(item)
                 self.InvoiceGeneralInfos.append(obj)
         self.Angle = params.get("Angle")
         self.RequestId = params.get("RequestId")
 
 
+class InvoiceItem(AbstractModel):
+    """混贴票据单张发票识别信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Code: 识别结果。
+OK：表示识别成功；FailedOperation.UnsupportedInvioce：表示不支持识别；
+FailedOperation.UnKnowError：表示识别失败；
+其它错误码见各个票据接口的定义。
+        :type Code: str
+        :param Type: 识别出的图片所属的票据类型。
+-1：未知类型
+0：出租车发票
+1：定额发票
+2：火车票
+3：增值税发票
+5：机票行程单
+8：通用机打发票
+9：汽车票
+10：轮船票
+11：增值税发票（卷票）
+12：购车发票
+13：过路过桥费发票
+15：非税发票
+16：全电发票
+        :type Type: int
+        :param Polygon: 旋转后的图片四点坐标。
+        :type Polygon: :class:`tencentcloud.ocr.v20181119.models.Polygon`
+        :param Angle: 识别出的图片在混贴票据图片中的旋转角度。
+        :type Angle: float
+        :param SingleInvoiceInfos: 识别到的内容。
+        :type SingleInvoiceInfos: :class:`tencentcloud.ocr.v20181119.models.SingleInvoiceItem`
+        :param Page: 发票处于识别图片或PDF文件中的页教，默认从1开始。
+        :type Page: int
+        :param SubType: 发票详细类型，详见下方 SubType 返回值说明
+        :type SubType: str
+        :param TypeDescription: 发票类型描述，详见下方 TypeDescription  返回值说明
+        :type TypeDescription: str
+        :param CutImage: 切割单图文件，Base64编码后的切图后的图片文件，开启 EnableCutImage 后进行返回
+        :type CutImage: str
+        :param SubTypeDescription: 发票详细类型描述，详见下方 SubType 返回值说明
+        :type SubTypeDescription: str
+        """
+        self.Code = None
+        self.Type = None
+        self.Polygon = None
+        self.Angle = None
+        self.SingleInvoiceInfos = None
+        self.Page = None
+        self.SubType = None
+        self.TypeDescription = None
+        self.CutImage = None
+        self.SubTypeDescription = None
+
+
+    def _deserialize(self, params):
+        self.Code = params.get("Code")
+        self.Type = params.get("Type")
+        if params.get("Polygon") is not None:
+            self.Polygon = Polygon()
+            self.Polygon._deserialize(params.get("Polygon"))
+        self.Angle = params.get("Angle")
+        if params.get("SingleInvoiceInfos") is not None:
+            self.SingleInvoiceInfos = SingleInvoiceItem()
+            self.SingleInvoiceInfos._deserialize(params.get("SingleInvoiceInfos"))
+        self.Page = params.get("Page")
+        self.SubType = params.get("SubType")
+        self.TypeDescription = params.get("TypeDescription")
+        self.CutImage = params.get("CutImage")
+        self.SubTypeDescription = params.get("SubTypeDescription")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ItemCoord(AbstractModel):
     """文本行在旋转纠正之后的图像中的像素坐标，表示为（左上角x, 左上角y，宽width，高height）
 
     """
 
     def __init__(self):
         r"""
@@ -3922,14 +4344,183 @@
         self.CodeSet = params.get("CodeSet")
         self.CodeCrc = params.get("CodeCrc")
         self.Surname = params.get("Surname")
         self.GivenName = params.get("GivenName")
         self.RequestId = params.get("RequestId")
 
 
+class MachinePrintedInvoice(AbstractModel):
+    """通用机打发票
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Title: 发票名称
+        :type Title: str
+        :param QRCodeMark: 是否存在二维码（1：有，0：无）
+        :type QRCodeMark: int
+        :param Code: 发票代码
+        :type Code: str
+        :param Number: 发票号码
+        :type Number: str
+        :param Date: 开票日期
+        :type Date: str
+        :param Time: 时间
+        :type Time: str
+        :param CheckCode: 校验码
+        :type CheckCode: str
+        :param Ciphertext: 密码区
+        :type Ciphertext: str
+        :param Category: 种类
+        :type Category: str
+        :param PretaxAmount: 税前金额
+        :type PretaxAmount: str
+        :param Total: 价税合计（小写）
+        :type Total: str
+        :param TotalCn: 价税合计（大写）
+        :type TotalCn: str
+        :param Tax: 合计税额
+        :type Tax: str
+        :param IndustryClass: 行业分类
+        :type IndustryClass: str
+        :param Seller: 销售方名称
+        :type Seller: str
+        :param SellerTaxID: 销售方纳税人识别号
+        :type SellerTaxID: str
+        :param SellerAddrTel: 销售方地址电话
+        :type SellerAddrTel: str
+        :param SellerBankAccount: 销售方银行账号
+        :type SellerBankAccount: str
+        :param Buyer: 购买方名称
+        :type Buyer: str
+        :param BuyerTaxID: 购买方纳税人识别号
+        :type BuyerTaxID: str
+        :param BuyerAddrTel: 购买方地址电话
+        :type BuyerAddrTel: str
+        :param BuyerBankAccount: 购买方银行账号
+        :type BuyerBankAccount: str
+        :param Kind: 发票消费类型
+        :type Kind: str
+        :param Province: 省
+        :type Province: str
+        :param City: 市
+        :type City: str
+        :param CompanySealMark: 是否有公司印章（0：没有，1：有）
+        :type CompanySealMark: int
+        :param ElectronicMark: 是否为浙江/广东通用机打发票（0：没有，1：有）
+        :type ElectronicMark: int
+        :param Issuer: 开票人
+        :type Issuer: str
+        :param Receiptor: 收款人
+        :type Receiptor: str
+        :param Reviewer: 复核人
+        :type Reviewer: str
+        :param Remark: 备注
+        :type Remark: str
+        :param PaymentInfo: 经办人支付信息
+        :type PaymentInfo: str
+        :param TicketPickupUser: 经办人取票用户
+        :type TicketPickupUser: str
+        :param MerchantNumber: 经办人商户号
+        :type MerchantNumber: str
+        :param OrderNumber: 经办人订单号
+        :type OrderNumber: str
+        :param GeneralMachineItems: 条目
+        :type GeneralMachineItems: list of GeneralMachineItem
+        """
+        self.Title = None
+        self.QRCodeMark = None
+        self.Code = None
+        self.Number = None
+        self.Date = None
+        self.Time = None
+        self.CheckCode = None
+        self.Ciphertext = None
+        self.Category = None
+        self.PretaxAmount = None
+        self.Total = None
+        self.TotalCn = None
+        self.Tax = None
+        self.IndustryClass = None
+        self.Seller = None
+        self.SellerTaxID = None
+        self.SellerAddrTel = None
+        self.SellerBankAccount = None
+        self.Buyer = None
+        self.BuyerTaxID = None
+        self.BuyerAddrTel = None
+        self.BuyerBankAccount = None
+        self.Kind = None
+        self.Province = None
+        self.City = None
+        self.CompanySealMark = None
+        self.ElectronicMark = None
+        self.Issuer = None
+        self.Receiptor = None
+        self.Reviewer = None
+        self.Remark = None
+        self.PaymentInfo = None
+        self.TicketPickupUser = None
+        self.MerchantNumber = None
+        self.OrderNumber = None
+        self.GeneralMachineItems = None
+
+
+    def _deserialize(self, params):
+        self.Title = params.get("Title")
+        self.QRCodeMark = params.get("QRCodeMark")
+        self.Code = params.get("Code")
+        self.Number = params.get("Number")
+        self.Date = params.get("Date")
+        self.Time = params.get("Time")
+        self.CheckCode = params.get("CheckCode")
+        self.Ciphertext = params.get("Ciphertext")
+        self.Category = params.get("Category")
+        self.PretaxAmount = params.get("PretaxAmount")
+        self.Total = params.get("Total")
+        self.TotalCn = params.get("TotalCn")
+        self.Tax = params.get("Tax")
+        self.IndustryClass = params.get("IndustryClass")
+        self.Seller = params.get("Seller")
+        self.SellerTaxID = params.get("SellerTaxID")
+        self.SellerAddrTel = params.get("SellerAddrTel")
+        self.SellerBankAccount = params.get("SellerBankAccount")
+        self.Buyer = params.get("Buyer")
+        self.BuyerTaxID = params.get("BuyerTaxID")
+        self.BuyerAddrTel = params.get("BuyerAddrTel")
+        self.BuyerBankAccount = params.get("BuyerBankAccount")
+        self.Kind = params.get("Kind")
+        self.Province = params.get("Province")
+        self.City = params.get("City")
+        self.CompanySealMark = params.get("CompanySealMark")
+        self.ElectronicMark = params.get("ElectronicMark")
+        self.Issuer = params.get("Issuer")
+        self.Receiptor = params.get("Receiptor")
+        self.Reviewer = params.get("Reviewer")
+        self.Remark = params.get("Remark")
+        self.PaymentInfo = params.get("PaymentInfo")
+        self.TicketPickupUser = params.get("TicketPickupUser")
+        self.MerchantNumber = params.get("MerchantNumber")
+        self.OrderNumber = params.get("OrderNumber")
+        if params.get("GeneralMachineItems") is not None:
+            self.GeneralMachineItems = []
+            for item in params.get("GeneralMachineItems"):
+                obj = GeneralMachineItem()
+                obj._deserialize(item)
+                self.GeneralMachineItems.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class MainlandPermitOCRRequest(AbstractModel):
     """MainlandPermitOCR请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4333,14 +4924,371 @@
             for item in params.get("MixedInvoiceItems"):
                 obj = MixedInvoiceItem()
                 obj._deserialize(item)
                 self.MixedInvoiceItems.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class MotorVehicleSaleInvoice(AbstractModel):
+    """机动车销售统一发票
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Title: 发票名称
+        :type Title: str
+        :param Code: 发票代码
+        :type Code: str
+        :param Number: 发票号码
+        :type Number: str
+        :param Date: 开票日期
+        :type Date: str
+        :param PretaxAmount: 税前金额
+        :type PretaxAmount: str
+        :param Total: 价税合计（小写）
+        :type Total: str
+        :param TotalCn: 价税合计（大写）
+        :type TotalCn: str
+        :param Seller: 销售方名称
+        :type Seller: str
+        :param SellerTaxID: 销售方单位代码
+        :type SellerTaxID: str
+        :param SellerTel: 销售方电话
+        :type SellerTel: str
+        :param SellerAddress: 销售方地址
+        :type SellerAddress: str
+        :param SellerBank: 销售方开户行
+        :type SellerBank: str
+        :param SellerBankAccount: 销售方银行账号
+        :type SellerBankAccount: str
+        :param Buyer: 购买方名称
+        :type Buyer: str
+        :param BuyerTaxID: 购买方纳税人识别号
+        :type BuyerTaxID: str
+        :param BuyerID: 购买方身份证号码/组织机构代码
+        :type BuyerID: str
+        :param TaxAuthorities: 主管税务机关
+        :type TaxAuthorities: str
+        :param TaxAuthoritiesCode: 主管税务机关代码
+        :type TaxAuthoritiesCode: str
+        :param VIN: 车辆识别代码
+        :type VIN: str
+        :param VehicleModel: 厂牌型号
+        :type VehicleModel: str
+        :param VehicleEngineCode: 发动机号码
+        :type VehicleEngineCode: str
+        :param CertificateNumber: 合格证号
+        :type CertificateNumber: str
+        :param InspectionNumber: 商检单号
+        :type InspectionNumber: str
+        :param MachineID: 机器编号
+        :type MachineID: str
+        :param VehicleType: 车辆类型
+        :type VehicleType: str
+        :param Kind: 发票消费类型
+        :type Kind: str
+        :param Province: 省
+        :type Province: str
+        :param City: 市
+        :type City: str
+        :param Tax: 合计税额
+        :type Tax: str
+        :param TaxRate: 税率
+        :type TaxRate: str
+        :param CompanySealMark: 是否有公司印章（0：没有，1：有）
+        :type CompanySealMark: int
+        :param Tonnage: 吨位
+        :type Tonnage: str
+        :param Remark: 备注
+        :type Remark: str
+        :param FormType: 发票联次
+        :type FormType: str
+        :param FormName: 发票联名
+        :type FormName: str
+        :param Issuer: 开票人
+        :type Issuer: str
+        :param TaxNum: 完税凭证号码
+        :type TaxNum: str
+        :param MaxPeopleNum: 限乘人数
+        :type MaxPeopleNum: str
+        :param Origin: 产地
+        :type Origin: str
+        :param MachineCode: 机打发票代码
+        :type MachineCode: str
+        :param MachineNumber: 机打发票号码
+        :type MachineNumber: str
+        :param QRCodeMark: 是否存在二维码（1：有，0：无）
+        :type QRCodeMark: int
+        """
+        self.Title = None
+        self.Code = None
+        self.Number = None
+        self.Date = None
+        self.PretaxAmount = None
+        self.Total = None
+        self.TotalCn = None
+        self.Seller = None
+        self.SellerTaxID = None
+        self.SellerTel = None
+        self.SellerAddress = None
+        self.SellerBank = None
+        self.SellerBankAccount = None
+        self.Buyer = None
+        self.BuyerTaxID = None
+        self.BuyerID = None
+        self.TaxAuthorities = None
+        self.TaxAuthoritiesCode = None
+        self.VIN = None
+        self.VehicleModel = None
+        self.VehicleEngineCode = None
+        self.CertificateNumber = None
+        self.InspectionNumber = None
+        self.MachineID = None
+        self.VehicleType = None
+        self.Kind = None
+        self.Province = None
+        self.City = None
+        self.Tax = None
+        self.TaxRate = None
+        self.CompanySealMark = None
+        self.Tonnage = None
+        self.Remark = None
+        self.FormType = None
+        self.FormName = None
+        self.Issuer = None
+        self.TaxNum = None
+        self.MaxPeopleNum = None
+        self.Origin = None
+        self.MachineCode = None
+        self.MachineNumber = None
+        self.QRCodeMark = None
+
+
+    def _deserialize(self, params):
+        self.Title = params.get("Title")
+        self.Code = params.get("Code")
+        self.Number = params.get("Number")
+        self.Date = params.get("Date")
+        self.PretaxAmount = params.get("PretaxAmount")
+        self.Total = params.get("Total")
+        self.TotalCn = params.get("TotalCn")
+        self.Seller = params.get("Seller")
+        self.SellerTaxID = params.get("SellerTaxID")
+        self.SellerTel = params.get("SellerTel")
+        self.SellerAddress = params.get("SellerAddress")
+        self.SellerBank = params.get("SellerBank")
+        self.SellerBankAccount = params.get("SellerBankAccount")
+        self.Buyer = params.get("Buyer")
+        self.BuyerTaxID = params.get("BuyerTaxID")
+        self.BuyerID = params.get("BuyerID")
+        self.TaxAuthorities = params.get("TaxAuthorities")
+        self.TaxAuthoritiesCode = params.get("TaxAuthoritiesCode")
+        self.VIN = params.get("VIN")
+        self.VehicleModel = params.get("VehicleModel")
+        self.VehicleEngineCode = params.get("VehicleEngineCode")
+        self.CertificateNumber = params.get("CertificateNumber")
+        self.InspectionNumber = params.get("InspectionNumber")
+        self.MachineID = params.get("MachineID")
+        self.VehicleType = params.get("VehicleType")
+        self.Kind = params.get("Kind")
+        self.Province = params.get("Province")
+        self.City = params.get("City")
+        self.Tax = params.get("Tax")
+        self.TaxRate = params.get("TaxRate")
+        self.CompanySealMark = params.get("CompanySealMark")
+        self.Tonnage = params.get("Tonnage")
+        self.Remark = params.get("Remark")
+        self.FormType = params.get("FormType")
+        self.FormName = params.get("FormName")
+        self.Issuer = params.get("Issuer")
+        self.TaxNum = params.get("TaxNum")
+        self.MaxPeopleNum = params.get("MaxPeopleNum")
+        self.Origin = params.get("Origin")
+        self.MachineCode = params.get("MachineCode")
+        self.MachineNumber = params.get("MachineNumber")
+        self.QRCodeMark = params.get("QRCodeMark")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class NonTaxIncomeBill(AbstractModel):
+    """非税收入
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Title: 发票名称
+        :type Title: str
+        :param Number: 发票号码
+        :type Number: str
+        :param Code: 发票代码
+        :type Code: str
+        :param CheckCode: 校验码
+        :type CheckCode: str
+        :param Date: 开票日期
+        :type Date: str
+        :param Total: 价税合计（小写）
+        :type Total: str
+        :param TotalCn: 价税合计（大写）
+        :type TotalCn: str
+        :param Buyer: 交款人名称
+        :type Buyer: str
+        :param BuyerTaxID: 交款人纳税人识别号
+        :type BuyerTaxID: str
+        :param Seller: 收款人名称
+        :type Seller: str
+        :param SellerCompany: 收款单位名称
+        :type SellerCompany: str
+        :param Remark: 备注
+        :type Remark: str
+        :param CurrencyCode: 币种
+        :type CurrencyCode: str
+        :param Reviewer: 复核人
+        :type Reviewer: str
+        :param QRCodeMark: 是否存在二维码（1：有，0：无）
+        :type QRCodeMark: int
+        :param OtherInfo: 其他信息
+        :type OtherInfo: str
+        :param PaymentCode: 缴款码
+        :type PaymentCode: str
+        :param ReceiveUnitCode: 执收单位编码
+        :type ReceiveUnitCode: str
+        :param Receiver: 执收单位名称
+        :type Receiver: str
+        :param Operator: 经办人
+        :type Operator: str
+        :param PayerAccount: 付款人账号
+        :type PayerAccount: str
+        :param PayerBank: 付款人开户银行
+        :type PayerBank: str
+        :param ReceiverAccount: 收款人账号
+        :type ReceiverAccount: str
+        :param ReceiverBank: 收款人开户银行
+        :type ReceiverBank: str
+        :param NonTaxItems: 条目
+        :type NonTaxItems: list of NonTaxItem
+        """
+        self.Title = None
+        self.Number = None
+        self.Code = None
+        self.CheckCode = None
+        self.Date = None
+        self.Total = None
+        self.TotalCn = None
+        self.Buyer = None
+        self.BuyerTaxID = None
+        self.Seller = None
+        self.SellerCompany = None
+        self.Remark = None
+        self.CurrencyCode = None
+        self.Reviewer = None
+        self.QRCodeMark = None
+        self.OtherInfo = None
+        self.PaymentCode = None
+        self.ReceiveUnitCode = None
+        self.Receiver = None
+        self.Operator = None
+        self.PayerAccount = None
+        self.PayerBank = None
+        self.ReceiverAccount = None
+        self.ReceiverBank = None
+        self.NonTaxItems = None
+
+
+    def _deserialize(self, params):
+        self.Title = params.get("Title")
+        self.Number = params.get("Number")
+        self.Code = params.get("Code")
+        self.CheckCode = params.get("CheckCode")
+        self.Date = params.get("Date")
+        self.Total = params.get("Total")
+        self.TotalCn = params.get("TotalCn")
+        self.Buyer = params.get("Buyer")
+        self.BuyerTaxID = params.get("BuyerTaxID")
+        self.Seller = params.get("Seller")
+        self.SellerCompany = params.get("SellerCompany")
+        self.Remark = params.get("Remark")
+        self.CurrencyCode = params.get("CurrencyCode")
+        self.Reviewer = params.get("Reviewer")
+        self.QRCodeMark = params.get("QRCodeMark")
+        self.OtherInfo = params.get("OtherInfo")
+        self.PaymentCode = params.get("PaymentCode")
+        self.ReceiveUnitCode = params.get("ReceiveUnitCode")
+        self.Receiver = params.get("Receiver")
+        self.Operator = params.get("Operator")
+        self.PayerAccount = params.get("PayerAccount")
+        self.PayerBank = params.get("PayerBank")
+        self.ReceiverAccount = params.get("ReceiverAccount")
+        self.ReceiverBank = params.get("ReceiverBank")
+        if params.get("NonTaxItems") is not None:
+            self.NonTaxItems = []
+            for item in params.get("NonTaxItems"):
+                obj = NonTaxItem()
+                obj._deserialize(item)
+                self.NonTaxItems.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class NonTaxItem(AbstractModel):
+    """非税收入条目
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ItemID: 项目编码
+        :type ItemID: str
+        :param Name: 项目名称
+        :type Name: str
+        :param Unit: 单位
+        :type Unit: str
+        :param Quantity: 数量
+        :type Quantity: str
+        :param Standard: 标准
+        :type Standard: str
+        :param Total: 金额
+        :type Total: str
+        """
+        self.ItemID = None
+        self.Name = None
+        self.Unit = None
+        self.Quantity = None
+        self.Standard = None
+        self.Total = None
+
+
+    def _deserialize(self, params):
+        self.ItemID = params.get("ItemID")
+        self.Name = params.get("Name")
+        self.Unit = params.get("Unit")
+        self.Quantity = params.get("Quantity")
+        self.Standard = params.get("Standard")
+        self.Total = params.get("Total")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class OnlineTaxiItineraryInfo(AbstractModel):
     """网约车行程单识别结果
 
     """
 
     def __init__(self):
         r"""
@@ -4434,14 +5382,117 @@
         self.OrgCode = params.get("OrgCode")
         self.Name = params.get("Name")
         self.Address = params.get("Address")
         self.ValidDate = params.get("ValidDate")
         self.RequestId = params.get("RequestId")
 
 
+class OtherInvoice(AbstractModel):
+    """其他发票
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Title: 发票名称
+        :type Title: str
+        :param Total: 金额
+        :type Total: str
+        :param OtherInvoiceListItems: 列表
+        :type OtherInvoiceListItems: list of OtherInvoiceItem
+        :param OtherInvoiceTableItems: 表格
+        :type OtherInvoiceTableItems: list of OtherInvoiceList
+        """
+        self.Title = None
+        self.Total = None
+        self.OtherInvoiceListItems = None
+        self.OtherInvoiceTableItems = None
+
+
+    def _deserialize(self, params):
+        self.Title = params.get("Title")
+        self.Total = params.get("Total")
+        if params.get("OtherInvoiceListItems") is not None:
+            self.OtherInvoiceListItems = []
+            for item in params.get("OtherInvoiceListItems"):
+                obj = OtherInvoiceItem()
+                obj._deserialize(item)
+                self.OtherInvoiceListItems.append(obj)
+        if params.get("OtherInvoiceTableItems") is not None:
+            self.OtherInvoiceTableItems = []
+            for item in params.get("OtherInvoiceTableItems"):
+                obj = OtherInvoiceList()
+                obj._deserialize(item)
+                self.OtherInvoiceTableItems.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class OtherInvoiceItem(AbstractModel):
+    """OtherInvoiceItem
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: 票面key值
+        :type Name: str
+        :param Value: 票面value值
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
+class OtherInvoiceList(AbstractModel):
+    """其他票Table
+
+    """
+
+    def __init__(self):
+        r"""
+        :param OtherInvoiceItemList: 列表
+        :type OtherInvoiceItemList: list of OtherInvoiceItem
+        """
+        self.OtherInvoiceItemList = None
+
+
+    def _deserialize(self, params):
+        if params.get("OtherInvoiceItemList") is not None:
+            self.OtherInvoiceItemList = []
+            for item in params.get("OtherInvoiceItemList"):
+                obj = OtherInvoiceItem()
+                obj._deserialize(item)
+                self.OtherInvoiceItemList.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class PassInvoiceInfo(AbstractModel):
     """通行费发票信息
 
     """
 
     def __init__(self):
         r"""
@@ -5199,14 +6250,74 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class QuotaInvoice(AbstractModel):
+    """定额发票
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Title: 发票名称
+        :type Title: str
+        :param Code: 发票代码
+        :type Code: str
+        :param Number: 发票号码
+        :type Number: str
+        :param Total: 价税合计（小写）
+        :type Total: str
+        :param TotalCn: 价税合计（大写）
+        :type TotalCn: str
+        :param Kind: 发票消费类型
+        :type Kind: str
+        :param Province: 省
+        :type Province: str
+        :param City: 市
+        :type City: str
+        :param QRCodeMark: 是否存在二维码（1：有，0：无）
+        :type QRCodeMark: int
+        :param CompanySealMark: 是否有公司印章（0：没有，1：有）
+        :type CompanySealMark: int
+        """
+        self.Title = None
+        self.Code = None
+        self.Number = None
+        self.Total = None
+        self.TotalCn = None
+        self.Kind = None
+        self.Province = None
+        self.City = None
+        self.QRCodeMark = None
+        self.CompanySealMark = None
+
+
+    def _deserialize(self, params):
+        self.Title = params.get("Title")
+        self.Code = params.get("Code")
+        self.Number = params.get("Number")
+        self.Total = params.get("Total")
+        self.TotalCn = params.get("TotalCn")
+        self.Kind = params.get("Kind")
+        self.Province = params.get("Province")
+        self.City = params.get("City")
+        self.QRCodeMark = params.get("QRCodeMark")
+        self.CompanySealMark = params.get("CompanySealMark")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class QuotaInvoiceOCRRequest(AbstractModel):
     """QuotaInvoiceOCR请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5392,14 +6503,118 @@
         self.CapacityFT3 = params.get("CapacityFT3")
         self.Warn = params.get("Warn")
         self.TareKG = params.get("TareKG")
         self.TareLB = params.get("TareLB")
         self.RequestId = params.get("RequestId")
 
 
+class RecognizeGeneralInvoiceRequest(AbstractModel):
+    """RecognizeGeneralInvoice请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ImageBase64: 图片的 Base64 值。
+支持的图片格式：PNG、JPG、JPEG、PDF，暂不支持 GIF 格式。
+支持的图片大小：所下载图片经Base64编码后不超过 7M。图片下载时间不超过 3 秒。
+图片的 ImageUrl、ImageBase64 必须提供一个，如果都提供，只使用 ImageUrl。
+        :type ImageBase64: str
+        :param ImageUrl: 图片的 Url 地址。
+支持的图片格式：PNG、JPG、JPEG、PDF，暂不支持 GIF 格式。
+支持的图片大小：所下载图片经 Base64 编码后不超过 7M。图片下载时间不超过 3 秒。
+图片存储于腾讯云的 Url 可保障更高的下载速度和稳定性，建议图片存储于腾讯云。
+非腾讯云存储的 Url 速度和稳定性可能受一定影响。
+        :type ImageUrl: str
+        :param Types: 需要识别的票据类型列表，为空或不填表示识别全部类型。
+0：出租车发票
+1：定额发票
+2：火车票
+3：增值税发票
+5：机票行程单
+8：通用机打发票
+9：汽车票
+10：轮船票
+11：增值税发票（卷票 ）
+12：购车发票
+13：过路过桥费发票
+15：非税发票
+16：全电发票
+----------------------
+-1：其他发票,（只传入此类型时，图片均采用其他票类型进行识别）
+        :type Types: list of int
+        :param EnableOther: 是否开启其他票识别，默认值为true，开启后可支持其他发票的智能识别。	
+        :type EnableOther: bool
+        :param EnablePdf: 是否开启PDF识别，默认值为true，开启后可同时支持图片和PDF的识别。
+        :type EnablePdf: bool
+        :param PdfPageNumber: 需要识别的PDF页面的对应页码，传入时仅支持PDF单页识别，当上传文件为PDF且EnablePdf参数值为true时有效，默认值为1。
+        :type PdfPageNumber: int
+        :param EnableMultiplePage: 是否开启PDF多页识别，默认值为false，开启后可同时支持多页PDF的识别返回，仅支持返回文件前30页。开启后EnablePdf和PdfPageNumber入参不进行控制。
+        :type EnableMultiplePage: bool
+        :param EnableCutImage: 是否返回切割图片base64，默认值为false。
+        :type EnableCutImage: bool
+        """
+        self.ImageBase64 = None
+        self.ImageUrl = None
+        self.Types = None
+        self.EnableOther = None
+        self.EnablePdf = None
+        self.PdfPageNumber = None
+        self.EnableMultiplePage = None
+        self.EnableCutImage = None
+
+
+    def _deserialize(self, params):
+        self.ImageBase64 = params.get("ImageBase64")
+        self.ImageUrl = params.get("ImageUrl")
+        self.Types = params.get("Types")
+        self.EnableOther = params.get("EnableOther")
+        self.EnablePdf = params.get("EnablePdf")
+        self.PdfPageNumber = params.get("PdfPageNumber")
+        self.EnableMultiplePage = params.get("EnableMultiplePage")
+        self.EnableCutImage = params.get("EnableCutImage")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RecognizeGeneralInvoiceResponse(AbstractModel):
+    """RecognizeGeneralInvoice返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param MixedInvoiceItems: 混贴票据识别结果，具体内容请点击左侧链接。
+        :type MixedInvoiceItems: list of InvoiceItem
+        :param TotalPDFCount: PDF文件总页码
+        :type TotalPDFCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.MixedInvoiceItems = None
+        self.TotalPDFCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("MixedInvoiceItems") is not None:
+            self.MixedInvoiceItems = []
+            for item in params.get("MixedInvoiceItems"):
+                obj = InvoiceItem()
+                obj._deserialize(item)
+                self.MixedInvoiceItems.append(obj)
+        self.TotalPDFCount = params.get("TotalPDFCount")
+        self.RequestId = params.get("RequestId")
+
+
 class RecognizeHealthCodeOCRRequest(AbstractModel):
     """RecognizeHealthCodeOCR请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -7071,14 +8286,90 @@
                 obj = ShipInvoiceInfo()
                 obj._deserialize(item)
                 self.ShipInvoiceInfos.append(obj)
         self.Angle = params.get("Angle")
         self.RequestId = params.get("RequestId")
 
 
+class ShippingInvoice(AbstractModel):
+    """轮船票
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Title: 发票名称
+        :type Title: str
+        :param QRCodeMark: 是否存在二维码（1：有，0：无）
+        :type QRCodeMark: int
+        :param Code: 发票代码
+        :type Code: str
+        :param Number: 发票号码
+        :type Number: str
+        :param UserName: 姓名
+        :type UserName: str
+        :param Date: 日期
+        :type Date: str
+        :param Time: 时间
+        :type Time: str
+        :param StationGetOn: 出发车站
+        :type StationGetOn: str
+        :param StationGetOff: 到达车站
+        :type StationGetOff: str
+        :param Total: 票价
+        :type Total: str
+        :param Kind: 发票消费类型
+        :type Kind: str
+        :param Province: 省
+        :type Province: str
+        :param City: 市
+        :type City: str
+        :param CurrencyCode: 币种
+        :type CurrencyCode: str
+        """
+        self.Title = None
+        self.QRCodeMark = None
+        self.Code = None
+        self.Number = None
+        self.UserName = None
+        self.Date = None
+        self.Time = None
+        self.StationGetOn = None
+        self.StationGetOff = None
+        self.Total = None
+        self.Kind = None
+        self.Province = None
+        self.City = None
+        self.CurrencyCode = None
+
+
+    def _deserialize(self, params):
+        self.Title = params.get("Title")
+        self.QRCodeMark = params.get("QRCodeMark")
+        self.Code = params.get("Code")
+        self.Number = params.get("Number")
+        self.UserName = params.get("UserName")
+        self.Date = params.get("Date")
+        self.Time = params.get("Time")
+        self.StationGetOn = params.get("StationGetOn")
+        self.StationGetOff = params.get("StationGetOff")
+        self.Total = params.get("Total")
+        self.Kind = params.get("Kind")
+        self.Province = params.get("Province")
+        self.City = params.get("City")
+        self.CurrencyCode = params.get("CurrencyCode")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class SingleInvoiceInfo(AbstractModel):
     """混贴票据中单张发票的内容
 
     """
 
     def __init__(self):
         r"""
@@ -7103,14 +8394,188 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class SingleInvoiceItem(AbstractModel):
+    """混贴票据中单张发票的内容
+
+    """
+
+    def __init__(self):
+        r"""
+        :param VatSpecialInvoice: 增值税专用发票
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VatSpecialInvoice: :class:`tencentcloud.ocr.v20181119.models.VatInvoiceInfo`
+        :param VatCommonInvoice: 增值税普通发票
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VatCommonInvoice: :class:`tencentcloud.ocr.v20181119.models.VatInvoiceInfo`
+        :param VatElectronicCommonInvoice: 增值税电子普通发票
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VatElectronicCommonInvoice: :class:`tencentcloud.ocr.v20181119.models.VatInvoiceInfo`
+        :param VatElectronicSpecialInvoice: 增值税电子专用发票
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VatElectronicSpecialInvoice: :class:`tencentcloud.ocr.v20181119.models.VatInvoiceInfo`
+        :param VatElectronicInvoiceBlockchain: 区块链电子发票
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VatElectronicInvoiceBlockchain: :class:`tencentcloud.ocr.v20181119.models.VatInvoiceInfo`
+        :param VatElectronicInvoiceToll: 增值税电子普通发票(通行费)
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VatElectronicInvoiceToll: :class:`tencentcloud.ocr.v20181119.models.VatInvoiceInfo`
+        :param VatElectronicSpecialInvoiceFull: 电子发票(专用发票)
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VatElectronicSpecialInvoiceFull: :class:`tencentcloud.ocr.v20181119.models.VatElectronicInfo`
+        :param VatElectronicInvoiceFull: 电子发票(普通发票)
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VatElectronicInvoiceFull: :class:`tencentcloud.ocr.v20181119.models.VatElectronicInfo`
+        :param MachinePrintedInvoice: 通用机打发票
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MachinePrintedInvoice: :class:`tencentcloud.ocr.v20181119.models.MachinePrintedInvoice`
+        :param BusInvoice: 汽车票
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BusInvoice: :class:`tencentcloud.ocr.v20181119.models.BusInvoice`
+        :param ShippingInvoice: 轮船票
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ShippingInvoice: :class:`tencentcloud.ocr.v20181119.models.ShippingInvoice`
+        :param TollInvoice: 过路过桥费发票
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TollInvoice: :class:`tencentcloud.ocr.v20181119.models.TollInvoice`
+        :param OtherInvoice: 其他发票
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OtherInvoice: :class:`tencentcloud.ocr.v20181119.models.OtherInvoice`
+        :param MotorVehicleSaleInvoice: 机动车销售统一发票
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MotorVehicleSaleInvoice: :class:`tencentcloud.ocr.v20181119.models.MotorVehicleSaleInvoice`
+        :param UsedCarPurchaseInvoice: 二手车销售统一发票
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UsedCarPurchaseInvoice: :class:`tencentcloud.ocr.v20181119.models.UsedCarPurchaseInvoice`
+        :param VatInvoiceRoll: 增值税普通发票(卷票)
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VatInvoiceRoll: :class:`tencentcloud.ocr.v20181119.models.VatInvoiceRoll`
+        :param TaxiTicket: 出租车发票
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaxiTicket: :class:`tencentcloud.ocr.v20181119.models.TaxiTicket`
+        :param QuotaInvoice: 定额发票
+注意：此字段可能返回 null，表示取不到有效值。
+        :type QuotaInvoice: :class:`tencentcloud.ocr.v20181119.models.QuotaInvoice`
+        :param AirTransport: 机票行程单
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AirTransport: :class:`tencentcloud.ocr.v20181119.models.AirTransport`
+        :param NonTaxIncomeGeneralBill: 非税收入通用票据
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NonTaxIncomeGeneralBill: :class:`tencentcloud.ocr.v20181119.models.NonTaxIncomeBill`
+        :param NonTaxIncomeElectronicBill: 非税收入一般缴款书(电子)
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NonTaxIncomeElectronicBill: :class:`tencentcloud.ocr.v20181119.models.NonTaxIncomeBill`
+        :param TrainTicket: 火车票
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TrainTicket: :class:`tencentcloud.ocr.v20181119.models.TrainTicket`
+        """
+        self.VatSpecialInvoice = None
+        self.VatCommonInvoice = None
+        self.VatElectronicCommonInvoice = None
+        self.VatElectronicSpecialInvoice = None
+        self.VatElectronicInvoiceBlockchain = None
+        self.VatElectronicInvoiceToll = None
+        self.VatElectronicSpecialInvoiceFull = None
+        self.VatElectronicInvoiceFull = None
+        self.MachinePrintedInvoice = None
+        self.BusInvoice = None
+        self.ShippingInvoice = None
+        self.TollInvoice = None
+        self.OtherInvoice = None
+        self.MotorVehicleSaleInvoice = None
+        self.UsedCarPurchaseInvoice = None
+        self.VatInvoiceRoll = None
+        self.TaxiTicket = None
+        self.QuotaInvoice = None
+        self.AirTransport = None
+        self.NonTaxIncomeGeneralBill = None
+        self.NonTaxIncomeElectronicBill = None
+        self.TrainTicket = None
+
+
+    def _deserialize(self, params):
+        if params.get("VatSpecialInvoice") is not None:
+            self.VatSpecialInvoice = VatInvoiceInfo()
+            self.VatSpecialInvoice._deserialize(params.get("VatSpecialInvoice"))
+        if params.get("VatCommonInvoice") is not None:
+            self.VatCommonInvoice = VatInvoiceInfo()
+            self.VatCommonInvoice._deserialize(params.get("VatCommonInvoice"))
+        if params.get("VatElectronicCommonInvoice") is not None:
+            self.VatElectronicCommonInvoice = VatInvoiceInfo()
+            self.VatElectronicCommonInvoice._deserialize(params.get("VatElectronicCommonInvoice"))
+        if params.get("VatElectronicSpecialInvoice") is not None:
+            self.VatElectronicSpecialInvoice = VatInvoiceInfo()
+            self.VatElectronicSpecialInvoice._deserialize(params.get("VatElectronicSpecialInvoice"))
+        if params.get("VatElectronicInvoiceBlockchain") is not None:
+            self.VatElectronicInvoiceBlockchain = VatInvoiceInfo()
+            self.VatElectronicInvoiceBlockchain._deserialize(params.get("VatElectronicInvoiceBlockchain"))
+        if params.get("VatElectronicInvoiceToll") is not None:
+            self.VatElectronicInvoiceToll = VatInvoiceInfo()
+            self.VatElectronicInvoiceToll._deserialize(params.get("VatElectronicInvoiceToll"))
+        if params.get("VatElectronicSpecialInvoiceFull") is not None:
+            self.VatElectronicSpecialInvoiceFull = VatElectronicInfo()
+            self.VatElectronicSpecialInvoiceFull._deserialize(params.get("VatElectronicSpecialInvoiceFull"))
+        if params.get("VatElectronicInvoiceFull") is not None:
+            self.VatElectronicInvoiceFull = VatElectronicInfo()
+            self.VatElectronicInvoiceFull._deserialize(params.get("VatElectronicInvoiceFull"))
+        if params.get("MachinePrintedInvoice") is not None:
+            self.MachinePrintedInvoice = MachinePrintedInvoice()
+            self.MachinePrintedInvoice._deserialize(params.get("MachinePrintedInvoice"))
+        if params.get("BusInvoice") is not None:
+            self.BusInvoice = BusInvoice()
+            self.BusInvoice._deserialize(params.get("BusInvoice"))
+        if params.get("ShippingInvoice") is not None:
+            self.ShippingInvoice = ShippingInvoice()
+            self.ShippingInvoice._deserialize(params.get("ShippingInvoice"))
+        if params.get("TollInvoice") is not None:
+            self.TollInvoice = TollInvoice()
+            self.TollInvoice._deserialize(params.get("TollInvoice"))
+        if params.get("OtherInvoice") is not None:
+            self.OtherInvoice = OtherInvoice()
+            self.OtherInvoice._deserialize(params.get("OtherInvoice"))
+        if params.get("MotorVehicleSaleInvoice") is not None:
+            self.MotorVehicleSaleInvoice = MotorVehicleSaleInvoice()
+            self.MotorVehicleSaleInvoice._deserialize(params.get("MotorVehicleSaleInvoice"))
+        if params.get("UsedCarPurchaseInvoice") is not None:
+            self.UsedCarPurchaseInvoice = UsedCarPurchaseInvoice()
+            self.UsedCarPurchaseInvoice._deserialize(params.get("UsedCarPurchaseInvoice"))
+        if params.get("VatInvoiceRoll") is not None:
+            self.VatInvoiceRoll = VatInvoiceRoll()
+            self.VatInvoiceRoll._deserialize(params.get("VatInvoiceRoll"))
+        if params.get("TaxiTicket") is not None:
+            self.TaxiTicket = TaxiTicket()
+            self.TaxiTicket._deserialize(params.get("TaxiTicket"))
+        if params.get("QuotaInvoice") is not None:
+            self.QuotaInvoice = QuotaInvoice()
+            self.QuotaInvoice._deserialize(params.get("QuotaInvoice"))
+        if params.get("AirTransport") is not None:
+            self.AirTransport = AirTransport()
+            self.AirTransport._deserialize(params.get("AirTransport"))
+        if params.get("NonTaxIncomeGeneralBill") is not None:
+            self.NonTaxIncomeGeneralBill = NonTaxIncomeBill()
+            self.NonTaxIncomeGeneralBill._deserialize(params.get("NonTaxIncomeGeneralBill"))
+        if params.get("NonTaxIncomeElectronicBill") is not None:
+            self.NonTaxIncomeElectronicBill = NonTaxIncomeBill()
+            self.NonTaxIncomeElectronicBill._deserialize(params.get("NonTaxIncomeElectronicBill"))
+        if params.get("TrainTicket") is not None:
+            self.TrainTicket = TrainTicket()
+            self.TrainTicket._deserialize(params.get("TrainTicket"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class SmartFormFileUrl(AbstractModel):
     """智慧表单上传文件信息
 
     """
 
     def __init__(self):
         r"""
@@ -7784,14 +9249,106 @@
         self.PlateNumber = params.get("PlateNumber")
         self.InvoiceType = params.get("InvoiceType")
         self.Province = params.get("Province")
         self.City = params.get("City")
         self.RequestId = params.get("RequestId")
 
 
+class TaxiTicket(AbstractModel):
+    """出租车发票
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Title: 发票名称
+        :type Title: str
+        :param QRCodeMark: 是否存在二维码（1：有，0：无）
+        :type QRCodeMark: int
+        :param Code: 发票代码
+        :type Code: str
+        :param Number: 发票号码
+        :type Number: str
+        :param Date: 开票日期
+        :type Date: str
+        :param TimeGetOn: 上车时间
+        :type TimeGetOn: str
+        :param TimeGetOff: 下车时间
+        :type TimeGetOff: str
+        :param Price: 单价
+        :type Price: str
+        :param Mileage: 里程
+        :type Mileage: str
+        :param Total: 总金额
+        :type Total: str
+        :param Place: 发票所在地
+        :type Place: str
+        :param Province: 省
+        :type Province: str
+        :param City: 市
+        :type City: str
+        :param Kind: 发票消费类型
+        :type Kind: str
+        :param LicensePlate: 车牌号
+        :type LicensePlate: str
+        :param FuelFee: 燃油附加费
+        :type FuelFee: str
+        :param BookingCallFee: 预约叫车服务费
+        :type BookingCallFee: str
+        :param CompanySealMark: 是否有公司印章（0：没有，1：有）
+        :type CompanySealMark: int
+        """
+        self.Title = None
+        self.QRCodeMark = None
+        self.Code = None
+        self.Number = None
+        self.Date = None
+        self.TimeGetOn = None
+        self.TimeGetOff = None
+        self.Price = None
+        self.Mileage = None
+        self.Total = None
+        self.Place = None
+        self.Province = None
+        self.City = None
+        self.Kind = None
+        self.LicensePlate = None
+        self.FuelFee = None
+        self.BookingCallFee = None
+        self.CompanySealMark = None
+
+
+    def _deserialize(self, params):
+        self.Title = params.get("Title")
+        self.QRCodeMark = params.get("QRCodeMark")
+        self.Code = params.get("Code")
+        self.Number = params.get("Number")
+        self.Date = params.get("Date")
+        self.TimeGetOn = params.get("TimeGetOn")
+        self.TimeGetOff = params.get("TimeGetOff")
+        self.Price = params.get("Price")
+        self.Mileage = params.get("Mileage")
+        self.Total = params.get("Total")
+        self.Place = params.get("Place")
+        self.Province = params.get("Province")
+        self.City = params.get("City")
+        self.Kind = params.get("Kind")
+        self.LicensePlate = params.get("LicensePlate")
+        self.FuelFee = params.get("FuelFee")
+        self.BookingCallFee = params.get("BookingCallFee")
+        self.CompanySealMark = params.get("CompanySealMark")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class TextArithmetic(AbstractModel):
     """算式识别结果
 
     """
 
     def __init__(self):
         r"""
@@ -8496,14 +10053,78 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class TollInvoice(AbstractModel):
+    """过路过桥费发票
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Title: 发票名称
+        :type Title: str
+        :param Code: 发票代码
+        :type Code: str
+        :param Number: 发票号码
+        :type Number: str
+        :param Total: 价税合计（小写）
+        :type Total: str
+        :param Kind: 发票消费类型
+        :type Kind: str
+        :param Date: 日期
+        :type Date: str
+        :param Time: 时间
+        :type Time: str
+        :param Entrance: 入口
+        :type Entrance: str
+        :param Exit: 出口
+        :type Exit: str
+        :param HighwayMark: 高速标志（0：没有，1：有）
+        :type HighwayMark: int
+        :param QRCodeMark: 是否存在二维码（1：有，0：无）
+        :type QRCodeMark: int
+        """
+        self.Title = None
+        self.Code = None
+        self.Number = None
+        self.Total = None
+        self.Kind = None
+        self.Date = None
+        self.Time = None
+        self.Entrance = None
+        self.Exit = None
+        self.HighwayMark = None
+        self.QRCodeMark = None
+
+
+    def _deserialize(self, params):
+        self.Title = params.get("Title")
+        self.Code = params.get("Code")
+        self.Number = params.get("Number")
+        self.Total = params.get("Total")
+        self.Kind = params.get("Kind")
+        self.Date = params.get("Date")
+        self.Time = params.get("Time")
+        self.Entrance = params.get("Entrance")
+        self.Exit = params.get("Exit")
+        self.HighwayMark = params.get("HighwayMark")
+        self.QRCodeMark = params.get("QRCodeMark")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class TollInvoiceInfo(AbstractModel):
     """过路过桥费字段信息
 
     """
 
     def __init__(self):
         r"""
@@ -8604,14 +10225,130 @@
                 obj = TollInvoiceInfo()
                 obj._deserialize(item)
                 self.TollInvoiceInfos.append(obj)
         self.Angle = params.get("Angle")
         self.RequestId = params.get("RequestId")
 
 
+class TrainTicket(AbstractModel):
+    """火车票
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Title: 发票名称
+        :type Title: str
+        :param Number: 发票号码
+        :type Number: str
+        :param DateGetOn: 乘车日期
+        :type DateGetOn: str
+        :param TimeGetOn: 乘车时间
+        :type TimeGetOn: str
+        :param Name: 乘车人姓名
+        :type Name: str
+        :param StationGetOn: 出发车站
+        :type StationGetOn: str
+        :param StationGetOff: 到达车站
+        :type StationGetOff: str
+        :param Seat: 座位类型
+        :type Seat: str
+        :param Total: 总金额
+        :type Total: str
+        :param Kind: 发票消费类型
+        :type Kind: str
+        :param SerialNumber: 序列号
+        :type SerialNumber: str
+        :param UserID: 身份证号
+        :type UserID: str
+        :param GateNumber: 检票口
+        :type GateNumber: str
+        :param TrainNumber: 车次
+        :type TrainNumber: str
+        :param HandlingFee: 手续费
+        :type HandlingFee: str
+        :param OriginalFare: 原票价
+        :type OriginalFare: str
+        :param TotalCn: 大写金额
+        :type TotalCn: str
+        :param SeatNumber: 座位号
+        :type SeatNumber: str
+        :param PickUpAddress: 取票地址
+        :type PickUpAddress: str
+        :param TicketChange: 是否始发改签
+        :type TicketChange: str
+        :param AdditionalFare: 加收票价
+        :type AdditionalFare: str
+        :param ReceiptNumber: 收据号码
+        :type ReceiptNumber: str
+        :param QRCodeMark: 是否存在二维码（1：有，0：无）
+        :type QRCodeMark: int
+        :param ReimburseOnlyMark: 是否仅供报销使用（0：没有，1：有）
+        :type ReimburseOnlyMark: int
+        """
+        self.Title = None
+        self.Number = None
+        self.DateGetOn = None
+        self.TimeGetOn = None
+        self.Name = None
+        self.StationGetOn = None
+        self.StationGetOff = None
+        self.Seat = None
+        self.Total = None
+        self.Kind = None
+        self.SerialNumber = None
+        self.UserID = None
+        self.GateNumber = None
+        self.TrainNumber = None
+        self.HandlingFee = None
+        self.OriginalFare = None
+        self.TotalCn = None
+        self.SeatNumber = None
+        self.PickUpAddress = None
+        self.TicketChange = None
+        self.AdditionalFare = None
+        self.ReceiptNumber = None
+        self.QRCodeMark = None
+        self.ReimburseOnlyMark = None
+
+
+    def _deserialize(self, params):
+        self.Title = params.get("Title")
+        self.Number = params.get("Number")
+        self.DateGetOn = params.get("DateGetOn")
+        self.TimeGetOn = params.get("TimeGetOn")
+        self.Name = params.get("Name")
+        self.StationGetOn = params.get("StationGetOn")
+        self.StationGetOff = params.get("StationGetOff")
+        self.Seat = params.get("Seat")
+        self.Total = params.get("Total")
+        self.Kind = params.get("Kind")
+        self.SerialNumber = params.get("SerialNumber")
+        self.UserID = params.get("UserID")
+        self.GateNumber = params.get("GateNumber")
+        self.TrainNumber = params.get("TrainNumber")
+        self.HandlingFee = params.get("HandlingFee")
+        self.OriginalFare = params.get("OriginalFare")
+        self.TotalCn = params.get("TotalCn")
+        self.SeatNumber = params.get("SeatNumber")
+        self.PickUpAddress = params.get("PickUpAddress")
+        self.TicketChange = params.get("TicketChange")
+        self.AdditionalFare = params.get("AdditionalFare")
+        self.ReceiptNumber = params.get("ReceiptNumber")
+        self.QRCodeMark = params.get("QRCodeMark")
+        self.ReimburseOnlyMark = params.get("ReimburseOnlyMark")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class TrainTicketOCRRequest(AbstractModel):
     """TrainTicketOCR请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -8744,14 +10481,166 @@
         self.OriginalPrice = params.get("OriginalPrice")
         self.InvoiceStyle = params.get("InvoiceStyle")
         self.ReceiptNumber = params.get("ReceiptNumber")
         self.IsReceipt = params.get("IsReceipt")
         self.RequestId = params.get("RequestId")
 
 
+class UsedCarPurchaseInvoice(AbstractModel):
+    """二手车销售统一发票
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Title: 发票名称
+        :type Title: str
+        :param QRCodeMark: 是否存在二维码（0：没有，1：有）
+        :type QRCodeMark: int
+        :param Code: 发票代码
+        :type Code: str
+        :param Number: 发票号码
+        :type Number: str
+        :param Date: 开票日期
+        :type Date: str
+        :param Total: 价税合计（小写）
+        :type Total: str
+        :param TotalCn: 价税合计（大写）
+        :type TotalCn: str
+        :param Seller: 销货单位名称
+        :type Seller: str
+        :param SellerTel: 销售方电话
+        :type SellerTel: str
+        :param SellerTaxID: 销售方单位代码/个人身份证号
+        :type SellerTaxID: str
+        :param SellerAddress: 销售方地址
+        :type SellerAddress: str
+        :param Buyer: 购买方名称
+        :type Buyer: str
+        :param BuyerID: 购买方单位代码/个人身份证号
+        :type BuyerID: str
+        :param BuyerAddress: 购买方地址
+        :type BuyerAddress: str
+        :param BuyerTel: 购买方电话
+        :type BuyerTel: str
+        :param CompanyName: 二手车市场
+        :type CompanyName: str
+        :param CompanyTaxID: 二手车市场纳税人识别号
+        :type CompanyTaxID: str
+        :param CompanyBankAccount: 二手车市场开户银行和账号
+        :type CompanyBankAccount: str
+        :param CompanyTel: 二手车市场电话
+        :type CompanyTel: str
+        :param CompanyAddress: 二手车市场地址
+        :type CompanyAddress: str
+        :param TransferAdministrationName: 转入地车辆管理所名称
+        :type TransferAdministrationName: str
+        :param LicensePlate: 车牌号
+        :type LicensePlate: str
+        :param RegistrationNumber: 登记证号
+        :type RegistrationNumber: str
+        :param VIN: 车辆识别代码
+        :type VIN: str
+        :param VehicleModel: 厂牌型号
+        :type VehicleModel: str
+        :param Kind: 发票消费类型
+        :type Kind: str
+        :param Province: 省
+        :type Province: str
+        :param City: 市
+        :type City: str
+        :param VehicleType: 车辆类型
+        :type VehicleType: str
+        :param Remark: 备注
+        :type Remark: str
+        :param FormType: 发票联次
+        :type FormType: str
+        :param FormName: 发票联名
+        :type FormName: str
+        :param CompanySealMark: 是否有公司印章（0：没有，1：有）
+        :type CompanySealMark: int
+        """
+        self.Title = None
+        self.QRCodeMark = None
+        self.Code = None
+        self.Number = None
+        self.Date = None
+        self.Total = None
+        self.TotalCn = None
+        self.Seller = None
+        self.SellerTel = None
+        self.SellerTaxID = None
+        self.SellerAddress = None
+        self.Buyer = None
+        self.BuyerID = None
+        self.BuyerAddress = None
+        self.BuyerTel = None
+        self.CompanyName = None
+        self.CompanyTaxID = None
+        self.CompanyBankAccount = None
+        self.CompanyTel = None
+        self.CompanyAddress = None
+        self.TransferAdministrationName = None
+        self.LicensePlate = None
+        self.RegistrationNumber = None
+        self.VIN = None
+        self.VehicleModel = None
+        self.Kind = None
+        self.Province = None
+        self.City = None
+        self.VehicleType = None
+        self.Remark = None
+        self.FormType = None
+        self.FormName = None
+        self.CompanySealMark = None
+
+
+    def _deserialize(self, params):
+        self.Title = params.get("Title")
+        self.QRCodeMark = params.get("QRCodeMark")
+        self.Code = params.get("Code")
+        self.Number = params.get("Number")
+        self.Date = params.get("Date")
+        self.Total = params.get("Total")
+        self.TotalCn = params.get("TotalCn")
+        self.Seller = params.get("Seller")
+        self.SellerTel = params.get("SellerTel")
+        self.SellerTaxID = params.get("SellerTaxID")
+        self.SellerAddress = params.get("SellerAddress")
+        self.Buyer = params.get("Buyer")
+        self.BuyerID = params.get("BuyerID")
+        self.BuyerAddress = params.get("BuyerAddress")
+        self.BuyerTel = params.get("BuyerTel")
+        self.CompanyName = params.get("CompanyName")
+        self.CompanyTaxID = params.get("CompanyTaxID")
+        self.CompanyBankAccount = params.get("CompanyBankAccount")
+        self.CompanyTel = params.get("CompanyTel")
+        self.CompanyAddress = params.get("CompanyAddress")
+        self.TransferAdministrationName = params.get("TransferAdministrationName")
+        self.LicensePlate = params.get("LicensePlate")
+        self.RegistrationNumber = params.get("RegistrationNumber")
+        self.VIN = params.get("VIN")
+        self.VehicleModel = params.get("VehicleModel")
+        self.Kind = params.get("Kind")
+        self.Province = params.get("Province")
+        self.City = params.get("City")
+        self.VehicleType = params.get("VehicleType")
+        self.Remark = params.get("Remark")
+        self.FormType = params.get("FormType")
+        self.FormName = params.get("FormName")
+        self.CompanySealMark = params.get("CompanySealMark")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class UsedVehicleInvoiceInfo(AbstractModel):
     """二手车销售统一发票信息
 
     """
 
     def __init__(self):
         r"""
@@ -8891,14 +10780,191 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class VatElectronicInfo(AbstractModel):
+    """电子发票返回值
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Title: 发票名称
+        :type Title: str
+        :param Number: 发票号码
+        :type Number: str
+        :param Date: 开票日期
+        :type Date: str
+        :param PretaxAmount: 税前金额
+        :type PretaxAmount: str
+        :param Tax: 合计税额
+        :type Tax: str
+        :param Total: 价税合计（小写）
+        :type Total: str
+        :param TotalCn: 价税合计（大写）
+        :type TotalCn: str
+        :param Seller: 销售方名称
+        :type Seller: str
+        :param SellerTaxID: 销售方纳税人识别号
+        :type SellerTaxID: str
+        :param Buyer: 购买方名称
+        :type Buyer: str
+        :param BuyerTaxID: 购买方纳税人识别号
+        :type BuyerTaxID: str
+        :param Issuer: 开票人
+        :type Issuer: str
+        :param Remark: 备注
+        :type Remark: str
+        :param SubTotal: 小计金额
+        :type SubTotal: str
+        :param SubTax: 小计税额
+        :type SubTax: str
+        :param VatElectronicItems: 电子发票详细条目信息
+        :type VatElectronicItems: list of VatElectronicItemInfo
+        """
+        self.Title = None
+        self.Number = None
+        self.Date = None
+        self.PretaxAmount = None
+        self.Tax = None
+        self.Total = None
+        self.TotalCn = None
+        self.Seller = None
+        self.SellerTaxID = None
+        self.Buyer = None
+        self.BuyerTaxID = None
+        self.Issuer = None
+        self.Remark = None
+        self.SubTotal = None
+        self.SubTax = None
+        self.VatElectronicItems = None
+
+
+    def _deserialize(self, params):
+        self.Title = params.get("Title")
+        self.Number = params.get("Number")
+        self.Date = params.get("Date")
+        self.PretaxAmount = params.get("PretaxAmount")
+        self.Tax = params.get("Tax")
+        self.Total = params.get("Total")
+        self.TotalCn = params.get("TotalCn")
+        self.Seller = params.get("Seller")
+        self.SellerTaxID = params.get("SellerTaxID")
+        self.Buyer = params.get("Buyer")
+        self.BuyerTaxID = params.get("BuyerTaxID")
+        self.Issuer = params.get("Issuer")
+        self.Remark = params.get("Remark")
+        self.SubTotal = params.get("SubTotal")
+        self.SubTax = params.get("SubTax")
+        if params.get("VatElectronicItems") is not None:
+            self.VatElectronicItems = []
+            for item in params.get("VatElectronicItems"):
+                obj = VatElectronicItemInfo()
+                obj._deserialize(item)
+                self.VatElectronicItems.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class VatElectronicItemInfo(AbstractModel):
+    """电子发票详细条目信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: 项目名称
+        :type Name: str
+        :param Quantity: 数量
+        :type Quantity: str
+        :param Specification: 规格型号
+        :type Specification: str
+        :param Price: 单价
+        :type Price: str
+        :param Total: 金额
+        :type Total: str
+        :param TaxRate: 税率
+        :type TaxRate: str
+        :param Tax: 税额
+        :type Tax: str
+        :param Unit: 单位
+        :type Unit: str
+        :param VehicleType: 运输工具类型
+        :type VehicleType: str
+        :param VehicleBrand: 运输工具牌号
+        :type VehicleBrand: str
+        :param DeparturePlace: 起始地
+        :type DeparturePlace: str
+        :param ArrivalPlace: 到达地
+        :type ArrivalPlace: str
+        :param TransportItemsName: 运输货物名称，仅货物运输服务发票返回
+        :type TransportItemsName: str
+        :param PlaceOfBuildingService: 建筑服务发生地，仅建筑发票返回
+        :type PlaceOfBuildingService: str
+        :param BuildingName: 建筑项目名称，仅建筑发票返回
+        :type BuildingName: str
+        :param EstateNumber: 产权证书/不动产权证号，仅不动产经营租赁服务发票返回
+        :type EstateNumber: str
+        :param AreaUnit: 面积单位，仅不动产经营租赁服务发票返回
+        :type AreaUnit: str
+        """
+        self.Name = None
+        self.Quantity = None
+        self.Specification = None
+        self.Price = None
+        self.Total = None
+        self.TaxRate = None
+        self.Tax = None
+        self.Unit = None
+        self.VehicleType = None
+        self.VehicleBrand = None
+        self.DeparturePlace = None
+        self.ArrivalPlace = None
+        self.TransportItemsName = None
+        self.PlaceOfBuildingService = None
+        self.BuildingName = None
+        self.EstateNumber = None
+        self.AreaUnit = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        self.Quantity = params.get("Quantity")
+        self.Specification = params.get("Specification")
+        self.Price = params.get("Price")
+        self.Total = params.get("Total")
+        self.TaxRate = params.get("TaxRate")
+        self.Tax = params.get("Tax")
+        self.Unit = params.get("Unit")
+        self.VehicleType = params.get("VehicleType")
+        self.VehicleBrand = params.get("VehicleBrand")
+        self.DeparturePlace = params.get("DeparturePlace")
+        self.ArrivalPlace = params.get("ArrivalPlace")
+        self.TransportItemsName = params.get("TransportItemsName")
+        self.PlaceOfBuildingService = params.get("PlaceOfBuildingService")
+        self.BuildingName = params.get("BuildingName")
+        self.EstateNumber = params.get("EstateNumber")
+        self.AreaUnit = params.get("AreaUnit")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class VatInvoice(AbstractModel):
     """增值税发票信息
 
     """
 
     def __init__(self):
         r"""
@@ -9082,14 +11148,195 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class VatInvoiceInfo(AbstractModel):
+    """增值税发票返回值
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CheckCode: 校验码
+        :type CheckCode: str
+        :param FormType: 发票联次
+        :type FormType: str
+        :param TravelTax: 车船税
+        :type TravelTax: str
+        :param BuyerAddrTel: 购买方地址电话
+        :type BuyerAddrTel: str
+        :param BuyerBankAccount: 购买方银行账号
+        :type BuyerBankAccount: str
+        :param CompanySealContent: 公司印章内容
+        :type CompanySealContent: str
+        :param TaxSealContent: 税务局章内容
+        :type TaxSealContent: str
+        :param ServiceName: 服务类型
+        :type ServiceName: str
+        :param City: 市
+        :type City: str
+        :param QRCodeMark: 是否存在二维码（0：没有，1：有）
+        :type QRCodeMark: int
+        :param AgentMark: 是否有代开标记（0：没有，1：有）
+        :type AgentMark: int
+        :param TransitMark: 是否有通行费标记（0：没有，1：有）
+        :type TransitMark: int
+        :param OilMark: 是否有成品油标记（0：没有，1：有）
+        :type OilMark: int
+        :param Title: 发票名称
+        :type Title: str
+        :param Kind: 发票消费类型
+        :type Kind: str
+        :param Code: 发票代码
+        :type Code: str
+        :param Number: 发票号码
+        :type Number: str
+        :param NumberConfirm: 机打发票号码
+        :type NumberConfirm: str
+        :param Date: 开票日期
+        :type Date: str
+        :param Total: 价税合计（小写）
+        :type Total: str
+        :param TotalCn: 价税合计（大写）
+        :type TotalCn: str
+        :param PretaxAmount: 税前金额
+        :type PretaxAmount: str
+        :param Tax: 合计税额
+        :type Tax: str
+        :param MachineCode: 机器编号
+        :type MachineCode: str
+        :param Ciphertext: 密码区
+        :type Ciphertext: str
+        :param Remark: 备注
+        :type Remark: str
+        :param Seller: 销售方名称
+        :type Seller: str
+        :param SellerTaxID: 销售方纳税人识别号
+        :type SellerTaxID: str
+        :param SellerAddrTel: 销售方地址电话
+        :type SellerAddrTel: str
+        :param SellerBankAccount: 销售方银行账号
+        :type SellerBankAccount: str
+        :param Buyer: 购买方名称
+        :type Buyer: str
+        :param BuyerTaxID: 购买方纳税人识别号
+        :type BuyerTaxID: str
+        :param CompanySealMark: 是否有公司印章（0：没有，1：有）
+        :type CompanySealMark: int
+        :param Issuer: 开票人
+        :type Issuer: str
+        :param Reviewer: 复核人
+        :type Reviewer: str
+        :param Province: 省
+        :type Province: str
+        :param VatInvoiceItemInfos: 增值税发票项目信息
+        :type VatInvoiceItemInfos: list of VatInvoiceItemInfo
+        :param CodeConfirm: 机打发票代码
+        :type CodeConfirm: str
+        :param Receiptor: 收款人
+        :type Receiptor: str
+        """
+        self.CheckCode = None
+        self.FormType = None
+        self.TravelTax = None
+        self.BuyerAddrTel = None
+        self.BuyerBankAccount = None
+        self.CompanySealContent = None
+        self.TaxSealContent = None
+        self.ServiceName = None
+        self.City = None
+        self.QRCodeMark = None
+        self.AgentMark = None
+        self.TransitMark = None
+        self.OilMark = None
+        self.Title = None
+        self.Kind = None
+        self.Code = None
+        self.Number = None
+        self.NumberConfirm = None
+        self.Date = None
+        self.Total = None
+        self.TotalCn = None
+        self.PretaxAmount = None
+        self.Tax = None
+        self.MachineCode = None
+        self.Ciphertext = None
+        self.Remark = None
+        self.Seller = None
+        self.SellerTaxID = None
+        self.SellerAddrTel = None
+        self.SellerBankAccount = None
+        self.Buyer = None
+        self.BuyerTaxID = None
+        self.CompanySealMark = None
+        self.Issuer = None
+        self.Reviewer = None
+        self.Province = None
+        self.VatInvoiceItemInfos = None
+        self.CodeConfirm = None
+        self.Receiptor = None
+
+
+    def _deserialize(self, params):
+        self.CheckCode = params.get("CheckCode")
+        self.FormType = params.get("FormType")
+        self.TravelTax = params.get("TravelTax")
+        self.BuyerAddrTel = params.get("BuyerAddrTel")
+        self.BuyerBankAccount = params.get("BuyerBankAccount")
+        self.CompanySealContent = params.get("CompanySealContent")
+        self.TaxSealContent = params.get("TaxSealContent")
+        self.ServiceName = params.get("ServiceName")
+        self.City = params.get("City")
+        self.QRCodeMark = params.get("QRCodeMark")
+        self.AgentMark = params.get("AgentMark")
+        self.TransitMark = params.get("TransitMark")
+        self.OilMark = params.get("OilMark")
+        self.Title = params.get("Title")
+        self.Kind = params.get("Kind")
+        self.Code = params.get("Code")
+        self.Number = params.get("Number")
+        self.NumberConfirm = params.get("NumberConfirm")
+        self.Date = params.get("Date")
+        self.Total = params.get("Total")
+        self.TotalCn = params.get("TotalCn")
+        self.PretaxAmount = params.get("PretaxAmount")
+        self.Tax = params.get("Tax")
+        self.MachineCode = params.get("MachineCode")
+        self.Ciphertext = params.get("Ciphertext")
+        self.Remark = params.get("Remark")
+        self.Seller = params.get("Seller")
+        self.SellerTaxID = params.get("SellerTaxID")
+        self.SellerAddrTel = params.get("SellerAddrTel")
+        self.SellerBankAccount = params.get("SellerBankAccount")
+        self.Buyer = params.get("Buyer")
+        self.BuyerTaxID = params.get("BuyerTaxID")
+        self.CompanySealMark = params.get("CompanySealMark")
+        self.Issuer = params.get("Issuer")
+        self.Reviewer = params.get("Reviewer")
+        self.Province = params.get("Province")
+        if params.get("VatInvoiceItemInfos") is not None:
+            self.VatInvoiceItemInfos = []
+            for item in params.get("VatInvoiceItemInfos"):
+                obj = VatInvoiceItemInfo()
+                obj._deserialize(item)
+                self.VatInvoiceItemInfos.append(obj)
+        self.CodeConfirm = params.get("CodeConfirm")
+        self.Receiptor = params.get("Receiptor")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class VatInvoiceItem(AbstractModel):
     """增值税发票项目明细
 
     """
 
     def __init__(self):
         r"""
@@ -9142,14 +11389,82 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class VatInvoiceItemInfo(AbstractModel):
+    """增值税发票项目信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: 项目名称
+        :type Name: str
+        :param Specification: 规格型号
+        :type Specification: str
+        :param Unit: 单位
+        :type Unit: str
+        :param Quantity: 数量
+        :type Quantity: str
+        :param Price: 单价
+        :type Price: str
+        :param Total: 金额
+        :type Total: str
+        :param TaxRate: 税率
+        :type TaxRate: str
+        :param Tax: 税额
+        :type Tax: str
+        :param DateStart: 通行日期起
+        :type DateStart: str
+        :param DateEnd: 通行日期止
+        :type DateEnd: str
+        :param LicensePlate: 车牌号
+        :type LicensePlate: str
+        :param VehicleType: 车辆类型
+        :type VehicleType: str
+        """
+        self.Name = None
+        self.Specification = None
+        self.Unit = None
+        self.Quantity = None
+        self.Price = None
+        self.Total = None
+        self.TaxRate = None
+        self.Tax = None
+        self.DateStart = None
+        self.DateEnd = None
+        self.LicensePlate = None
+        self.VehicleType = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        self.Specification = params.get("Specification")
+        self.Unit = params.get("Unit")
+        self.Quantity = params.get("Quantity")
+        self.Price = params.get("Price")
+        self.Total = params.get("Total")
+        self.TaxRate = params.get("TaxRate")
+        self.Tax = params.get("Tax")
+        self.DateStart = params.get("DateStart")
+        self.DateEnd = params.get("DateEnd")
+        self.LicensePlate = params.get("LicensePlate")
+        self.VehicleType = params.get("VehicleType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class VatInvoiceOCRRequest(AbstractModel):
     """VatInvoiceOCR请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -9228,14 +11543,127 @@
                 obj._deserialize(item)
                 self.Items.append(obj)
         self.PdfPageSize = params.get("PdfPageSize")
         self.Angle = params.get("Angle")
         self.RequestId = params.get("RequestId")
 
 
+class VatInvoiceRoll(AbstractModel):
+    """增值税普通发票(卷票)
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Title: 发票名称
+        :type Title: str
+        :param Code: 发票代码
+        :type Code: str
+        :param Number: 发票号码
+        :type Number: str
+        :param NumberConfirm: 机打发票号码
+        :type NumberConfirm: str
+        :param Date: 开票日期
+        :type Date: str
+        :param CheckCode: 校验码
+        :type CheckCode: str
+        :param Seller: 销售方名称
+        :type Seller: str
+        :param SellerTaxID: 销售方纳税人识别号
+        :type SellerTaxID: str
+        :param Buyer: 购买方名称
+        :type Buyer: str
+        :param BuyerTaxID: 购买方纳税人识别号
+        :type BuyerTaxID: str
+        :param Category: 种类
+        :type Category: str
+        :param Total: 价税合计（小写）
+        :type Total: str
+        :param TotalCn: 价税合计（大写）
+        :type TotalCn: str
+        :param Kind: 发票消费类型
+        :type Kind: str
+        :param Province: 省
+        :type Province: str
+        :param City: 市
+        :type City: str
+        :param CompanySealMark: 是否有公司印章（0：没有，1：有）
+        :type CompanySealMark: int
+        :param QRCodeMark: 是否存在二维码（1：有，0：无）
+        :type QRCodeMark: int
+        :param ServiceName: 服务类型
+        :type ServiceName: str
+        :param CompanySealContent: 公司印章内容
+        :type CompanySealContent: str
+        :param TaxSealContent: 税务局章内容
+        :type TaxSealContent: str
+        :param VatRollItems: 条目
+        :type VatRollItems: list of VatRollItem
+        """
+        self.Title = None
+        self.Code = None
+        self.Number = None
+        self.NumberConfirm = None
+        self.Date = None
+        self.CheckCode = None
+        self.Seller = None
+        self.SellerTaxID = None
+        self.Buyer = None
+        self.BuyerTaxID = None
+        self.Category = None
+        self.Total = None
+        self.TotalCn = None
+        self.Kind = None
+        self.Province = None
+        self.City = None
+        self.CompanySealMark = None
+        self.QRCodeMark = None
+        self.ServiceName = None
+        self.CompanySealContent = None
+        self.TaxSealContent = None
+        self.VatRollItems = None
+
+
+    def _deserialize(self, params):
+        self.Title = params.get("Title")
+        self.Code = params.get("Code")
+        self.Number = params.get("Number")
+        self.NumberConfirm = params.get("NumberConfirm")
+        self.Date = params.get("Date")
+        self.CheckCode = params.get("CheckCode")
+        self.Seller = params.get("Seller")
+        self.SellerTaxID = params.get("SellerTaxID")
+        self.Buyer = params.get("Buyer")
+        self.BuyerTaxID = params.get("BuyerTaxID")
+        self.Category = params.get("Category")
+        self.Total = params.get("Total")
+        self.TotalCn = params.get("TotalCn")
+        self.Kind = params.get("Kind")
+        self.Province = params.get("Province")
+        self.City = params.get("City")
+        self.CompanySealMark = params.get("CompanySealMark")
+        self.QRCodeMark = params.get("QRCodeMark")
+        self.ServiceName = params.get("ServiceName")
+        self.CompanySealContent = params.get("CompanySealContent")
+        self.TaxSealContent = params.get("TaxSealContent")
+        if params.get("VatRollItems") is not None:
+            self.VatRollItems = []
+            for item in params.get("VatRollItems"):
+                obj = VatRollItem()
+                obj._deserialize(item)
+                self.VatRollItems.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class VatInvoiceUserInfo(AbstractModel):
     """发票人员信息
 
     """
 
     def __init__(self):
         r"""
@@ -9557,14 +11985,50 @@
                 obj = VatRollInvoiceInfo()
                 obj._deserialize(item)
                 self.VatRollInvoiceInfos.append(obj)
         self.Angle = params.get("Angle")
         self.RequestId = params.get("RequestId")
 
 
+class VatRollItem(AbstractModel):
+    """增值税普通发票（卷票）条目
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: 项目名称
+        :type Name: str
+        :param Quantity: 数量
+        :type Quantity: str
+        :param Price: 单价
+        :type Price: str
+        :param Total: 金额
+        :type Total: str
+        """
+        self.Name = None
+        self.Quantity = None
+        self.Price = None
+        self.Total = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        self.Quantity = params.get("Quantity")
+        self.Price = params.get("Price")
+        self.Total = params.get("Total")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class VehicleInvoiceInfo(AbstractModel):
     """机动车销售统一发票信息
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.886/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.885/setup.py` & `tencentcloud-sdk-python-ocr-3.0.886/setup.py`

 * *Files identical despite different names*

