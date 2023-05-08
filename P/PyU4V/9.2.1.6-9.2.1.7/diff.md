# Comparing `tmp/PyU4V-9.2.1.6.tar.gz` & `tmp/PyU4V-9.2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyU4V-9.2.1.6.tar", last modified: Thu Feb  3 12:17:40 2022, max compression
+gzip compressed data, was "/PyU4V/dist/tmpfgmua9np/PyU4V-9.2.1.7.tar", last modified: Wed Feb  8 11:48:37 2023, max compression
```

## Comparing `PyU4V-9.2.1.6.tar` & `PyU4V-9.2.1.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 stack     (1001) stack     (1001)        0 2022-02-03 12:17:40.293474 PyU4V-9.2.1.6/
--rw-rw-r--   0 stack     (1001) stack     (1001)     9566 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/LICENSE
--rw-rw-r--   0 stack     (1001) stack     (1001)    12003 2022-02-03 12:17:40.293474 PyU4V-9.2.1.6/PKG-INFO
-drwxrwxr-x   0 stack     (1001) stack     (1001)        0 2022-02-03 12:17:40.289474 PyU4V-9.2.1.6/PyU4V/
--rw-rw-r--   0 stack     (1001) stack     (1001)     1127 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/__init__.py
--rw-rw-r--   0 stack     (1001) stack     (1001)    31886 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/common.py
--rw-rw-r--   0 stack     (1001) stack     (1001)    14523 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/metro_dr.py
--rw-rw-r--   0 stack     (1001) stack     (1001)     8683 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/migration.py
--rw-rw-r--   0 stack     (1001) stack     (1001)   116498 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/performance.py
--rw-rw-r--   0 stack     (1001) stack     (1001)   130414 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/provisioning.py
--rw-rw-r--   0 stack     (1001) stack     (1001)    23146 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/real_time.py
--rw-rw-r--   0 stack     (1001) stack     (1001)    71326 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/replication.py
--rw-rw-r--   0 stack     (1001) stack     (1001)    10157 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/rest_requests.py
--rw-rw-r--   0 stack     (1001) stack     (1001)    32811 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/snapshot_policy.py
--rw-rw-r--   0 stack     (1001) stack     (1001)    41778 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/system.py
-drwxrwxr-x   0 stack     (1001) stack     (1001)        0 2022-02-03 12:17:40.289474 PyU4V-9.2.1.6/PyU4V/tools/
--rw-rw-r--   0 stack     (1001) stack     (1001)       20 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/tools/__init__.py
-drwxrwxr-x   0 stack     (1001) stack     (1001)        0 2022-02-03 12:17:40.289474 PyU4V-9.2.1.6/PyU4V/tools/openstack/
--rw-rw-r--   0 stack     (1001) stack     (1001)       19 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/tools/openstack/__init__.py
--rw-rw-r--   0 stack     (1001) stack     (1001)     7265 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/tools/openstack/migrate.py
--rw-rw-r--   0 stack     (1001) stack     (1001)    38251 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/tools/openstack/migrate_utils.py
--rw-rw-r--   0 stack     (1001) stack     (1001)     6757 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/univmax_conn.py
-drwxrwxr-x   0 stack     (1001) stack     (1001)        0 2022-02-03 12:17:40.293474 PyU4V-9.2.1.6/PyU4V/utils/
--rw-rw-r--   0 stack     (1001) stack     (1001)      620 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/utils/__init__.py
--rw-rw-r--   0 stack     (1001) stack     (1001)     2324 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/utils/config_handler.py
--rw-rw-r--   0 stack     (1001) stack     (1001)     1468 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/utils/console.py
--rw-rw-r--   0 stack     (1001) stack     (1001)    11825 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/utils/constants.py
--rw-rw-r--   0 stack     (1001) stack     (1001)     3661 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/utils/decorators.py
--rw-rw-r--   0 stack     (1001) stack     (1001)     2830 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/utils/exception.py
--rw-rw-r--   0 stack     (1001) stack     (1001)     6694 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/utils/file_handler.py
--rw-rw-r--   0 stack     (1001) stack     (1001)    44133 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/utils/performance_category_map.py
--rw-rw-r--   0 stack     (1001) stack     (1001)     6091 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/utils/performance_constants.py
--rw-rw-r--   0 stack     (1001) stack     (1001)     2650 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/utils/time_handler.py
--rw-rw-r--   0 stack     (1001) stack     (1001)     3200 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/PyU4V/workload_planner.py
-drwxrwxr-x   0 stack     (1001) stack     (1001)        0 2022-02-03 12:17:40.289474 PyU4V-9.2.1.6/PyU4V.egg-info/
--rw-rw-r--   0 stack     (1001) stack     (1001)    12003 2022-02-03 12:17:40.000000 PyU4V-9.2.1.6/PyU4V.egg-info/PKG-INFO
--rw-rw-r--   0 stack     (1001) stack     (1001)      853 2022-02-03 12:17:40.000000 PyU4V-9.2.1.6/PyU4V.egg-info/SOURCES.txt
--rw-rw-r--   0 stack     (1001) stack     (1001)        1 2022-02-03 12:17:40.000000 PyU4V-9.2.1.6/PyU4V.egg-info/dependency_links.txt
--rw-rw-r--   0 stack     (1001) stack     (1001)       33 2022-02-03 12:17:40.000000 PyU4V-9.2.1.6/PyU4V.egg-info/requires.txt
--rw-rw-r--   0 stack     (1001) stack     (1001)        6 2022-02-03 12:17:40.000000 PyU4V-9.2.1.6/PyU4V.egg-info/top_level.txt
--rw-rw-r--   0 stack     (1001) stack     (1001)    11013 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/README.rst
--rw-rw-r--   0 stack     (1001) stack     (1001)       38 2022-02-03 12:17:40.293474 PyU4V-9.2.1.6/setup.cfg
--rw-rw-r--   0 stack     (1001) stack     (1001)     1976 2022-02-03 12:17:14.000000 PyU4V-9.2.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 11:48:37.000000 PyU4V-9.2.1.7/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 11:48:37.000000 PyU4V-9.2.1.7/PyU4V/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 11:48:37.000000 PyU4V-9.2.1.7/PyU4V/tools/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 11:48:37.000000 PyU4V-9.2.1.7/PyU4V/tools/openstack/
+-rw-r--r--   0 root         (0) root         (0)       19 2019-12-19 06:11:55.000000 PyU4V-9.2.1.7/PyU4V/tools/openstack/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7265 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/tools/openstack/migrate.py
+-rw-r--r--   0 root         (0) root         (0)    38251 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/tools/openstack/migrate_utils.py
+-rw-r--r--   0 root         (0) root         (0)       20 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 11:48:37.000000 PyU4V-9.2.1.7/PyU4V/utils/
+-rw-r--r--   0 root         (0) root         (0)      620 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/utils/config_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1468 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/utils/console.py
+-rw-r--r--   0 root         (0) root         (0)    11782 2023-02-08 11:44:29.000000 PyU4V-9.2.1.7/PyU4V/utils/constants.py
+-rw-r--r--   0 root         (0) root         (0)     3661 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/utils/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     2830 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/utils/exception.py
+-rw-r--r--   0 root         (0) root         (0)     6694 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/utils/file_handler.py
+-rw-r--r--   0 root         (0) root         (0)    44133 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/utils/performance_category_map.py
+-rw-r--r--   0 root         (0) root         (0)     6091 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/utils/performance_constants.py
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/utils/time_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-02-08 11:44:29.000000 PyU4V-9.2.1.7/PyU4V/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31886 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/common.py
+-rw-r--r--   0 root         (0) root         (0)    14523 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/metro_dr.py
+-rw-r--r--   0 root         (0) root         (0)     8683 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/migration.py
+-rw-r--r--   0 root         (0) root         (0)   116498 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/performance.py
+-rw-r--r--   0 root         (0) root         (0)   120563 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/provisioning.py
+-rw-r--r--   0 root         (0) root         (0)    23146 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/real_time.py
+-rw-r--r--   0 root         (0) root         (0)    71326 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/replication.py
+-rw-r--r--   0 root         (0) root         (0)    10241 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/rest_requests.py
+-rw-r--r--   0 root         (0) root         (0)    32811 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/snapshot_policy.py
+-rw-r--r--   0 root         (0) root         (0)    41778 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/system.py
+-rw-r--r--   0 root         (0) root         (0)     6780 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/univmax_conn.py
+-rw-r--r--   0 root         (0) root         (0)     3200 2023-02-07 10:39:01.000000 PyU4V-9.2.1.7/PyU4V/workload_planner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 11:48:37.000000 PyU4V-9.2.1.7/PyU4V.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12004 2023-02-08 11:48:37.000000 PyU4V-9.2.1.7/PyU4V.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      853 2023-02-08 11:48:37.000000 PyU4V-9.2.1.7/PyU4V.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-08 11:48:37.000000 PyU4V-9.2.1.7/PyU4V.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-02-08 11:48:37.000000 PyU4V-9.2.1.7/PyU4V.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-02-08 11:48:37.000000 PyU4V-9.2.1.7/PyU4V.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     9566 2019-12-19 06:11:55.000000 PyU4V-9.2.1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11014 2023-02-08 11:44:29.000000 PyU4V-9.2.1.7/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-02-08 11:44:29.000000 PyU4V-9.2.1.7/setup.py
+-rw-r--r--   0 root         (0) root         (0)    12004 2023-02-08 11:48:37.000000 PyU4V-9.2.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-08 11:48:37.000000 PyU4V-9.2.1.7/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `PyU4V-9.2.1.6/LICENSE` & `PyU4V-9.2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PKG-INFO` & `PyU4V-9.2.1.7/PyU4V.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyU4V
-Version: 9.2.1.6
+Version: 9.2.1.7
 Summary: A Python library for use with Dell EMC's Unisphere for PowerMax REST API.
 Home-page: https://github.com/dell/PyU4V/
 Author: Dell Inc. or its subsidiaries
 Author-email: paule.martin@dell.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -47,15 +47,15 @@
 
 PyU4V Version 9.2
 -----------------
 
 +-------------------------------+----------------------------+
 | **Author**                    | Dell EMC                   |
 +-------------------------------+----------------------------+
-| **PyU4V Version**             | 9.2.1.6                    |
+| **PyU4V Version**             | 9.2.1.7                    |
 +-------------------------------+----------------------------+
 | **Minimum Unisphere Version** | 9.2.0.1                    |
 +-------------------------------+----------------------------+
 | **Array Model**               | VMAX-3, VMAX AFA, PowerMax |
 +-------------------------------+----------------------------+
 | **Array uCode**               | HyperMax OS, PowerMax OS   |
 +-------------------------------+----------------------------+
@@ -101,15 +101,15 @@
     $ pip install .
 
 Installing via ``pip`` without cloning from source can be achieved by
 specifying ``PyU4V`` as the install package for ``pip``::
 
     $ pip install PyU4V
     # Install a specific version
-    $ pip install PyU4V==9.2.1.6
+    $ pip install PyU4V==9.2.1.7
 
 Copy the sample ``PyU4V.conf`` provided with PyU4V to either your working
 directory or within a directory named ``.PyU4V`` in your current users home
 directory. The ``.sample`` suffix has to be removed for the configuration file
 to become valid for loading by PyU4V::
 
     $ mkdir ~/.PyU4V
@@ -285,7 +285,8 @@
 .. _Requests: https://realpython.com/python-requests/
 .. _Six: https://six.readthedocs.io/
 .. _urllib3: https://urllib3.readthedocs.io/en/latest/
 .. _ReadTheDocs: https://pyu4v.readthedocs.io/en/latest/
 .. _GitHub-Issues: https://github.com/dell/PyU4V/issues
 .. _StackOverFlow: https://stackoverflow.com/search?q=PyU4V
 
+
```

