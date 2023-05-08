# Comparing `tmp/antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2.tar.gz` & `tmp/antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2.tar", last modified: Mon May  8 02:35:38 2023, max compression
+gzip compressed data, was "dist/antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0.tar", last modified: Mon May  8 11:01:44 2023, max compression
```

## Comparing `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2.tar` & `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:35:38.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-08 02:35:37.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-08 02:35:37.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-08 02:35:38.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-05-08 02:35:37.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-05-08 02:35:37.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:35:38.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-08 02:35:38.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-08 02:35:38.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 02:35:38.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-08 02:35:38.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-08 02:35:38.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:35:38.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-08 02:35:37.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49422 2023-05-08 02:35:37.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/client.py
--rw-r--r--   0 root         (0) root         (0)    46245 2023-05-08 02:35:37.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-08 02:35:38.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-05-08 02:35:37.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:01:44.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-08 11:01:43.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-08 11:01:43.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-08 11:01:44.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-05-08 11:01:43.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-08 11:01:43.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:01:44.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-08 11:01:44.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-08 11:01:44.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 11:01:44.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-08 11:01:44.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-08 11:01:44.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:01:44.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-08 11:01:43.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49422 2023-05-08 11:01:43.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/client.py
+-rw-r--r--   0 root         (0) root         (0)    46245 2023-05-08 11:01:43.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-08 11:01:44.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-05-08 11:01:43.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/setup.py
```

### Comparing `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/LICENSE` & `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/PKG-INFO` & `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_ee637c8293f64104af9686dc12e0cd18
-Version: 1.0.2
+Version: 1.1.0
 Summary: Ant Chain Ak_ee637c8293f64104af9686dc12e0cd18 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/README-CN.md` & `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/README.md` & `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/PKG-INFO` & `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-ee637c8293f64104af9686dc12e0cd18
-Version: 1.0.2
+Version: 1.1.0
 Summary: Ant Chain Ak_ee637c8293f64104af9686dc12e0cd18 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/SOURCES.txt` & `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/client.py` & `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.2',
+                    'sdk_version': '1.1.0',
                     '_prod_code': 'ak_ee637c8293f64104af9686dc12e0cd18',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.2',
+                    'sdk_version': '1.1.0',
                     '_prod_code': 'ak_ee637c8293f64104af9686dc12e0cd18',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/models.py` & `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/models.py`

 * *Files identical despite different names*

### Comparing `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.2/setup.py` & `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.1.0/setup.py`

 * *Files identical despite different names*

