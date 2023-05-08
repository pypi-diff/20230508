# Comparing `tmp/clearblade-cloud-iot-1.0.7.tar.gz` & `tmp/clearblade-cloud-iot-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clearblade-cloud-iot-1.0.7.tar", last modified: Fri Mar 24 21:22:44 2023, max compression
+gzip compressed data, was "dist/clearblade-cloud-iot-2.0.0.tar", last modified: Mon May  8 18:05:12 2023, max compression
```

## Comparing `clearblade-cloud-iot-1.0.7.tar` & `clearblade-cloud-iot-2.0.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/clearblade/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/clearblade/cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/clearblade/cloud/iot_v1/
--rw-rw-r--   0 root         (0) root         (0)    20915 2023-03-24 21:20:19.000000 clearblade-cloud-iot-1.0.7/clearblade/cloud/iot_v1/device_types.py
--rw-rw-r--   0 root         (0) root         (0)    11457 2023-01-10 13:33:26.000000 clearblade-cloud-iot-1.0.7/clearblade/cloud/iot_v1/developer_tests.py
--rw-rw-r--   0 root         (0) root         (0)     2113 2023-01-10 13:33:26.000000 clearblade-cloud-iot-1.0.7/clearblade/cloud/iot_v1/resources.py
--rw-rw-r--   0 root         (0) root         (0)     7129 2023-01-10 13:33:26.000000 clearblade-cloud-iot-1.0.7/clearblade/cloud/iot_v1/registry.py
--rw-rw-r--   0 root         (0) root         (0)     5295 2022-12-28 20:22:40.000000 clearblade-cloud-iot-1.0.7/clearblade/cloud/iot_v1/config_manager.py
--rw-rw-r--   0 root         (0) root         (0)     5999 2023-01-10 13:33:26.000000 clearblade-cloud-iot-1.0.7/clearblade/cloud/iot_v1/registry_types.py
--rw-rw-r--   0 root         (0) root         (0)     1540 2023-01-10 13:33:26.000000 clearblade-cloud-iot-1.0.7/clearblade/cloud/iot_v1/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6184 2022-12-28 16:41:28.000000 clearblade-cloud-iot-1.0.7/clearblade/cloud/iot_v1/http_client.py
--rw-rw-r--   0 root         (0) root         (0)      740 2022-12-08 12:14:06.000000 clearblade-cloud-iot-1.0.7/clearblade/cloud/iot_v1/config.py
--rw-rw-r--   0 root         (0) root         (0)    21608 2023-02-28 17:43:26.000000 clearblade-cloud-iot-1.0.7/clearblade/cloud/iot_v1/devices.py
--rw-rw-r--   0 root         (0) root         (0)     8103 2022-12-28 16:41:28.000000 clearblade-cloud-iot-1.0.7/clearblade/cloud/iot_v1/client.py
--rw-rw-r--   0 root         (0) root         (0)     5420 2022-12-08 12:14:06.000000 clearblade-cloud-iot-1.0.7/clearblade/cloud/iot_v1/pagers.py
--rw-rw-r--   0 root         (0) root         (0)     1015 2023-03-22 18:07:52.000000 clearblade-cloud-iot-1.0.7/clearblade/cloud/iot_v1/utils.py
--rw-rw-r--   0 root         (0) root         (0)    11358 2022-11-02 06:10:48.000000 clearblade-cloud-iot-1.0.7/LICENSE
--rw-rw-r--   0 root         (0) root         (0)     1442 2023-02-20 19:02:15.000000 clearblade-cloud-iot-1.0.7/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)     4414 2023-02-28 17:43:26.000000 clearblade-cloud-iot-1.0.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/google/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/google/cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/google/cloud/iot/
--rw-rw-r--   0 root         (0) root         (0)       77 2022-11-02 06:10:48.000000 clearblade-cloud-iot-1.0.7/google/cloud/iot/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/google/cloud/iot_v1/
--rw-rw-r--   0 root         (0) root         (0)       77 2022-11-02 06:10:48.000000 clearblade-cloud-iot-1.0.7/google/cloud/iot_v1/py.typed
--rw-rw-r--   0 root         (0) root         (0)     5506 2022-11-02 06:10:48.000000 clearblade-cloud-iot-1.0.7/google/cloud/iot_v1/gapic_metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/tests/unit/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/tests/unit/gapic/
--rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-1.0.7/tests/unit/gapic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/tests/unit/gapic/iot_v1/
--rw-rw-r--   0 root         (0) root         (0)   235456 2023-02-20 19:02:15.000000 clearblade-cloud-iot-1.0.7/tests/unit/gapic/iot_v1/test_device_manager.py
--rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-1.0.7/tests/unit/gapic/iot_v1/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-1.0.7/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/tests/system/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/tests/system/gapic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/tests/system/gapic/v1/
--rw-rw-r--   0 root         (0) root         (0)     1557 2023-02-20 19:02:15.000000 clearblade-cloud-iot-1.0.7/tests/system/gapic/v1/test_system_device_manager_v1.py
--rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-1.0.7/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       67 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2835 2023-03-24 21:21:34.000000 clearblade-cloud-iot-1.0.7/setup.py
--rw-r--r--   0 root         (0) root         (0)     6198 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/clearblade_cloud_iot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1152 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/clearblade_cloud_iot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/clearblade_cloud_iot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/clearblade_cloud_iot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/clearblade_cloud_iot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     6198 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/clearblade_cloud_iot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-13 22:31:57.000000 clearblade-cloud-iot-1.0.7/clearblade_cloud_iot.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       28 2023-03-24 21:22:44.000000 clearblade-cloud-iot-1.0.7/clearblade_cloud_iot.egg-info/namespace_packages.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/clearblade/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/clearblade/cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/clearblade/cloud/iot_v1/
+-rw-rw-r--   0 root         (0) root         (0)    22073 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.0/clearblade/cloud/iot_v1/device_types.py
+-rw-rw-r--   0 root         (0) root         (0)    13659 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.0/clearblade/cloud/iot_v1/developer_tests.py
+-rw-rw-r--   0 root         (0) root         (0)     6471 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.0/clearblade/cloud/iot_v1/resources.py
+-rw-rw-r--   0 root         (0) root         (0)     9331 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.0/clearblade/cloud/iot_v1/registry.py
+-rw-rw-r--   0 root         (0) root         (0)     7497 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.0/clearblade/cloud/iot_v1/config_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     8201 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.0/clearblade/cloud/iot_v1/registry_types.py
+-rw-rw-r--   0 root         (0) root         (0)     3742 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.0/clearblade/cloud/iot_v1/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8386 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.0/clearblade/cloud/iot_v1/http_client.py
+-rw-rw-r--   0 root         (0) root         (0)     2942 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.0/clearblade/cloud/iot_v1/config.py
+-rw-rw-r--   0 root         (0) root         (0)    22724 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.0/clearblade/cloud/iot_v1/devices.py
+-rw-rw-r--   0 root         (0) root         (0)    10305 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.0/clearblade/cloud/iot_v1/client.py
+-rw-rw-r--   0 root         (0) root         (0)     7622 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.0/clearblade/cloud/iot_v1/pagers.py
+-rw-rw-r--   0 root         (0) root         (0)     3217 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.0/clearblade/cloud/iot_v1/utils.py
+-rw-rw-r--   0 root         (0) root         (0)    11358 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)     1442 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.0/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)     5090 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/google/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/google/cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/google/cloud/iot/
+-rw-rw-r--   0 root         (0) root         (0)       77 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.0/google/cloud/iot/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/google/cloud/iot_v1/
+-rw-rw-r--   0 root         (0) root         (0)       77 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.0/google/cloud/iot_v1/py.typed
+-rw-rw-r--   0 root         (0) root         (0)     5506 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.0/google/cloud/iot_v1/gapic_metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/tests/unit/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.0/tests/unit/gapic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/tests/unit/gapic/iot_v1/
+-rw-rw-r--   0 root         (0) root         (0)   235456 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.0/tests/unit/gapic/iot_v1/test_device_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.0/tests/unit/gapic/iot_v1/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.0/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/tests/system/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/tests/system/gapic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/tests/system/gapic/v1/
+-rw-rw-r--   0 root         (0) root         (0)     1557 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.0/tests/system/gapic/v1/test_system_device_manager_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.0/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2835 2023-05-08 18:03:03.000000 clearblade-cloud-iot-2.0.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     7002 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/clearblade_cloud_iot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/clearblade_cloud_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/clearblade_cloud_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/clearblade_cloud_iot.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/clearblade_cloud_iot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     7002 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/clearblade_cloud_iot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-13 22:31:57.000000 clearblade-cloud-iot-2.0.0/clearblade_cloud_iot.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-08 18:05:12.000000 clearblade-cloud-iot-2.0.0/clearblade_cloud_iot.egg-info/namespace_packages.txt
```

### Comparing `clearblade-cloud-iot-1.0.7/clearblade/cloud/iot_v1/device_types.py` & `clearblade-cloud-iot-2.0.0/clearblade/cloud/iot_v1/device_types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,66 @@
-# -*- coding: utf-8 -*-
-# Copyright 2023 ClearBlade Inc.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright 2022 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
+"""
+"Copyright 2023 ClearBlade Inc."
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+https://www.apache.org/licenses/LICENSE-2.0
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+Copyright 2018 Google LLC
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+https://www.apache.org/licenses/LICENSE-2.0
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+Copyright 2023 ClearBlade Inc.
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+https://www.apache.org/licenses/LICENSE-2.0
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+Copyright 2018 Google LLC
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+https://www.apache.org/licenses/LICENSE-2.0
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 from typing import List
-from .resources import GatewayType, LogLevel
+from .resources import GatewayType, LogLevel, PublicKeyFormat, PublicKeyCredential, DeviceCredential
 from .utils import get_value
 import os
 from proto.datetime_helpers import DatetimeWithNanoseconds
 import base64
 
+def convertCredentialsFormatsFromString(credentials):
+    # Converts public Key Format from string to object of class PublicKeyFormat
+    for index, credential in enumerate(credentials):
+        if 'publicKey' in credential:
+            credential['publicKey']['format'] = PublicKeyFormat(credential['publicKey']['format'])
+            credentials[index] = DeviceCredential(credential['publicKey'], credential['expirationTime'])
+    return credentials
+
 class Device():
     """
     Data class for Clearblade Device
     """
     # TODO: find a better way to construct the Device object. I dont like so much parameter in a constructor
 
     def __init__(self, id: str, num_id: str = None,
@@ -89,44 +112,28 @@
             last_heartbeat_time = lastHeartbeatTimeFromJson
             last_event_time = lastEventTimeFromJson
             last_state_time = lastStateTimeFromJson
             last_config_ack_time = lastConfigAckTimeFromJson
             last_config_send_time = lastConfigSendTimeFromJson
             last_error_time = lastErrorTimeFromJson
 
-        if (configFromJson):
-            deviceConfig = DeviceConfig.from_json(configFromJson)
-            config = { "version": deviceConfig.version, "cloudUpdateTime": deviceConfig.cloud_update_time }
-            if (deviceConfig.binary_data not in [None, ""]):
-                config["binaryData"] = deviceConfig.binary_data
-            if (deviceConfig.device_ack_time not in [None, ""]):
-                config["deviceAckTime"] = deviceConfig.device_ack_time
-        else:
-            config = configFromJson
-        
-        if (stateFromJson):
-            deviceState = DeviceState.from_json(stateFromJson)
-            state = { "updateTime": deviceState.update_time, "binaryData": deviceState.binary_data }
-        else:
-            state = stateFromJson
-
         return Device(
             id=get_value(json, 'id'),
             num_id=get_value(json, 'numId'),
-            credentials=get_value(json, 'credentials'),
+            credentials=convertCredentialsFormatsFromString(get_value(json, 'credentials')),
             last_heartbeat_time=last_heartbeat_time,
             last_event_time=last_event_time,
             last_state_time=last_state_time,
             last_config_ack_time=last_config_ack_time,
             last_config_send_time=last_config_send_time,
             last_error_time=last_error_time,
             blocked=get_value(json, 'blocked'),
             last_error_status_code=get_value(json, 'lastErrorStatus'),
-            config=config,
-            state=state,
+            config=DeviceConfig.from_json(configFromJson),
+            state=DeviceState.from_json(stateFromJson),
             log_level=get_value(json, 'logLevel'),
             meta_data=get_value(json, 'metadata'),
             gateway_config=get_value(json, 'gatewayConfig')
         )
 
     @property
     def id(self):
@@ -217,24 +224,30 @@
         self._blocked = blocked
 
 
 # classes to mock googles request & response
 
 class DeviceState():
     def __init__(self, update_time: str = None, binary_data:str = None) -> None:
-        self._update_time = update_time
-        self._binary_data = binary_data
+        self.updateTime = update_time
+        self.binaryData = binary_data
+
+    def __getitem__(self, arg):
+        return getattr(self, arg)
+
+    def get(self, arg):
+        return getattr(self, arg)
 
     @property
     def update_time(self):
-        return self._update_time
+        return self.updateTime
 
     @property
     def binary_data(self):
-        return self._binary_data
+        return self.binaryData
 
     @staticmethod
     def from_json(response_json):
         updateTimeFromJson = get_value(response_json, 'updateTime')
         binaryDataFromJson = get_value(response_json, 'binaryData')
         
         convert_times_to_datetime_with_nanoseconds = (False if os.environ.get("BINARYDATA_AND_TIME_GOOGLE_FORMAT") == None else os.environ.get("BINARYDATA_AND_TIME_GOOGLE_FORMAT").lower() == "true")
@@ -250,16 +263,15 @@
             else:
                 binary_data = binaryDataFromJson
         else:
             binary_data = binaryDataFromJson
 
         return DeviceState(update_time=update_time,
                            binary_data=binary_data)
-
-
+       
 class Request():
     def __init__(self, parent) -> None:
         self._parent = parent
 
     @property
     def parent(self):
         return self._parent
@@ -314,33 +326,39 @@
     def __init__(self, name,
                  version,
                  cloud_update_time,
                  device_ack_time,
                  binary_data) -> None:
         super().__init__(name)
         self._version = version
-        self._cloud_update_time = cloud_update_time
-        self._device_ack_time = device_ack_time
-        self._binary_data = binary_data
+        self.cloudUpdateTime = cloud_update_time
+        self.deviceAckTime = device_ack_time
+        self.binaryData = binary_data
+
+    def __getitem__(self, arg):
+        return getattr(self, arg)
+
+    def get(self, arg):
+        return getattr(self, arg)
 
     @property
     def version(self):
         return self._version
 
     @property
     def cloud_update_time(self):
-        return self._cloud_update_time
+        return self.cloudUpdateTime
 
     @property
     def device_ack_time(self):
-        return self._device_ack_time
+        return self.deviceAckTime
 
     @property
     def binary_data(self):
-        return self._binary_data
+        return self.binaryData
 
     @staticmethod
     def from_json(json):
         cloudUpdateTimeFromJson = get_value(json,'cloudUpdateTime')
         deviceAckTimeFromJson = get_value(json, 'deviceAckTime')
         binaryDataFromJson = get_value(json,'binaryData')
 
@@ -489,16 +507,16 @@
             body['logLevel'] = self._device.log_level
         if self._device.gateway_config is not None:
             body['gatewayConfig'] = self._device.gateway_config
         if self._device.meta_data is not None:
             body['metadata'] = self._device.meta_data
         if self._device._blocked is not None:
             body['blocked'] = self._device._blocked
-        if self._device.credentials is not None:
-            body['credentials'] = self._device.credentials
+        if self._device._credentials is not None:
+            body['credentials'] = DeviceCredential.convert_credentials_for_create_update(self._device._credentials)
 
         return params, body
 
 
 class ListDevicesRequest(Request):
     def __init__(self, parent:str = None ,
                  deviceNumIds: str = None,
```

### Comparing `clearblade-cloud-iot-1.0.7/clearblade/cloud/iot_v1/devices.py` & `clearblade-cloud-iot-2.0.0/clearblade/cloud/iot_v1/devices.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,57 @@
-# -*- coding: utf-8 -*-
-# Copyright 2023 ClearBlade Inc.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright 2022 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
+"""
+"Copyright 2023 ClearBlade Inc."
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+https://www.apache.org/licenses/LICENSE-2.0
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+Copyright 2018 Google LLC
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+https://www.apache.org/licenses/LICENSE-2.0
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+Copyright 2023 ClearBlade Inc.
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+https://www.apache.org/licenses/LICENSE-2.0
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+Copyright 2018 Google LLC
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+https://www.apache.org/licenses/LICENSE-2.0
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 from .config_manager import ClearBladeConfigManager
 from .device_types import *
 from .http_client import AsyncClient, SyncClient
 from .pagers import ListDevicesAsyncPager, ListDevicesPager
 import base64