### Comparing `PyU4V-9.2.1.6/PyU4V/__init__.py` & `PyU4V-9.2.1.7/PyU4V/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,11 +19,11 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """__init__.py."""
 
 from .univmax_conn import U4VConn  # noqa: F401
 
 __title__ = 'pyu4v'
-__version__ = '9.2.1.6'
+__version__ = '9.2.1.7'
 __author__ = 'Dell EMC or its subsidiaries'
 __license__ = 'Apache 2.0'
 __copyright__ = 'Copyright 2020 Dell EMC Inc'
```

### Comparing `PyU4V-9.2.1.6/PyU4V/common.py` & `PyU4V-9.2.1.7/PyU4V/common.py`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PyU4V/metro_dr.py` & `PyU4V-9.2.1.7/PyU4V/metro_dr.py`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PyU4V/migration.py` & `PyU4V-9.2.1.7/PyU4V/migration.py`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PyU4V/performance.py` & `PyU4V-9.2.1.7/PyU4V/performance.py`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PyU4V/provisioning.py` & `PyU4V-9.2.1.7/PyU4V/provisioning.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,16 +43,14 @@
 SLO = constants.SLO
 SRP = constants.SRP
 COMPRESSIBILITY_REPORT = constants.COMPRESSIBILITY_REPORT
 STORAGEGROUP = constants.STORAGEGROUP
 SG_DEMAND_REPORT = constants.SG_DEMAND_REPORT
 VOLUME = constants.VOLUME
 WORKLOADTYPE = constants.WORKLOADTYPE
