# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.885.tar", last modified: Mon May  1 00:59:12 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.886.tar", last modified: Mon May  8 04:21:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.885.tar` & `tencentcloud-sdk-python-vpc-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/vpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   328818 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)    40497 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   839190 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/vpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:59:12.000000 tencentcloud-sdk-python-vpc-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:21:58.000000 tencentcloud-sdk-python-vpc-3.0.886/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:21:58.000000 tencentcloud-sdk-python-vpc-3.0.886/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 04:21:58.000000 tencentcloud-sdk-python-vpc-3.0.886/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-08 04:21:58.000000 tencentcloud-sdk-python-vpc-3.0.886/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 04:21:58.000000 tencentcloud-sdk-python-vpc-3.0.886/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 04:21:58.000000 tencentcloud-sdk-python-vpc-3.0.886/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-08 04:21:57.000000 tencentcloud-sdk-python-vpc-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:21:58.000000 tencentcloud-sdk-python-vpc-3.0.886/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:21:58.000000 tencentcloud-sdk-python-vpc-3.0.886/tencentcloud/vpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:21:58.000000 tencentcloud-sdk-python-vpc-3.0.886/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   328818 2023-05-08 04:21:57.000000 tencentcloud-sdk-python-vpc-3.0.886/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)    40770 2023-05-08 04:21:57.000000 tencentcloud-sdk-python-vpc-3.0.886/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:21:57.000000 tencentcloud-sdk-python-vpc-3.0.886/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   839190 2023-05-08 04:21:57.000000 tencentcloud-sdk-python-vpc-3.0.886/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:21:57.000000 tencentcloud-sdk-python-vpc-3.0.886/tencentcloud/vpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 04:21:57.000000 tencentcloud-sdk-python-vpc-3.0.886/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 04:21:58.000000 tencentcloud-sdk-python-vpc-3.0.886/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-08 04:21:57.000000 tencentcloud-sdk-python-vpc-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 04:21:58.000000 tencentcloud-sdk-python-vpc-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.885/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.886/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.885/README.rst` & `tencentcloud-sdk-python-vpc-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.886/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.886/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,14 +244,17 @@
 
 # 无效的IPv6地址。
 INVALIDPARAMETERVALUE_INVALIDIPV6 = 'InvalidParameterValue.InvalidIpv6'
 
 # 该Tag不合法。
 INVALIDPARAMETERVALUE_INVALIDTAG = 'InvalidParameterValue.InvalidTag'
 
+# 未查询到该IPv6翻译器。
+INVALIDPARAMETERVALUE_IP6TRANSLATORNOTFOUND = 'InvalidParameterValue.Ip6TranslatorNotFound'
+
 # 负载均衡实例已经绑定了EIP。
 INVALIDPARAMETERVALUE_LBALREADYBINDEIP = 'InvalidParameterValue.LBAlreadyBindEip'
 
 # 参数值超出限制。
 INVALIDPARAMETERVALUE_LIMITEXCEEDED = 'InvalidParameterValue.LimitExceeded'
 
 # 入参格式不合法。
@@ -784,14 +787,17 @@
 
 # SNAT/DNAT转换规则所指定的内网IP已绑定了其他的规则，无法重复绑定。
 UNSUPPORTEDOPERATION_NATGATEWAYRULEPIPEXISTS = 'UnsupportedOperation.NatGatewayRulePipExists'
 
 # SNAT转换规则的内网IP需为虚拟机上网卡所用的IP。
 UNSUPPORTEDOPERATION_NATGATEWAYSNATPIPNEEDVM = 'UnsupportedOperation.NatGatewaySnatPipNeedVm'
 
+# NAT网关的SNAT转换规则不存在。
+UNSUPPORTEDOPERATION_NATGATEWAYSNATRULENOTEXISTS = 'UnsupportedOperation.NatGatewaySnatRuleNotExists'
+
 # NAT网关类型不支持SNAT规则。
 UNSUPPORTEDOPERATION_NATGATEWAYTYPENOTSUPPORTSNAT = 'UnsupportedOperation.NatGatewayTypeNotSupportSNAT'
 
 # NAT实例不支持该操作。
 UNSUPPORTEDOPERATION_NATNOTSUPPORTED = 'UnsupportedOperation.NatNotSupported'
 
 # 指定的子网不支持创建本地网关类型的路由。
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.886/tencentcloud/vpc/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vpc-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.886/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.885/setup.py` & `tencentcloud-sdk-python-vpc-3.0.886/setup.py`

 * *Files identical despite different names*