-
+from .resources import DeviceCredential
 
 class ClearBladeDeviceManager():
 
     def __init__(self) -> None:
         # create the ClearBladeConfig object
         self._config_manager = ClearBladeConfigManager()
 
@@ -57,15 +72,15 @@
         params = {'name':request.parent,'method':'sendCommandToDevice'}
         body = {'binaryData':base64.b64encode(request.binary_data).decode("utf-8"), 'subfolder':request.sub_folder}
 
         return params,body
 
     def _create_device_body(self, device: Device) :
         return {'id':device.id,
-                'credentials':device.credentials,
+                'credentials':DeviceCredential.convert_credentials_for_create_update(device.credentials),
                 'config':device.config,
                 'blocked': device.blocked,
                 'logLevel':device.log_level, 'metadata':device.meta_data,
                 'gatewayConfig':device.gateway_config}
 
     def _create_device_from_response(self, json_response) -> Device :
         return Device.from_json(json=json_response)
```

### Comparing `clearblade-cloud-iot-1.0.7/LICENSE` & `clearblade-cloud-iot-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-1.0.7/MANIFEST.in` & `clearblade-cloud-iot-2.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-1.0.7/README.rst` & `clearblade-cloud-iot-2.0.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -112,8 +112,24 @@
 
 
 - To return these parameters using the same types used by the **Google IoTCore Python SDK**, set environment variable **BINARYDATA_AND_TIME_GOOGLE_FORMAT** to **True** (case-insensitive string). This will ensure the following parameters are returned as the shown types:
 
 1. All times: **DatetimeWithNanoseconds** (defined in the **proto.datetime_helpers** module)
 2. All **binaryData** (CONFIG, STATE etc.): **BYTE ARRAYS**
 