-FICON_SPLIT = constants.FICON_SPLIT
-CU_IMAGE = constants.CU_IMAGE
 
 
 class ProvisioningFunctions(object):
     """ProvisioningFunctions."""
 
     def __init__(self, array_id, rest_client):
         """__init__."""
@@ -1553,16 +1551,15 @@
         sg = self.get_storage_group(parent_name)
         return sg.get('child_storage_group', list()) if sg else list()
 
     def create_storage_group(
             self, srp_id, sg_id, slo=None, workload=None,
             do_disable_compression=False, num_vols=0, vol_size=0,
             cap_unit='GB', allocate_full=False, _async=False,
-            vol_name=None, snapshot_policy_ids=None, enable_mobility_id=False,
-            emulation_type='FBA'):
+            vol_name=None, snapshot_policy_ids=None, enable_mobility_id=False):
         """Create a storage group with optional volumes on create operation.
 
         :param srp_id: SRP id -- str
         :param sg_id: storage group id -- str
         :param slo: service level id -- str
         :param workload: workload id -- str
         :param do_disable_compression: disable compression -- bool
@@ -1572,24 +1569,23 @@
         :param allocate_full: allocate full capacity -- bool
         :param _async: if call should be async -- bool
         :param vol_name: name to give to the volume, optional -- str
         :param snapshot_policy_ids: list of one or more snapshot policies
                                     to associate with storage group -- list
         :param enable_mobility_id: enables unique volume WWN not tied to array
                                    serial number -- bool
-        :param emulation_type: device emulation type (CKD, FBA) -- str
         :returns: storage group details -- dict
         """
         srp_id = srp_id if srp_id else 'None'
         slo = slo if slo else 'None'
         workload = workload if workload else 'None'
 
         payload = ({'srpId': srp_id,
                     'storageGroupId': sg_id,
-                    'emulation': emulation_type})
+                    'emulation': 'FBA'})
 
         volume_attributes = {'volume_size': str(vol_size),
                              'capacityUnit': cap_unit,
                              'num_of_vols': num_vols}
         if vol_name:
             volume_identifier = {'identifier_name': vol_name,
                                  'volumeIdentifierChoice': 'identifier_name'}
