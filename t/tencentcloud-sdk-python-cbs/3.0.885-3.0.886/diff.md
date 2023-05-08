# Comparing `tmp/tencentcloud-sdk-python-cbs-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-cbs-3.0.886.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cbs-3.0.885.tar", last modified: Mon May  1 00:30:35 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cbs-3.0.886.tar", last modified: Mon May  8 02:56:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cbs-3.0.885.tar` & `tencentcloud-sdk-python-cbs-3.0.886.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:30:35.000000 tencentcloud-sdk-python-cbs-3.0.885/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:30:35.000000 tencentcloud-sdk-python-cbs-3.0.885/tencentcloud_sdk_python_cbs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:30:35.000000 tencentcloud-sdk-python-cbs-3.0.885/tencentcloud_sdk_python_cbs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-01 00:30:35.000000 tencentcloud-sdk-python-cbs-3.0.885/tencentcloud_sdk_python_cbs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:30:35.000000 tencentcloud-sdk-python-cbs-3.0.885/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:30:35.000000 tencentcloud-sdk-python-cbs-3.0.885/tencentcloud_sdk_python_cbs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-01 00:30:34.000000 tencentcloud-sdk-python-cbs-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:30:35.000000 tencentcloud-sdk-python-cbs-3.0.885/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:30:34.000000 tencentcloud-sdk-python-cbs-3.0.885/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:30:35.000000 tencentcloud-sdk-python-cbs-3.0.885/tencentcloud/cbs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:30:35.000000 tencentcloud-sdk-python-cbs-3.0.885/tencentcloud/cbs/v20170312/
--rw-r--r--   0 root         (0) root         (0)     7755 2023-05-01 00:30:34.000000 tencentcloud-sdk-python-cbs-3.0.885/tencentcloud/cbs/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53378 2023-05-01 00:30:34.000000 tencentcloud-sdk-python-cbs-3.0.885/tencentcloud/cbs/v20170312/cbs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:30:34.000000 tencentcloud-sdk-python-cbs-3.0.885/tencentcloud/cbs/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   158971 2023-05-01 00:30:34.000000 tencentcloud-sdk-python-cbs-3.0.885/tencentcloud/cbs/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:30:34.000000 tencentcloud-sdk-python-cbs-3.0.885/tencentcloud/cbs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:30:35.000000 tencentcloud-sdk-python-cbs-3.0.885/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-01 00:30:34.000000 tencentcloud-sdk-python-cbs-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:30:35.000000 tencentcloud-sdk-python-cbs-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:56:57.000000 tencentcloud-sdk-python-cbs-3.0.886/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:56:57.000000 tencentcloud-sdk-python-cbs-3.0.886/tencentcloud_sdk_python_cbs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 02:56:57.000000 tencentcloud-sdk-python-cbs-3.0.886/tencentcloud_sdk_python_cbs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-08 02:56:57.000000 tencentcloud-sdk-python-cbs-3.0.886/tencentcloud_sdk_python_cbs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 02:56:57.000000 tencentcloud-sdk-python-cbs-3.0.886/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 02:56:57.000000 tencentcloud-sdk-python-cbs-3.0.886/tencentcloud_sdk_python_cbs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-08 02:56:57.000000 tencentcloud-sdk-python-cbs-3.0.886/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:56:57.000000 tencentcloud-sdk-python-cbs-3.0.886/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 02:56:57.000000 tencentcloud-sdk-python-cbs-3.0.886/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:56:57.000000 tencentcloud-sdk-python-cbs-3.0.886/tencentcloud/cbs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:56:57.000000 tencentcloud-sdk-python-cbs-3.0.886/tencentcloud/cbs/v20170312/
+-rw-r--r--   0 root         (0) root         (0)     7755 2023-05-08 02:56:57.000000 tencentcloud-sdk-python-cbs-3.0.886/tencentcloud/cbs/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53378 2023-05-08 02:56:57.000000 tencentcloud-sdk-python-cbs-3.0.886/tencentcloud/cbs/v20170312/cbs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 02:56:57.000000 tencentcloud-sdk-python-cbs-3.0.886/tencentcloud/cbs/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   159212 2023-05-08 02:56:57.000000 tencentcloud-sdk-python-cbs-3.0.886/tencentcloud/cbs/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 02:56:57.000000 tencentcloud-sdk-python-cbs-3.0.886/tencentcloud/cbs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 02:56:57.000000 tencentcloud-sdk-python-cbs-3.0.886/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-08 02:56:57.000000 tencentcloud-sdk-python-cbs-3.0.886/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 02:56:57.000000 tencentcloud-sdk-python-cbs-3.0.886/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.885/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cbs-3.0.886/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cbs
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Cbs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.885/README.rst` & `tencentcloud-sdk-python-cbs-3.0.886/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cbs-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cbs-3.0.886/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cbs-3.0.885/tencentcloud/cbs/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cbs-3.0.886/tencentcloud/cbs/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cbs-3.0.885/tencentcloud/cbs/v20170312/cbs_client.py` & `tencentcloud-sdk-python-cbs-3.0.886/tencentcloud/cbs/v20170312/cbs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cbs-3.0.885/tencentcloud/cbs/v20170312/models.py` & `tencentcloud-sdk-python-cbs-3.0.886/tencentcloud/cbs/v20170312/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1453,15 +1453,15 @@
 class DescribeDisksRequest(AbstractModel):
     """DescribeDisks请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Filters: 过滤条件。参数不支持同时指定`DiskIds`和`Filters`。<br><li>disk-usage - Array of String - 是否必填：否 -（过滤条件）按云盘类型过滤。 (SYSTEM_DISK：表示系统盘 | DATA_DISK：表示数据盘)<br><li>disk-charge-type - Array of String - 是否必填：否 -（过滤条件）按照云硬盘计费模式过滤。 (PREPAID：表示预付费，即包年包月 | POSTPAID_BY_HOUR：表示后付费，即按量计费。)<br><li>portable - Array of String - 是否必填：否 -（过滤条件）按是否为弹性云盘过滤。 (TRUE：表示弹性云盘 | FALSE：表示非弹性云盘。)<br><li>project-id - Array of Integer - 是否必填：否 -（过滤条件）按云硬盘所属项目ID过滤。<br><li>disk-id - Array of String - 是否必填：否 -（过滤条件）按照云硬盘ID过滤。云盘ID形如：`disk-11112222`。<br><li>disk-name - Array of String - 是否必填：否 -（过滤条件）按照云盘名称过滤。<br><li>disk-type - Array of String - 是否必填：否 -（过滤条件）按照云盘介质类型过滤。(CLOUD_BASIC：表示普通云硬盘 | CLOUD_PREMIUM：表示高性能云硬盘。| CLOUD_SSD：表示SSD云硬盘 | CLOUD_HSSD：表示增强型SSD云硬盘。| CLOUD_TSSD：表示极速型云硬盘。)<br><li>disk-state - Array of String - 是否必填：否 -（过滤条件）按照云盘状态过滤。(UNATTACHED：未挂载 | ATTACHING：挂载中 | ATTACHED：已挂载 | DETACHING：解挂中 | EXPANDING：扩容中 | ROLLBACKING：回滚中 | TORECYCLE：待回收。)<br><li>instance-id - Array of String - 是否必填：否 -（过滤条件）按照云盘挂载的云主机实例ID过滤。可根据此参数查询挂载在指定云主机下的云硬盘。<br><li>zone - Array of String - 是否必填：否 -（过滤条件）按照[可用区](/document/product/213/15753#ZoneInfo)过滤。<br><li>instance-ip-address - Array of String - 是否必填：否 -（过滤条件）按云盘所挂载云主机的内网或外网IP过滤。<br><li>instance-name - Array of String - 是否必填：否 -（过滤条件）按云盘所挂载的实例名称过滤。<br><li>tag-key - Array of String - 是否必填：否 -（过滤条件）按照标签键进行过滤。<br><li>tag-value - Array of String - 是否必填：否 -（过滤条件）照标签值进行过滤。<br><li>tag:tag-key - Array of String - 是否必填：否 -（过滤条件）按照标签键值对进行过滤。 tag-key使用具体的标签键进行替换。
+        :param Filters: 过滤条件。参数不支持同时指定`DiskIds`和`Filters`。<br><li>disk-usage - Array of String - 是否必填：否 -（过滤条件）按云盘类型过滤。 (SYSTEM_DISK：表示系统盘 | DATA_DISK：表示数据盘)<br><li>disk-charge-type - Array of String - 是否必填：否 -（过滤条件）按照云硬盘计费模式过滤。 (PREPAID：表示预付费，即包年包月 | POSTPAID_BY_HOUR：表示后付费，即按量计费。)<br><li>portable - Array of String - 是否必填：否 -（过滤条件）按是否为弹性云盘过滤。 (TRUE：表示弹性云盘 | FALSE：表示非弹性云盘。)<br><li>project-id - Array of Integer - 是否必填：否 -（过滤条件）按云硬盘所属项目ID过滤。<br><li>disk-id - Array of String - 是否必填：否 -（过滤条件）按照云硬盘ID过滤。云盘ID形如：`disk-11112222`。<br><li>disk-name - Array of String - 是否必填：否 -（过滤条件）按照云盘名称过滤。<br><li>disk-type - Array of String - 是否必填：否 -（过滤条件）按照云盘介质类型过滤。(CLOUD_BASIC：表示普通云硬盘 | CLOUD_PREMIUM：表示高性能云硬盘。| CLOUD_SSD：表示SSD云硬盘 | CLOUD_HSSD：表示增强型SSD云硬盘。| CLOUD_TSSD：表示极速型云硬盘。)<br><li>disk-state - Array of String - 是否必填：否 -（过滤条件）按照云盘状态过滤。(UNATTACHED：未挂载 | ATTACHING：挂载中 | ATTACHED：已挂载 | DETACHING：解挂中 | EXPANDING：扩容中 | ROLLBACKING：回滚中 | TORECYCLE：待回收。)<br><li>instance-id - Array of String - 是否必填：否 -（过滤条件）按照云盘挂载的云主机实例ID过滤。可根据此参数查询挂载在指定云主机下的云硬盘。<br><li>zone - Array of String - 是否必填：否 -（过滤条件）按照[可用区](/document/product/213/15753#ZoneInfo)过滤。<br><li>instance-ip-address - Array of String - 是否必填：否 -（过滤条件）按云盘所挂载云主机的内网或外网IP过滤。<br><li>instance-name - Array of String - 是否必填：否 -（过滤条件）按云盘所挂载的实例名称过滤。<br><li>tag-key - Array of String - 是否必填：否 -（过滤条件）按照标签键进行过滤。<br><li>tag-value - Array of String - 是否必填：否 -（过滤条件）照标签值进行过滤。<br><li>tag:tag-key - Array of String - 是否必填：否 -（过滤条件）按照标签键值对进行过滤。 tag-key使用具体的标签键进行替换。<br><li>dedicated-cluster-id - Array of String - 是否必填：否 -（过滤条件）按照 CDC 独享集群 ID 进行过滤。<br><li>cluster-group-id - String - 是否必填：否 -（过滤条件）按照 集群群组 ID 进行过滤。
         :type Filters: list of Filter
         :param Limit: 返回数量，默认为20，最大值为100。关于`Limit`的更进一步介绍请参考 API [简介](/document/product/362/15633)中的相关小节。
         :type Limit: int
         :param OrderField: 云盘列表排序的依据字段。取值范围：<br><li>CREATE_TIME：依据云盘的创建时间排序<br><li>DEADLINE：依据云盘的到期时间排序<br>默认按云盘创建时间排序。
         :type OrderField: str
         :param Offset: 偏移量，默认为0。关于`Offset`的更进一步介绍请参考API[简介](/document/product/362/15633)中的相关小节。
         :type Offset: int
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-cbs-3.0.886/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cbs
-Version: 3.0.885
+Version: 3.0.886
 Summary: Tencent Cloud Cbs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.885/setup.py` & `tencentcloud-sdk-python-cbs-3.0.886/setup.py`

 * *Files identical despite different names*