-- If this environment variable is not set, or is set to any unexpeced values, then the default types listed previously are used.
+- If this environment variable is not set, or is set to any unexpeced values, then the default types listed previously are used.
+
+Note about running from source instead of PyPi (pip) module:
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+- To temporarily use the source code in this repo. instead of the installed PyPi (pip) module do the following:
+
+1. Clone this repo.
+2. Checkout the desired branch using **git checkout <branch>**.
+3. In your code find where **clearblade** or **clearblade.cloud** is being imported.
+4. Precede that line with **import sys** and **sys.path.insert(0, <path_to_python-iot>)**. The path must end with "python-iot". So for example:
+
+.. code-block:: console
+
+    import sys
+    sys.path.insert(0, "path/to/python-iot")
+
+    from clearblade.cloud import iot_v1
```

### Comparing `clearblade-cloud-iot-1.0.7/google/cloud/iot_v1/gapic_metadata.json` & `clearblade-cloud-iot-2.0.0/google/cloud/iot_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-1.0.7/tests/unit/gapic/__init__.py` & `clearblade-cloud-iot-2.0.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-1.0.7/tests/unit/gapic/iot_v1/test_device_manager.py` & `clearblade-cloud-iot-2.0.0/tests/unit/gapic/iot_v1/test_device_manager.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-1.0.7/tests/unit/gapic/iot_v1/__init__.py` & `clearblade-cloud-iot-2.0.0/tests/unit/gapic/iot_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-1.0.7/tests/unit/__init__.py` & `clearblade-cloud-iot-2.0.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-1.0.7/tests/system/gapic/v1/test_system_device_manager_v1.py` & `clearblade-cloud-iot-2.0.0/tests/system/gapic/v1/test_system_device_manager_v1.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-1.0.7/tests/__init__.py` & `clearblade-cloud-iot-2.0.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-1.0.7/setup.py` & `clearblade-cloud-iot-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import io
 import os
 
 import setuptools
 
 name = "clearblade-cloud-iot"
 description = "Cloud IoT API client library"