@@ -1659,16 +1655,15 @@
         return self.create_non_empty_storage_group(
             srp_id, sg_id, slo, workload, num_vols, vol_size, cap_unit,
             disable_compression, _async)
 
     def create_non_empty_storage_group(
             self, srp_id, storage_group_id, service_level, workload, num_vols,
             vol_size, cap_unit, disable_compression=False, _async=False,
-            vol_name=None, snapshot_policy_ids=None, enable_mobility_id=False,
-            emulation_type='FBA'):
+            vol_name=None, snapshot_policy_ids=None, enable_mobility_id=False):
         """Create a new storage group with the specified volumes.
 
         Generates a dictionary for json formatting and calls the create_sg
         function to create a new storage group with the specified volumes. Set
         the disable_compression flag for disabling compression on an All Flash
         array (where compression is on by default).
 
@@ -1682,25 +1677,23 @@
         :param disable_compression: disable compression -- bool
         :param _async: if call should be async -- bool
         :param vol_name: name to give to the volume, optional -- str
         :param snapshot_policy_ids: list of one or more snapshot policies
                                     to associate with storage group -- list
         :param enable_mobility_id: enables unique volume WWN not tied to array
                                    serial number -- bool
-        :param emulation_type: device emulation type (CKD, FBA) -- str
         :returns: storage group details -- dict
         """
         return self.create_storage_group(
             srp_id, storage_group_id, service_level, workload,
             do_disable_compression=disable_compression,
             num_vols=num_vols, vol_size=vol_size, cap_unit=cap_unit,
             _async=_async, vol_name=vol_name,
             snapshot_policy_ids=snapshot_policy_ids,
-            enable_mobility_id=enable_mobility_id,
-            emulation_type=emulation_type)
+            enable_mobility_id=enable_mobility_id)
 
     @decorators.refactoring_notice(
         'ProvisioningFunctions',
         'ProvisioningFunctions.create_empty_storage_group', 9.1, 10.0)
     def create_empty_sg(self, srp_id, sg_id, slo, workload,
                         disable_compression=False, _async=False):
         """Create an empty storage group.
@@ -1723,36 +1716,34 @@
         """
         return self.create_empty_storage_group(
             srp_id, sg_id, slo, workload, disable_compression, _async)
 
     def create_empty_storage_group(
             self, srp_id, storage_group_id, service_level, workload,
             disable_compression=False, _async=False,
-            snapshot_policy_ids=None, emulation_type='FBA'):
+            snapshot_policy_ids=None):
         """Create an empty storage group.
 
         Set the disable_compression flag for disabling compression on an All
         Flash array (where compression is on by default).
 
         :param srp_id: SRP id -- str
         :param storage_group_id: storage group id -- str
         :param service_level: service level id -- str
         :param workload: workload id -- str
         :param disable_compression: disable compression -- bool
         :param _async: if call should be async -- bool
         :param snapshot_policy_ids: list of one or more snapshot policies
                                     to associate with storage group -- list
-        :param emulation_type: device emulation type (CKD, FBA) -- str
         :returns: storage group details -- dict
         """
         return self.create_storage_group(
             srp_id, storage_group_id, service_level, workload,
             do_disable_compression=disable_compression, _async=_async,
-            snapshot_policy_ids=snapshot_policy_ids,
-            emulation_type=emulation_type)
+            snapshot_policy_ids=snapshot_policy_ids)
 
     def modify_storage_group(self, storage_group_id, payload):
         """Modify a storage group.
 
         :param storage_group_id: storage group id -- str
         :param payload: request payload -- dict
         :returns: modified storage group details -- dict
@@ -1864,15 +1855,15 @@
             create_new_volumes)
 
     def add_new_volume_to_storage_group(
             self, storage_group_id, num_vols, vol_size, cap_unit, _async=False,
             vol_name=None, create_new_volumes=None,
             remote_array_1_id=None, remote_array_1_sgs=None,
             remote_array_2_id=None, remote_array_2_sgs=None,
-            enable_mobility_id=False, emulation_type='FBA'):
+            enable_mobility_id=False):
         """Expand an existing storage group by adding new volumes.
 
         :param storage_group_id: storage group id -- str
         :param num_vols: number of volumes to be created -- int
         :param vol_size: the volume size -- str
         :param cap_unit: capacity unit (MB, GB, TB, CYL) -- str
         :param _async: if call should be async -- bool
@@ -1888,18 +1879,17 @@
         :param remote_array_2_id: optional digit serial number of remote array,
                                   only used in multihop SRDF, e.g. R11, or
                                   R1 - R21 - R2 optional -- str
         :param remote_array_2_sgs: storage groups on remote array, optional
                                    -- str or list
         :param enable_mobility_id: enables unique volume WWN not tied to array
                                    serial number -- bool
-        :param emulation_type: device emulation type (CKD, FBA) -- str
         :returns: storage group details -- dict
         """
-        add_volume_param = {'emulation': emulation_type}
+        add_volume_param = {'emulation': 'FBA'}
 
         if not create_new_volumes:
             add_volume_param.update({'create_new_volumes': False})
 
         volume_attributes = ({
             'num_of_vols': num_vols,
             'volume_size': vol_size,
@@ -2057,31 +2047,29 @@
         :returns: device id -- str
         """
         return self.create_volume_from_storage_group_return_id(
             volume_name, storagegroup_name, vol_size, cap_unit)
 
     def create_volume_from_storage_group_return_id(
             self, volume_name, storage_group_id, vol_size, cap_unit='GB',
-            enable_mobility_id=False, emulation_type='FBA'):
+            enable_mobility_id=False):
         """Create a new volume in the given storage group.
 
         :param volume_name: volume name -- str
         :param storage_group_id: storage group id -- str
         :param vol_size: volume size -- str
         :param cap_unit: capacity unit (MB, GB, TB, CYL) -- str
         :param enable_mobility_id: enables unique volume WWN not tied to array
                                    serial number -- bool
-        :param emulation_type: device emulation type (CKD, FBA) -- str
         :returns: device id -- str
         """
         job = self.add_new_volume_to_storage_group(
             storage_group_id, 1, vol_size, cap_unit,
             _async=True, vol_name=volume_name,
-            enable_mobility_id=enable_mobility_id,
-            emulation_type=emulation_type)
+            enable_mobility_id=enable_mobility_id)
 
         task = self.common.wait_for_job('Create volume from storage group',
                                         202, job)
 
         # Find the newly created volume.
         device_id = None
         if task:
@@ -2803,210 +2791,7 @@
                 if len(split_port_id) > 1:
                     corrected_port_id = split_port_id[-1]
                     symmetrix_port_key[index][
                         constants.PORT_ID] = corrected_port_id
             port_group_details[
                 constants.SYMMETRIX_PORT_KEY] = symmetrix_port_key
         return port_group_details