-version = "1.0.7"
+version = "2.0.0"
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = ["httpx", "proto-plus"]
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
```

### Comparing `clearblade-cloud-iot-1.0.7/PKG-INFO` & `clearblade-cloud-iot-2.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: clearblade-cloud-iot
-Version: 1.0.7
+Version: 2.0.0
 Summary: Cloud IoT API client library
 Home-page: https://github.com/clearblade/python-iot
 Author: Clearblade
 Author-email: googleapis-packages@oogle.com
 License: Apache 2.0
 Description: .. Copyright 2023 ClearBlade Inc.
             Licensed under the Apache License, Version 2.0 (the "License");
@@ -121,14 +121,30 @@
         
         - To return these parameters using the same types used by the **Google IoTCore Python SDK**, set environment variable **BINARYDATA_AND_TIME_GOOGLE_FORMAT** to **True** (case-insensitive string). This will ensure the following parameters are returned as the shown types:
         
         1. All times: **DatetimeWithNanoseconds** (defined in the **proto.datetime_helpers** module)
         2. All **binaryData** (CONFIG, STATE etc.): **BYTE ARRAYS**
         
         - If this environment variable is not set, or is set to any unexpeced values, then the default types listed previously are used.
+        
+        Note about running from source instead of PyPi (pip) module:
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        - To temporarily use the source code in this repo. instead of the installed PyPi (pip) module do the following:
+        
+        1. Clone this repo.
+        2. Checkout the desired branch using **git checkout <branch>**.
+        3. In your code find where **clearblade** or **clearblade.cloud** is being imported.
+        4. Precede that line with **import sys** and **sys.path.insert(0, <path_to_python-iot>)**. The path must end with "python-iot". So for example:
+        
+        .. code-block:: console
+        
+            import sys
+            sys.path.insert(0, "path/to/python-iot")
+        
+            from clearblade.cloud import iot_v1
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `clearblade-cloud-iot-1.0.7/clearblade_cloud_iot.egg-info/SOURCES.txt` & `clearblade-cloud-iot-2.0.0/clearblade_cloud_iot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-1.0.7/clearblade_cloud_iot.egg-info/PKG-INFO` & `clearblade-cloud-iot-2.0.0/clearblade_cloud_iot.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: clearblade-cloud-iot
-Version: 1.0.7
+Version: 2.0.0
 Summary: Cloud IoT API client library
 Home-page: https://github.com/clearblade/python-iot
 Author: Clearblade
 Author-email: googleapis-packages@oogle.com
 License: Apache 2.0
 Description: .. Copyright 2023 ClearBlade Inc.
             Licensed under the Apache License, Version 2.0 (the "License");
@@ -121,14 +121,30 @@
         
         - To return these parameters using the same types used by the **Google IoTCore Python SDK**, set environment variable **BINARYDATA_AND_TIME_GOOGLE_FORMAT** to **True** (case-insensitive string). This will ensure the following parameters are returned as the shown types:
         
         1. All times: **DatetimeWithNanoseconds** (defined in the **proto.datetime_helpers** module)
         2. All **binaryData** (CONFIG, STATE etc.): **BYTE ARRAYS**
         
         - If this environment variable is not set, or is set to any unexpeced values, then the default types listed previously are used.
+        
+        Note about running from source instead of PyPi (pip) module:
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        - To temporarily use the source code in this repo. instead of the installed PyPi (pip) module do the following:
+        
+        1. Clone this repo.
+        2. Checkout the desired branch using **git checkout <branch>**.
+        3. In your code find where **clearblade** or **clearblade.cloud** is being imported.
+        4. Precede that line with **import sys** and **sys.path.insert(0, <path_to_python-iot>)**. The path must end with "python-iot". So for example:
+        
+        .. code-block:: console
+        
+            import sys
+            sys.path.insert(0, "path/to/python-iot")
+        
+            from clearblade.cloud import iot_v1
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