-
-    def get_split_list(self):
-        """Get list of FICON splits from array.
-
-        :returns: split ids -- list
-        """
-        split_id_list = list()
-        response = self.common.get_resource(category=SLOPROVISIONING,
-                                            resource_level=SYMMETRIX,
-                                            resource_level_id=self.array_id,
-                                            resource_type=FICON_SPLIT)
-        if response and response.get('splitId'):
-            split_id_list = response['splitId']
-        return split_id_list
-
-    def get_split(self, split_id: str):
-        """Get details of a specified FICON split.
-
-        :param split_id: split id -- str
-        :returns: split details -- dict
-        """
-        return self.common.get_resource(category=SLOPROVISIONING,
-                                        resource_level=SYMMETRIX,
-                                        resource_level_id=self.array_id,
-                                        resource_type=FICON_SPLIT,
-                                        resource_type_id=split_id)
-
-    def get_cu_image_list(self, split_id: str):
-        """Get list of CU Image SSIDs within a specific FICON Split.
-
-        :param split_id: split id -- str
-        :returns: CU Image ssids -- list
-        """
-        cu_image_ssid_list = list()
-        response = self.common.get_resource(category=SLOPROVISIONING,
-                                            resource_level=SYMMETRIX,
-                                            resource_level_id=self.array_id,
-                                            resource_type=FICON_SPLIT,
-                                            resource_type_id=split_id,
-                                            resource=CU_IMAGE)
-        if response and response.get('cuImageSSID'):
-            cu_image_ssid_list = response['cuImageSSID']
-        return cu_image_ssid_list
-
-    def get_cu_image(self, split_id: str, cu_ssid: str):
-        """Get details of a specified CU Image.
-
-        :param split_id: split id -- str
-        :param cu_ssid: cu image ssid -- str
-        :returns: CU Image details -- dict
-        """
-        return self.common.get_resource(category=SLOPROVISIONING,
-                                        resource_level=SYMMETRIX,
-                                        resource_level_id=self.array_id,
-                                        resource_type=FICON_SPLIT,
-                                        resource_type_id=split_id,
-                                        resource=CU_IMAGE,
-                                        resource_id=cu_ssid)
-
-    def create_cu_image(self, split_id: str,
-                        cu_number: str, cu_ssid: str, cu_base_address: str,
-                        vol_id: str):
-        """Creates a new CU image under the specified split.
-
-        :param split_id: split id -- str
-        :param cu_number: cu image number -- str
-        :param cu_ssid: cu image ssid -- str
-        :param cu_base_address: cu image ssid -- str
-        :param vol_id volume device id be mapped to the cu -- str
-
-        :returns: None
-        """
-        new_cu_data = {"cuImageSSID": cu_ssid,
-                       "cuImageNumber": cu_number,
-                       "startBaseAddress": cu_base_address,
-                       "volumeId": [vol_id]
-                       }
-        # FIXME This call takes over 5 minutes on my powermax 8000 -
-        # so need to force async call
-        new_cu_data.update(ASYNC_UPDATE)
-
-        create_cu_async_job = (
-            self.common.create_resource(category=SLOPROVISIONING,
-                                        resource_level=SYMMETRIX,
-                                        resource_level_id=self.array_id,
-                                        resource_type=FICON_SPLIT,
-                                        resource_type_id=split_id,
-                                        resource=CU_IMAGE,
-                                        payload=new_cu_data))
-        return self.common.wait_for_job(
-            operation='Create CU Image with volume',
-            status_code=constants.STATUS_202,
-            job=create_cu_async_job)
-
-    def get_cu_image_volumes(self, split_id: str, cu_ssid: str):
-        """Get list of Volumes from a specified CU Image.
-
-        :param split_id: split id -- str
-        :param cu_ssid: cu image ssid -- str
-        :returns: Volume ids -- list
-        """
-        volume_id_list = list()
-        response = self.common.get_resource(category=SLOPROVISIONING,
-                                            resource_level=SYMMETRIX,
-                                            resource_level_id=self.array_id,
-                                            resource_type=FICON_SPLIT,
-                                            resource_type_id=split_id,
-                                            resource=CU_IMAGE,
-                                            resource_id=cu_ssid,
-                                            object_type=VOLUME)
-        if response and response.get('volumeId'):
-            volume_id_list = response['volumeId']
-        return volume_id_list
-
-    def get_cu_image_volume(self, split_id: str, cu_ssid: str, vol_id: str):
-        """Get details of a volume mapped to a specified CU Image.
-
-        :param split_id: split id -- str
-        :param cu_ssid: cu image ssid -- str
-        :pamam vol_id volume device id to be mapped to the cu -- str
-        :returns: volume details -- dict
-        """
-        return self.common.get_resource(category=SLOPROVISIONING,
-                                        resource_level=SYMMETRIX,
-                                        resource_level_id=self.array_id,
-                                        resource_type=FICON_SPLIT,
-                                        resource_type_id=split_id,
-                                        resource=CU_IMAGE,
-                                        resource_id=cu_ssid,
-                                        object_type=VOLUME,
-                                        object_type_id=vol_id)
-
-    def modify_cu_image(self, split_id: str, cu_ssid: str,
-                        assign_alias_dict=None,
-                        remove_alias_dict=None,
-                        map_start_address=None,
-                        map_volume_list=None,
-                        unmap_volume_list=None):
-        """Modify an existing cu image.
-
-        :param split_id: split id -- str
-        :param cu_ssid: cu image ssid -- str
-        :param assign_alias_dict: alias range to be assigned -- dict
-        :param remove_alias_dict: alias range to be removed -- dict
-        :param map_start_address:
-        :param map_volume_list: volumes to be mapped -- list
-        :param unmap_volume_list: volumes to be unmapped -- list
-        """
-        if assign_alias_dict:
-            operation = 'Edit CU Image - Assign Alias'
-            edit_cu_data = {
-                'editCUImageActionParam': {
-                    'assignAliasRangeParam': assign_alias_dict
-                }
-            }
-        elif remove_alias_dict:
-            operation = 'Edit CU Image - Remove Alias'
-            edit_cu_data = {
-                'editCUImageActionParam': {
-                    'removeAliasRangeParam': remove_alias_dict
-                }
-            }
-        elif map_volume_list:
-            operation = 'Edit CU Image - Map Volume(s)'
-            edit_cu_data = {
-                'editCUImageActionParam': {
-                    'mapVolumeParam': {
-                        'startBaseAddress': map_start_address,
-                        'volumeId': map_volume_list
-                    }
-                }
-            }
-        elif unmap_volume_list:
-            operation = 'Edit CU Image - Unmap Volume(s)'
-            edit_cu_data = {
-                'editCUImageActionParam': {
-                    'unmapVolumeParam': {
-                        'volumeId': unmap_volume_list
-                    }
-                }
-            }
-        else:
-            msg = ('No modify cu image parameters chosen - please supply '
-                   'one of the following: assign_alias_dict, '
-                   'remove_alias_dict, map_volume_list, or unmap_volume_list.')
-            raise exception.InvalidInputException(data=msg)
-
-        # FIXME This call takes over 5 minutes on my powermax 8000
-        #  - so need to force async call
-        edit_cu_data.update(ASYNC_UPDATE)
-
-        edit_cu_async_job = (
-            self.common.modify_resource(category=SLOPROVISIONING,
-                                        resource_level=SYMMETRIX,
-                                        resource_level_id=self.array_id,
-                                        resource_type=FICON_SPLIT,
-                                        resource_type_id=split_id,
-                                        resource=CU_IMAGE,
-                                        resource_id=cu_ssid,
-                                        payload=edit_cu_data))
-        return self.common.wait_for_job(
-            operation=operation, status_code=constants.STATUS_202,
-            job=edit_cu_async_job)
```

### Comparing `PyU4V-9.2.1.6/PyU4V/real_time.py` & `PyU4V-9.2.1.7/PyU4V/real_time.py`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PyU4V/replication.py` & `PyU4V-9.2.1.7/PyU4V/replication.py`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PyU4V/rest_requests.py` & `PyU4V-9.2.1.7/PyU4V/rest_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,38 +47,40 @@
 APP_MPART = constants.APP_MPART
 
 
 class RestRequests(object):
     """RestRequests."""
 
     def __init__(self, username, password, verify, base_url, interval, retries,
-                 application_type=None):
+                 application_type=None, proxies=None):
         """__init__."""
         self.username = username
         self.password = password
         self.verify_ssl = verify
         self.base_url = base_url
         self.headers = {CONTENT_TYPE: APP_JSON,
                         ACCEPT: APP_JSON,
                         USER_AGENT: ua_details,
                         APP_TYPE: application_type}
         self.timeout = 120
         self.interval = interval
         self.retries = retries
+        self.proxies = proxies
         self.session = self.establish_rest_session()
 
     def establish_rest_session(self, headers=None):
         """Establish a REST session.
 
         :returns: session -- object
         """
         session = requests.session()
         session.headers = self.headers if not headers else headers
         session.auth = HTTPBasicAuth(self.username, self.password)
         session.verify = self.verify_ssl
+        session.proxies = self.proxies
         return session
 
     def rest_request(self, target_url, method,
                      params=None, request_object=None, timeout=None):
         """Send a request to the target api.
 
         Valid methods are 'GET', 'POST', 'PUT', 'DELETE'.
```

### Comparing `PyU4V-9.2.1.6/PyU4V/snapshot_policy.py` & `PyU4V-9.2.1.7/PyU4V/snapshot_policy.py`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PyU4V/system.py` & `PyU4V-9.2.1.7/PyU4V/system.py`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PyU4V/tools/openstack/migrate.py` & `PyU4V-9.2.1.7/PyU4V/tools/openstack/migrate.py`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PyU4V/tools/openstack/migrate_utils.py` & `PyU4V-9.2.1.7/PyU4V/tools/openstack/migrate_utils.py`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PyU4V/univmax_conn.py` & `PyU4V-9.2.1.7/PyU4V/univmax_conn.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     """U4VConn."""
 
     def __init__(self, username=None, password=None, server_ip=None,
                  port=None, verify=None,
                  u4v_version=constants.UNISPHERE_VERSION,
                  interval=5, retries=200, array_id=None,
                  application_type=app_type, remote_array=None,
-                 remote_array_2=None):
+                 remote_array_2=None, proxies=None):
         """__init__."""
         config = config_handler.set_logger_and_config(file_path)
         self.end_date = int(round(time.time() * 1000))
         self.start_date = (self.end_date - 3600000)
         self.array_id = array_id
         # Set array ID
         if not self.array_id:
@@ -106,15 +106,15 @@
             raise exception.MissingConfigurationException
         # Initialise REST session
         base_url = 'https://{server_ip}:{port}/univmax/restapi'.format(
             server_ip=server_ip, port=port)
 
         self.rest_client = RestRequests(
             username, password, verify, base_url, interval, retries,
-            application_type)
+            application_type, proxies)
         self.request = self.rest_client.rest_request
         self.common = CommonFunctions(self.rest_client)
         self.provisioning = ProvisioningFunctions(self.array_id,
                                                   self.rest_client)
         self.performance = PerformanceFunctions(self.array_id,
                                                 self.rest_client)
         self.replication = ReplicationFunctions(self.array_id,
```

### Comparing `PyU4V-9.2.1.6/PyU4V/utils/__init__.py` & `PyU4V-9.2.1.7/PyU4V/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PyU4V/utils/config_handler.py` & `PyU4V-9.2.1.7/PyU4V/utils/config_handler.py`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PyU4V/utils/console.py` & `PyU4V-9.2.1.7/PyU4V/utils/console.py`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PyU4V/utils/constants.py` & `PyU4V-9.2.1.7/PyU4V/utils/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 USER_AGENT = 'user-agent'
 APP_TYPE = 'application-type'
 APP_JSON = 'application/json'
 APP_OCT = 'application/octet-stream'
 APP_MPART = 'multipart/form-data'
 
 # Unisphere REST URI constants
-PYU4V_VERSION = '9.2.1.6'
+PYU4V_VERSION = '9.2.1.7'
 UNISPHERE_VERSION = '92'
 VERSION = 'version'
 ITERATOR = 'Iterator'
 PAGE = 'page'
 JOB = 'job'
 SYMMETRIX = 'symmetrix'
 SLOPROVISIONING = 'sloprovisioning'
@@ -81,16 +81,14 @@
 RDF_GROUP = 'rdf_group'
 GB_HEADROOM = 'gbHeadroom'
 RDF_DIRECTOR = 'rdf_director'
 REMOTE_PORT = 'remote_port'
 ALERT = 'alert'
 ALERT_SUMMARY = 'alert_summary'
 COMPLIANCE = 'compliance'
-FICON_SPLIT = 'split'
-CU_IMAGE = 'cuimage'
 
 # Status Codes
 STATUS_200 = 200
 STATUS_201 = 201
 STATUS_202 = 202
 STATUS_204 = 204
 STATUS_401 = 401
```

### Comparing `PyU4V-9.2.1.6/PyU4V/utils/decorators.py` & `PyU4V-9.2.1.7/PyU4V/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PyU4V/utils/exception.py` & `PyU4V-9.2.1.7/PyU4V/utils/exception.py`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PyU4V/utils/file_handler.py` & `PyU4V-9.2.1.7/PyU4V/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PyU4V/utils/performance_category_map.py` & `PyU4V-9.2.1.7/PyU4V/utils/performance_category_map.py`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PyU4V/utils/performance_constants.py` & `PyU4V-9.2.1.7/PyU4V/utils/performance_constants.py`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PyU4V/utils/time_handler.py` & `PyU4V-9.2.1.7/PyU4V/utils/time_handler.py`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PyU4V/workload_planner.py` & `PyU4V-9.2.1.7/PyU4V/workload_planner.py`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/PyU4V.egg-info/PKG-INFO` & `PyU4V-9.2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyU4V
-Version: 9.2.1.6
+Version: 9.2.1.7
 Summary: A Python library for use with Dell EMC's Unisphere for PowerMax REST API.
 Home-page: https://github.com/dell/PyU4V/
 Author: Dell Inc. or its subsidiaries
 Author-email: paule.martin@dell.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -47,15 +47,15 @@
 
 PyU4V Version 9.2
 -----------------
 
 +-------------------------------+----------------------------+
 | **Author**                    | Dell EMC                   |
 +-------------------------------+----------------------------+
-| **PyU4V Version**             | 9.2.1.6                    |
+| **PyU4V Version**             | 9.2.1.7                    |
 +-------------------------------+----------------------------+
 | **Minimum Unisphere Version** | 9.2.0.1                    |
 +-------------------------------+----------------------------+
 | **Array Model**               | VMAX-3, VMAX AFA, PowerMax |
 +-------------------------------+----------------------------+
 | **Array uCode**               | HyperMax OS, PowerMax OS   |
 +-------------------------------+----------------------------+
@@ -101,15 +101,15 @@
     $ pip install .
 
 Installing via ``pip`` without cloning from source can be achieved by
 specifying ``PyU4V`` as the install package for ``pip``::
 
     $ pip install PyU4V
     # Install a specific version
-    $ pip install PyU4V==9.2.1.6
+    $ pip install PyU4V==9.2.1.7
 
 Copy the sample ``PyU4V.conf`` provided with PyU4V to either your working
 directory or within a directory named ``.PyU4V`` in your current users home
 directory. The ``.sample`` suffix has to be removed for the configuration file
 to become valid for loading by PyU4V::
 
     $ mkdir ~/.PyU4V
@@ -285,7 +285,8 @@
 .. _Requests: https://realpython.com/python-requests/
 .. _Six: https://six.readthedocs.io/
 .. _urllib3: https://urllib3.readthedocs.io/en/latest/
 .. _ReadTheDocs: https://pyu4v.readthedocs.io/en/latest/
 .. _GitHub-Issues: https://github.com/dell/PyU4V/issues
 .. _StackOverFlow: https://stackoverflow.com/search?q=PyU4V
 
+
```

### Comparing `PyU4V-9.2.1.6/PyU4V.egg-info/SOURCES.txt` & `PyU4V-9.2.1.7/PyU4V.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyU4V-9.2.1.6/README.rst` & `PyU4V-9.2.1.7/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 PyU4V Version 9.2
 -----------------
 
 +-------------------------------+----------------------------+
 | **Author**                    | Dell EMC                   |
 +-------------------------------+----------------------------+
-| **PyU4V Version**             | 9.2.1.6                    |
+| **PyU4V Version**             | 9.2.1.7                    |
 +-------------------------------+----------------------------+
 | **Minimum Unisphere Version** | 9.2.0.1                    |
 +-------------------------------+----------------------------+
 | **Array Model**               | VMAX-3, VMAX AFA, PowerMax |
 +-------------------------------+----------------------------+
 | **Array uCode**               | HyperMax OS, PowerMax OS   |
 +-------------------------------+----------------------------+
@@ -76,15 +76,15 @@
     $ pip install .
 
 Installing via ``pip`` without cloning from source can be achieved by
 specifying ``PyU4V`` as the install package for ``pip``::
 
     $ pip install PyU4V
     # Install a specific version
-    $ pip install PyU4V==9.2.1.6
+    $ pip install PyU4V==9.2.1.7
 
 Copy the sample ``PyU4V.conf`` provided with PyU4V to either your working
 directory or within a directory named ``.PyU4V`` in your current users home
 directory. The ``.sample`` suffix has to be removed for the configuration file
 to become valid for loading by PyU4V::
 
     $ mkdir ~/.PyU4V
@@ -258,8 +258,8 @@
 .. README URL Links
 
 .. _Requests: https://realpython.com/python-requests/
 .. _Six: https://six.readthedocs.io/
 .. _urllib3: https://urllib3.readthedocs.io/en/latest/
 .. _ReadTheDocs: https://pyu4v.readthedocs.io/en/latest/
 .. _GitHub-Issues: https://github.com/dell/PyU4V/issues
-.. _StackOverFlow: https://stackoverflow.com/search?q=PyU4V
+.. _StackOverFlow: https://stackoverflow.com/search?q=PyU4V
```

### Comparing `PyU4V-9.2.1.6/setup.py` & `PyU4V-9.2.1.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import setuptools
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='PyU4V',
-    version='9.2.1.6',
+    version='9.2.1.7',
     url='https://github.com/dell/PyU4V/',
     author='Dell Inc. or its subsidiaries',
     author_email='paule.martin@dell.com',
     description="A Python library for use with Dell EMC's Unisphere for "
                 "PowerMax REST API.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
```

