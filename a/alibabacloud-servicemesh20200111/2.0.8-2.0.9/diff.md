# Comparing `tmp/alibabacloud_servicemesh20200111-2.0.8.tar.gz` & `tmp/alibabacloud_servicemesh20200111-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_servicemesh20200111-2.0.8.tar", last modified: Wed Mar 16 03:29:48 2022, max compression
+gzip compressed data, was "dist/alibabacloud_servicemesh20200111-2.0.9.tar", last modified: Wed Mar 16 05:47:48 2022, max compression
```

## Comparing `alibabacloud_servicemesh20200111-2.0.8.tar` & `alibabacloud_servicemesh20200111-2.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 03:29:48.000000 alibabacloud_servicemesh20200111-2.0.8/
--rw-r--r--   0 root         (0) root         (0)      992 2022-03-16 03:29:47.000000 alibabacloud_servicemesh20200111-2.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-03-16 03:29:47.000000 alibabacloud_servicemesh20200111-2.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-03-16 03:29:47.000000 alibabacloud_servicemesh20200111-2.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2391 2022-03-16 03:29:48.000000 alibabacloud_servicemesh20200111-2.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1046 2022-03-16 03:29:47.000000 alibabacloud_servicemesh20200111-2.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2022-03-16 03:29:47.000000 alibabacloud_servicemesh20200111-2.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 03:29:48.000000 alibabacloud_servicemesh20200111-2.0.8/alibabacloud_servicemesh20200111/
--rw-r--r--   0 root         (0) root         (0)       21 2022-03-16 03:29:47.000000 alibabacloud_servicemesh20200111-2.0.8/alibabacloud_servicemesh20200111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   197226 2022-03-16 03:29:47.000000 alibabacloud_servicemesh20200111-2.0.8/alibabacloud_servicemesh20200111/client.py
--rw-r--r--   0 root         (0) root         (0)   365168 2022-03-16 03:29:47.000000 alibabacloud_servicemesh20200111-2.0.8/alibabacloud_servicemesh20200111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 03:29:48.000000 alibabacloud_servicemesh20200111-2.0.8/alibabacloud_servicemesh20200111.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2391 2022-03-16 03:29:48.000000 alibabacloud_servicemesh20200111-2.0.8/alibabacloud_servicemesh20200111.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2022-03-16 03:29:48.000000 alibabacloud_servicemesh20200111-2.0.8/alibabacloud_servicemesh20200111.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-16 03:29:48.000000 alibabacloud_servicemesh20200111-2.0.8/alibabacloud_servicemesh20200111.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-03-16 03:29:48.000000 alibabacloud_servicemesh20200111-2.0.8/alibabacloud_servicemesh20200111.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2022-03-16 03:29:48.000000 alibabacloud_servicemesh20200111-2.0.8/alibabacloud_servicemesh20200111.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-03-16 03:29:48.000000 alibabacloud_servicemesh20200111-2.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2665 2022-03-16 03:29:47.000000 alibabacloud_servicemesh20200111-2.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 05:47:48.000000 alibabacloud_servicemesh20200111-2.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1042 2022-03-16 05:47:47.000000 alibabacloud_servicemesh20200111-2.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-03-16 05:47:47.000000 alibabacloud_servicemesh20200111-2.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-03-16 05:47:47.000000 alibabacloud_servicemesh20200111-2.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2391 2022-03-16 05:47:48.000000 alibabacloud_servicemesh20200111-2.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1046 2022-03-16 05:47:47.000000 alibabacloud_servicemesh20200111-2.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2022-03-16 05:47:47.000000 alibabacloud_servicemesh20200111-2.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 05:47:48.000000 alibabacloud_servicemesh20200111-2.0.9/alibabacloud_servicemesh20200111/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-03-16 05:47:47.000000 alibabacloud_servicemesh20200111-2.0.9/alibabacloud_servicemesh20200111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   194646 2022-03-16 05:47:47.000000 alibabacloud_servicemesh20200111-2.0.9/alibabacloud_servicemesh20200111/client.py
+-rw-r--r--   0 root         (0) root         (0)   362647 2022-03-16 05:47:47.000000 alibabacloud_servicemesh20200111-2.0.9/alibabacloud_servicemesh20200111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 05:47:48.000000 alibabacloud_servicemesh20200111-2.0.9/alibabacloud_servicemesh20200111.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2391 2022-03-16 05:47:47.000000 alibabacloud_servicemesh20200111-2.0.9/alibabacloud_servicemesh20200111.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2022-03-16 05:47:48.000000 alibabacloud_servicemesh20200111-2.0.9/alibabacloud_servicemesh20200111.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-16 05:47:47.000000 alibabacloud_servicemesh20200111-2.0.9/alibabacloud_servicemesh20200111.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-03-16 05:47:47.000000 alibabacloud_servicemesh20200111-2.0.9/alibabacloud_servicemesh20200111.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2022-03-16 05:47:47.000000 alibabacloud_servicemesh20200111-2.0.9/alibabacloud_servicemesh20200111.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-03-16 05:47:48.000000 alibabacloud_servicemesh20200111-2.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2665 2022-03-16 05:47:47.000000 alibabacloud_servicemesh20200111-2.0.9/setup.py
```

### Comparing `alibabacloud_servicemesh20200111-2.0.8/ChangeLog.md` & `alibabacloud_servicemesh20200111-2.0.9/ChangeLog.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2022-03-16 Version: 2.0.8
+- New build from amp.
+
+
 2022-02-22 Version: 2.0.7
 - New build from amp.
 
 
 2022-02-17 Version: 2.0.6
 - New build from amp.
```

### Comparing `alibabacloud_servicemesh20200111-2.0.8/LICENSE` & `alibabacloud_servicemesh20200111-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_servicemesh20200111-2.0.8/PKG-INFO` & `alibabacloud_servicemesh20200111-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_servicemesh20200111
-Version: 2.0.8
+Version: 2.0.9
 Summary: Alibaba Cloud Alibaba Cloud Service Mesh (20200111) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_servicemesh20200111-2.0.8/README-CN.md` & `alibabacloud_servicemesh20200111-2.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_servicemesh20200111-2.0.8/README.md` & `alibabacloud_servicemesh20200111-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_servicemesh20200111-2.0.8/alibabacloud_servicemesh20200111/client.py` & `alibabacloud_servicemesh20200111-2.0.9/alibabacloud_servicemesh20200111/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -3601,84 +3601,14 @@
     async def revoke_kubeconfig_async(
         self,
         request: servicemesh_20200111_models.RevokeKubeconfigRequest,
     ) -> servicemesh_20200111_models.RevokeKubeconfigResponse:
         runtime = util_models.RuntimeOptions()
         return await self.revoke_kubeconfig_with_options_async(request, runtime)
 
-    def run_diagnosis_with_options(
-        self,
-        request: servicemesh_20200111_models.RunDiagnosisRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> servicemesh_20200111_models.RunDiagnosisResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.service_mesh_id):
-            body['ServiceMeshId'] = request.service_mesh_id
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RunDiagnosis',
-            version='2020-01-11',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            servicemesh_20200111_models.RunDiagnosisResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def run_diagnosis_with_options_async(
-        self,
-        request: servicemesh_20200111_models.RunDiagnosisRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> servicemesh_20200111_models.RunDiagnosisResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.service_mesh_id):
-            body['ServiceMeshId'] = request.service_mesh_id
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RunDiagnosis',
-            version='2020-01-11',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            servicemesh_20200111_models.RunDiagnosisResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def run_diagnosis(
-        self,
-        request: servicemesh_20200111_models.RunDiagnosisRequest,
-    ) -> servicemesh_20200111_models.RunDiagnosisResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.run_diagnosis_with_options(request, runtime)
-
-    async def run_diagnosis_async(
-        self,
-        request: servicemesh_20200111_models.RunDiagnosisRequest,
-    ) -> servicemesh_20200111_models.RunDiagnosisResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.run_diagnosis_with_options_async(request, runtime)
-
     def update_asmgateway_with_options(
         self,
         request: servicemesh_20200111_models.UpdateASMGatewayRequest,
         runtime: util_models.RuntimeOptions,
     ) -> servicemesh_20200111_models.UpdateASMGatewayResponse:
         UtilClient.validate_model(request)
         body = {}
```

### Comparing `alibabacloud_servicemesh20200111-2.0.8/alibabacloud_servicemesh20200111/models.py` & `alibabacloud_servicemesh20200111-2.0.9/alibabacloud_servicemesh20200111/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -19682,3142 +19682,2985 @@
 0004ce10: 6c20 3d20 5265 766f 6b65 4b75 6265 636f  l = RevokeKubeco
 0004ce20: 6e66 6967 5265 7370 6f6e 7365 426f 6479  nfigResponseBody
 0004ce30: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
 0004ce40: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
 0004ce50: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
 0004ce60: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
 0004ce70: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-0004ce80: 636c 6173 7320 5275 6e44 6961 676e 6f73  class RunDiagnos
-0004ce90: 6973 5265 7175 6573 7428 5465 614d 6f64  isRequest(TeaMod
-0004cea0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-0004ceb0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-0004cec0: 656c 662c 0a20 2020 2020 2020 2073 6572  elf,.        ser
-0004ced0: 7669 6365 5f6d 6573 685f 6964 3a20 7374  vice_mesh_id: st
-0004cee0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 293a  r = None,.    ):
-0004cef0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0004cf00: 7276 6963 655f 6d65 7368 5f69 6420 3d20  rvice_mesh_id = 
-0004cf10: 7365 7276 6963 655f 6d65 7368 5f69 640a  service_mesh_id.
-0004cf20: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-0004cf30: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-0004cf40: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
-0004cf50: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-0004cf60: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-0004cf70: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-0004cf80: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-0004cf90: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0004cfa0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-0004cfb0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-0004cfc0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-0004cfd0: 2020 2069 6620 7365 6c66 2e73 6572 7669     if self.servi
-0004cfe0: 6365 5f6d 6573 685f 6964 2069 7320 6e6f  ce_mesh_id is no
-0004cff0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0004d000: 2020 2020 7265 7375 6c74 5b27 5365 7276      result['Serv
-0004d010: 6963 654d 6573 6849 6427 5d20 3d20 7365  iceMeshId'] = se
-0004d020: 6c66 2e73 6572 7669 6365 5f6d 6573 685f  lf.service_mesh_
-0004d030: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
-0004d040: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-0004d050: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-0004d060: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-0004d070: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-0004d080: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-0004d090: 2020 6966 206d 2e67 6574 2827 5365 7276    if m.get('Serv
-0004d0a0: 6963 654d 6573 6849 6427 2920 6973 206e  iceMeshId') is n
-0004d0b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0004d0c0: 2020 2020 2073 656c 662e 7365 7276 6963       self.servic
-0004d0d0: 655f 6d65 7368 5f69 6420 3d20 6d2e 6765  e_mesh_id = m.ge
-0004d0e0: 7428 2753 6572 7669 6365 4d65 7368 4964  t('ServiceMeshId
-0004d0f0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-0004d100: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2052  n self...class R
-0004d110: 756e 4469 6167 6e6f 7369 7352 6573 706f  unDiagnosisRespo
-0004d120: 6e73 6542 6f64 7928 5465 614d 6f64 656c  nseBody(TeaModel
-0004d130: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-0004d140: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-0004d150: 662c 0a20 2020 2020 2020 2072 6571 7565  f,.        reque
-0004d160: 7374 5f69 643a 2073 7472 203d 204e 6f6e  st_id: str = Non
-0004d170: 652c 0a20 2020 2020 2020 2072 6573 756c  e,.        resul
-0004d180: 743a 2073 7472 203d 204e 6f6e 652c 0a20  t: str = None,. 
-0004d190: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-0004d1a0: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-0004d1b0: 7265 7175 6573 745f 6964 0a20 2020 2020  request_id.     
-0004d1c0: 2020 2073 656c 662e 7265 7375 6c74 203d     self.result =
-0004d1d0: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
-0004d1e0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-0004d1f0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-0004d200: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-0004d210: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-0004d220: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-0004d230: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-0004d240: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-0004d250: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0004d260: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-0004d270: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-0004d280: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0004d290: 6c66 2e72 6571 7565 7374 5f69 6420 6973  lf.request_id is
-0004d2a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0004d2b0: 2020 2020 2020 2072 6573 756c 745b 2752         result['R
-0004d2c0: 6571 7565 7374 4964 275d 203d 2073 656c  equestId'] = sel
-0004d2d0: 662e 7265 7175 6573 745f 6964 0a20 2020  f.request_id.   
-0004d2e0: 2020 2020 2069 6620 7365 6c66 2e72 6573       if self.res
-0004d2f0: 756c 7420 6973 206e 6f74 204e 6f6e 653a  ult is not None:
-0004d300: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0004d310: 756c 745b 2752 6573 756c 7427 5d20 3d20  ult['Result'] = 
-0004d320: 7365 6c66 2e72 6573 756c 740a 2020 2020  self.result.    
-0004d330: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-0004d340: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-0004d350: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-0004d360: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-0004d370: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-0004d380: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-0004d390: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
-0004d3a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0004d3b0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0004d3c0: 6571 7565 7374 5f69 6420 3d20 6d2e 6765  equest_id = m.ge
-0004d3d0: 7428 2752 6571 7565 7374 4964 2729 0a20  t('RequestId'). 
-0004d3e0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0004d3f0: 2752 6573 756c 7427 2920 6973 206e 6f74  'Result') is not
-0004d400: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0004d410: 2020 2073 656c 662e 7265 7375 6c74 203d     self.result =
-0004d420: 206d 2e67 6574 2827 5265 7375 6c74 2729   m.get('Result')
-0004d430: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0004d440: 7365 6c66 0a0a 0a63 6c61 7373 2052 756e  self...class Run
-0004d450: 4469 6167 6e6f 7369 7352 6573 706f 6e73  DiagnosisRespons
-0004d460: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
-0004d470: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-0004d480: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0004d490: 2020 2020 2068 6561 6465 7273 3a20 4469       headers: Di
-0004d4a0: 6374 5b73 7472 2c20 7374 725d 203d 204e  ct[str, str] = N
-0004d4b0: 6f6e 652c 0a20 2020 2020 2020 2062 6f64  one,.        bod
-0004d4c0: 793a 2052 756e 4469 6167 6e6f 7369 7352  y: RunDiagnosisR
-0004d4d0: 6573 706f 6e73 6542 6f64 7920 3d20 4e6f  esponseBody = No
-0004d4e0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-0004d4f0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-0004d500: 3d20 6865 6164 6572 730a 2020 2020 2020  = headers.      
-0004d510: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
-0004d520: 6479 0a0a 2020 2020 6465 6620 7661 6c69  dy..    def vali
-0004d530: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-0004d540: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
-0004d550: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
-0004d560: 6865 6164 6572 732c 2027 6865 6164 6572  headers, 'header
-0004d570: 7327 290a 2020 2020 2020 2020 7365 6c66  s').        self
-0004d580: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
-0004d590: 6564 2873 656c 662e 626f 6479 2c20 2762  ed(self.body, 'b
-0004d5a0: 6f64 7927 290a 2020 2020 2020 2020 6966  ody').        if
-0004d5b0: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
-0004d5c0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-0004d5d0: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
-0004d5e0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-0004d5f0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-0004d600: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-0004d610: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-0004d620: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-0004d630: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0004d640: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-0004d650: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-0004d660: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0004d670: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
-0004d680: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0004d690: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
-0004d6a0: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
-0004d6b0: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
-0004d6c0: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
-0004d6d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0004d6e0: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
-0004d6f0: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
-0004d700: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
-0004d710: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-0004d720: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-0004d730: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
-0004d740: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-0004d750: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-0004d760: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
-0004d770: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
-0004d780: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0004d790: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
-0004d7a0: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-0004d7b0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0004d7c0: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
-0004d7d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0004d7e0: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
-0004d7f0: 2052 756e 4469 6167 6e6f 7369 7352 6573   RunDiagnosisRes
-0004d800: 706f 6e73 6542 6f64 7928 290a 2020 2020  ponseBody().    
-0004d810: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-0004d820: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
-0004d830: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
-0004d840: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
-0004d850: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2055  n self...class U
-0004d860: 7064 6174 6541 534d 4761 7465 7761 7952  pdateASMGatewayR
-0004d870: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
-0004d880: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0004d890: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-0004d8a0: 2c0a 2020 2020 2020 2020 626f 6479 3a20  ,.        body: 
-0004d8b0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-0004d8c0: 2020 2020 6973 7469 6f5f 6761 7465 7761      istio_gatewa
-0004d8d0: 795f 6e61 6d65 3a20 7374 7220 3d20 4e6f  y_name: str = No
-0004d8e0: 6e65 2c0a 2020 2020 2020 2020 7365 7276  ne,.        serv
-0004d8f0: 6963 655f 6d65 7368 5f69 643a 2073 7472  ice_mesh_id: str
-0004d900: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-0004d910: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-0004d920: 7920 3d20 626f 6479 0a20 2020 2020 2020  y = body.       
-0004d930: 2073 656c 662e 6973 7469 6f5f 6761 7465   self.istio_gate
-0004d940: 7761 795f 6e61 6d65 203d 2069 7374 696f  way_name = istio
-0004d950: 5f67 6174 6577 6179 5f6e 616d 650a 2020  _gateway_name.  
-0004d960: 2020 2020 2020 7365 6c66 2e73 6572 7669        self.servi
-0004d970: 6365 5f6d 6573 685f 6964 203d 2073 6572  ce_mesh_id = ser
-0004d980: 7669 6365 5f6d 6573 685f 6964 0a0a 2020  vice_mesh_id..  
-0004d990: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-0004d9a0: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-0004d9b0: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
-0004d9c0: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-0004d9d0: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
-0004d9e0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0004d9f0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-0004da00: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0004da10: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-0004da20: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0004da30: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0004da40: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
-0004da50: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0004da60: 2020 2020 2020 7265 7375 6c74 5b27 426f        result['Bo
-0004da70: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
-0004da80: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0004da90: 2e69 7374 696f 5f67 6174 6577 6179 5f6e  .istio_gateway_n
-0004daa0: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
-0004dab0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0004dac0: 756c 745b 2749 7374 696f 4761 7465 7761  ult['IstioGatewa
-0004dad0: 794e 616d 6527 5d20 3d20 7365 6c66 2e69  yName'] = self.i
-0004dae0: 7374 696f 5f67 6174 6577 6179 5f6e 616d  stio_gateway_nam
-0004daf0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-0004db00: 662e 7365 7276 6963 655f 6d65 7368 5f69  f.service_mesh_i
-0004db10: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-0004db20: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0004db30: 745b 2753 6572 7669 6365 4d65 7368 4964  t['ServiceMeshId
-0004db40: 275d 203d 2073 656c 662e 7365 7276 6963  '] = self.servic
-0004db50: 655f 6d65 7368 5f69 640a 2020 2020 2020  e_mesh_id.      
-0004db60: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-0004db70: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-0004db80: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
-0004db90: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-0004dba0: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-0004dbb0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0004dbc0: 7428 2742 6f64 7927 2920 6973 206e 6f74  t('Body') is not
-0004dbd0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0004dbe0: 2020 2073 656c 662e 626f 6479 203d 206d     self.body = m
-0004dbf0: 2e67 6574 2827 426f 6479 2729 0a20 2020  .get('Body').   
-0004dc00: 2020 2020 2069 6620 6d2e 6765 7428 2749       if m.get('I
-0004dc10: 7374 696f 4761 7465 7761 794e 616d 6527  stioGatewayName'
-0004dc20: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0004dc30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0004dc40: 6973 7469 6f5f 6761 7465 7761 795f 6e61  istio_gateway_na
-0004dc50: 6d65 203d 206d 2e67 6574 2827 4973 7469  me = m.get('Isti
-0004dc60: 6f47 6174 6577 6179 4e61 6d65 2729 0a20  oGatewayName'). 
-0004dc70: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0004dc80: 2753 6572 7669 6365 4d65 7368 4964 2729  'ServiceMeshId')
-0004dc90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0004dca0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0004dcb0: 6572 7669 6365 5f6d 6573 685f 6964 203d  ervice_mesh_id =
-0004dcc0: 206d 2e67 6574 2827 5365 7276 6963 654d   m.get('ServiceM
-0004dcd0: 6573 6849 6427 290a 2020 2020 2020 2020  eshId').        
-0004dce0: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-0004dcf0: 6173 7320 5570 6461 7465 4153 4d47 6174  ass UpdateASMGat
-0004dd00: 6577 6179 5265 7370 6f6e 7365 426f 6479  ewayResponseBody
-0004dd10: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-0004dd20: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-0004dd30: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0004dd40: 2020 2020 7265 7175 6573 745f 6964 3a20      request_id: 
-0004dd50: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-0004dd60: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-0004dd70: 7265 7175 6573 745f 6964 203d 2072 6571  request_id = req
-0004dd80: 7565 7374 5f69 640a 0a20 2020 2064 6566  uest_id..    def
-0004dd90: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-0004dda0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-0004ddb0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-0004ddc0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-0004ddd0: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-0004dde0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-0004ddf0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-0004de00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0004de10: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-0004de20: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-0004de30: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0004de40: 6c66 2e72 6571 7565 7374 5f69 6420 6973  lf.request_id is
-0004de50: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0004de60: 2020 2020 2020 2072 6573 756c 745b 2752         result['R
-0004de70: 6571 7565 7374 4964 275d 203d 2073 656c  equestId'] = sel
-0004de80: 662e 7265 7175 6573 745f 6964 0a20 2020  f.request_id.   
-0004de90: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-0004dea0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-0004deb0: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
-0004dec0: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
-0004ded0: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-0004dee0: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-0004def0: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
-0004df00: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0004df10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0004df20: 7265 7175 6573 745f 6964 203d 206d 2e67  request_id = m.g
-0004df30: 6574 2827 5265 7175 6573 7449 6427 290a  et('RequestId').
-0004df40: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0004df50: 656c 660a 0a0a 636c 6173 7320 5570 6461  elf...class Upda
-0004df60: 7465 4153 4d47 6174 6577 6179 5265 7370  teASMGatewayResp
-0004df70: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
-0004df80: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0004df90: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-0004dfa0: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
-0004dfb0: 2044 6963 745b 7374 722c 2073 7472 5d20   Dict[str, str] 
-0004dfc0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0004dfd0: 626f 6479 3a20 5570 6461 7465 4153 4d47  body: UpdateASMG
-0004dfe0: 6174 6577 6179 5265 7370 6f6e 7365 426f  atewayResponseBo
-0004dff0: 6479 203d 204e 6f6e 652c 0a20 2020 2029  dy = None,.    )
-0004e000: 3a0a 2020 2020 2020 2020 7365 6c66 2e68  :.        self.h
-0004e010: 6561 6465 7273 203d 2068 6561 6465 7273  eaders = headers
-0004e020: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
-0004e030: 6479 203d 2062 6f64 790a 0a20 2020 2064  dy = body..    d
-0004e040: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-0004e050: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-0004e060: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
-0004e070: 6428 7365 6c66 2e68 6561 6465 7273 2c20  d(self.headers, 
-0004e080: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
-0004e090: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
-0004e0a0: 5f72 6571 7569 7265 6428 7365 6c66 2e62  _required(self.b
-0004e0b0: 6f64 792c 2027 626f 6479 2729 0a20 2020  ody, 'body').   
-0004e0c0: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-0004e0d0: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-0004e0e0: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
-0004e0f0: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
-0004e100: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-0004e110: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-0004e120: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-0004e130: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-0004e140: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0004e150: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-0004e160: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0004e170: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0004e180: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
-0004e190: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0004e1a0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0004e1b0: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
-0004e1c0: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
-0004e1d0: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
-0004e1e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0004e1f0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0004e200: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
-0004e210: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
-0004e220: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-0004e230: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-0004e240: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
-0004e250: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
-0004e260: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-0004e270: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-0004e280: 2e67 6574 2827 6865 6164 6572 7327 2920  .get('headers') 
-0004e290: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0004e2a0: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
-0004e2b0: 6164 6572 7320 3d20 6d2e 6765 7428 2768  aders = m.get('h
-0004e2c0: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
-0004e2d0: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
-0004e2e0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0004e2f0: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-0004e300: 6d6f 6465 6c20 3d20 5570 6461 7465 4153  model = UpdateAS
-0004e310: 4d47 6174 6577 6179 5265 7370 6f6e 7365  MGatewayResponse
-0004e320: 426f 6479 2829 0a20 2020 2020 2020 2020  Body().         
-0004e330: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
-0004e340: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
-0004e350: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
-0004e360: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0004e370: 660a 0a0a 636c 6173 7320 5570 6461 7465  f...class Update
-0004e380: 4153 4d47 6174 6577 6179 496d 706f 7274  ASMGatewayImport
-0004e390: 6564 5365 7276 6963 6573 5265 7175 6573  edServicesReques
-0004e3a0: 7428 5465 614d 6f64 656c 293a 0a20 2020  t(TeaModel):.   
-0004e3b0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-0004e3c0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0004e3d0: 2020 2020 2061 736d 6761 7465 7761 795f       asmgateway_
-0004e3e0: 6e61 6d65 3a20 7374 7220 3d20 4e6f 6e65  name: str = None
-0004e3f0: 2c0a 2020 2020 2020 2020 7365 7276 6963  ,.        servic
-0004e400: 655f 6d65 7368 5f69 643a 2073 7472 203d  e_mesh_id: str =
-0004e410: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
-0004e420: 6572 7669 6365 5f6e 616d 6573 3a20 7374  ervice_names: st
-0004e430: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-0004e440: 2020 7365 7276 6963 655f 6e61 6d65 7370    service_namesp
-0004e450: 6163 653a 2073 7472 203d 204e 6f6e 652c  ace: str = None,
-0004e460: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-0004e470: 7365 6c66 2e61 736d 6761 7465 7761 795f  self.asmgateway_
-0004e480: 6e61 6d65 203d 2061 736d 6761 7465 7761  name = asmgatewa
-0004e490: 795f 6e61 6d65 0a20 2020 2020 2020 2073  y_name.        s
-0004e4a0: 656c 662e 7365 7276 6963 655f 6d65 7368  elf.service_mesh
-0004e4b0: 5f69 6420 3d20 7365 7276 6963 655f 6d65  _id = service_me
-0004e4c0: 7368 5f69 640a 2020 2020 2020 2020 7365  sh_id.        se
-0004e4d0: 6c66 2e73 6572 7669 6365 5f6e 616d 6573  lf.service_names
-0004e4e0: 203d 2073 6572 7669 6365 5f6e 616d 6573   = service_names
-0004e4f0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0004e500: 7276 6963 655f 6e61 6d65 7370 6163 6520  rvice_namespace 
-0004e510: 3d20 7365 7276 6963 655f 6e61 6d65 7370  = service_namesp
-0004e520: 6163 650a 0a20 2020 2064 6566 2076 616c  ace..    def val
-0004e530: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-0004e540: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-0004e550: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-0004e560: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-0004e570: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-0004e580: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-0004e590: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0004e5a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0004e5b0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-0004e5c0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-0004e5d0: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
-0004e5e0: 736d 6761 7465 7761 795f 6e61 6d65 2069  smgateway_name i
-0004e5f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0004e600: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0004e610: 4153 4d47 6174 6577 6179 4e61 6d65 275d  ASMGatewayName']
-0004e620: 203d 2073 656c 662e 6173 6d67 6174 6577   = self.asmgatew
-0004e630: 6179 5f6e 616d 650a 2020 2020 2020 2020  ay_name.        
-0004e640: 6966 2073 656c 662e 7365 7276 6963 655f  if self.service_
-0004e650: 6d65 7368 5f69 6420 6973 206e 6f74 204e  mesh_id is not N
-0004e660: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0004e670: 2072 6573 756c 745b 2753 6572 7669 6365   result['Service
-0004e680: 4d65 7368 4964 275d 203d 2073 656c 662e  MeshId'] = self.
-0004e690: 7365 7276 6963 655f 6d65 7368 5f69 640a  service_mesh_id.
-0004e6a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0004e6b0: 7365 7276 6963 655f 6e61 6d65 7320 6973  service_names is
-0004e6c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0004e6d0: 2020 2020 2020 2072 6573 756c 745b 2753         result['S
-0004e6e0: 6572 7669 6365 4e61 6d65 7327 5d20 3d20  erviceNames'] = 
-0004e6f0: 7365 6c66 2e73 6572 7669 6365 5f6e 616d  self.service_nam
-0004e700: 6573 0a20 2020 2020 2020 2069 6620 7365  es.        if se
-0004e710: 6c66 2e73 6572 7669 6365 5f6e 616d 6573  lf.service_names
-0004e720: 7061 6365 2069 7320 6e6f 7420 4e6f 6e65  pace is not None
-0004e730: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0004e740: 7375 6c74 5b27 5365 7276 6963 654e 616d  sult['ServiceNam
-0004e750: 6573 7061 6365 275d 203d 2073 656c 662e  espace'] = self.
-0004e760: 7365 7276 6963 655f 6e61 6d65 7370 6163  service_namespac
-0004e770: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-0004e780: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
-0004e790: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
-0004e7a0: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
-0004e7b0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-0004e7c0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-0004e7d0: 2069 6620 6d2e 6765 7428 2741 534d 4761   if m.get('ASMGa
-0004e7e0: 7465 7761 794e 616d 6527 2920 6973 206e  tewayName') is n
-0004e7f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0004e800: 2020 2020 2073 656c 662e 6173 6d67 6174       self.asmgat
-0004e810: 6577 6179 5f6e 616d 6520 3d20 6d2e 6765  eway_name = m.ge
-0004e820: 7428 2741 534d 4761 7465 7761 794e 616d  t('ASMGatewayNam
-0004e830: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
-0004e840: 2e67 6574 2827 5365 7276 6963 654d 6573  .get('ServiceMes
-0004e850: 6849 6427 2920 6973 206e 6f74 204e 6f6e  hId') is not Non
-0004e860: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0004e870: 656c 662e 7365 7276 6963 655f 6d65 7368  elf.service_mesh
-0004e880: 5f69 6420 3d20 6d2e 6765 7428 2753 6572  _id = m.get('Ser
-0004e890: 7669 6365 4d65 7368 4964 2729 0a20 2020  viceMeshId').   
-0004e8a0: 2020 2020 2069 6620 6d2e 6765 7428 2753       if m.get('S
-0004e8b0: 6572 7669 6365 4e61 6d65 7327 2920 6973  erviceNames') is
-0004e8c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0004e8d0: 2020 2020 2020 2073 656c 662e 7365 7276         self.serv
-0004e8e0: 6963 655f 6e61 6d65 7320 3d20 6d2e 6765  ice_names = m.ge
-0004e8f0: 7428 2753 6572 7669 6365 4e61 6d65 7327  t('ServiceNames'
-0004e900: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0004e910: 6574 2827 5365 7276 6963 654e 616d 6573  et('ServiceNames
-0004e920: 7061 6365 2729 2069 7320 6e6f 7420 4e6f  pace') is not No
-0004e930: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0004e940: 7365 6c66 2e73 6572 7669 6365 5f6e 616d  self.service_nam
-0004e950: 6573 7061 6365 203d 206d 2e67 6574 2827  espace = m.get('
-0004e960: 5365 7276 6963 654e 616d 6573 7061 6365  ServiceNamespace
-0004e970: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-0004e980: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2055  n self...class U
-0004e990: 7064 6174 6541 534d 4761 7465 7761 7949  pdateASMGatewayI
-0004e9a0: 6d70 6f72 7465 6453 6572 7669 6365 7352  mportedServicesR
-0004e9b0: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
-0004e9c0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-0004e9d0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-0004e9e0: 2073 656c 662c 0a20 2020 2020 2020 2072   self,.        r
-0004e9f0: 6571 7565 7374 5f69 643a 2073 7472 203d  equest_id: str =
-0004ea00: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-0004ea10: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
-0004ea20: 7374 5f69 6420 3d20 7265 7175 6573 745f  st_id = request_
-0004ea30: 6964 0a0a 2020 2020 6465 6620 7661 6c69  id..    def vali
-0004ea40: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-0004ea50: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-0004ea60: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-0004ea70: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-0004ea80: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
-0004ea90: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-0004eaa0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0004eab0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0004eac0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-0004ead0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-0004eae0: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
-0004eaf0: 7175 6573 745f 6964 2069 7320 6e6f 7420  quest_id is not 
-0004eb00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0004eb10: 2020 7265 7375 6c74 5b27 5265 7175 6573    result['Reques
-0004eb20: 7449 6427 5d20 3d20 7365 6c66 2e72 6571  tId'] = self.req
-0004eb30: 7565 7374 5f69 640a 2020 2020 2020 2020  uest_id.        
-0004eb40: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-0004eb50: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-0004eb60: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-0004eb70: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-0004eb80: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-0004eb90: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0004eba0: 2752 6571 7565 7374 4964 2729 2069 7320  'RequestId') is 
-0004ebb0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0004ebc0: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
-0004ebd0: 7374 5f69 6420 3d20 6d2e 6765 7428 2752  st_id = m.get('R
-0004ebe0: 6571 7565 7374 4964 2729 0a20 2020 2020  equestId').     
-0004ebf0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-0004ec00: 0a63 6c61 7373 2055 7064 6174 6541 534d  .class UpdateASM
-0004ec10: 4761 7465 7761 7949 6d70 6f72 7465 6453  GatewayImportedS
-0004ec20: 6572 7669 6365 7352 6573 706f 6e73 6528  ervicesResponse(
-0004ec30: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-0004ec40: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-0004ec50: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0004ec60: 2020 2068 6561 6465 7273 3a20 4469 6374     headers: Dict
-0004ec70: 5b73 7472 2c20 7374 725d 203d 204e 6f6e  [str, str] = Non
-0004ec80: 652c 0a20 2020 2020 2020 2062 6f64 793a  e,.        body:
-0004ec90: 2055 7064 6174 6541 534d 4761 7465 7761   UpdateASMGatewa
-0004eca0: 7949 6d70 6f72 7465 6453 6572 7669 6365  yImportedService
-0004ecb0: 7352 6573 706f 6e73 6542 6f64 7920 3d20  sResponseBody = 
-0004ecc0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-0004ecd0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-0004ece0: 7320 3d20 6865 6164 6572 730a 2020 2020  s = headers.    
-0004ecf0: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-0004ed00: 626f 6479 0a0a 2020 2020 6465 6620 7661  body..    def va
-0004ed10: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-0004ed20: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
-0004ed30: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
-0004ed40: 662e 6865 6164 6572 732c 2027 6865 6164  f.headers, 'head
-0004ed50: 6572 7327 290a 2020 2020 2020 2020 7365  ers').        se
-0004ed60: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
-0004ed70: 6972 6564 2873 656c 662e 626f 6479 2c20  ired(self.body, 
-0004ed80: 2762 6f64 7927 290a 2020 2020 2020 2020  'body').        
-0004ed90: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
-0004eda0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-0004edb0: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
-0004edc0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-0004edd0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-0004ede0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-0004edf0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-0004ee00: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-0004ee10: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0004ee20: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-0004ee30: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-0004ee40: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-0004ee50: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
-0004ee60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0004ee70: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
-0004ee80: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
-0004ee90: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
-0004eea0: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
-0004eeb0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0004eec0: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
-0004eed0: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
-0004eee0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-0004eef0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-0004ef00: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-0004ef10: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-0004ef20: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-0004ef30: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-0004ef40: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0004ef50: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
-0004ef60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0004ef70: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-0004ef80: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
-0004ef90: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
-0004efa0: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
-0004efb0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0004efc0: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
-0004efd0: 203d 2055 7064 6174 6541 534d 4761 7465   = UpdateASMGate
-0004efe0: 7761 7949 6d70 6f72 7465 6453 6572 7669  wayImportedServi
-0004eff0: 6365 7352 6573 706f 6e73 6542 6f64 7928  cesResponseBody(
-0004f000: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0004f010: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
-0004f020: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
-0004f030: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
-0004f040: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-0004f050: 6c61 7373 2055 7064 6174 654d 6573 6846  lass UpdateMeshF
-0004f060: 6561 7475 7265 5265 7175 6573 7428 5465  eatureRequest(Te
-0004f070: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-0004f080: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-0004f090: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0004f0a0: 2061 6363 6573 735f 6c6f 675f 656e 6162   access_log_enab
-0004f0b0: 6c65 643a 2062 6f6f 6c20 3d20 4e6f 6e65  led: bool = None
-0004f0c0: 2c0a 2020 2020 2020 2020 6163 6365 7373  ,.        access
-0004f0d0: 5f6c 6f67 5f66 696c 653a 2073 7472 203d  _log_file: str =
-0004f0e0: 204e 6f6e 652c 0a20 2020 2020 2020 2061   None,.        a
-0004f0f0: 6363 6573 735f 6c6f 675f 666f 726d 6174  ccess_log_format
-0004f100: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-0004f110: 2020 2020 2020 6163 6365 7373 5f6c 6f67        access_log
-0004f120: 5f70 726f 6a65 6374 3a20 7374 7220 3d20  _project: str = 
-0004f130: 4e6f 6e65 2c0a 2020 2020 2020 2020 6163  None,.        ac
-0004f140: 6365 7373 5f6c 6f67 5f73 6572 7669 6365  cess_log_service
-0004f150: 5f65 6e61 626c 6564 3a20 626f 6f6c 203d  _enabled: bool =
-0004f160: 204e 6f6e 652c 0a20 2020 2020 2020 2061   None,.        a
-0004f170: 6363 6573 735f 6c6f 675f 7365 7276 6963  ccess_log_servic
-0004f180: 655f 686f 7374 3a20 7374 7220 3d20 4e6f  e_host: str = No
-0004f190: 6e65 2c0a 2020 2020 2020 2020 6163 6365  ne,.        acce
-0004f1a0: 7373 5f6c 6f67 5f73 6572 7669 6365 5f70  ss_log_service_p
-0004f1b0: 6f72 743a 2069 6e74 203d 204e 6f6e 652c  ort: int = None,
-0004f1c0: 0a20 2020 2020 2020 2061 7564 6974 5f70  .        audit_p
-0004f1d0: 726f 6a65 6374 3a20 7374 7220 3d20 4e6f  roject: str = No
-0004f1e0: 6e65 2c0a 2020 2020 2020 2020 6175 746f  ne,.        auto
-0004f1f0: 5f69 6e6a 6563 7469 6f6e 5f70 6f6c 6963  _injection_polic
-0004f200: 795f 656e 6162 6c65 643a 2062 6f6f 6c20  y_enabled: bool 
-0004f210: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0004f220: 6372 6167 6772 6567 6174 696f 6e5f 656e  craggregation_en
-0004f230: 6162 6c65 643a 2062 6f6f 6c20 3d20 4e6f  abled: bool = No
-0004f240: 6e65 2c0a 2020 2020 2020 2020 636c 7573  ne,.        clus
-0004f250: 7465 725f 7370 6563 3a20 7374 7220 3d20  ter_spec: str = 
-0004f260: 4e6f 6e65 2c0a 2020 2020 2020 2020 636e  None,.        cn
-0004f270: 695f 656e 6162 6c65 643a 2062 6f6f 6c20  i_enabled: bool 
-0004f280: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0004f290: 636e 695f 6578 636c 7564 655f 6e61 6d65  cni_exclude_name
-0004f2a0: 7370 6163 6573 3a20 7374 7220 3d20 4e6f  spaces: str = No
-0004f2b0: 6e65 2c0a 2020 2020 2020 2020 636f 6e66  ne,.        conf
-0004f2c0: 6967 5f73 6f75 7263 655f 656e 6162 6c65  ig_source_enable
-0004f2d0: 643a 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a  d: bool = None,.
-0004f2e0: 2020 2020 2020 2020 636f 6e66 6967 5f73          config_s
-0004f2f0: 6f75 7263 655f 6e61 636f 735f 6964 3a20  ource_nacos_id: 
-0004f300: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-0004f310: 2020 2020 6375 7374 6f6d 697a 6564 5f70      customized_p
-0004f320: 726f 6d65 7468 6575 733a 2062 6f6f 6c20  rometheus: bool 
-0004f330: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0004f340: 6375 7374 6f6d 697a 6564 5f7a 6970 6b69  customized_zipki
-0004f350: 6e3a 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a  n: bool = None,.
-0004f360: 2020 2020 2020 2020 646e 7370 726f 7879          dnsproxy
-0004f370: 696e 675f 656e 6162 6c65 643a 2062 6f6f  ing_enabled: boo
-0004f380: 6c20 3d20 4e6f 6e65 2c0a 2020 2020 2020  l = None,.      
-0004f390: 2020 6469 7363 6f76 6572 795f 7365 6c65    discovery_sele
-0004f3a0: 6374 6f72 733a 2073 7472 203d 204e 6f6e  ctors: str = Non
-0004f3b0: 652c 0a20 2020 2020 2020 2064 7562 626f  e,.        dubbo
-0004f3c0: 5f66 696c 7465 725f 656e 6162 6c65 643a  _filter_enabled:
-0004f3d0: 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020   bool = None,.  
-0004f3e0: 2020 2020 2020 656e 6162 6c65 5f61 7564        enable_aud
-0004f3f0: 6974 3a20 626f 6f6c 203d 204e 6f6e 652c  it: bool = None,
-0004f400: 0a20 2020 2020 2020 2065 6e61 626c 655f  .        enable_
-0004f410: 6372 6869 7374 6f72 793a 2062 6f6f 6c20  crhistory: bool 
-0004f420: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0004f430: 656e 6162 6c65 5f6e 616d 6573 7061 6365  enable_namespace
-0004f440: 735f 6279 5f64 6566 6175 6c74 3a20 626f  s_by_default: bo
-0004f450: 6f6c 203d 204e 6f6e 652c 0a20 2020 2020  ol = None,.     
-0004f460: 2020 2065 6e61 626c 655f 7364 7373 6572     enable_sdsser
-0004f470: 7665 723a 2062 6f6f 6c20 3d20 4e6f 6e65  ver: bool = None
-0004f480: 2c0a 2020 2020 2020 2020 6578 636c 7564  ,.        exclud
-0004f490: 655f 6970 7261 6e67 6573 3a20 7374 7220  e_ipranges: str 
-0004f4a0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0004f4b0: 6578 636c 7564 655f 696e 626f 756e 645f  exclude_inbound_
-0004f4c0: 706f 7274 733a 2073 7472 203d 204e 6f6e  ports: str = Non
-0004f4d0: 652c 0a20 2020 2020 2020 2065 7863 6c75  e,.        exclu
-0004f4e0: 6465 5f6f 7574 626f 756e 645f 706f 7274  de_outbound_port
-0004f4f0: 733a 2073 7472 203d 204e 6f6e 652c 0a20  s: str = None,. 
-0004f500: 2020 2020 2020 2066 696c 7465 725f 6761         filter_ga
-0004f510: 7465 7761 795f 636c 7573 7465 725f 636f  teway_cluster_co
-0004f520: 6e66 6967 3a20 626f 6f6c 203d 204e 6f6e  nfig: bool = Non
-0004f530: 652c 0a20 2020 2020 2020 2067 6174 6577  e,.        gatew
-0004f540: 6179 5f61 7069 656e 6162 6c65 643a 2062  ay_apienabled: b
-0004f550: 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020 2020  ool = None,.    
-0004f560: 2020 2020 676c 6f62 616c 5f72 6174 655f      global_rate_
-0004f570: 6c69 6d69 745f 656e 6162 6c65 643a 2062  limit_enabled: b
-0004f580: 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020 2020  ool = None,.    
-0004f590: 2020 2020 6874 7470 5f31 3065 6e61 626c      http_10enabl
-0004f5a0: 6564 3a20 626f 6f6c 203d 204e 6f6e 652c  ed: bool = None,
-0004f5b0: 0a20 2020 2020 2020 2069 6e63 6c75 6465  .        include
-0004f5c0: 5f69 7072 616e 6765 733a 2073 7472 203d  _ipranges: str =
-0004f5d0: 204e 6f6e 652c 0a20 2020 2020 2020 2069   None,.        i
-0004f5e0: 6e63 6c75 6465 5f69 6e62 6f75 6e64 5f70  nclude_inbound_p
-0004f5f0: 6f72 7473 3a20 7374 7220 3d20 4e6f 6e65  orts: str = None
-0004f600: 2c0a 2020 2020 2020 2020 6b69 616c 695f  ,.        kiali_
-0004f610: 656e 6162 6c65 643a 2062 6f6f 6c20 3d20  enabled: bool = 
-0004f620: 4e6f 6e65 2c0a 2020 2020 2020 2020 6c69  None,.        li
-0004f630: 6665 6379 636c 653a 2073 7472 203d 204e  fecycle: str = N
-0004f640: 6f6e 652c 0a20 2020 2020 2020 206c 6f63  one,.        loc
-0004f650: 616c 6974 795f 6c62 636f 6e66 3a20 7374  ality_lbconf: st
-0004f660: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-0004f670: 2020 6c6f 6361 6c69 7479 5f6c 6f61 645f    locality_load_
-0004f680: 6261 6c61 6e63 696e 673a 2062 6f6f 6c20  balancing: bool 
-0004f690: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0004f6a0: 6d73 6565 6e61 626c 6564 3a20 626f 6f6c  mseenabled: bool
-0004f6b0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0004f6c0: 206d 756c 7469 5f62 7566 6665 725f 656e   multi_buffer_en
-0004f6d0: 6162 6c65 643a 2062 6f6f 6c20 3d20 4e6f  abled: bool = No
-0004f6e0: 6e65 2c0a 2020 2020 2020 2020 6d75 6c74  ne,.        mult
-0004f6f0: 695f 6275 6666 6572 5f70 6f6c 6c5f 6465  i_buffer_poll_de
-0004f700: 6c61 793a 2073 7472 203d 204e 6f6e 652c  lay: str = None,
-0004f710: 0a20 2020 2020 2020 206d 7973 716c 5f66  .        mysql_f
-0004f720: 696c 7465 725f 656e 6162 6c65 643a 2062  ilter_enabled: b
-0004f730: 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020 2020  ool = None,.    
-0004f740: 2020 2020 6f70 616c 696d 6974 5f63 7075      opalimit_cpu
-0004f750: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-0004f760: 2020 2020 2020 6f70 616c 696d 6974 5f6d        opalimit_m
-0004f770: 656d 6f72 793a 2073 7472 203d 204e 6f6e  emory: str = Non
-0004f780: 652c 0a20 2020 2020 2020 206f 7061 6c6f  e,.        opalo
-0004f790: 675f 6c65 7665 6c3a 2073 7472 203d 204e  g_level: str = N
-0004f7a0: 6f6e 652c 0a20 2020 2020 2020 206f 7061  one,.        opa
-0004f7b0: 7265 7175 6573 745f 6370 753a 2073 7472  request_cpu: str
-0004f7c0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0004f7d0: 206f 7061 7265 7175 6573 745f 6d65 6d6f   oparequest_memo
-0004f7e0: 7279 3a20 7374 7220 3d20 4e6f 6e65 2c0a  ry: str = None,.
-0004f7f0: 2020 2020 2020 2020 6f70 615f 656e 6162          opa_enab
-0004f800: 6c65 643a 2062 6f6f 6c20 3d20 4e6f 6e65  led: bool = None
-0004f810: 2c0a 2020 2020 2020 2020 6f70 656e 5f61  ,.        open_a
-0004f820: 6765 6e74 5f70 6f6c 6963 793a 2062 6f6f  gent_policy: boo
-0004f830: 6c20 3d20 4e6f 6e65 2c0a 2020 2020 2020  l = None,.      
-0004f840: 2020 6f75 7462 6f75 6e64 5f74 7261 6666    outbound_traff
-0004f850: 6963 5f70 6f6c 6963 793a 2073 7472 203d  ic_policy: str =
-0004f860: 204e 6f6e 652c 0a20 2020 2020 2020 2070   None,.        p
-0004f870: 726f 6d65 7468 6575 735f 7572 6c3a 2073  rometheus_url: s
-0004f880: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-0004f890: 2020 2070 726f 7879 5f69 6e69 745f 6370     proxy_init_cp
-0004f8a0: 7572 6573 6f75 7263 655f 6c69 6d69 743a  uresource_limit:
-0004f8b0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-0004f8c0: 2020 2020 2070 726f 7879 5f69 6e69 745f       proxy_init_
-0004f8d0: 6370 7572 6573 6f75 7263 655f 7265 7175  cpuresource_requ
-0004f8e0: 6573 743a 2073 7472 203d 204e 6f6e 652c  est: str = None,
-0004f8f0: 0a20 2020 2020 2020 2070 726f 7879 5f69  .        proxy_i
-0004f900: 6e69 745f 6d65 6d6f 7279 5f72 6573 6f75  nit_memory_resou
-0004f910: 7263 655f 6c69 6d69 743a 2073 7472 203d  rce_limit: str =
-0004f920: 204e 6f6e 652c 0a20 2020 2020 2020 2070   None,.        p
-0004f930: 726f 7879 5f69 6e69 745f 6d65 6d6f 7279  roxy_init_memory
-0004f940: 5f72 6573 6f75 7263 655f 7265 7175 6573  _resource_reques
-0004f950: 743a 2073 7472 203d 204e 6f6e 652c 0a20  t: str = None,. 
-0004f960: 2020 2020 2020 2070 726f 7879 5f6c 696d         proxy_lim
-0004f970: 6974 5f63 7075 3a20 7374 7220 3d20 4e6f  it_cpu: str = No
-0004f980: 6e65 2c0a 2020 2020 2020 2020 7072 6f78  ne,.        prox
-0004f990: 795f 6c69 6d69 745f 6d65 6d6f 7279 3a20  y_limit_memory: 
-0004f9a0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-0004f9b0: 2020 2020 7072 6f78 795f 7265 7175 6573      proxy_reques
-0004f9c0: 745f 6370 753a 2073 7472 203d 204e 6f6e  t_cpu: str = Non
-0004f9d0: 652c 0a20 2020 2020 2020 2070 726f 7879  e,.        proxy
-0004f9e0: 5f72 6571 7565 7374 5f6d 656d 6f72 793a  _request_memory:
-0004f9f0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-0004fa00: 2020 2020 2072 6564 6973 5f66 696c 7465       redis_filte
-0004fa10: 725f 656e 6162 6c65 643a 2062 6f6f 6c20  r_enabled: bool 
-0004fa20: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0004fa30: 7365 7276 6963 655f 6d65 7368 5f69 643a  service_mesh_id:
-0004fa40: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-0004fa50: 2020 2020 2073 6964 6563 6172 5f69 6e6a       sidecar_inj
-0004fa60: 6563 746f 725f 6c69 6d69 745f 6370 753a  ector_limit_cpu:
-0004fa70: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-0004fa80: 2020 2020 2073 6964 6563 6172 5f69 6e6a       sidecar_inj
-0004fa90: 6563 746f 725f 6c69 6d69 745f 6d65 6d6f  ector_limit_memo
-0004faa0: 7279 3a20 7374 7220 3d20 4e6f 6e65 2c0a  ry: str = None,.
-0004fab0: 2020 2020 2020 2020 7369 6465 6361 725f          sidecar_
-0004fac0: 696e 6a65 6374 6f72 5f72 6571 7565 7374  injector_request
-0004fad0: 5f63 7075 3a20 7374 7220 3d20 4e6f 6e65  _cpu: str = None
-0004fae0: 2c0a 2020 2020 2020 2020 7369 6465 6361  ,.        sideca
-0004faf0: 725f 696e 6a65 6374 6f72 5f72 6571 7565  r_injector_reque
-0004fb00: 7374 5f6d 656d 6f72 793a 2073 7472 203d  st_memory: str =
-0004fb10: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
-0004fb20: 6964 6563 6172 5f69 6e6a 6563 746f 725f  idecar_injector_
-0004fb30: 7765 6268 6f6f 6b5f 6173 5f79 616d 6c3a  webhook_as_yaml:
-0004fb40: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-0004fb50: 2020 2020 2074 656c 656d 6574 7279 3a20       telemetry: 
-0004fb60: 626f 6f6c 203d 204e 6f6e 652c 0a20 2020  bool = None,.   
-0004fb70: 2020 2020 2074 6572 6d69 6e61 7469 6f6e       termination
-0004fb80: 5f64 7261 696e 5f64 7572 6174 696f 6e3a  _drain_duration:
-0004fb90: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-0004fba0: 2020 2020 2074 6872 6966 745f 6669 6c74       thrift_filt
-0004fbb0: 6572 5f65 6e61 626c 6564 3a20 626f 6f6c  er_enabled: bool
-0004fbc0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0004fbd0: 2074 7261 6365 5f73 616d 706c 696e 673a   trace_sampling:
-0004fbe0: 2066 6c6f 6174 203d 204e 6f6e 652c 0a20   float = None,. 
-0004fbf0: 2020 2020 2020 2074 7261 6369 6e67 3a20         tracing: 
-0004fc00: 626f 6f6c 203d 204e 6f6e 652c 0a20 2020  bool = None,.   
-0004fc10: 2020 2020 2077 6562 5f61 7373 656d 626c       web_assembl
-0004fc20: 795f 6669 6c74 6572 5f65 6e61 626c 6564  y_filter_enabled
-0004fc30: 3a20 626f 6f6c 203d 204e 6f6e 652c 0a20  : bool = None,. 
-0004fc40: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-0004fc50: 6c66 2e61 6363 6573 735f 6c6f 675f 656e  lf.access_log_en
-0004fc60: 6162 6c65 6420 3d20 6163 6365 7373 5f6c  abled = access_l
-0004fc70: 6f67 5f65 6e61 626c 6564 0a20 2020 2020  og_enabled.     
-0004fc80: 2020 2073 656c 662e 6163 6365 7373 5f6c     self.access_l
-0004fc90: 6f67 5f66 696c 6520 3d20 6163 6365 7373  og_file = access
-0004fca0: 5f6c 6f67 5f66 696c 650a 2020 2020 2020  _log_file.      
-0004fcb0: 2020 7365 6c66 2e61 6363 6573 735f 6c6f    self.access_lo
-0004fcc0: 675f 666f 726d 6174 203d 2061 6363 6573  g_format = acces
-0004fcd0: 735f 6c6f 675f 666f 726d 6174 0a20 2020  s_log_format.   
-0004fce0: 2020 2020 2073 656c 662e 6163 6365 7373       self.access
-0004fcf0: 5f6c 6f67 5f70 726f 6a65 6374 203d 2061  _log_project = a
-0004fd00: 6363 6573 735f 6c6f 675f 7072 6f6a 6563  ccess_log_projec
-0004fd10: 740a 2020 2020 2020 2020 7365 6c66 2e61  t.        self.a
-0004fd20: 6363 6573 735f 6c6f 675f 7365 7276 6963  ccess_log_servic
-0004fd30: 655f 656e 6162 6c65 6420 3d20 6163 6365  e_enabled = acce
-0004fd40: 7373 5f6c 6f67 5f73 6572 7669 6365 5f65  ss_log_service_e
-0004fd50: 6e61 626c 6564 0a20 2020 2020 2020 2073  nabled.        s
-0004fd60: 656c 662e 6163 6365 7373 5f6c 6f67 5f73  elf.access_log_s
-0004fd70: 6572 7669 6365 5f68 6f73 7420 3d20 6163  ervice_host = ac
-0004fd80: 6365 7373 5f6c 6f67 5f73 6572 7669 6365  cess_log_service
-0004fd90: 5f68 6f73 740a 2020 2020 2020 2020 7365  _host.        se
-0004fda0: 6c66 2e61 6363 6573 735f 6c6f 675f 7365  lf.access_log_se
-0004fdb0: 7276 6963 655f 706f 7274 203d 2061 6363  rvice_port = acc
-0004fdc0: 6573 735f 6c6f 675f 7365 7276 6963 655f  ess_log_service_
-0004fdd0: 706f 7274 0a20 2020 2020 2020 2073 656c  port.        sel
-0004fde0: 662e 6175 6469 745f 7072 6f6a 6563 7420  f.audit_project 
-0004fdf0: 3d20 6175 6469 745f 7072 6f6a 6563 740a  = audit_project.
-0004fe00: 2020 2020 2020 2020 7365 6c66 2e61 7574          self.aut
-0004fe10: 6f5f 696e 6a65 6374 696f 6e5f 706f 6c69  o_injection_poli
-0004fe20: 6379 5f65 6e61 626c 6564 203d 2061 7574  cy_enabled = aut
-0004fe30: 6f5f 696e 6a65 6374 696f 6e5f 706f 6c69  o_injection_poli
-0004fe40: 6379 5f65 6e61 626c 6564 0a20 2020 2020  cy_enabled.     
-0004fe50: 2020 2073 656c 662e 6372 6167 6772 6567     self.craggreg
-0004fe60: 6174 696f 6e5f 656e 6162 6c65 6420 3d20  ation_enabled = 
-0004fe70: 6372 6167 6772 6567 6174 696f 6e5f 656e  craggregation_en
-0004fe80: 6162 6c65 640a 2020 2020 2020 2020 7365  abled.        se
-0004fe90: 6c66 2e63 6c75 7374 6572 5f73 7065 6320  lf.cluster_spec 
-0004fea0: 3d20 636c 7573 7465 725f 7370 6563 0a20  = cluster_spec. 
-0004feb0: 2020 2020 2020 2073 656c 662e 636e 695f         self.cni_
-0004fec0: 656e 6162 6c65 6420 3d20 636e 695f 656e  enabled = cni_en
-0004fed0: 6162 6c65 640a 2020 2020 2020 2020 7365  abled.        se
-0004fee0: 6c66 2e63 6e69 5f65 7863 6c75 6465 5f6e  lf.cni_exclude_n
-0004fef0: 616d 6573 7061 6365 7320 3d20 636e 695f  amespaces = cni_
-0004ff00: 6578 636c 7564 655f 6e61 6d65 7370 6163  exclude_namespac
-0004ff10: 6573 0a20 2020 2020 2020 2073 656c 662e  es.        self.
-0004ff20: 636f 6e66 6967 5f73 6f75 7263 655f 656e  config_source_en
-0004ff30: 6162 6c65 6420 3d20 636f 6e66 6967 5f73  abled = config_s
-0004ff40: 6f75 7263 655f 656e 6162 6c65 640a 2020  ource_enabled.  
-0004ff50: 2020 2020 2020 7365 6c66 2e63 6f6e 6669        self.confi
-0004ff60: 675f 736f 7572 6365 5f6e 6163 6f73 5f69  g_source_nacos_i
-0004ff70: 6420 3d20 636f 6e66 6967 5f73 6f75 7263  d = config_sourc
-0004ff80: 655f 6e61 636f 735f 6964 0a20 2020 2020  e_nacos_id.     
-0004ff90: 2020 2073 656c 662e 6375 7374 6f6d 697a     self.customiz
-0004ffa0: 6564 5f70 726f 6d65 7468 6575 7320 3d20  ed_prometheus = 
-0004ffb0: 6375 7374 6f6d 697a 6564 5f70 726f 6d65  customized_prome
-0004ffc0: 7468 6575 730a 2020 2020 2020 2020 7365  theus.        se
-0004ffd0: 6c66 2e63 7573 746f 6d69 7a65 645f 7a69  lf.customized_zi
-0004ffe0: 706b 696e 203d 2063 7573 746f 6d69 7a65  pkin = customize
-0004fff0: 645f 7a69 706b 696e 0a20 2020 2020 2020  d_zipkin.       
-00050000: 2073 656c 662e 646e 7370 726f 7879 696e   self.dnsproxyin
-00050010: 675f 656e 6162 6c65 6420 3d20 646e 7370  g_enabled = dnsp
-00050020: 726f 7879 696e 675f 656e 6162 6c65 640a  roxying_enabled.
-00050030: 2020 2020 2020 2020 7365 6c66 2e64 6973          self.dis
-00050040: 636f 7665 7279 5f73 656c 6563 746f 7273  covery_selectors
-00050050: 203d 2064 6973 636f 7665 7279 5f73 656c   = discovery_sel
-00050060: 6563 746f 7273 0a20 2020 2020 2020 2073  ectors.        s
-00050070: 656c 662e 6475 6262 6f5f 6669 6c74 6572  elf.dubbo_filter
-00050080: 5f65 6e61 626c 6564 203d 2064 7562 626f  _enabled = dubbo
-00050090: 5f66 696c 7465 725f 656e 6162 6c65 640a  _filter_enabled.
-000500a0: 2020 2020 2020 2020 7365 6c66 2e65 6e61          self.ena
-000500b0: 626c 655f 6175 6469 7420 3d20 656e 6162  ble_audit = enab
-000500c0: 6c65 5f61 7564 6974 0a20 2020 2020 2020  le_audit.       
-000500d0: 2073 656c 662e 656e 6162 6c65 5f63 7268   self.enable_crh
-000500e0: 6973 746f 7279 203d 2065 6e61 626c 655f  istory = enable_
-000500f0: 6372 6869 7374 6f72 790a 2020 2020 2020  crhistory.      
-00050100: 2020 7365 6c66 2e65 6e61 626c 655f 6e61    self.enable_na
-00050110: 6d65 7370 6163 6573 5f62 795f 6465 6661  mespaces_by_defa
-00050120: 756c 7420 3d20 656e 6162 6c65 5f6e 616d  ult = enable_nam
-00050130: 6573 7061 6365 735f 6279 5f64 6566 6175  espaces_by_defau
-00050140: 6c74 0a20 2020 2020 2020 2073 656c 662e  lt.        self.
-00050150: 656e 6162 6c65 5f73 6473 7365 7276 6572  enable_sdsserver
-00050160: 203d 2065 6e61 626c 655f 7364 7373 6572   = enable_sdsser
-00050170: 7665 720a 2020 2020 2020 2020 7365 6c66  ver.        self
-00050180: 2e65 7863 6c75 6465 5f69 7072 616e 6765  .exclude_iprange
-00050190: 7320 3d20 6578 636c 7564 655f 6970 7261  s = exclude_ipra
-000501a0: 6e67 6573 0a20 2020 2020 2020 2073 656c  nges.        sel
-000501b0: 662e 6578 636c 7564 655f 696e 626f 756e  f.exclude_inboun
-000501c0: 645f 706f 7274 7320 3d20 6578 636c 7564  d_ports = exclud
-000501d0: 655f 696e 626f 756e 645f 706f 7274 730a  e_inbound_ports.
-000501e0: 2020 2020 2020 2020 7365 6c66 2e65 7863          self.exc
-000501f0: 6c75 6465 5f6f 7574 626f 756e 645f 706f  lude_outbound_po
-00050200: 7274 7320 3d20 6578 636c 7564 655f 6f75  rts = exclude_ou
-00050210: 7462 6f75 6e64 5f70 6f72 7473 0a20 2020  tbound_ports.   
-00050220: 2020 2020 2073 656c 662e 6669 6c74 6572       self.filter
-00050230: 5f67 6174 6577 6179 5f63 6c75 7374 6572  _gateway_cluster
-00050240: 5f63 6f6e 6669 6720 3d20 6669 6c74 6572  _config = filter
-00050250: 5f67 6174 6577 6179 5f63 6c75 7374 6572  _gateway_cluster
-00050260: 5f63 6f6e 6669 670a 2020 2020 2020 2020  _config.        
-00050270: 7365 6c66 2e67 6174 6577 6179 5f61 7069  self.gateway_api
-00050280: 656e 6162 6c65 6420 3d20 6761 7465 7761  enabled = gatewa
-00050290: 795f 6170 6965 6e61 626c 6564 0a20 2020  y_apienabled.   
-000502a0: 2020 2020 2073 656c 662e 676c 6f62 616c       self.global
-000502b0: 5f72 6174 655f 6c69 6d69 745f 656e 6162  _rate_limit_enab
-000502c0: 6c65 6420 3d20 676c 6f62 616c 5f72 6174  led = global_rat
-000502d0: 655f 6c69 6d69 745f 656e 6162 6c65 640a  e_limit_enabled.
-000502e0: 2020 2020 2020 2020 7365 6c66 2e68 7474          self.htt
-000502f0: 705f 3130 656e 6162 6c65 6420 3d20 6874  p_10enabled = ht
-00050300: 7470 5f31 3065 6e61 626c 6564 0a20 2020  tp_10enabled.   
-00050310: 2020 2020 2073 656c 662e 696e 636c 7564       self.includ
-00050320: 655f 6970 7261 6e67 6573 203d 2069 6e63  e_ipranges = inc
-00050330: 6c75 6465 5f69 7072 616e 6765 730a 2020  lude_ipranges.  
-00050340: 2020 2020 2020 7365 6c66 2e69 6e63 6c75        self.inclu
-00050350: 6465 5f69 6e62 6f75 6e64 5f70 6f72 7473  de_inbound_ports
-00050360: 203d 2069 6e63 6c75 6465 5f69 6e62 6f75   = include_inbou
-00050370: 6e64 5f70 6f72 7473 0a20 2020 2020 2020  nd_ports.       
-00050380: 2073 656c 662e 6b69 616c 695f 656e 6162   self.kiali_enab
-00050390: 6c65 6420 3d20 6b69 616c 695f 656e 6162  led = kiali_enab
-000503a0: 6c65 640a 2020 2020 2020 2020 7365 6c66  led.        self
-000503b0: 2e6c 6966 6563 7963 6c65 203d 206c 6966  .lifecycle = lif
-000503c0: 6563 7963 6c65 0a20 2020 2020 2020 2073  ecycle.        s
-000503d0: 656c 662e 6c6f 6361 6c69 7479 5f6c 6263  elf.locality_lbc
-000503e0: 6f6e 6620 3d20 6c6f 6361 6c69 7479 5f6c  onf = locality_l
-000503f0: 6263 6f6e 660a 2020 2020 2020 2020 7365  bconf.        se
-00050400: 6c66 2e6c 6f63 616c 6974 795f 6c6f 6164  lf.locality_load
-00050410: 5f62 616c 616e 6369 6e67 203d 206c 6f63  _balancing = loc
-00050420: 616c 6974 795f 6c6f 6164 5f62 616c 616e  ality_load_balan
-00050430: 6369 6e67 0a20 2020 2020 2020 2073 656c  cing.        sel
-00050440: 662e 6d73 6565 6e61 626c 6564 203d 206d  f.mseenabled = m
-00050450: 7365 656e 6162 6c65 640a 2020 2020 2020  seenabled.      
-00050460: 2020 7365 6c66 2e6d 756c 7469 5f62 7566    self.multi_buf
-00050470: 6665 725f 656e 6162 6c65 6420 3d20 6d75  fer_enabled = mu
-00050480: 6c74 695f 6275 6666 6572 5f65 6e61 626c  lti_buffer_enabl
-00050490: 6564 0a20 2020 2020 2020 2073 656c 662e  ed.        self.
-000504a0: 6d75 6c74 695f 6275 6666 6572 5f70 6f6c  multi_buffer_pol
-000504b0: 6c5f 6465 6c61 7920 3d20 6d75 6c74 695f  l_delay = multi_
-000504c0: 6275 6666 6572 5f70 6f6c 6c5f 6465 6c61  buffer_poll_dela
-000504d0: 790a 2020 2020 2020 2020 7365 6c66 2e6d  y.        self.m
-000504e0: 7973 716c 5f66 696c 7465 725f 656e 6162  ysql_filter_enab
-000504f0: 6c65 6420 3d20 6d79 7371 6c5f 6669 6c74  led = mysql_filt
-00050500: 6572 5f65 6e61 626c 6564 0a20 2020 2020  er_enabled.     
-00050510: 2020 2073 656c 662e 6f70 616c 696d 6974     self.opalimit
-00050520: 5f63 7075 203d 206f 7061 6c69 6d69 745f  _cpu = opalimit_
-00050530: 6370 750a 2020 2020 2020 2020 7365 6c66  cpu.        self
-00050540: 2e6f 7061 6c69 6d69 745f 6d65 6d6f 7279  .opalimit_memory
-00050550: 203d 206f 7061 6c69 6d69 745f 6d65 6d6f   = opalimit_memo
-00050560: 7279 0a20 2020 2020 2020 2073 656c 662e  ry.        self.
-00050570: 6f70 616c 6f67 5f6c 6576 656c 203d 206f  opalog_level = o
-00050580: 7061 6c6f 675f 6c65 7665 6c0a 2020 2020  palog_level.    
-00050590: 2020 2020 7365 6c66 2e6f 7061 7265 7175      self.oparequ
-000505a0: 6573 745f 6370 7520 3d20 6f70 6172 6571  est_cpu = opareq
-000505b0: 7565 7374 5f63 7075 0a20 2020 2020 2020  uest_cpu.       
-000505c0: 2073 656c 662e 6f70 6172 6571 7565 7374   self.oparequest
-000505d0: 5f6d 656d 6f72 7920 3d20 6f70 6172 6571  _memory = opareq
-000505e0: 7565 7374 5f6d 656d 6f72 790a 2020 2020  uest_memory.    
-000505f0: 2020 2020 7365 6c66 2e6f 7061 5f65 6e61      self.opa_ena
-00050600: 626c 6564 203d 206f 7061 5f65 6e61 626c  bled = opa_enabl
-00050610: 6564 0a20 2020 2020 2020 2073 656c 662e  ed.        self.
-00050620: 6f70 656e 5f61 6765 6e74 5f70 6f6c 6963  open_agent_polic
-00050630: 7920 3d20 6f70 656e 5f61 6765 6e74 5f70  y = open_agent_p
-00050640: 6f6c 6963 790a 2020 2020 2020 2020 7365  olicy.        se
-00050650: 6c66 2e6f 7574 626f 756e 645f 7472 6166  lf.outbound_traf
-00050660: 6669 635f 706f 6c69 6379 203d 206f 7574  fic_policy = out
-00050670: 626f 756e 645f 7472 6166 6669 635f 706f  bound_traffic_po
-00050680: 6c69 6379 0a20 2020 2020 2020 2073 656c  licy.        sel
-00050690: 662e 7072 6f6d 6574 6865 7573 5f75 726c  f.prometheus_url
-000506a0: 203d 2070 726f 6d65 7468 6575 735f 7572   = prometheus_ur
-000506b0: 6c0a 2020 2020 2020 2020 7365 6c66 2e70  l.        self.p
-000506c0: 726f 7879 5f69 6e69 745f 6370 7572 6573  roxy_init_cpures
-000506d0: 6f75 7263 655f 6c69 6d69 7420 3d20 7072  ource_limit = pr
-000506e0: 6f78 795f 696e 6974 5f63 7075 7265 736f  oxy_init_cpureso
-000506f0: 7572 6365 5f6c 696d 6974 0a20 2020 2020  urce_limit.     
-00050700: 2020 2073 656c 662e 7072 6f78 795f 696e     self.proxy_in
-00050710: 6974 5f63 7075 7265 736f 7572 6365 5f72  it_cpuresource_r
-00050720: 6571 7565 7374 203d 2070 726f 7879 5f69  equest = proxy_i
-00050730: 6e69 745f 6370 7572 6573 6f75 7263 655f  nit_cpuresource_
-00050740: 7265 7175 6573 740a 2020 2020 2020 2020  request.        
-00050750: 7365 6c66 2e70 726f 7879 5f69 6e69 745f  self.proxy_init_
-00050760: 6d65 6d6f 7279 5f72 6573 6f75 7263 655f  memory_resource_
-00050770: 6c69 6d69 7420 3d20 7072 6f78 795f 696e  limit = proxy_in
-00050780: 6974 5f6d 656d 6f72 795f 7265 736f 7572  it_memory_resour
-00050790: 6365 5f6c 696d 6974 0a20 2020 2020 2020  ce_limit.       
-000507a0: 2073 656c 662e 7072 6f78 795f 696e 6974   self.proxy_init
-000507b0: 5f6d 656d 6f72 795f 7265 736f 7572 6365  _memory_resource
-000507c0: 5f72 6571 7565 7374 203d 2070 726f 7879  _request = proxy
-000507d0: 5f69 6e69 745f 6d65 6d6f 7279 5f72 6573  _init_memory_res
-000507e0: 6f75 7263 655f 7265 7175 6573 740a 2020  ource_request.  
-000507f0: 2020 2020 2020 7365 6c66 2e70 726f 7879        self.proxy
-00050800: 5f6c 696d 6974 5f63 7075 203d 2070 726f  _limit_cpu = pro
-00050810: 7879 5f6c 696d 6974 5f63 7075 0a20 2020  xy_limit_cpu.   
-00050820: 2020 2020 2073 656c 662e 7072 6f78 795f       self.proxy_
-00050830: 6c69 6d69 745f 6d65 6d6f 7279 203d 2070  limit_memory = p
-00050840: 726f 7879 5f6c 696d 6974 5f6d 656d 6f72  roxy_limit_memor
-00050850: 790a 2020 2020 2020 2020 7365 6c66 2e70  y.        self.p
-00050860: 726f 7879 5f72 6571 7565 7374 5f63 7075  roxy_request_cpu
-00050870: 203d 2070 726f 7879 5f72 6571 7565 7374   = proxy_request
-00050880: 5f63 7075 0a20 2020 2020 2020 2073 656c  _cpu.        sel
-00050890: 662e 7072 6f78 795f 7265 7175 6573 745f  f.proxy_request_
-000508a0: 6d65 6d6f 7279 203d 2070 726f 7879 5f72  memory = proxy_r
-000508b0: 6571 7565 7374 5f6d 656d 6f72 790a 2020  equest_memory.  
-000508c0: 2020 2020 2020 7365 6c66 2e72 6564 6973        self.redis
-000508d0: 5f66 696c 7465 725f 656e 6162 6c65 6420  _filter_enabled 
-000508e0: 3d20 7265 6469 735f 6669 6c74 6572 5f65  = redis_filter_e
-000508f0: 6e61 626c 6564 0a20 2020 2020 2020 2073  nabled.        s
-00050900: 656c 662e 7365 7276 6963 655f 6d65 7368  elf.service_mesh
-00050910: 5f69 6420 3d20 7365 7276 6963 655f 6d65  _id = service_me
-00050920: 7368 5f69 640a 2020 2020 2020 2020 7365  sh_id.        se
-00050930: 6c66 2e73 6964 6563 6172 5f69 6e6a 6563  lf.sidecar_injec
-00050940: 746f 725f 6c69 6d69 745f 6370 7520 3d20  tor_limit_cpu = 
-00050950: 7369 6465 6361 725f 696e 6a65 6374 6f72  sidecar_injector
-00050960: 5f6c 696d 6974 5f63 7075 0a20 2020 2020  _limit_cpu.     
-00050970: 2020 2073 656c 662e 7369 6465 6361 725f     self.sidecar_
-00050980: 696e 6a65 6374 6f72 5f6c 696d 6974 5f6d  injector_limit_m
-00050990: 656d 6f72 7920 3d20 7369 6465 6361 725f  emory = sidecar_
-000509a0: 696e 6a65 6374 6f72 5f6c 696d 6974 5f6d  injector_limit_m
-000509b0: 656d 6f72 790a 2020 2020 2020 2020 7365  emory.        se
-000509c0: 6c66 2e73 6964 6563 6172 5f69 6e6a 6563  lf.sidecar_injec
-000509d0: 746f 725f 7265 7175 6573 745f 6370 7520  tor_request_cpu 
-000509e0: 3d20 7369 6465 6361 725f 696e 6a65 6374  = sidecar_inject
-000509f0: 6f72 5f72 6571 7565 7374 5f63 7075 0a20  or_request_cpu. 
-00050a00: 2020 2020 2020 2073 656c 662e 7369 6465         self.side
-00050a10: 6361 725f 696e 6a65 6374 6f72 5f72 6571  car_injector_req
-00050a20: 7565 7374 5f6d 656d 6f72 7920 3d20 7369  uest_memory = si
-00050a30: 6465 6361 725f 696e 6a65 6374 6f72 5f72  decar_injector_r
-00050a40: 6571 7565 7374 5f6d 656d 6f72 790a 2020  equest_memory.  
-00050a50: 2020 2020 2020 7365 6c66 2e73 6964 6563        self.sidec
-00050a60: 6172 5f69 6e6a 6563 746f 725f 7765 6268  ar_injector_webh
-00050a70: 6f6f 6b5f 6173 5f79 616d 6c20 3d20 7369  ook_as_yaml = si
-00050a80: 6465 6361 725f 696e 6a65 6374 6f72 5f77  decar_injector_w
-00050a90: 6562 686f 6f6b 5f61 735f 7961 6d6c 0a20  ebhook_as_yaml. 
-00050aa0: 2020 2020 2020 2073 656c 662e 7465 6c65         self.tele
-00050ab0: 6d65 7472 7920 3d20 7465 6c65 6d65 7472  metry = telemetr
-00050ac0: 790a 2020 2020 2020 2020 7365 6c66 2e74  y.        self.t
-00050ad0: 6572 6d69 6e61 7469 6f6e 5f64 7261 696e  ermination_drain
-00050ae0: 5f64 7572 6174 696f 6e20 3d20 7465 726d  _duration = term
-00050af0: 696e 6174 696f 6e5f 6472 6169 6e5f 6475  ination_drain_du
-00050b00: 7261 7469 6f6e 0a20 2020 2020 2020 2073  ration.        s
-00050b10: 656c 662e 7468 7269 6674 5f66 696c 7465  elf.thrift_filte
-00050b20: 725f 656e 6162 6c65 6420 3d20 7468 7269  r_enabled = thri
-00050b30: 6674 5f66 696c 7465 725f 656e 6162 6c65  ft_filter_enable
-00050b40: 640a 2020 2020 2020 2020 7365 6c66 2e74  d.        self.t
-00050b50: 7261 6365 5f73 616d 706c 696e 6720 3d20  race_sampling = 
-00050b60: 7472 6163 655f 7361 6d70 6c69 6e67 0a20  trace_sampling. 
-00050b70: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
-00050b80: 696e 6720 3d20 7472 6163 696e 670a 2020  ing = tracing.  
-00050b90: 2020 2020 2020 7365 6c66 2e77 6562 5f61        self.web_a
-00050ba0: 7373 656d 626c 795f 6669 6c74 6572 5f65  ssembly_filter_e
-00050bb0: 6e61 626c 6564 203d 2077 6562 5f61 7373  nabled = web_ass
-00050bc0: 656d 626c 795f 6669 6c74 6572 5f65 6e61  embly_filter_ena
-00050bd0: 626c 6564 0a0a 2020 2020 6465 6620 7661  bled..    def va
-00050be0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-00050bf0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00050c00: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
-00050c10: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
-00050c20: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
-00050c30: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
-00050c40: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
-00050c50: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00050c60: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
-00050c70: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
-00050c80: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00050c90: 6163 6365 7373 5f6c 6f67 5f65 6e61 626c  access_log_enabl
-00050ca0: 6564 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ed is not None:.
-00050cb0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00050cc0: 6c74 5b27 4163 6365 7373 4c6f 6745 6e61  lt['AccessLogEna
-00050cd0: 626c 6564 275d 203d 2073 656c 662e 6163  bled'] = self.ac
-00050ce0: 6365 7373 5f6c 6f67 5f65 6e61 626c 6564  cess_log_enabled
-00050cf0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00050d00: 2e61 6363 6573 735f 6c6f 675f 6669 6c65  .access_log_file
-00050d10: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00050d20: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00050d30: 5b27 4163 6365 7373 4c6f 6746 696c 6527  ['AccessLogFile'
-00050d40: 5d20 3d20 7365 6c66 2e61 6363 6573 735f  ] = self.access_
-00050d50: 6c6f 675f 6669 6c65 0a20 2020 2020 2020  log_file.       
-00050d60: 2069 6620 7365 6c66 2e61 6363 6573 735f   if self.access_
-00050d70: 6c6f 675f 666f 726d 6174 2069 7320 6e6f  log_format is no
-00050d80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00050d90: 2020 2020 7265 7375 6c74 5b27 4163 6365      result['Acce
-00050da0: 7373 4c6f 6746 6f72 6d61 7427 5d20 3d20  ssLogFormat'] = 
-00050db0: 7365 6c66 2e61 6363 6573 735f 6c6f 675f  self.access_log_
-00050dc0: 666f 726d 6174 0a20 2020 2020 2020 2069  format.        i
-00050dd0: 6620 7365 6c66 2e61 6363 6573 735f 6c6f  f self.access_lo
-00050de0: 675f 7072 6f6a 6563 7420 6973 206e 6f74  g_project is not
-00050df0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00050e00: 2020 2072 6573 756c 745b 2741 6363 6573     result['Acces
-00050e10: 734c 6f67 5072 6f6a 6563 7427 5d20 3d20  sLogProject'] = 
-00050e20: 7365 6c66 2e61 6363 6573 735f 6c6f 675f  self.access_log_
-00050e30: 7072 6f6a 6563 740a 2020 2020 2020 2020  project.        
-00050e40: 6966 2073 656c 662e 6163 6365 7373 5f6c  if self.access_l
-00050e50: 6f67 5f73 6572 7669 6365 5f65 6e61 626c  og_service_enabl
-00050e60: 6564 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ed is not None:.
-00050e70: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00050e80: 6c74 5b27 4163 6365 7373 4c6f 6753 6572  lt['AccessLogSer
-00050e90: 7669 6365 456e 6162 6c65 6427 5d20 3d20  viceEnabled'] = 
-00050ea0: 7365 6c66 2e61 6363 6573 735f 6c6f 675f  self.access_log_
-00050eb0: 7365 7276 6963 655f 656e 6162 6c65 640a  service_enabled.
-00050ec0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00050ed0: 6163 6365 7373 5f6c 6f67 5f73 6572 7669  access_log_servi
-00050ee0: 6365 5f68 6f73 7420 6973 206e 6f74 204e  ce_host is not N
-00050ef0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00050f00: 2072 6573 756c 745b 2741 6363 6573 734c   result['AccessL
-00050f10: 6f67 5365 7276 6963 6548 6f73 7427 5d20  ogServiceHost'] 
-00050f20: 3d20 7365 6c66 2e61 6363 6573 735f 6c6f  = self.access_lo
-00050f30: 675f 7365 7276 6963 655f 686f 7374 0a20  g_service_host. 
-00050f40: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
-00050f50: 6363 6573 735f 6c6f 675f 7365 7276 6963  ccess_log_servic
-00050f60: 655f 706f 7274 2069 7320 6e6f 7420 4e6f  e_port is not No
-00050f70: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00050f80: 7265 7375 6c74 5b27 4163 6365 7373 4c6f  result['AccessLo
-00050f90: 6753 6572 7669 6365 506f 7274 275d 203d  gServicePort'] =
-00050fa0: 2073 656c 662e 6163 6365 7373 5f6c 6f67   self.access_log
-00050fb0: 5f73 6572 7669 6365 5f70 6f72 740a 2020  _service_port.  
-00050fc0: 2020 2020 2020 6966 2073 656c 662e 6175        if self.au
-00050fd0: 6469 745f 7072 6f6a 6563 7420 6973 206e  dit_project is n
-00050fe0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00050ff0: 2020 2020 2072 6573 756c 745b 2741 7564       result['Aud
-00051000: 6974 5072 6f6a 6563 7427 5d20 3d20 7365  itProject'] = se
-00051010: 6c66 2e61 7564 6974 5f70 726f 6a65 6374  lf.audit_project
-00051020: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00051030: 2e61 7574 6f5f 696e 6a65 6374 696f 6e5f  .auto_injection_
-00051040: 706f 6c69 6379 5f65 6e61 626c 6564 2069  policy_enabled i
-00051050: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00051060: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00051070: 4175 746f 496e 6a65 6374 696f 6e50 6f6c  AutoInjectionPol
-00051080: 6963 7945 6e61 626c 6564 275d 203d 2073  icyEnabled'] = s
-00051090: 656c 662e 6175 746f 5f69 6e6a 6563 7469  elf.auto_injecti
-000510a0: 6f6e 5f70 6f6c 6963 795f 656e 6162 6c65  on_policy_enable
-000510b0: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-000510c0: 662e 6372 6167 6772 6567 6174 696f 6e5f  f.craggregation_
-000510d0: 656e 6162 6c65 6420 6973 206e 6f74 204e  enabled is not N
-000510e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000510f0: 2072 6573 756c 745b 2743 5241 6767 7265   result['CRAggre
-00051100: 6761 7469 6f6e 456e 6162 6c65 6427 5d20  gationEnabled'] 
-00051110: 3d20 7365 6c66 2e63 7261 6767 7265 6761  = self.craggrega
-00051120: 7469 6f6e 5f65 6e61 626c 6564 0a20 2020  tion_enabled.   
-00051130: 2020 2020 2069 6620 7365 6c66 2e63 6c75       if self.clu
-00051140: 7374 6572 5f73 7065 6320 6973 206e 6f74  ster_spec is not
-00051150: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00051160: 2020 2072 6573 756c 745b 2743 6c75 7374     result['Clust
-00051170: 6572 5370 6563 275d 203d 2073 656c 662e  erSpec'] = self.
-00051180: 636c 7573 7465 725f 7370 6563 0a20 2020  cluster_spec.   
-00051190: 2020 2020 2069 6620 7365 6c66 2e63 6e69       if self.cni
-000511a0: 5f65 6e61 626c 6564 2069 7320 6e6f 7420  _enabled is not 
-000511b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000511c0: 2020 7265 7375 6c74 5b27 436e 6945 6e61    result['CniEna
-000511d0: 626c 6564 275d 203d 2073 656c 662e 636e  bled'] = self.cn
-000511e0: 695f 656e 6162 6c65 640a 2020 2020 2020  i_enabled.      
-000511f0: 2020 6966 2073 656c 662e 636e 695f 6578    if self.cni_ex
-00051200: 636c 7564 655f 6e61 6d65 7370 6163 6573  clude_namespaces
-00051210: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00051220: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00051230: 5b27 436e 6945 7863 6c75 6465 4e61 6d65  ['CniExcludeName
-00051240: 7370 6163 6573 275d 203d 2073 656c 662e  spaces'] = self.
-00051250: 636e 695f 6578 636c 7564 655f 6e61 6d65  cni_exclude_name
-00051260: 7370 6163 6573 0a20 2020 2020 2020 2069  spaces.        i
-00051270: 6620 7365 6c66 2e63 6f6e 6669 675f 736f  f self.config_so
-00051280: 7572 6365 5f65 6e61 626c 6564 2069 7320  urce_enabled is 
-00051290: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000512a0: 2020 2020 2020 7265 7375 6c74 5b27 436f        result['Co
-000512b0: 6e66 6967 536f 7572 6365 456e 6162 6c65  nfigSourceEnable
-000512c0: 6427 5d20 3d20 7365 6c66 2e63 6f6e 6669  d'] = self.confi
-000512d0: 675f 736f 7572 6365 5f65 6e61 626c 6564  g_source_enabled
-000512e0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000512f0: 2e63 6f6e 6669 675f 736f 7572 6365 5f6e  .config_source_n
-00051300: 6163 6f73 5f69 6420 6973 206e 6f74 204e  acos_id is not N
-00051310: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00051320: 2072 6573 756c 745b 2743 6f6e 6669 6753   result['ConfigS
-00051330: 6f75 7263 654e 6163 6f73 4944 275d 203d  ourceNacosID'] =
-00051340: 2073 656c 662e 636f 6e66 6967 5f73 6f75   self.config_sou
-00051350: 7263 655f 6e61 636f 735f 6964 0a20 2020  rce_nacos_id.   
-00051360: 2020 2020 2069 6620 7365 6c66 2e63 7573       if self.cus
-00051370: 746f 6d69 7a65 645f 7072 6f6d 6574 6865  tomized_promethe
-00051380: 7573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  us is not None:.
-00051390: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000513a0: 6c74 5b27 4375 7374 6f6d 697a 6564 5072  lt['CustomizedPr
-000513b0: 6f6d 6574 6865 7573 275d 203d 2073 656c  ometheus'] = sel
-000513c0: 662e 6375 7374 6f6d 697a 6564 5f70 726f  f.customized_pro
-000513d0: 6d65 7468 6575 730a 2020 2020 2020 2020  metheus.        
-000513e0: 6966 2073 656c 662e 6375 7374 6f6d 697a  if self.customiz
-000513f0: 6564 5f7a 6970 6b69 6e20 6973 206e 6f74  ed_zipkin is not
-00051400: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00051410: 2020 2072 6573 756c 745b 2743 7573 746f     result['Custo
-00051420: 6d69 7a65 645a 6970 6b69 6e27 5d20 3d20  mizedZipkin'] = 
-00051430: 7365 6c66 2e63 7573 746f 6d69 7a65 645f  self.customized_
-00051440: 7a69 706b 696e 0a20 2020 2020 2020 2069  zipkin.        i
-00051450: 6620 7365 6c66 2e64 6e73 7072 6f78 7969  f self.dnsproxyi
-00051460: 6e67 5f65 6e61 626c 6564 2069 7320 6e6f  ng_enabled is no
-00051470: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00051480: 2020 2020 7265 7375 6c74 5b27 444e 5350      result['DNSP
-00051490: 726f 7879 696e 6745 6e61 626c 6564 275d  roxyingEnabled']
-000514a0: 203d 2073 656c 662e 646e 7370 726f 7879   = self.dnsproxy
-000514b0: 696e 675f 656e 6162 6c65 640a 2020 2020  ing_enabled.    
-000514c0: 2020 2020 6966 2073 656c 662e 6469 7363      if self.disc
-000514d0: 6f76 6572 795f 7365 6c65 6374 6f72 7320  overy_selectors 
-000514e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000514f0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00051500: 2744 6973 636f 7665 7279 5365 6c65 6374  'DiscoverySelect
-00051510: 6f72 7327 5d20 3d20 7365 6c66 2e64 6973  ors'] = self.dis
-00051520: 636f 7665 7279 5f73 656c 6563 746f 7273  covery_selectors
-00051530: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00051540: 2e64 7562 626f 5f66 696c 7465 725f 656e  .dubbo_filter_en
-00051550: 6162 6c65 6420 6973 206e 6f74 204e 6f6e  abled is not Non
-00051560: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00051570: 6573 756c 745b 2744 7562 626f 4669 6c74  esult['DubboFilt
-00051580: 6572 456e 6162 6c65 6427 5d20 3d20 7365  erEnabled'] = se
-00051590: 6c66 2e64 7562 626f 5f66 696c 7465 725f  lf.dubbo_filter_
-000515a0: 656e 6162 6c65 640a 2020 2020 2020 2020  enabled.        
-000515b0: 6966 2073 656c 662e 656e 6162 6c65 5f61  if self.enable_a
-000515c0: 7564 6974 2069 7320 6e6f 7420 4e6f 6e65  udit is not None
-000515d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000515e0: 7375 6c74 5b27 456e 6162 6c65 4175 6469  sult['EnableAudi
-000515f0: 7427 5d20 3d20 7365 6c66 2e65 6e61 626c  t'] = self.enabl
-00051600: 655f 6175 6469 740a 2020 2020 2020 2020  e_audit.        
-00051610: 6966 2073 656c 662e 656e 6162 6c65 5f63  if self.enable_c
-00051620: 7268 6973 746f 7279 2069 7320 6e6f 7420  rhistory is not 
-00051630: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00051640: 2020 7265 7375 6c74 5b27 456e 6162 6c65    result['Enable
-00051650: 4352 4869 7374 6f72 7927 5d20 3d20 7365  CRHistory'] = se
-00051660: 6c66 2e65 6e61 626c 655f 6372 6869 7374  lf.enable_crhist
-00051670: 6f72 790a 2020 2020 2020 2020 6966 2073  ory.        if s
-00051680: 656c 662e 656e 6162 6c65 5f6e 616d 6573  elf.enable_names
-00051690: 7061 6365 735f 6279 5f64 6566 6175 6c74  paces_by_default
-000516a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000516b0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000516c0: 5b27 456e 6162 6c65 4e61 6d65 7370 6163  ['EnableNamespac
-000516d0: 6573 4279 4465 6661 756c 7427 5d20 3d20  esByDefault'] = 
-000516e0: 7365 6c66 2e65 6e61 626c 655f 6e61 6d65  self.enable_name
-000516f0: 7370 6163 6573 5f62 795f 6465 6661 756c  spaces_by_defaul
-00051700: 740a 2020 2020 2020 2020 6966 2073 656c  t.        if sel
-00051710: 662e 656e 6162 6c65 5f73 6473 7365 7276  f.enable_sdsserv
-00051720: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
-00051730: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00051740: 6c74 5b27 456e 6162 6c65 5344 5353 6572  lt['EnableSDSSer
-00051750: 7665 7227 5d20 3d20 7365 6c66 2e65 6e61  ver'] = self.ena
-00051760: 626c 655f 7364 7373 6572 7665 720a 2020  ble_sdsserver.  
-00051770: 2020 2020 2020 6966 2073 656c 662e 6578        if self.ex
-00051780: 636c 7564 655f 6970 7261 6e67 6573 2069  clude_ipranges i
-00051790: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000517a0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000517b0: 4578 636c 7564 6549 5052 616e 6765 7327  ExcludeIPRanges'
-000517c0: 5d20 3d20 7365 6c66 2e65 7863 6c75 6465  ] = self.exclude
-000517d0: 5f69 7072 616e 6765 730a 2020 2020 2020  _ipranges.      
-000517e0: 2020 6966 2073 656c 662e 6578 636c 7564    if self.exclud
-000517f0: 655f 696e 626f 756e 645f 706f 7274 7320  e_inbound_ports 
-00051800: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00051810: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00051820: 2745 7863 6c75 6465 496e 626f 756e 6450  'ExcludeInboundP
-00051830: 6f72 7473 275d 203d 2073 656c 662e 6578  orts'] = self.ex
-00051840: 636c 7564 655f 696e 626f 756e 645f 706f  clude_inbound_po
-00051850: 7274 730a 2020 2020 2020 2020 6966 2073  rts.        if s
-00051860: 656c 662e 6578 636c 7564 655f 6f75 7462  elf.exclude_outb
-00051870: 6f75 6e64 5f70 6f72 7473 2069 7320 6e6f  ound_ports is no
-00051880: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00051890: 2020 2020 7265 7375 6c74 5b27 4578 636c      result['Excl
-000518a0: 7564 654f 7574 626f 756e 6450 6f72 7473  udeOutboundPorts
-000518b0: 275d 203d 2073 656c 662e 6578 636c 7564  '] = self.exclud
-000518c0: 655f 6f75 7462 6f75 6e64 5f70 6f72 7473  e_outbound_ports
-000518d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000518e0: 2e66 696c 7465 725f 6761 7465 7761 795f  .filter_gateway_
-000518f0: 636c 7573 7465 725f 636f 6e66 6967 2069  cluster_config i
-00051900: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00051910: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00051920: 4669 6c74 6572 4761 7465 7761 7943 6c75  FilterGatewayClu
-00051930: 7374 6572 436f 6e66 6967 275d 203d 2073  sterConfig'] = s
-00051940: 656c 662e 6669 6c74 6572 5f67 6174 6577  elf.filter_gatew
-00051950: 6179 5f63 6c75 7374 6572 5f63 6f6e 6669  ay_cluster_confi
-00051960: 670a 2020 2020 2020 2020 6966 2073 656c  g.        if sel
-00051970: 662e 6761 7465 7761 795f 6170 6965 6e61  f.gateway_apiena
-00051980: 626c 6564 2069 7320 6e6f 7420 4e6f 6e65  bled is not None
-00051990: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000519a0: 7375 6c74 5b27 4761 7465 7761 7941 5049  sult['GatewayAPI
-000519b0: 456e 6162 6c65 6427 5d20 3d20 7365 6c66  Enabled'] = self
-000519c0: 2e67 6174 6577 6179 5f61 7069 656e 6162  .gateway_apienab
-000519d0: 6c65 640a 2020 2020 2020 2020 6966 2073  led.        if s
-000519e0: 656c 662e 676c 6f62 616c 5f72 6174 655f  elf.global_rate_
-000519f0: 6c69 6d69 745f 656e 6162 6c65 6420 6973  limit_enabled is
-00051a00: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00051a10: 2020 2020 2020 2072 6573 756c 745b 2747         result['G
-00051a20: 6c6f 6261 6c52 6174 654c 696d 6974 456e  lobalRateLimitEn
-00051a30: 6162 6c65 6427 5d20 3d20 7365 6c66 2e67  abled'] = self.g
-00051a40: 6c6f 6261 6c5f 7261 7465 5f6c 696d 6974  lobal_rate_limit
-00051a50: 5f65 6e61 626c 6564 0a20 2020 2020 2020  _enabled.       
-00051a60: 2069 6620 7365 6c66 2e68 7474 705f 3130   if self.http_10
-00051a70: 656e 6162 6c65 6420 6973 206e 6f74 204e  enabled is not N
-00051a80: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00051a90: 2072 6573 756c 745b 2748 7474 7031 3045   result['Http10E
-00051aa0: 6e61 626c 6564 275d 203d 2073 656c 662e  nabled'] = self.
-00051ab0: 6874 7470 5f31 3065 6e61 626c 6564 0a20  http_10enabled. 
-00051ac0: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
-00051ad0: 6e63 6c75 6465 5f69 7072 616e 6765 7320  nclude_ipranges 
-00051ae0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00051af0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00051b00: 2749 6e63 6c75 6465 4950 5261 6e67 6573  'IncludeIPRanges
-00051b10: 275d 203d 2073 656c 662e 696e 636c 7564  '] = self.includ
-00051b20: 655f 6970 7261 6e67 6573 0a20 2020 2020  e_ipranges.     
-00051b30: 2020 2069 6620 7365 6c66 2e69 6e63 6c75     if self.inclu
-00051b40: 6465 5f69 6e62 6f75 6e64 5f70 6f72 7473  de_inbound_ports
-00051b50: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00051b60: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00051b70: 5b27 496e 636c 7564 6549 6e62 6f75 6e64  ['IncludeInbound
-00051b80: 506f 7274 7327 5d20 3d20 7365 6c66 2e69  Ports'] = self.i
-00051b90: 6e63 6c75 6465 5f69 6e62 6f75 6e64 5f70  nclude_inbound_p
-00051ba0: 6f72 7473 0a20 2020 2020 2020 2069 6620  orts.        if 
-00051bb0: 7365 6c66 2e6b 6961 6c69 5f65 6e61 626c  self.kiali_enabl
-00051bc0: 6564 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ed is not None:.
-00051bd0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00051be0: 6c74 5b27 4b69 616c 6945 6e61 626c 6564  lt['KialiEnabled
-00051bf0: 275d 203d 2073 656c 662e 6b69 616c 695f  '] = self.kiali_
-00051c00: 656e 6162 6c65 640a 2020 2020 2020 2020  enabled.        
-00051c10: 6966 2073 656c 662e 6c69 6665 6379 636c  if self.lifecycl
-00051c20: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00051c30: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00051c40: 745b 274c 6966 6563 7963 6c65 275d 203d  t['Lifecycle'] =
-00051c50: 2073 656c 662e 6c69 6665 6379 636c 650a   self.lifecycle.
-00051c60: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00051c70: 6c6f 6361 6c69 7479 5f6c 6263 6f6e 6620  locality_lbconf 
-00051c80: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00051c90: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00051ca0: 274c 6f63 616c 6974 794c 4243 6f6e 6627  'LocalityLBConf'
-00051cb0: 5d20 3d20 7365 6c66 2e6c 6f63 616c 6974  ] = self.localit
-00051cc0: 795f 6c62 636f 6e66 0a20 2020 2020 2020  y_lbconf.       
-00051cd0: 2069 6620 7365 6c66 2e6c 6f63 616c 6974   if self.localit
-00051ce0: 795f 6c6f 6164 5f62 616c 616e 6369 6e67  y_load_balancing
-00051cf0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00051d00: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00051d10: 5b27 4c6f 6361 6c69 7479 4c6f 6164 4261  ['LocalityLoadBa
-00051d20: 6c61 6e63 696e 6727 5d20 3d20 7365 6c66  lancing'] = self
-00051d30: 2e6c 6f63 616c 6974 795f 6c6f 6164 5f62  .locality_load_b
-00051d40: 616c 616e 6369 6e67 0a20 2020 2020 2020  alancing.       
-00051d50: 2069 6620 7365 6c66 2e6d 7365 656e 6162   if self.mseenab
-00051d60: 6c65 6420 6973 206e 6f74 204e 6f6e 653a  led is not None:
-00051d70: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00051d80: 756c 745b 274d 5345 456e 6162 6c65 6427  ult['MSEEnabled'
-00051d90: 5d20 3d20 7365 6c66 2e6d 7365 656e 6162  ] = self.mseenab
-00051da0: 6c65 640a 2020 2020 2020 2020 6966 2073  led.        if s
-00051db0: 656c 662e 6d75 6c74 695f 6275 6666 6572  elf.multi_buffer
-00051dc0: 5f65 6e61 626c 6564 2069 7320 6e6f 7420  _enabled is not 
-00051dd0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00051de0: 2020 7265 7375 6c74 5b27 4d75 6c74 6942    result['MultiB
-00051df0: 7566 6665 7245 6e61 626c 6564 275d 203d  ufferEnabled'] =
-00051e00: 2073 656c 662e 6d75 6c74 695f 6275 6666   self.multi_buff
-00051e10: 6572 5f65 6e61 626c 6564 0a20 2020 2020  er_enabled.     
-00051e20: 2020 2069 6620 7365 6c66 2e6d 756c 7469     if self.multi
-00051e30: 5f62 7566 6665 725f 706f 6c6c 5f64 656c  _buffer_poll_del
-00051e40: 6179 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ay is not None:.
-00051e50: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00051e60: 6c74 5b27 4d75 6c74 6942 7566 6665 7250  lt['MultiBufferP
-00051e70: 6f6c 6c44 656c 6179 275d 203d 2073 656c  ollDelay'] = sel
-00051e80: 662e 6d75 6c74 695f 6275 6666 6572 5f70  f.multi_buffer_p
-00051e90: 6f6c 6c5f 6465 6c61 790a 2020 2020 2020  oll_delay.      
-00051ea0: 2020 6966 2073 656c 662e 6d79 7371 6c5f    if self.mysql_
-00051eb0: 6669 6c74 6572 5f65 6e61 626c 6564 2069  filter_enabled i
-00051ec0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00051ed0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00051ee0: 4d79 7371 6c46 696c 7465 7245 6e61 626c  MysqlFilterEnabl
-00051ef0: 6564 275d 203d 2073 656c 662e 6d79 7371  ed'] = self.mysq
-00051f00: 6c5f 6669 6c74 6572 5f65 6e61 626c 6564  l_filter_enabled
-00051f10: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00051f20: 2e6f 7061 6c69 6d69 745f 6370 7520 6973  .opalimit_cpu is
-00051f30: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00051f40: 2020 2020 2020 2072 6573 756c 745b 274f         result['O
-00051f50: 5041 4c69 6d69 7443 5055 275d 203d 2073  PALimitCPU'] = s
-00051f60: 656c 662e 6f70 616c 696d 6974 5f63 7075  elf.opalimit_cpu
-00051f70: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00051f80: 2e6f 7061 6c69 6d69 745f 6d65 6d6f 7279  .opalimit_memory
-00051f90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00051fa0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00051fb0: 5b27 4f50 414c 696d 6974 4d65 6d6f 7279  ['OPALimitMemory
-00051fc0: 275d 203d 2073 656c 662e 6f70 616c 696d  '] = self.opalim
-00051fd0: 6974 5f6d 656d 6f72 790a 2020 2020 2020  it_memory.      
-00051fe0: 2020 6966 2073 656c 662e 6f70 616c 6f67    if self.opalog
-00051ff0: 5f6c 6576 656c 2069 7320 6e6f 7420 4e6f  _level is not No
-00052000: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00052010: 7265 7375 6c74 5b27 4f50 414c 6f67 4c65  result['OPALogLe
-00052020: 7665 6c27 5d20 3d20 7365 6c66 2e6f 7061  vel'] = self.opa
-00052030: 6c6f 675f 6c65 7665 6c0a 2020 2020 2020  log_level.      
-00052040: 2020 6966 2073 656c 662e 6f70 6172 6571    if self.opareq
-00052050: 7565 7374 5f63 7075 2069 7320 6e6f 7420  uest_cpu is not 
-00052060: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00052070: 2020 7265 7375 6c74 5b27 4f50 4152 6571    result['OPAReq
-00052080: 7565 7374 4350 5527 5d20 3d20 7365 6c66  uestCPU'] = self
-00052090: 2e6f 7061 7265 7175 6573 745f 6370 750a  .oparequest_cpu.
-000520a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000520b0: 6f70 6172 6571 7565 7374 5f6d 656d 6f72  oparequest_memor
-000520c0: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
-000520d0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000520e0: 745b 274f 5041 5265 7175 6573 744d 656d  t['OPARequestMem
-000520f0: 6f72 7927 5d20 3d20 7365 6c66 2e6f 7061  ory'] = self.opa
-00052100: 7265 7175 6573 745f 6d65 6d6f 7279 0a20  request_memory. 
-00052110: 2020 2020 2020 2069 6620 7365 6c66 2e6f         if self.o
-00052120: 7061 5f65 6e61 626c 6564 2069 7320 6e6f  pa_enabled is no
-00052130: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00052140: 2020 2020 7265 7375 6c74 5b27 4f70 6145      result['OpaE
-00052150: 6e61 626c 6564 275d 203d 2073 656c 662e  nabled'] = self.
-00052160: 6f70 615f 656e 6162 6c65 640a 2020 2020  opa_enabled.    
-00052170: 2020 2020 6966 2073 656c 662e 6f70 656e      if self.open
-00052180: 5f61 6765 6e74 5f70 6f6c 6963 7920 6973  _agent_policy is
-00052190: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000521a0: 2020 2020 2020 2072 6573 756c 745b 274f         result['O
-000521b0: 7065 6e41 6765 6e74 506f 6c69 6379 275d  penAgentPolicy']
-000521c0: 203d 2073 656c 662e 6f70 656e 5f61 6765   = self.open_age
-000521d0: 6e74 5f70 6f6c 6963 790a 2020 2020 2020  nt_policy.      
-000521e0: 2020 6966 2073 656c 662e 6f75 7462 6f75    if self.outbou
-000521f0: 6e64 5f74 7261 6666 6963 5f70 6f6c 6963  nd_traffic_polic
-00052200: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
-00052210: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00052220: 745b 274f 7574 626f 756e 6454 7261 6666  t['OutboundTraff
-00052230: 6963 506f 6c69 6379 275d 203d 2073 656c  icPolicy'] = sel
-00052240: 662e 6f75 7462 6f75 6e64 5f74 7261 6666  f.outbound_traff
-00052250: 6963 5f70 6f6c 6963 790a 2020 2020 2020  ic_policy.      
-00052260: 2020 6966 2073 656c 662e 7072 6f6d 6574    if self.promet
-00052270: 6865 7573 5f75 726c 2069 7320 6e6f 7420  heus_url is not 
-00052280: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00052290: 2020 7265 7375 6c74 5b27 5072 6f6d 6574    result['Promet
-000522a0: 6865 7573 5572 6c27 5d20 3d20 7365 6c66  heusUrl'] = self
-000522b0: 2e70 726f 6d65 7468 6575 735f 7572 6c0a  .prometheus_url.
-000522c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000522d0: 7072 6f78 795f 696e 6974 5f63 7075 7265  proxy_init_cpure
-000522e0: 736f 7572 6365 5f6c 696d 6974 2069 7320  source_limit is 
-000522f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00052300: 2020 2020 2020 7265 7375 6c74 5b27 5072        result['Pr
-00052310: 6f78 7949 6e69 7443 5055 5265 736f 7572  oxyInitCPUResour
-00052320: 6365 4c69 6d69 7427 5d20 3d20 7365 6c66  ceLimit'] = self
-00052330: 2e70 726f 7879 5f69 6e69 745f 6370 7572  .proxy_init_cpur
-00052340: 6573 6f75 7263 655f 6c69 6d69 740a 2020  esource_limit.  
-00052350: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-00052360: 6f78 795f 696e 6974 5f63 7075 7265 736f  oxy_init_cpureso
-00052370: 7572 6365 5f72 6571 7565 7374 2069 7320  urce_request is 
-00052380: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00052390: 2020 2020 2020 7265 7375 6c74 5b27 5072        result['Pr
-000523a0: 6f78 7949 6e69 7443 5055 5265 736f 7572  oxyInitCPUResour
-000523b0: 6365 5265 7175 6573 7427 5d20 3d20 7365  ceRequest'] = se
-000523c0: 6c66 2e70 726f 7879 5f69 6e69 745f 6370  lf.proxy_init_cp
-000523d0: 7572 6573 6f75 7263 655f 7265 7175 6573  uresource_reques
-000523e0: 740a 2020 2020 2020 2020 6966 2073 656c  t.        if sel
-000523f0: 662e 7072 6f78 795f 696e 6974 5f6d 656d  f.proxy_init_mem
-00052400: 6f72 795f 7265 736f 7572 6365 5f6c 696d  ory_resource_lim
-00052410: 6974 2069 7320 6e6f 7420 4e6f 6e65 3a0a  it is not None:.
-00052420: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00052430: 6c74 5b27 5072 6f78 7949 6e69 744d 656d  lt['ProxyInitMem
-00052440: 6f72 7952 6573 6f75 7263 654c 696d 6974  oryResourceLimit
-00052450: 275d 203d 2073 656c 662e 7072 6f78 795f  '] = self.proxy_
-00052460: 696e 6974 5f6d 656d 6f72 795f 7265 736f  init_memory_reso
-00052470: 7572 6365 5f6c 696d 6974 0a20 2020 2020  urce_limit.     
-00052480: 2020 2069 6620 7365 6c66 2e70 726f 7879     if self.proxy
-00052490: 5f69 6e69 745f 6d65 6d6f 7279 5f72 6573  _init_memory_res
-000524a0: 6f75 7263 655f 7265 7175 6573 7420 6973  ource_request is
-000524b0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000524c0: 2020 2020 2020 2072 6573 756c 745b 2750         result['P
-000524d0: 726f 7879 496e 6974 4d65 6d6f 7279 5265  roxyInitMemoryRe
-000524e0: 736f 7572 6365 5265 7175 6573 7427 5d20  sourceRequest'] 
-000524f0: 3d20 7365 6c66 2e70 726f 7879 5f69 6e69  = self.proxy_ini
-00052500: 745f 6d65 6d6f 7279 5f72 6573 6f75 7263  t_memory_resourc
-00052510: 655f 7265 7175 6573 740a 2020 2020 2020  e_request.      
-00052520: 2020 6966 2073 656c 662e 7072 6f78 795f    if self.proxy_
-00052530: 6c69 6d69 745f 6370 7520 6973 206e 6f74  limit_cpu is not
-00052540: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00052550: 2020 2072 6573 756c 745b 2750 726f 7879     result['Proxy
-00052560: 4c69 6d69 7443 5055 275d 203d 2073 656c  LimitCPU'] = sel
-00052570: 662e 7072 6f78 795f 6c69 6d69 745f 6370  f.proxy_limit_cp
-00052580: 750a 2020 2020 2020 2020 6966 2073 656c  u.        if sel
-00052590: 662e 7072 6f78 795f 6c69 6d69 745f 6d65  f.proxy_limit_me
-000525a0: 6d6f 7279 2069 7320 6e6f 7420 4e6f 6e65  mory is not None
-000525b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000525c0: 7375 6c74 5b27 5072 6f78 794c 696d 6974  sult['ProxyLimit
-000525d0: 4d65 6d6f 7279 275d 203d 2073 656c 662e  Memory'] = self.
-000525e0: 7072 6f78 795f 6c69 6d69 745f 6d65 6d6f  proxy_limit_memo
-000525f0: 7279 0a20 2020 2020 2020 2069 6620 7365  ry.        if se
-00052600: 6c66 2e70 726f 7879 5f72 6571 7565 7374  lf.proxy_request
-00052610: 5f63 7075 2069 7320 6e6f 7420 4e6f 6e65  _cpu is not None
-00052620: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00052630: 7375 6c74 5b27 5072 6f78 7952 6571 7565  sult['ProxyReque
-00052640: 7374 4350 5527 5d20 3d20 7365 6c66 2e70  stCPU'] = self.p
-00052650: 726f 7879 5f72 6571 7565 7374 5f63 7075  roxy_request_cpu
-00052660: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00052670: 2e70 726f 7879 5f72 6571 7565 7374 5f6d  .proxy_request_m
-00052680: 656d 6f72 7920 6973 206e 6f74 204e 6f6e  emory is not Non
-00052690: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000526a0: 6573 756c 745b 2750 726f 7879 5265 7175  esult['ProxyRequ
-000526b0: 6573 744d 656d 6f72 7927 5d20 3d20 7365  estMemory'] = se
-000526c0: 6c66 2e70 726f 7879 5f72 6571 7565 7374  lf.proxy_request
-000526d0: 5f6d 656d 6f72 790a 2020 2020 2020 2020  _memory.        
-000526e0: 6966 2073 656c 662e 7265 6469 735f 6669  if self.redis_fi
-000526f0: 6c74 6572 5f65 6e61 626c 6564 2069 7320  lter_enabled is 
-00052700: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00052710: 2020 2020 2020 7265 7375 6c74 5b27 5265        result['Re
-00052720: 6469 7346 696c 7465 7245 6e61 626c 6564  disFilterEnabled
-00052730: 275d 203d 2073 656c 662e 7265 6469 735f  '] = self.redis_
-00052740: 6669 6c74 6572 5f65 6e61 626c 6564 0a20  filter_enabled. 
-00052750: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00052760: 6572 7669 6365 5f6d 6573 685f 6964 2069  ervice_mesh_id i
-00052770: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00052780: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00052790: 5365 7276 6963 654d 6573 6849 6427 5d20  ServiceMeshId'] 
-000527a0: 3d20 7365 6c66 2e73 6572 7669 6365 5f6d  = self.service_m
-000527b0: 6573 685f 6964 0a20 2020 2020 2020 2069  esh_id.        i
-000527c0: 6620 7365 6c66 2e73 6964 6563 6172 5f69  f self.sidecar_i
-000527d0: 6e6a 6563 746f 725f 6c69 6d69 745f 6370  njector_limit_cp
-000527e0: 7520 6973 206e 6f74 204e 6f6e 653a 0a20  u is not None:. 
-000527f0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00052800: 745b 2753 6964 6563 6172 496e 6a65 6374  t['SidecarInject
-00052810: 6f72 4c69 6d69 7443 5055 275d 203d 2073  orLimitCPU'] = s
-00052820: 656c 662e 7369 6465 6361 725f 696e 6a65  elf.sidecar_inje
-00052830: 6374 6f72 5f6c 696d 6974 5f63 7075 0a20  ctor_limit_cpu. 
-00052840: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00052850: 6964 6563 6172 5f69 6e6a 6563 746f 725f  idecar_injector_
-00052860: 6c69 6d69 745f 6d65 6d6f 7279 2069 7320  limit_memory is 
-00052870: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00052880: 2020 2020 2020 7265 7375 6c74 5b27 5369        result['Si
-00052890: 6465 6361 7249 6e6a 6563 746f 724c 696d  decarInjectorLim
-000528a0: 6974 4d65 6d6f 7279 275d 203d 2073 656c  itMemory'] = sel
-000528b0: 662e 7369 6465 6361 725f 696e 6a65 6374  f.sidecar_inject
-000528c0: 6f72 5f6c 696d 6974 5f6d 656d 6f72 790a  or_limit_memory.
-000528d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000528e0: 7369 6465 6361 725f 696e 6a65 6374 6f72  sidecar_injector
-000528f0: 5f72 6571 7565 7374 5f63 7075 2069 7320  _request_cpu is 
-00052900: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00052910: 2020 2020 2020 7265 7375 6c74 5b27 5369        result['Si
-00052920: 6465 6361 7249 6e6a 6563 746f 7252 6571  decarInjectorReq
-00052930: 7565 7374 4350 5527 5d20 3d20 7365 6c66  uestCPU'] = self
-00052940: 2e73 6964 6563 6172 5f69 6e6a 6563 746f  .sidecar_injecto
-00052950: 725f 7265 7175 6573 745f 6370 750a 2020  r_request_cpu.  
-00052960: 2020 2020 2020 6966 2073 656c 662e 7369        if self.si
-00052970: 6465 6361 725f 696e 6a65 6374 6f72 5f72  decar_injector_r
-00052980: 6571 7565 7374 5f6d 656d 6f72 7920 6973  equest_memory is
-00052990: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000529a0: 2020 2020 2020 2072 6573 756c 745b 2753         result['S
-000529b0: 6964 6563 6172 496e 6a65 6374 6f72 5265  idecarInjectorRe
-000529c0: 7175 6573 744d 656d 6f72 7927 5d20 3d20  questMemory'] = 
-000529d0: 7365 6c66 2e73 6964 6563 6172 5f69 6e6a  self.sidecar_inj
-000529e0: 6563 746f 725f 7265 7175 6573 745f 6d65  ector_request_me
-000529f0: 6d6f 7279 0a20 2020 2020 2020 2069 6620  mory.        if 
-00052a00: 7365 6c66 2e73 6964 6563 6172 5f69 6e6a  self.sidecar_inj
-00052a10: 6563 746f 725f 7765 6268 6f6f 6b5f 6173  ector_webhook_as
-00052a20: 5f79 616d 6c20 6973 206e 6f74 204e 6f6e  _yaml is not Non
-00052a30: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00052a40: 6573 756c 745b 2753 6964 6563 6172 496e  esult['SidecarIn
-00052a50: 6a65 6374 6f72 5765 6268 6f6f 6b41 7359  jectorWebhookAsY
-00052a60: 616d 6c27 5d20 3d20 7365 6c66 2e73 6964  aml'] = self.sid
-00052a70: 6563 6172 5f69 6e6a 6563 746f 725f 7765  ecar_injector_we
-00052a80: 6268 6f6f 6b5f 6173 5f79 616d 6c0a 2020  bhook_as_yaml.  
-00052a90: 2020 2020 2020 6966 2073 656c 662e 7465        if self.te
-00052aa0: 6c65 6d65 7472 7920 6973 206e 6f74 204e  lemetry is not N
-00052ab0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00052ac0: 2072 6573 756c 745b 2754 656c 656d 6574   result['Telemet
-00052ad0: 7279 275d 203d 2073 656c 662e 7465 6c65  ry'] = self.tele
-00052ae0: 6d65 7472 790a 2020 2020 2020 2020 6966  metry.        if
-00052af0: 2073 656c 662e 7465 726d 696e 6174 696f   self.terminatio
-00052b00: 6e5f 6472 6169 6e5f 6475 7261 7469 6f6e  n_drain_duration
-00052b10: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00052b20: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00052b30: 5b27 5465 726d 696e 6174 696f 6e44 7261  ['TerminationDra
-00052b40: 696e 4475 7261 7469 6f6e 275d 203d 2073  inDuration'] = s
-00052b50: 656c 662e 7465 726d 696e 6174 696f 6e5f  elf.termination_
-00052b60: 6472 6169 6e5f 6475 7261 7469 6f6e 0a20  drain_duration. 
-00052b70: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
-00052b80: 6872 6966 745f 6669 6c74 6572 5f65 6e61  hrift_filter_ena
-00052b90: 626c 6564 2069 7320 6e6f 7420 4e6f 6e65  bled is not None
-00052ba0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00052bb0: 7375 6c74 5b27 5468 7269 6674 4669 6c74  sult['ThriftFilt
-00052bc0: 6572 456e 6162 6c65 6427 5d20 3d20 7365  erEnabled'] = se
-00052bd0: 6c66 2e74 6872 6966 745f 6669 6c74 6572  lf.thrift_filter
-00052be0: 5f65 6e61 626c 6564 0a20 2020 2020 2020  _enabled.       
-00052bf0: 2069 6620 7365 6c66 2e74 7261 6365 5f73   if self.trace_s
-00052c00: 616d 706c 696e 6720 6973 206e 6f74 204e  ampling is not N
-00052c10: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00052c20: 2072 6573 756c 745b 2754 7261 6365 5361   result['TraceSa
-00052c30: 6d70 6c69 6e67 275d 203d 2073 656c 662e  mpling'] = self.
-00052c40: 7472 6163 655f 7361 6d70 6c69 6e67 0a20  trace_sampling. 
-00052c50: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
-00052c60: 7261 6369 6e67 2069 7320 6e6f 7420 4e6f  racing is not No
-00052c70: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00052c80: 7265 7375 6c74 5b27 5472 6163 696e 6727  result['Tracing'
-00052c90: 5d20 3d20 7365 6c66 2e74 7261 6369 6e67  ] = self.tracing
-00052ca0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00052cb0: 2e77 6562 5f61 7373 656d 626c 795f 6669  .web_assembly_fi
-00052cc0: 6c74 6572 5f65 6e61 626c 6564 2069 7320  lter_enabled is 
-00052cd0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00052ce0: 2020 2020 2020 7265 7375 6c74 5b27 5765        result['We
-00052cf0: 6241 7373 656d 626c 7946 696c 7465 7245  bAssemblyFilterE
-00052d00: 6e61 626c 6564 275d 203d 2073 656c 662e  nabled'] = self.
-00052d10: 7765 625f 6173 7365 6d62 6c79 5f66 696c  web_assembly_fil
-00052d20: 7465 725f 656e 6162 6c65 640a 2020 2020  ter_enabled.    
-00052d30: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00052d40: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-00052d50: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-00052d60: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-00052d70: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-00052d80: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-00052d90: 6765 7428 2741 6363 6573 734c 6f67 456e  get('AccessLogEn
-00052da0: 6162 6c65 6427 2920 6973 206e 6f74 204e  abled') is not N
-00052db0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00052dc0: 2073 656c 662e 6163 6365 7373 5f6c 6f67   self.access_log
-00052dd0: 5f65 6e61 626c 6564 203d 206d 2e67 6574  _enabled = m.get
-00052de0: 2827 4163 6365 7373 4c6f 6745 6e61 626c  ('AccessLogEnabl
-00052df0: 6564 2729 0a20 2020 2020 2020 2069 6620  ed').        if 
-00052e00: 6d2e 6765 7428 2741 6363 6573 734c 6f67  m.get('AccessLog
-00052e10: 4669 6c65 2729 2069 7320 6e6f 7420 4e6f  File') is not No
-00052e20: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00052e30: 7365 6c66 2e61 6363 6573 735f 6c6f 675f  self.access_log_
-00052e40: 6669 6c65 203d 206d 2e67 6574 2827 4163  file = m.get('Ac
-00052e50: 6365 7373 4c6f 6746 696c 6527 290a 2020  cessLogFile').  
-00052e60: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00052e70: 4163 6365 7373 4c6f 6746 6f72 6d61 7427  AccessLogFormat'
-00052e80: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00052e90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00052ea0: 6163 6365 7373 5f6c 6f67 5f66 6f72 6d61  access_log_forma
-00052eb0: 7420 3d20 6d2e 6765 7428 2741 6363 6573  t = m.get('Acces
-00052ec0: 734c 6f67 466f 726d 6174 2729 0a20 2020  sLogFormat').   
-00052ed0: 2020 2020 2069 6620 6d2e 6765 7428 2741       if m.get('A
-00052ee0: 6363 6573 734c 6f67 5072 6f6a 6563 7427  ccessLogProject'
-00052ef0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00052f00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00052f10: 6163 6365 7373 5f6c 6f67 5f70 726f 6a65  access_log_proje
-00052f20: 6374 203d 206d 2e67 6574 2827 4163 6365  ct = m.get('Acce
-00052f30: 7373 4c6f 6750 726f 6a65 6374 2729 0a20  ssLogProject'). 
-00052f40: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00052f50: 2741 6363 6573 734c 6f67 5365 7276 6963  'AccessLogServic
-00052f60: 6545 6e61 626c 6564 2729 2069 7320 6e6f  eEnabled') is no
-00052f70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00052f80: 2020 2020 7365 6c66 2e61 6363 6573 735f      self.access_
-00052f90: 6c6f 675f 7365 7276 6963 655f 656e 6162  log_service_enab
-00052fa0: 6c65 6420 3d20 6d2e 6765 7428 2741 6363  led = m.get('Acc
-00052fb0: 6573 734c 6f67 5365 7276 6963 6545 6e61  essLogServiceEna
-00052fc0: 626c 6564 2729 0a20 2020 2020 2020 2069  bled').        i
-00052fd0: 6620 6d2e 6765 7428 2741 6363 6573 734c  f m.get('AccessL
-00052fe0: 6f67 5365 7276 6963 6548 6f73 7427 2920  ogServiceHost') 
-00052ff0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00053000: 2020 2020 2020 2020 2073 656c 662e 6163           self.ac
-00053010: 6365 7373 5f6c 6f67 5f73 6572 7669 6365  cess_log_service
-00053020: 5f68 6f73 7420 3d20 6d2e 6765 7428 2741  _host = m.get('A
-00053030: 6363 6573 734c 6f67 5365 7276 6963 6548  ccessLogServiceH
-00053040: 6f73 7427 290a 2020 2020 2020 2020 6966  ost').        if
-00053050: 206d 2e67 6574 2827 4163 6365 7373 4c6f   m.get('AccessLo
-00053060: 6753 6572 7669 6365 506f 7274 2729 2069  gServicePort') i
-00053070: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00053080: 2020 2020 2020 2020 7365 6c66 2e61 6363          self.acc
-00053090: 6573 735f 6c6f 675f 7365 7276 6963 655f  ess_log_service_
-000530a0: 706f 7274 203d 206d 2e67 6574 2827 4163  port = m.get('Ac
-000530b0: 6365 7373 4c6f 6753 6572 7669 6365 506f  cessLogServicePo
-000530c0: 7274 2729 0a20 2020 2020 2020 2069 6620  rt').        if 
-000530d0: 6d2e 6765 7428 2741 7564 6974 5072 6f6a  m.get('AuditProj
-000530e0: 6563 7427 2920 6973 206e 6f74 204e 6f6e  ect') is not Non
-000530f0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00053100: 656c 662e 6175 6469 745f 7072 6f6a 6563  elf.audit_projec
-00053110: 7420 3d20 6d2e 6765 7428 2741 7564 6974  t = m.get('Audit
-00053120: 5072 6f6a 6563 7427 290a 2020 2020 2020  Project').      
-00053130: 2020 6966 206d 2e67 6574 2827 4175 746f    if m.get('Auto
-00053140: 496e 6a65 6374 696f 6e50 6f6c 6963 7945  InjectionPolicyE
-00053150: 6e61 626c 6564 2729 2069 7320 6e6f 7420  nabled') is not 
-00053160: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00053170: 2020 7365 6c66 2e61 7574 6f5f 696e 6a65    self.auto_inje
-00053180: 6374 696f 6e5f 706f 6c69 6379 5f65 6e61  ction_policy_ena
-00053190: 626c 6564 203d 206d 2e67 6574 2827 4175  bled = m.get('Au
-000531a0: 746f 496e 6a65 6374 696f 6e50 6f6c 6963  toInjectionPolic
-000531b0: 7945 6e61 626c 6564 2729 0a20 2020 2020  yEnabled').     
-000531c0: 2020 2069 6620 6d2e 6765 7428 2743 5241     if m.get('CRA
-000531d0: 6767 7265 6761 7469 6f6e 456e 6162 6c65  ggregationEnable
-000531e0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-000531f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00053200: 662e 6372 6167 6772 6567 6174 696f 6e5f  f.craggregation_
-00053210: 656e 6162 6c65 6420 3d20 6d2e 6765 7428  enabled = m.get(
-00053220: 2743 5241 6767 7265 6761 7469 6f6e 456e  'CRAggregationEn
-00053230: 6162 6c65 6427 290a 2020 2020 2020 2020  abled').        
-00053240: 6966 206d 2e67 6574 2827 436c 7573 7465  if m.get('Cluste
-00053250: 7253 7065 6327 2920 6973 206e 6f74 204e  rSpec') is not N
-00053260: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00053270: 2073 656c 662e 636c 7573 7465 725f 7370   self.cluster_sp
-00053280: 6563 203d 206d 2e67 6574 2827 436c 7573  ec = m.get('Clus
-00053290: 7465 7253 7065 6327 290a 2020 2020 2020  terSpec').      
-000532a0: 2020 6966 206d 2e67 6574 2827 436e 6945    if m.get('CniE
-000532b0: 6e61 626c 6564 2729 2069 7320 6e6f 7420  nabled') is not 
-000532c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000532d0: 2020 7365 6c66 2e63 6e69 5f65 6e61 626c    self.cni_enabl
-000532e0: 6564 203d 206d 2e67 6574 2827 436e 6945  ed = m.get('CniE
-000532f0: 6e61 626c 6564 2729 0a20 2020 2020 2020  nabled').       
-00053300: 2069 6620 6d2e 6765 7428 2743 6e69 4578   if m.get('CniEx
-00053310: 636c 7564 654e 616d 6573 7061 6365 7327  cludeNamespaces'
-00053320: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00053330: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00053340: 636e 695f 6578 636c 7564 655f 6e61 6d65  cni_exclude_name
-00053350: 7370 6163 6573 203d 206d 2e67 6574 2827  spaces = m.get('
-00053360: 436e 6945 7863 6c75 6465 4e61 6d65 7370  CniExcludeNamesp
-00053370: 6163 6573 2729 0a20 2020 2020 2020 2069  aces').        i
-00053380: 6620 6d2e 6765 7428 2743 6f6e 6669 6753  f m.get('ConfigS
-00053390: 6f75 7263 6545 6e61 626c 6564 2729 2069  ourceEnabled') i
-000533a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000533b0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-000533c0: 6669 675f 736f 7572 6365 5f65 6e61 626c  fig_source_enabl
-000533d0: 6564 203d 206d 2e67 6574 2827 436f 6e66  ed = m.get('Conf
-000533e0: 6967 536f 7572 6365 456e 6162 6c65 6427  igSourceEnabled'
-000533f0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00053400: 6574 2827 436f 6e66 6967 536f 7572 6365  et('ConfigSource
-00053410: 4e61 636f 7349 4427 2920 6973 206e 6f74  NacosID') is not
-00053420: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00053430: 2020 2073 656c 662e 636f 6e66 6967 5f73     self.config_s
-00053440: 6f75 7263 655f 6e61 636f 735f 6964 203d  ource_nacos_id =
-00053450: 206d 2e67 6574 2827 436f 6e66 6967 536f   m.get('ConfigSo
-00053460: 7572 6365 4e61 636f 7349 4427 290a 2020  urceNacosID').  
-00053470: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00053480: 4375 7374 6f6d 697a 6564 5072 6f6d 6574  CustomizedPromet
-00053490: 6865 7573 2729 2069 7320 6e6f 7420 4e6f  heus') is not No
-000534a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000534b0: 7365 6c66 2e63 7573 746f 6d69 7a65 645f  self.customized_
-000534c0: 7072 6f6d 6574 6865 7573 203d 206d 2e67  prometheus = m.g
-000534d0: 6574 2827 4375 7374 6f6d 697a 6564 5072  et('CustomizedPr
-000534e0: 6f6d 6574 6865 7573 2729 0a20 2020 2020  ometheus').     
-000534f0: 2020 2069 6620 6d2e 6765 7428 2743 7573     if m.get('Cus
-00053500: 746f 6d69 7a65 645a 6970 6b69 6e27 2920  tomizedZipkin') 
-00053510: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00053520: 2020 2020 2020 2020 2073 656c 662e 6375           self.cu
-00053530: 7374 6f6d 697a 6564 5f7a 6970 6b69 6e20  stomized_zipkin 
-00053540: 3d20 6d2e 6765 7428 2743 7573 746f 6d69  = m.get('Customi
-00053550: 7a65 645a 6970 6b69 6e27 290a 2020 2020  zedZipkin').    
-00053560: 2020 2020 6966 206d 2e67 6574 2827 444e      if m.get('DN
-00053570: 5350 726f 7879 696e 6745 6e61 626c 6564  SProxyingEnabled
-00053580: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00053590: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000535a0: 2e64 6e73 7072 6f78 7969 6e67 5f65 6e61  .dnsproxying_ena
-000535b0: 626c 6564 203d 206d 2e67 6574 2827 444e  bled = m.get('DN
-000535c0: 5350 726f 7879 696e 6745 6e61 626c 6564  SProxyingEnabled
-000535d0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000535e0: 6765 7428 2744 6973 636f 7665 7279 5365  get('DiscoverySe
-000535f0: 6c65 6374 6f72 7327 2920 6973 206e 6f74  lectors') is not
-00053600: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00053610: 2020 2073 656c 662e 6469 7363 6f76 6572     self.discover
-00053620: 795f 7365 6c65 6374 6f72 7320 3d20 6d2e  y_selectors = m.
-00053630: 6765 7428 2744 6973 636f 7665 7279 5365  get('DiscoverySe
-00053640: 6c65 6374 6f72 7327 290a 2020 2020 2020  lectors').      
-00053650: 2020 6966 206d 2e67 6574 2827 4475 6262    if m.get('Dubb
-00053660: 6f46 696c 7465 7245 6e61 626c 6564 2729  oFilterEnabled')
-00053670: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00053680: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00053690: 7562 626f 5f66 696c 7465 725f 656e 6162  ubbo_filter_enab
-000536a0: 6c65 6420 3d20 6d2e 6765 7428 2744 7562  led = m.get('Dub
-000536b0: 626f 4669 6c74 6572 456e 6162 6c65 6427  boFilterEnabled'
-000536c0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000536d0: 6574 2827 456e 6162 6c65 4175 6469 7427  et('EnableAudit'
-000536e0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000536f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00053700: 656e 6162 6c65 5f61 7564 6974 203d 206d  enable_audit = m
-00053710: 2e67 6574 2827 456e 6162 6c65 4175 6469  .get('EnableAudi
-00053720: 7427 290a 2020 2020 2020 2020 6966 206d  t').        if m
-00053730: 2e67 6574 2827 456e 6162 6c65 4352 4869  .get('EnableCRHi
-00053740: 7374 6f72 7927 2920 6973 206e 6f74 204e  story') is not N
-00053750: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00053760: 2073 656c 662e 656e 6162 6c65 5f63 7268   self.enable_crh
-00053770: 6973 746f 7279 203d 206d 2e67 6574 2827  istory = m.get('
-00053780: 456e 6162 6c65 4352 4869 7374 6f72 7927  EnableCRHistory'
-00053790: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000537a0: 6574 2827 456e 6162 6c65 4e61 6d65 7370  et('EnableNamesp
-000537b0: 6163 6573 4279 4465 6661 756c 7427 2920  acesByDefault') 
-000537c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000537d0: 2020 2020 2020 2020 2073 656c 662e 656e           self.en
-000537e0: 6162 6c65 5f6e 616d 6573 7061 6365 735f  able_namespaces_
-000537f0: 6279 5f64 6566 6175 6c74 203d 206d 2e67  by_default = m.g
-00053800: 6574 2827 456e 6162 6c65 4e61 6d65 7370  et('EnableNamesp
-00053810: 6163 6573 4279 4465 6661 756c 7427 290a  acesByDefault').
-00053820: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00053830: 2827 456e 6162 6c65 5344 5353 6572 7665  ('EnableSDSServe
-00053840: 7227 2920 6973 206e 6f74 204e 6f6e 653a  r') is not None:
-00053850: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00053860: 662e 656e 6162 6c65 5f73 6473 7365 7276  f.enable_sdsserv
-00053870: 6572 203d 206d 2e67 6574 2827 456e 6162  er = m.get('Enab
-00053880: 6c65 5344 5353 6572 7665 7227 290a 2020  leSDSServer').  
-00053890: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000538a0: 4578 636c 7564 6549 5052 616e 6765 7327  ExcludeIPRanges'
-000538b0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000538c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000538d0: 6578 636c 7564 655f 6970 7261 6e67 6573  exclude_ipranges
-000538e0: 203d 206d 2e67 6574 2827 4578 636c 7564   = m.get('Exclud
-000538f0: 6549 5052 616e 6765 7327 290a 2020 2020  eIPRanges').    
-00053900: 2020 2020 6966 206d 2e67 6574 2827 4578      if m.get('Ex
-00053910: 636c 7564 6549 6e62 6f75 6e64 506f 7274  cludeInboundPort
-00053920: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
-00053930: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00053940: 662e 6578 636c 7564 655f 696e 626f 756e  f.exclude_inboun
-00053950: 645f 706f 7274 7320 3d20 6d2e 6765 7428  d_ports = m.get(
-00053960: 2745 7863 6c75 6465 496e 626f 756e 6450  'ExcludeInboundP
-00053970: 6f72 7473 2729 0a20 2020 2020 2020 2069  orts').        i
-00053980: 6620 6d2e 6765 7428 2745 7863 6c75 6465  f m.get('Exclude
-00053990: 4f75 7462 6f75 6e64 506f 7274 7327 2920  OutboundPorts') 
-000539a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000539b0: 2020 2020 2020 2020 2073 656c 662e 6578           self.ex
-000539c0: 636c 7564 655f 6f75 7462 6f75 6e64 5f70  clude_outbound_p
-000539d0: 6f72 7473 203d 206d 2e67 6574 2827 4578  orts = m.get('Ex
-000539e0: 636c 7564 654f 7574 626f 756e 6450 6f72  cludeOutboundPor
-000539f0: 7473 2729 0a20 2020 2020 2020 2069 6620  ts').        if 
-00053a00: 6d2e 6765 7428 2746 696c 7465 7247 6174  m.get('FilterGat
-00053a10: 6577 6179 436c 7573 7465 7243 6f6e 6669  ewayClusterConfi
-00053a20: 6727 2920 6973 206e 6f74 204e 6f6e 653a  g') is not None:
-00053a30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00053a40: 662e 6669 6c74 6572 5f67 6174 6577 6179  f.filter_gateway
-00053a50: 5f63 6c75 7374 6572 5f63 6f6e 6669 6720  _cluster_config 
-00053a60: 3d20 6d2e 6765 7428 2746 696c 7465 7247  = m.get('FilterG
-00053a70: 6174 6577 6179 436c 7573 7465 7243 6f6e  atewayClusterCon
-00053a80: 6669 6727 290a 2020 2020 2020 2020 6966  fig').        if
-00053a90: 206d 2e67 6574 2827 4761 7465 7761 7941   m.get('GatewayA
-00053aa0: 5049 456e 6162 6c65 6427 2920 6973 206e  PIEnabled') is n
-00053ab0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00053ac0: 2020 2020 2073 656c 662e 6761 7465 7761       self.gatewa
-00053ad0: 795f 6170 6965 6e61 626c 6564 203d 206d  y_apienabled = m
-00053ae0: 2e67 6574 2827 4761 7465 7761 7941 5049  .get('GatewayAPI
-00053af0: 456e 6162 6c65 6427 290a 2020 2020 2020  Enabled').      
-00053b00: 2020 6966 206d 2e67 6574 2827 476c 6f62    if m.get('Glob
-00053b10: 616c 5261 7465 4c69 6d69 7445 6e61 626c  alRateLimitEnabl
-00053b20: 6564 2729 2069 7320 6e6f 7420 4e6f 6e65  ed') is not None
-00053b30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00053b40: 6c66 2e67 6c6f 6261 6c5f 7261 7465 5f6c  lf.global_rate_l
-00053b50: 696d 6974 5f65 6e61 626c 6564 203d 206d  imit_enabled = m
-00053b60: 2e67 6574 2827 476c 6f62 616c 5261 7465  .get('GlobalRate
-00053b70: 4c69 6d69 7445 6e61 626c 6564 2729 0a20  LimitEnabled'). 
-00053b80: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00053b90: 2748 7474 7031 3045 6e61 626c 6564 2729  'Http10Enabled')
-00053ba0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00053bb0: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
-00053bc0: 7474 705f 3130 656e 6162 6c65 6420 3d20  ttp_10enabled = 
-00053bd0: 6d2e 6765 7428 2748 7474 7031 3045 6e61  m.get('Http10Ena
-00053be0: 626c 6564 2729 0a20 2020 2020 2020 2069  bled').        i
-00053bf0: 6620 6d2e 6765 7428 2749 6e63 6c75 6465  f m.get('Include
-00053c00: 4950 5261 6e67 6573 2729 2069 7320 6e6f  IPRanges') is no
-00053c10: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00053c20: 2020 2020 7365 6c66 2e69 6e63 6c75 6465      self.include
-00053c30: 5f69 7072 616e 6765 7320 3d20 6d2e 6765  _ipranges = m.ge
-00053c40: 7428 2749 6e63 6c75 6465 4950 5261 6e67  t('IncludeIPRang
-00053c50: 6573 2729 0a20 2020 2020 2020 2069 6620  es').        if 
-00053c60: 6d2e 6765 7428 2749 6e63 6c75 6465 496e  m.get('IncludeIn
-00053c70: 626f 756e 6450 6f72 7473 2729 2069 7320  boundPorts') is 
-00053c80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00053c90: 2020 2020 2020 7365 6c66 2e69 6e63 6c75        self.inclu
-00053ca0: 6465 5f69 6e62 6f75 6e64 5f70 6f72 7473  de_inbound_ports
-00053cb0: 203d 206d 2e67 6574 2827 496e 636c 7564   = m.get('Includ
-00053cc0: 6549 6e62 6f75 6e64 506f 7274 7327 290a  eInboundPorts').
-00053cd0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00053ce0: 2827 4b69 616c 6945 6e61 626c 6564 2729  ('KialiEnabled')
-00053cf0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00053d00: 2020 2020 2020 2020 2020 7365 6c66 2e6b            self.k
-00053d10: 6961 6c69 5f65 6e61 626c 6564 203d 206d  iali_enabled = m
-00053d20: 2e67 6574 2827 4b69 616c 6945 6e61 626c  .get('KialiEnabl
-00053d30: 6564 2729 0a20 2020 2020 2020 2069 6620  ed').        if 
-00053d40: 6d2e 6765 7428 274c 6966 6563 7963 6c65  m.get('Lifecycle
-00053d50: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00053d60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00053d70: 2e6c 6966 6563 7963 6c65 203d 206d 2e67  .lifecycle = m.g
-00053d80: 6574 2827 4c69 6665 6379 636c 6527 290a  et('Lifecycle').
-00053d90: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00053da0: 2827 4c6f 6361 6c69 7479 4c42 436f 6e66  ('LocalityLBConf
-00053db0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00053dc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00053dd0: 2e6c 6f63 616c 6974 795f 6c62 636f 6e66  .locality_lbconf
-00053de0: 203d 206d 2e67 6574 2827 4c6f 6361 6c69   = m.get('Locali
-00053df0: 7479 4c42 436f 6e66 2729 0a20 2020 2020  tyLBConf').     
-00053e00: 2020 2069 6620 6d2e 6765 7428 274c 6f63     if m.get('Loc
-00053e10: 616c 6974 794c 6f61 6442 616c 616e 6369  alityLoadBalanci
-00053e20: 6e67 2729 2069 7320 6e6f 7420 4e6f 6e65  ng') is not None
-00053e30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00053e40: 6c66 2e6c 6f63 616c 6974 795f 6c6f 6164  lf.locality_load
-00053e50: 5f62 616c 616e 6369 6e67 203d 206d 2e67  _balancing = m.g
-00053e60: 6574 2827 4c6f 6361 6c69 7479 4c6f 6164  et('LocalityLoad
-00053e70: 4261 6c61 6e63 696e 6727 290a 2020 2020  Balancing').    
-00053e80: 2020 2020 6966 206d 2e67 6574 2827 4d53      if m.get('MS
-00053e90: 4545 6e61 626c 6564 2729 2069 7320 6e6f  EEnabled') is no
-00053ea0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00053eb0: 2020 2020 7365 6c66 2e6d 7365 656e 6162      self.mseenab
-00053ec0: 6c65 6420 3d20 6d2e 6765 7428 274d 5345  led = m.get('MSE
-00053ed0: 456e 6162 6c65 6427 290a 2020 2020 2020  Enabled').      
-00053ee0: 2020 6966 206d 2e67 6574 2827 4d75 6c74    if m.get('Mult
-00053ef0: 6942 7566 6665 7245 6e61 626c 6564 2729  iBufferEnabled')
-00053f00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00053f10: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00053f20: 756c 7469 5f62 7566 6665 725f 656e 6162  ulti_buffer_enab
-00053f30: 6c65 6420 3d20 6d2e 6765 7428 274d 756c  led = m.get('Mul
-00053f40: 7469 4275 6666 6572 456e 6162 6c65 6427  tiBufferEnabled'
-00053f50: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00053f60: 6574 2827 4d75 6c74 6942 7566 6665 7250  et('MultiBufferP
-00053f70: 6f6c 6c44 656c 6179 2729 2069 7320 6e6f  ollDelay') is no
-00053f80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00053f90: 2020 2020 7365 6c66 2e6d 756c 7469 5f62      self.multi_b
-00053fa0: 7566 6665 725f 706f 6c6c 5f64 656c 6179  uffer_poll_delay
-00053fb0: 203d 206d 2e67 6574 2827 4d75 6c74 6942   = m.get('MultiB
-00053fc0: 7566 6665 7250 6f6c 6c44 656c 6179 2729  ufferPollDelay')
-00053fd0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00053fe0: 7428 274d 7973 716c 4669 6c74 6572 456e  t('MysqlFilterEn
-00053ff0: 6162 6c65 6427 2920 6973 206e 6f74 204e  abled') is not N
-00054000: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00054010: 2073 656c 662e 6d79 7371 6c5f 6669 6c74   self.mysql_filt
-00054020: 6572 5f65 6e61 626c 6564 203d 206d 2e67  er_enabled = m.g
-00054030: 6574 2827 4d79 7371 6c46 696c 7465 7245  et('MysqlFilterE
-00054040: 6e61 626c 6564 2729 0a20 2020 2020 2020  nabled').       
-00054050: 2069 6620 6d2e 6765 7428 274f 5041 4c69   if m.get('OPALi
-00054060: 6d69 7443 5055 2729 2069 7320 6e6f 7420  mitCPU') is not 
-00054070: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00054080: 2020 7365 6c66 2e6f 7061 6c69 6d69 745f    self.opalimit_
-00054090: 6370 7520 3d20 6d2e 6765 7428 274f 5041  cpu = m.get('OPA
-000540a0: 4c69 6d69 7443 5055 2729 0a20 2020 2020  LimitCPU').     
-000540b0: 2020 2069 6620 6d2e 6765 7428 274f 5041     if m.get('OPA
-000540c0: 4c69 6d69 744d 656d 6f72 7927 2920 6973  LimitMemory') is
-000540d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000540e0: 2020 2020 2020 2073 656c 662e 6f70 616c         self.opal
-000540f0: 696d 6974 5f6d 656d 6f72 7920 3d20 6d2e  imit_memory = m.
-00054100: 6765 7428 274f 5041 4c69 6d69 744d 656d  get('OPALimitMem
-00054110: 6f72 7927 290a 2020 2020 2020 2020 6966  ory').        if
-00054120: 206d 2e67 6574 2827 4f50 414c 6f67 4c65   m.get('OPALogLe
-00054130: 7665 6c27 2920 6973 206e 6f74 204e 6f6e  vel') is not Non
-00054140: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00054150: 656c 662e 6f70 616c 6f67 5f6c 6576 656c  elf.opalog_level
-00054160: 203d 206d 2e67 6574 2827 4f50 414c 6f67   = m.get('OPALog
-00054170: 4c65 7665 6c27 290a 2020 2020 2020 2020  Level').        
-00054180: 6966 206d 2e67 6574 2827 4f50 4152 6571  if m.get('OPAReq
-00054190: 7565 7374 4350 5527 2920 6973 206e 6f74  uestCPU') is not
-000541a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000541b0: 2020 2073 656c 662e 6f70 6172 6571 7565     self.opareque
-000541c0: 7374 5f63 7075 203d 206d 2e67 6574 2827  st_cpu = m.get('
-000541d0: 4f50 4152 6571 7565 7374 4350 5527 290a  OPARequestCPU').
-000541e0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000541f0: 2827 4f50 4152 6571 7565 7374 4d65 6d6f  ('OPARequestMemo
-00054200: 7279 2729 2069 7320 6e6f 7420 4e6f 6e65  ry') is not None
-00054210: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00054220: 6c66 2e6f 7061 7265 7175 6573 745f 6d65  lf.oparequest_me
-00054230: 6d6f 7279 203d 206d 2e67 6574 2827 4f50  mory = m.get('OP
-00054240: 4152 6571 7565 7374 4d65 6d6f 7279 2729  ARequestMemory')
-00054250: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00054260: 7428 274f 7061 456e 6162 6c65 6427 2920  t('OpaEnabled') 
-00054270: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00054280: 2020 2020 2020 2020 2073 656c 662e 6f70           self.op
-00054290: 615f 656e 6162 6c65 6420 3d20 6d2e 6765  a_enabled = m.ge
-000542a0: 7428 274f 7061 456e 6162 6c65 6427 290a  t('OpaEnabled').
-000542b0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000542c0: 2827 4f70 656e 4167 656e 7450 6f6c 6963  ('OpenAgentPolic
-000542d0: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
-000542e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000542f0: 662e 6f70 656e 5f61 6765 6e74 5f70 6f6c  f.open_agent_pol
-00054300: 6963 7920 3d20 6d2e 6765 7428 274f 7065  icy = m.get('Ope
-00054310: 6e41 6765 6e74 506f 6c69 6379 2729 0a20  nAgentPolicy'). 
-00054320: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00054330: 274f 7574 626f 756e 6454 7261 6666 6963  'OutboundTraffic
-00054340: 506f 6c69 6379 2729 2069 7320 6e6f 7420  Policy') is not 
-00054350: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00054360: 2020 7365 6c66 2e6f 7574 626f 756e 645f    self.outbound_
-00054370: 7472 6166 6669 635f 706f 6c69 6379 203d  traffic_policy =
-00054380: 206d 2e67 6574 2827 4f75 7462 6f75 6e64   m.get('Outbound
-00054390: 5472 6166 6669 6350 6f6c 6963 7927 290a  TrafficPolicy').
-000543a0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000543b0: 2827 5072 6f6d 6574 6865 7573 5572 6c27  ('PrometheusUrl'
-000543c0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000543d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000543e0: 7072 6f6d 6574 6865 7573 5f75 726c 203d  prometheus_url =
-000543f0: 206d 2e67 6574 2827 5072 6f6d 6574 6865   m.get('Promethe
-00054400: 7573 5572 6c27 290a 2020 2020 2020 2020  usUrl').        
-00054410: 6966 206d 2e67 6574 2827 5072 6f78 7949  if m.get('ProxyI
-00054420: 6e69 7443 5055 5265 736f 7572 6365 4c69  nitCPUResourceLi
-00054430: 6d69 7427 2920 6973 206e 6f74 204e 6f6e  mit') is not Non
-00054440: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00054450: 656c 662e 7072 6f78 795f 696e 6974 5f63  elf.proxy_init_c
-00054460: 7075 7265 736f 7572 6365 5f6c 696d 6974  puresource_limit
-00054470: 203d 206d 2e67 6574 2827 5072 6f78 7949   = m.get('ProxyI
-00054480: 6e69 7443 5055 5265 736f 7572 6365 4c69  nitCPUResourceLi
-00054490: 6d69 7427 290a 2020 2020 2020 2020 6966  mit').        if
-000544a0: 206d 2e67 6574 2827 5072 6f78 7949 6e69   m.get('ProxyIni
-000544b0: 7443 5055 5265 736f 7572 6365 5265 7175  tCPUResourceRequ
-000544c0: 6573 7427 2920 6973 206e 6f74 204e 6f6e  est') is not Non
-000544d0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000544e0: 656c 662e 7072 6f78 795f 696e 6974 5f63  elf.proxy_init_c
-000544f0: 7075 7265 736f 7572 6365 5f72 6571 7565  puresource_reque
-00054500: 7374 203d 206d 2e67 6574 2827 5072 6f78  st = m.get('Prox
-00054510: 7949 6e69 7443 5055 5265 736f 7572 6365  yInitCPUResource
-00054520: 5265 7175 6573 7427 290a 2020 2020 2020  Request').      
-00054530: 2020 6966 206d 2e67 6574 2827 5072 6f78    if m.get('Prox
-00054540: 7949 6e69 744d 656d 6f72 7952 6573 6f75  yInitMemoryResou
-00054550: 7263 654c 696d 6974 2729 2069 7320 6e6f  rceLimit') is no
-00054560: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00054570: 2020 2020 7365 6c66 2e70 726f 7879 5f69      self.proxy_i
-00054580: 6e69 745f 6d65 6d6f 7279 5f72 6573 6f75  nit_memory_resou
-00054590: 7263 655f 6c69 6d69 7420 3d20 6d2e 6765  rce_limit = m.ge
-000545a0: 7428 2750 726f 7879 496e 6974 4d65 6d6f  t('ProxyInitMemo
-000545b0: 7279 5265 736f 7572 6365 4c69 6d69 7427  ryResourceLimit'
-000545c0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000545d0: 6574 2827 5072 6f78 7949 6e69 744d 656d  et('ProxyInitMem
-000545e0: 6f72 7952 6573 6f75 7263 6552 6571 7565  oryResourceReque
-000545f0: 7374 2729 2069 7320 6e6f 7420 4e6f 6e65  st') is not None
-00054600: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00054610: 6c66 2e70 726f 7879 5f69 6e69 745f 6d65  lf.proxy_init_me
-00054620: 6d6f 7279 5f72 6573 6f75 7263 655f 7265  mory_resource_re
-00054630: 7175 6573 7420 3d20 6d2e 6765 7428 2750  quest = m.get('P
-00054640: 726f 7879 496e 6974 4d65 6d6f 7279 5265  roxyInitMemoryRe
-00054650: 736f 7572 6365 5265 7175 6573 7427 290a  sourceRequest').
-00054660: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00054670: 2827 5072 6f78 794c 696d 6974 4350 5527  ('ProxyLimitCPU'
-00054680: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00054690: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000546a0: 7072 6f78 795f 6c69 6d69 745f 6370 7520  proxy_limit_cpu 
-000546b0: 3d20 6d2e 6765 7428 2750 726f 7879 4c69  = m.get('ProxyLi
-000546c0: 6d69 7443 5055 2729 0a20 2020 2020 2020  mitCPU').       
-000546d0: 2069 6620 6d2e 6765 7428 2750 726f 7879   if m.get('Proxy
-000546e0: 4c69 6d69 744d 656d 6f72 7927 2920 6973  LimitMemory') is
-000546f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00054700: 2020 2020 2020 2073 656c 662e 7072 6f78         self.prox
-00054710: 795f 6c69 6d69 745f 6d65 6d6f 7279 203d  y_limit_memory =
-00054720: 206d 2e67 6574 2827 5072 6f78 794c 696d   m.get('ProxyLim
-00054730: 6974 4d65 6d6f 7279 2729 0a20 2020 2020  itMemory').     
-00054740: 2020 2069 6620 6d2e 6765 7428 2750 726f     if m.get('Pro
-00054750: 7879 5265 7175 6573 7443 5055 2729 2069  xyRequestCPU') i
-00054760: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00054770: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-00054780: 7879 5f72 6571 7565 7374 5f63 7075 203d  xy_request_cpu =
-00054790: 206d 2e67 6574 2827 5072 6f78 7952 6571   m.get('ProxyReq
-000547a0: 7565 7374 4350 5527 290a 2020 2020 2020  uestCPU').      
-000547b0: 2020 6966 206d 2e67 6574 2827 5072 6f78    if m.get('Prox
-000547c0: 7952 6571 7565 7374 4d65 6d6f 7279 2729  yRequestMemory')
-000547d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000547e0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-000547f0: 726f 7879 5f72 6571 7565 7374 5f6d 656d  roxy_request_mem
-00054800: 6f72 7920 3d20 6d2e 6765 7428 2750 726f  ory = m.get('Pro
-00054810: 7879 5265 7175 6573 744d 656d 6f72 7927  xyRequestMemory'
-00054820: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00054830: 6574 2827 5265 6469 7346 696c 7465 7245  et('RedisFilterE
-00054840: 6e61 626c 6564 2729 2069 7320 6e6f 7420  nabled') is not 
-00054850: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00054860: 2020 7365 6c66 2e72 6564 6973 5f66 696c    self.redis_fil
-00054870: 7465 725f 656e 6162 6c65 6420 3d20 6d2e  ter_enabled = m.
-00054880: 6765 7428 2752 6564 6973 4669 6c74 6572  get('RedisFilter
-00054890: 456e 6162 6c65 6427 290a 2020 2020 2020  Enabled').      
-000548a0: 2020 6966 206d 2e67 6574 2827 5365 7276    if m.get('Serv
-000548b0: 6963 654d 6573 6849 6427 2920 6973 206e  iceMeshId') is n
-000548c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000548d0: 2020 2020 2073 656c 662e 7365 7276 6963       self.servic
-000548e0: 655f 6d65 7368 5f69 6420 3d20 6d2e 6765  e_mesh_id = m.ge
-000548f0: 7428 2753 6572 7669 6365 4d65 7368 4964  t('ServiceMeshId
-00054900: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00054910: 6765 7428 2753 6964 6563 6172 496e 6a65  get('SidecarInje
-00054920: 6374 6f72 4c69 6d69 7443 5055 2729 2069  ctorLimitCPU') i
-00054930: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00054940: 2020 2020 2020 2020 7365 6c66 2e73 6964          self.sid
-00054950: 6563 6172 5f69 6e6a 6563 746f 725f 6c69  ecar_injector_li
-00054960: 6d69 745f 6370 7520 3d20 6d2e 6765 7428  mit_cpu = m.get(
-00054970: 2753 6964 6563 6172 496e 6a65 6374 6f72  'SidecarInjector
-00054980: 4c69 6d69 7443 5055 2729 0a20 2020 2020  LimitCPU').     
-00054990: 2020 2069 6620 6d2e 6765 7428 2753 6964     if m.get('Sid
-000549a0: 6563 6172 496e 6a65 6374 6f72 4c69 6d69  ecarInjectorLimi
-000549b0: 744d 656d 6f72 7927 2920 6973 206e 6f74  tMemory') is not
-000549c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000549d0: 2020 2073 656c 662e 7369 6465 6361 725f     self.sidecar_
-000549e0: 696e 6a65 6374 6f72 5f6c 696d 6974 5f6d  injector_limit_m
-000549f0: 656d 6f72 7920 3d20 6d2e 6765 7428 2753  emory = m.get('S
-00054a00: 6964 6563 6172 496e 6a65 6374 6f72 4c69  idecarInjectorLi
-00054a10: 6d69 744d 656d 6f72 7927 290a 2020 2020  mitMemory').    
-00054a20: 2020 2020 6966 206d 2e67 6574 2827 5369      if m.get('Si
-00054a30: 6465 6361 7249 6e6a 6563 746f 7252 6571  decarInjectorReq
-00054a40: 7565 7374 4350 5527 2920 6973 206e 6f74  uestCPU') is not
-00054a50: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00054a60: 2020 2073 656c 662e 7369 6465 6361 725f     self.sidecar_
-00054a70: 696e 6a65 6374 6f72 5f72 6571 7565 7374  injector_request
-00054a80: 5f63 7075 203d 206d 2e67 6574 2827 5369  _cpu = m.get('Si
-00054a90: 6465 6361 7249 6e6a 6563 746f 7252 6571  decarInjectorReq
-00054aa0: 7565 7374 4350 5527 290a 2020 2020 2020  uestCPU').      
-00054ab0: 2020 6966 206d 2e67 6574 2827 5369 6465    if m.get('Side
-00054ac0: 6361 7249 6e6a 6563 746f 7252 6571 7565  carInjectorReque
-00054ad0: 7374 4d65 6d6f 7279 2729 2069 7320 6e6f  stMemory') is no
-00054ae0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00054af0: 2020 2020 7365 6c66 2e73 6964 6563 6172      self.sidecar
-00054b00: 5f69 6e6a 6563 746f 725f 7265 7175 6573  _injector_reques
-00054b10: 745f 6d65 6d6f 7279 203d 206d 2e67 6574  t_memory = m.get
-00054b20: 2827 5369 6465 6361 7249 6e6a 6563 746f  ('SidecarInjecto
-00054b30: 7252 6571 7565 7374 4d65 6d6f 7279 2729  rRequestMemory')
-00054b40: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00054b50: 7428 2753 6964 6563 6172 496e 6a65 6374  t('SidecarInject
-00054b60: 6f72 5765 6268 6f6f 6b41 7359 616d 6c27  orWebhookAsYaml'
-00054b70: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00054b80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00054b90: 7369 6465 6361 725f 696e 6a65 6374 6f72  sidecar_injector
-00054ba0: 5f77 6562 686f 6f6b 5f61 735f 7961 6d6c  _webhook_as_yaml
-00054bb0: 203d 206d 2e67 6574 2827 5369 6465 6361   = m.get('Sideca
-00054bc0: 7249 6e6a 6563 746f 7257 6562 686f 6f6b  rInjectorWebhook
-00054bd0: 4173 5961 6d6c 2729 0a20 2020 2020 2020  AsYaml').       
-00054be0: 2069 6620 6d2e 6765 7428 2754 656c 656d   if m.get('Telem
-00054bf0: 6574 7279 2729 2069 7320 6e6f 7420 4e6f  etry') is not No
-00054c00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00054c10: 7365 6c66 2e74 656c 656d 6574 7279 203d  self.telemetry =
-00054c20: 206d 2e67 6574 2827 5465 6c65 6d65 7472   m.get('Telemetr
-00054c30: 7927 290a 2020 2020 2020 2020 6966 206d  y').        if m
-00054c40: 2e67 6574 2827 5465 726d 696e 6174 696f  .get('Terminatio
-00054c50: 6e44 7261 696e 4475 7261 7469 6f6e 2729  nDrainDuration')
-00054c60: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00054c70: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00054c80: 6572 6d69 6e61 7469 6f6e 5f64 7261 696e  ermination_drain
-00054c90: 5f64 7572 6174 696f 6e20 3d20 6d2e 6765  _duration = m.ge
-00054ca0: 7428 2754 6572 6d69 6e61 7469 6f6e 4472  t('TerminationDr
-00054cb0: 6169 6e44 7572 6174 696f 6e27 290a 2020  ainDuration').  
-00054cc0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00054cd0: 5468 7269 6674 4669 6c74 6572 456e 6162  ThriftFilterEnab
-00054ce0: 6c65 6427 2920 6973 206e 6f74 204e 6f6e  led') is not Non
-00054cf0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00054d00: 656c 662e 7468 7269 6674 5f66 696c 7465  elf.thrift_filte
-00054d10: 725f 656e 6162 6c65 6420 3d20 6d2e 6765  r_enabled = m.ge
-00054d20: 7428 2754 6872 6966 7446 696c 7465 7245  t('ThriftFilterE
-00054d30: 6e61 626c 6564 2729 0a20 2020 2020 2020  nabled').       
-00054d40: 2069 6620 6d2e 6765 7428 2754 7261 6365   if m.get('Trace
-00054d50: 5361 6d70 6c69 6e67 2729 2069 7320 6e6f  Sampling') is no
-00054d60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00054d70: 2020 2020 7365 6c66 2e74 7261 6365 5f73      self.trace_s
-00054d80: 616d 706c 696e 6720 3d20 6d2e 6765 7428  ampling = m.get(
-00054d90: 2754 7261 6365 5361 6d70 6c69 6e67 2729  'TraceSampling')
-00054da0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00054db0: 7428 2754 7261 6369 6e67 2729 2069 7320  t('Tracing') is 
-00054dc0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00054dd0: 2020 2020 2020 7365 6c66 2e74 7261 6369        self.traci
-00054de0: 6e67 203d 206d 2e67 6574 2827 5472 6163  ng = m.get('Trac
-00054df0: 696e 6727 290a 2020 2020 2020 2020 6966  ing').        if
-00054e00: 206d 2e67 6574 2827 5765 6241 7373 656d   m.get('WebAssem
-00054e10: 626c 7946 696c 7465 7245 6e61 626c 6564  blyFilterEnabled
-00054e20: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00054e30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00054e40: 2e77 6562 5f61 7373 656d 626c 795f 6669  .web_assembly_fi
-00054e50: 6c74 6572 5f65 6e61 626c 6564 203d 206d  lter_enabled = m
-00054e60: 2e67 6574 2827 5765 6241 7373 656d 626c  .get('WebAssembl
-00054e70: 7946 696c 7465 7245 6e61 626c 6564 2729  yFilterEnabled')
-00054e80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00054e90: 7365 6c66 0a0a 0a63 6c61 7373 2055 7064  self...class Upd
-00054ea0: 6174 654d 6573 6846 6561 7475 7265 5265  ateMeshFeatureRe
-00054eb0: 7370 6f6e 7365 426f 6479 2854 6561 4d6f  sponseBody(TeaMo
-00054ec0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-00054ed0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-00054ee0: 7365 6c66 2c0a 2020 2020 2020 2020 7265  self,.        re
-00054ef0: 7175 6573 745f 6964 3a20 7374 7220 3d20  quest_id: str = 
-00054f00: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-00054f10: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
-00054f20: 745f 6964 203d 2072 6571 7565 7374 5f69  t_id = request_i
-00054f30: 640a 0a20 2020 2064 6566 2076 616c 6964  d..    def valid
-00054f40: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-00054f50: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-00054f60: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-00054f70: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-00054f80: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
-00054f90: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-00054fa0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00054fb0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00054fc0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-00054fd0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-00054fe0: 2020 2020 2069 6620 7365 6c66 2e72 6571       if self.req
-00054ff0: 7565 7374 5f69 6420 6973 206e 6f74 204e  uest_id is not N
-00055000: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00055010: 2072 6573 756c 745b 2752 6571 7565 7374   result['Request
-00055020: 4964 275d 203d 2073 656c 662e 7265 7175  Id'] = self.requ
-00055030: 6573 745f 6964 0a20 2020 2020 2020 2072  est_id.        r
-00055040: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-00055050: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-00055060: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-00055070: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-00055080: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-00055090: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000550a0: 5265 7175 6573 7449 6427 2920 6973 206e  RequestId') is n
-000550b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000550c0: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
-000550d0: 745f 6964 203d 206d 2e67 6574 2827 5265  t_id = m.get('Re
-000550e0: 7175 6573 7449 6427 290a 2020 2020 2020  questId').      
-000550f0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-00055100: 636c 6173 7320 5570 6461 7465 4d65 7368  class UpdateMesh
-00055110: 4665 6174 7572 6552 6573 706f 6e73 6528  FeatureResponse(
-00055120: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-00055130: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-00055140: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00055150: 2020 2068 6561 6465 7273 3a20 4469 6374     headers: Dict
-00055160: 5b73 7472 2c20 7374 725d 203d 204e 6f6e  [str, str] = Non
-00055170: 652c 0a20 2020 2020 2020 2062 6f64 793a  e,.        body:
-00055180: 2055 7064 6174 654d 6573 6846 6561 7475   UpdateMeshFeatu
-00055190: 7265 5265 7370 6f6e 7365 426f 6479 203d  reResponseBody =
-000551a0: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-000551b0: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-000551c0: 7273 203d 2068 6561 6465 7273 0a20 2020  rs = headers.   
-000551d0: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-000551e0: 2062 6f64 790a 0a20 2020 2064 6566 2076   body..    def v
-000551f0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-00055200: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-00055210: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-00055220: 6c66 2e68 6561 6465 7273 2c20 2768 6561  lf.headers, 'hea
-00055230: 6465 7273 2729 0a20 2020 2020 2020 2073  ders').        s
-00055240: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-00055250: 7569 7265 6428 7365 6c66 2e62 6f64 792c  uired(self.body,
-00055260: 2027 626f 6479 2729 0a20 2020 2020 2020   'body').       
-00055270: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
-00055280: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00055290: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
-000552a0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-000552b0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-000552c0: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
-000552d0: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-000552e0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-000552f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00055300: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-00055310: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-00055320: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-00055330: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
-00055340: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00055350: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
-00055360: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
-00055370: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
-00055380: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
-00055390: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000553a0: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
-000553b0: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
-000553c0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-000553d0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-000553e0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-000553f0: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
-00055400: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-00055410: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-00055420: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00055430: 2827 6865 6164 6572 7327 2920 6973 206e  ('headers') is n
-00055440: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00055450: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-00055460: 7320 3d20 6d2e 6765 7428 2768 6561 6465  s = m.get('heade
-00055470: 7273 2729 0a20 2020 2020 2020 2069 6620  rs').        if 
-00055480: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
-00055490: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000554a0: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
-000554b0: 6c20 3d20 5570 6461 7465 4d65 7368 4665  l = UpdateMeshFe
-000554c0: 6174 7572 6552 6573 706f 6e73 6542 6f64  atureResponseBod
-000554d0: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
-000554e0: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
-000554f0: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
-00055500: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
-00055510: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-00055520: 0a63 6c61 7373 2055 7064 6174 654e 616d  .class UpdateNam
-00055530: 6573 7061 6365 5363 6f70 6553 6964 6563  espaceScopeSidec
-00055540: 6172 436f 6e66 6967 5265 7175 6573 7428  arConfigRequest(
-00055550: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-00055560: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-00055570: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00055580: 2020 2065 7863 6c75 6465 5f69 7072 616e     exclude_ipran
-00055590: 6765 733a 2073 7472 203d 204e 6f6e 652c  ges: str = None,
-000555a0: 0a20 2020 2020 2020 2065 7863 6c75 6465  .        exclude
-000555b0: 5f69 6e62 6f75 6e64 5f70 6f72 7473 3a20  _inbound_ports: 
-000555c0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-000555d0: 2020 2020 6578 636c 7564 655f 6f75 7462      exclude_outb
-000555e0: 6f75 6e64 5f70 6f72 7473 3a20 7374 7220  ound_ports: str 
-000555f0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00055600: 696e 636c 7564 655f 6970 7261 6e67 6573  include_ipranges
-00055610: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00055620: 2020 2020 2020 696e 636c 7564 655f 696e        include_in
-00055630: 626f 756e 645f 706f 7274 733a 2073 7472  bound_ports: str
-00055640: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00055650: 2069 6e63 6c75 6465 5f6f 7574 626f 756e   include_outboun
-00055660: 645f 706f 7274 733a 2073 7472 203d 204e  d_ports: str = N
-00055670: 6f6e 652c 0a20 2020 2020 2020 2069 7374  one,.        ist
-00055680: 696f 5f64 6e73 7072 6f78 795f 656e 6162  io_dnsproxy_enab
-00055690: 6c65 643a 2062 6f6f 6c20 3d20 4e6f 6e65  led: bool = None
-000556a0: 2c0a 2020 2020 2020 2020 6c69 6665 6379  ,.        lifecy
-000556b0: 636c 653a 2073 7472 203d 204e 6f6e 652c  cle: str = None,
-000556c0: 0a20 2020 2020 2020 206e 616d 6573 7061  .        namespa
-000556d0: 6365 3a20 7374 7220 3d20 4e6f 6e65 2c0a  ce: str = None,.
-000556e0: 2020 2020 2020 2020 7072 6f78 795f 696e          proxy_in
-000556f0: 6974 5f63 7075 7265 736f 7572 6365 5f6c  it_cpuresource_l
-00055700: 696d 6974 3a20 7374 7220 3d20 4e6f 6e65  imit: str = None
-00055710: 2c0a 2020 2020 2020 2020 7072 6f78 795f  ,.        proxy_
-00055720: 696e 6974 5f63 7075 7265 736f 7572 6365  init_cpuresource
-00055730: 5f72 6571 7565 7374 3a20 7374 7220 3d20  _request: str = 
-00055740: 4e6f 6e65 2c0a 2020 2020 2020 2020 7072  None,.        pr
-00055750: 6f78 795f 696e 6974 5f6d 656d 6f72 795f  oxy_init_memory_
-00055760: 7265 736f 7572 6365 5f6c 696d 6974 3a20  resource_limit: 
-00055770: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-00055780: 2020 2020 7072 6f78 795f 696e 6974 5f6d      proxy_init_m
-00055790: 656d 6f72 795f 7265 736f 7572 6365 5f72  emory_resource_r
-000557a0: 6571 7565 7374 3a20 7374 7220 3d20 4e6f  equest: str = No
-000557b0: 6e65 2c0a 2020 2020 2020 2020 7365 7276  ne,.        serv
-000557c0: 6963 655f 6d65 7368 5f69 643a 2073 7472  ice_mesh_id: str
-000557d0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000557e0: 2073 6964 6563 6172 5f70 726f 7879 5f63   sidecar_proxy_c
-000557f0: 7075 7265 736f 7572 6365 5f6c 696d 6974  puresource_limit
-00055800: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00055810: 2020 2020 2020 7369 6465 6361 725f 7072        sidecar_pr
-00055820: 6f78 795f 6370 7572 6573 6f75 7263 655f  oxy_cpuresource_
-00055830: 7265 7175 6573 743a 2073 7472 203d 204e  request: str = N
-00055840: 6f6e 652c 0a20 2020 2020 2020 2073 6964  one,.        sid
-00055850: 6563 6172 5f70 726f 7879 5f6d 656d 6f72  ecar_proxy_memor
-00055860: 795f 7265 736f 7572 6365 5f6c 696d 6974  y_resource_limit
-00055870: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00055880: 2020 2020 2020 7369 6465 6361 725f 7072        sidecar_pr
-00055890: 6f78 795f 6d65 6d6f 7279 5f72 6573 6f75  oxy_memory_resou
-000558a0: 7263 655f 7265 7175 6573 743a 2073 7472  rce_request: str
-000558b0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000558c0: 2074 6572 6d69 6e61 7469 6f6e 5f64 7261   termination_dra
-000558d0: 696e 5f64 7572 6174 696f 6e3a 2073 7472  in_duration: str
-000558e0: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-000558f0: 2020 2020 2020 2020 7365 6c66 2e65 7863          self.exc
-00055900: 6c75 6465 5f69 7072 616e 6765 7320 3d20  lude_ipranges = 
-00055910: 6578 636c 7564 655f 6970 7261 6e67 6573  exclude_ipranges
-00055920: 0a20 2020 2020 2020 2073 656c 662e 6578  .        self.ex
-00055930: 636c 7564 655f 696e 626f 756e 645f 706f  clude_inbound_po
-00055940: 7274 7320 3d20 6578 636c 7564 655f 696e  rts = exclude_in
-00055950: 626f 756e 645f 706f 7274 730a 2020 2020  bound_ports.    
-00055960: 2020 2020 7365 6c66 2e65 7863 6c75 6465      self.exclude
-00055970: 5f6f 7574 626f 756e 645f 706f 7274 7320  _outbound_ports 
-00055980: 3d20 6578 636c 7564 655f 6f75 7462 6f75  = exclude_outbou
-00055990: 6e64 5f70 6f72 7473 0a20 2020 2020 2020  nd_ports.       
-000559a0: 2073 656c 662e 696e 636c 7564 655f 6970   self.include_ip
-000559b0: 7261 6e67 6573 203d 2069 6e63 6c75 6465  ranges = include
-000559c0: 5f69 7072 616e 6765 730a 2020 2020 2020  _ipranges.      
-000559d0: 2020 7365 6c66 2e69 6e63 6c75 6465 5f69    self.include_i
-000559e0: 6e62 6f75 6e64 5f70 6f72 7473 203d 2069  nbound_ports = i
-000559f0: 6e63 6c75 6465 5f69 6e62 6f75 6e64 5f70  nclude_inbound_p
-00055a00: 6f72 7473 0a20 2020 2020 2020 2073 656c  orts.        sel
-00055a10: 662e 696e 636c 7564 655f 6f75 7462 6f75  f.include_outbou
-00055a20: 6e64 5f70 6f72 7473 203d 2069 6e63 6c75  nd_ports = inclu
-00055a30: 6465 5f6f 7574 626f 756e 645f 706f 7274  de_outbound_port
-00055a40: 730a 2020 2020 2020 2020 7365 6c66 2e69  s.        self.i
-00055a50: 7374 696f 5f64 6e73 7072 6f78 795f 656e  stio_dnsproxy_en
-00055a60: 6162 6c65 6420 3d20 6973 7469 6f5f 646e  abled = istio_dn
-00055a70: 7370 726f 7879 5f65 6e61 626c 6564 0a20  sproxy_enabled. 
-00055a80: 2020 2020 2020 2073 656c 662e 6c69 6665         self.life
-00055a90: 6379 636c 6520 3d20 6c69 6665 6379 636c  cycle = lifecycl
-00055aa0: 650a 2020 2020 2020 2020 7365 6c66 2e6e  e.        self.n
-00055ab0: 616d 6573 7061 6365 203d 206e 616d 6573  amespace = names
-00055ac0: 7061 6365 0a20 2020 2020 2020 2073 656c  pace.        sel
-00055ad0: 662e 7072 6f78 795f 696e 6974 5f63 7075  f.proxy_init_cpu
-00055ae0: 7265 736f 7572 6365 5f6c 696d 6974 203d  resource_limit =
-00055af0: 2070 726f 7879 5f69 6e69 745f 6370 7572   proxy_init_cpur
-00055b00: 6573 6f75 7263 655f 6c69 6d69 740a 2020  esource_limit.  
-00055b10: 2020 2020 2020 7365 6c66 2e70 726f 7879        self.proxy
-00055b20: 5f69 6e69 745f 6370 7572 6573 6f75 7263  _init_cpuresourc
-00055b30: 655f 7265 7175 6573 7420 3d20 7072 6f78  e_request = prox
-00055b40: 795f 696e 6974 5f63 7075 7265 736f 7572  y_init_cpuresour
-00055b50: 6365 5f72 6571 7565 7374 0a20 2020 2020  ce_request.     
-00055b60: 2020 2073 656c 662e 7072 6f78 795f 696e     self.proxy_in
-00055b70: 6974 5f6d 656d 6f72 795f 7265 736f 7572  it_memory_resour
-00055b80: 6365 5f6c 696d 6974 203d 2070 726f 7879  ce_limit = proxy
-00055b90: 5f69 6e69 745f 6d65 6d6f 7279 5f72 6573  _init_memory_res
-00055ba0: 6f75 7263 655f 6c69 6d69 740a 2020 2020  ource_limit.    
-00055bb0: 2020 2020 7365 6c66 2e70 726f 7879 5f69      self.proxy_i
-00055bc0: 6e69 745f 6d65 6d6f 7279 5f72 6573 6f75  nit_memory_resou
-00055bd0: 7263 655f 7265 7175 6573 7420 3d20 7072  rce_request = pr
-00055be0: 6f78 795f 696e 6974 5f6d 656d 6f72 795f  oxy_init_memory_
-00055bf0: 7265 736f 7572 6365 5f72 6571 7565 7374  resource_request
-00055c00: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00055c10: 7276 6963 655f 6d65 7368 5f69 6420 3d20  rvice_mesh_id = 
-00055c20: 7365 7276 6963 655f 6d65 7368 5f69 640a  service_mesh_id.
-00055c30: 2020 2020 2020 2020 7365 6c66 2e73 6964          self.sid
-00055c40: 6563 6172 5f70 726f 7879 5f63 7075 7265  ecar_proxy_cpure
-00055c50: 736f 7572 6365 5f6c 696d 6974 203d 2073  source_limit = s
-00055c60: 6964 6563 6172 5f70 726f 7879 5f63 7075  idecar_proxy_cpu
-00055c70: 7265 736f 7572 6365 5f6c 696d 6974 0a20  resource_limit. 
-00055c80: 2020 2020 2020 2073 656c 662e 7369 6465         self.side
-00055c90: 6361 725f 7072 6f78 795f 6370 7572 6573  car_proxy_cpures
-00055ca0: 6f75 7263 655f 7265 7175 6573 7420 3d20  ource_request = 
-00055cb0: 7369 6465 6361 725f 7072 6f78 795f 6370  sidecar_proxy_cp
-00055cc0: 7572 6573 6f75 7263 655f 7265 7175 6573  uresource_reques
-00055cd0: 740a 2020 2020 2020 2020 7365 6c66 2e73  t.        self.s
-00055ce0: 6964 6563 6172 5f70 726f 7879 5f6d 656d  idecar_proxy_mem
-00055cf0: 6f72 795f 7265 736f 7572 6365 5f6c 696d  ory_resource_lim
-00055d00: 6974 203d 2073 6964 6563 6172 5f70 726f  it = sidecar_pro
-00055d10: 7879 5f6d 656d 6f72 795f 7265 736f 7572  xy_memory_resour
-00055d20: 6365 5f6c 696d 6974 0a20 2020 2020 2020  ce_limit.       
+0004ce80: 636c 6173 7320 5570 6461 7465 4153 4d47  class UpdateASMG
+0004ce90: 6174 6577 6179 5265 7175 6573 7428 5465  atewayRequest(Te
+0004cea0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+0004ceb0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+0004cec0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0004ced0: 2062 6f64 793a 2073 7472 203d 204e 6f6e   body: str = Non
+0004cee0: 652c 0a20 2020 2020 2020 2069 7374 696f  e,.        istio
+0004cef0: 5f67 6174 6577 6179 5f6e 616d 653a 2073  _gateway_name: s
+0004cf00: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0004cf10: 2020 2073 6572 7669 6365 5f6d 6573 685f     service_mesh_
+0004cf20: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+0004cf30: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+0004cf40: 656c 662e 626f 6479 203d 2062 6f64 790a  elf.body = body.
+0004cf50: 2020 2020 2020 2020 7365 6c66 2e69 7374          self.ist
+0004cf60: 696f 5f67 6174 6577 6179 5f6e 616d 6520  io_gateway_name 
+0004cf70: 3d20 6973 7469 6f5f 6761 7465 7761 795f  = istio_gateway_
+0004cf80: 6e61 6d65 0a20 2020 2020 2020 2073 656c  name.        sel
+0004cf90: 662e 7365 7276 6963 655f 6d65 7368 5f69  f.service_mesh_i
+0004cfa0: 6420 3d20 7365 7276 6963 655f 6d65 7368  d = service_mesh
+0004cfb0: 5f69 640a 0a20 2020 2064 6566 2076 616c  _id..    def val
+0004cfc0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+0004cfd0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+0004cfe0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+0004cff0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+0004d000: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+0004d010: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+0004d020: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0004d030: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0004d040: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+0004d050: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+0004d060: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+0004d070: 6f64 7920 6973 206e 6f74 204e 6f6e 653a  ody is not None:
+0004d080: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0004d090: 756c 745b 2742 6f64 7927 5d20 3d20 7365  ult['Body'] = se
+0004d0a0: 6c66 2e62 6f64 790a 2020 2020 2020 2020  lf.body.        
+0004d0b0: 6966 2073 656c 662e 6973 7469 6f5f 6761  if self.istio_ga
+0004d0c0: 7465 7761 795f 6e61 6d65 2069 7320 6e6f  teway_name is no
+0004d0d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0004d0e0: 2020 2020 7265 7375 6c74 5b27 4973 7469      result['Isti
+0004d0f0: 6f47 6174 6577 6179 4e61 6d65 275d 203d  oGatewayName'] =
+0004d100: 2073 656c 662e 6973 7469 6f5f 6761 7465   self.istio_gate
+0004d110: 7761 795f 6e61 6d65 0a20 2020 2020 2020  way_name.       
+0004d120: 2069 6620 7365 6c66 2e73 6572 7669 6365   if self.service
+0004d130: 5f6d 6573 685f 6964 2069 7320 6e6f 7420  _mesh_id is not 
+0004d140: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0004d150: 2020 7265 7375 6c74 5b27 5365 7276 6963    result['Servic
+0004d160: 654d 6573 6849 6427 5d20 3d20 7365 6c66  eMeshId'] = self
+0004d170: 2e73 6572 7669 6365 5f6d 6573 685f 6964  .service_mesh_id
+0004d180: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0004d190: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+0004d1a0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+0004d1b0: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+0004d1c0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+0004d1d0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0004d1e0: 6966 206d 2e67 6574 2827 426f 6479 2729  if m.get('Body')
+0004d1f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0004d200: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+0004d210: 6f64 7920 3d20 6d2e 6765 7428 2742 6f64  ody = m.get('Bod
+0004d220: 7927 290a 2020 2020 2020 2020 6966 206d  y').        if m
+0004d230: 2e67 6574 2827 4973 7469 6f47 6174 6577  .get('IstioGatew
+0004d240: 6179 4e61 6d65 2729 2069 7320 6e6f 7420  ayName') is not 
+0004d250: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0004d260: 2020 7365 6c66 2e69 7374 696f 5f67 6174    self.istio_gat
+0004d270: 6577 6179 5f6e 616d 6520 3d20 6d2e 6765  eway_name = m.ge
+0004d280: 7428 2749 7374 696f 4761 7465 7761 794e  t('IstioGatewayN
+0004d290: 616d 6527 290a 2020 2020 2020 2020 6966  ame').        if
+0004d2a0: 206d 2e67 6574 2827 5365 7276 6963 654d   m.get('ServiceM
+0004d2b0: 6573 6849 6427 2920 6973 206e 6f74 204e  eshId') is not N
+0004d2c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0004d2d0: 2073 656c 662e 7365 7276 6963 655f 6d65   self.service_me
+0004d2e0: 7368 5f69 6420 3d20 6d2e 6765 7428 2753  sh_id = m.get('S
+0004d2f0: 6572 7669 6365 4d65 7368 4964 2729 0a20  erviceMeshId'). 
+0004d300: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0004d310: 6c66 0a0a 0a63 6c61 7373 2055 7064 6174  lf...class Updat
+0004d320: 6541 534d 4761 7465 7761 7952 6573 706f  eASMGatewayRespo
+0004d330: 6e73 6542 6f64 7928 5465 614d 6f64 656c  nseBody(TeaModel
+0004d340: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+0004d350: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+0004d360: 662c 0a20 2020 2020 2020 2072 6571 7565  f,.        reque
+0004d370: 7374 5f69 643a 2073 7472 203d 204e 6f6e  st_id: str = Non
+0004d380: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+0004d390: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
+0004d3a0: 6420 3d20 7265 7175 6573 745f 6964 0a0a  d = request_id..
+0004d3b0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+0004d3c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0004d3d0: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+0004d3e0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+0004d3f0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+0004d400: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
+0004d410: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+0004d420: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0004d430: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+0004d440: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+0004d450: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+0004d460: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
+0004d470: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
+0004d480: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0004d490: 7375 6c74 5b27 5265 7175 6573 7449 6427  sult['RequestId'
+0004d4a0: 5d20 3d20 7365 6c66 2e72 6571 7565 7374  ] = self.request
+0004d4b0: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
+0004d4c0: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+0004d4d0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+0004d4e0: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
+0004d4f0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+0004d500: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+0004d510: 2020 2069 6620 6d2e 6765 7428 2752 6571     if m.get('Req
+0004d520: 7565 7374 4964 2729 2069 7320 6e6f 7420  uestId') is not 
+0004d530: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0004d540: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
+0004d550: 6420 3d20 6d2e 6765 7428 2752 6571 7565  d = m.get('Reque
+0004d560: 7374 4964 2729 0a20 2020 2020 2020 2072  stId').        r
+0004d570: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+0004d580: 7373 2055 7064 6174 6541 534d 4761 7465  ss UpdateASMGate
+0004d590: 7761 7952 6573 706f 6e73 6528 5465 614d  wayResponse(TeaM
+0004d5a0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+0004d5b0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+0004d5c0: 2073 656c 662c 0a20 2020 2020 2020 2068   self,.        h
+0004d5d0: 6561 6465 7273 3a20 4469 6374 5b73 7472  eaders: Dict[str
+0004d5e0: 2c20 7374 725d 203d 204e 6f6e 652c 0a20  , str] = None,. 
+0004d5f0: 2020 2020 2020 2062 6f64 793a 2055 7064         body: Upd
+0004d600: 6174 6541 534d 4761 7465 7761 7952 6573  ateASMGatewayRes
+0004d610: 706f 6e73 6542 6f64 7920 3d20 4e6f 6e65  ponseBody = None
+0004d620: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+0004d630: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+0004d640: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
+0004d650: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
+0004d660: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+0004d670: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+0004d680: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+0004d690: 7265 7175 6972 6564 2873 656c 662e 6865  required(self.he
+0004d6a0: 6164 6572 732c 2027 6865 6164 6572 7327  aders, 'headers'
+0004d6b0: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+0004d6c0: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
+0004d6d0: 2873 656c 662e 626f 6479 2c20 2762 6f64  (self.body, 'bod
+0004d6e0: 7927 290a 2020 2020 2020 2020 6966 2073  y').        if s
+0004d6f0: 656c 662e 626f 6479 3a0a 2020 2020 2020  elf.body:.      
+0004d700: 2020 2020 2020 7365 6c66 2e62 6f64 792e        self.body.
+0004d710: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
+0004d720: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+0004d730: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+0004d740: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+0004d750: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+0004d760: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+0004d770: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0004d780: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+0004d790: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+0004d7a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0004d7b0: 6865 6164 6572 7320 6973 206e 6f74 204e  headers is not N
+0004d7c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0004d7d0: 2072 6573 756c 745b 2768 6561 6465 7273   result['headers
+0004d7e0: 275d 203d 2073 656c 662e 6865 6164 6572  '] = self.header
+0004d7f0: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
+0004d800: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
+0004d810: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0004d820: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
+0004d830: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
+0004d840: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
+0004d850: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+0004d860: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+0004d870: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
+0004d880: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+0004d890: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+0004d8a0: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
+0004d8b0: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
+0004d8c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0004d8d0: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
+0004d8e0: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
+0004d8f0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0004d900: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
+0004d910: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0004d920: 2020 7465 6d70 5f6d 6f64 656c 203d 2055    temp_model = U
+0004d930: 7064 6174 6541 534d 4761 7465 7761 7952  pdateASMGatewayR
+0004d940: 6573 706f 6e73 6542 6f64 7928 290a 2020  esponseBody().  
+0004d950: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+0004d960: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
+0004d970: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
+0004d980: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
+0004d990: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+0004d9a0: 2055 7064 6174 6541 534d 4761 7465 7761   UpdateASMGatewa
+0004d9b0: 7949 6d70 6f72 7465 6453 6572 7669 6365  yImportedService
+0004d9c0: 7352 6571 7565 7374 2854 6561 4d6f 6465  sRequest(TeaMode
+0004d9d0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+0004d9e0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+0004d9f0: 6c66 2c0a 2020 2020 2020 2020 6173 6d67  lf,.        asmg
+0004da00: 6174 6577 6179 5f6e 616d 653a 2073 7472  ateway_name: str
+0004da10: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0004da20: 2073 6572 7669 6365 5f6d 6573 685f 6964   service_mesh_id
+0004da30: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+0004da40: 2020 2020 2020 7365 7276 6963 655f 6e61        service_na
+0004da50: 6d65 733a 2073 7472 203d 204e 6f6e 652c  mes: str = None,
+0004da60: 0a20 2020 2020 2020 2073 6572 7669 6365  .        service
+0004da70: 5f6e 616d 6573 7061 6365 3a20 7374 7220  _namespace: str 
+0004da80: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
+0004da90: 2020 2020 2020 2073 656c 662e 6173 6d67         self.asmg
+0004daa0: 6174 6577 6179 5f6e 616d 6520 3d20 6173  ateway_name = as
+0004dab0: 6d67 6174 6577 6179 5f6e 616d 650a 2020  mgateway_name.  
+0004dac0: 2020 2020 2020 7365 6c66 2e73 6572 7669        self.servi
+0004dad0: 6365 5f6d 6573 685f 6964 203d 2073 6572  ce_mesh_id = ser
+0004dae0: 7669 6365 5f6d 6573 685f 6964 0a20 2020  vice_mesh_id.   
+0004daf0: 2020 2020 2073 656c 662e 7365 7276 6963       self.servic
+0004db00: 655f 6e61 6d65 7320 3d20 7365 7276 6963  e_names = servic
+0004db10: 655f 6e61 6d65 730a 2020 2020 2020 2020  e_names.        
+0004db20: 7365 6c66 2e73 6572 7669 6365 5f6e 616d  self.service_nam
+0004db30: 6573 7061 6365 203d 2073 6572 7669 6365  espace = service
+0004db40: 5f6e 616d 6573 7061 6365 0a0a 2020 2020  _namespace..    
+0004db50: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+0004db60: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+0004db70: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+0004db80: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0004db90: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+0004dba0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+0004dbb0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+0004dbc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0004dbd0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+0004dbe0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+0004dbf0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+0004dc00: 2073 656c 662e 6173 6d67 6174 6577 6179   self.asmgateway
+0004dc10: 5f6e 616d 6520 6973 206e 6f74 204e 6f6e  _name is not Non
+0004dc20: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0004dc30: 6573 756c 745b 2741 534d 4761 7465 7761  esult['ASMGatewa
+0004dc40: 794e 616d 6527 5d20 3d20 7365 6c66 2e61  yName'] = self.a
+0004dc50: 736d 6761 7465 7761 795f 6e61 6d65 0a20  smgateway_name. 
+0004dc60: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+0004dc70: 6572 7669 6365 5f6d 6573 685f 6964 2069  ervice_mesh_id i
+0004dc80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0004dc90: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0004dca0: 5365 7276 6963 654d 6573 6849 6427 5d20  ServiceMeshId'] 
+0004dcb0: 3d20 7365 6c66 2e73 6572 7669 6365 5f6d  = self.service_m
+0004dcc0: 6573 685f 6964 0a20 2020 2020 2020 2069  esh_id.        i
+0004dcd0: 6620 7365 6c66 2e73 6572 7669 6365 5f6e  f self.service_n
+0004dce0: 616d 6573 2069 7320 6e6f 7420 4e6f 6e65  ames is not None
+0004dcf0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0004dd00: 7375 6c74 5b27 5365 7276 6963 654e 616d  sult['ServiceNam
+0004dd10: 6573 275d 203d 2073 656c 662e 7365 7276  es'] = self.serv
+0004dd20: 6963 655f 6e61 6d65 730a 2020 2020 2020  ice_names.      
+0004dd30: 2020 6966 2073 656c 662e 7365 7276 6963    if self.servic
+0004dd40: 655f 6e61 6d65 7370 6163 6520 6973 206e  e_namespace is n
+0004dd50: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0004dd60: 2020 2020 2072 6573 756c 745b 2753 6572       result['Ser
+0004dd70: 7669 6365 4e61 6d65 7370 6163 6527 5d20  viceNamespace'] 
+0004dd80: 3d20 7365 6c66 2e73 6572 7669 6365 5f6e  = self.service_n
+0004dd90: 616d 6573 7061 6365 0a20 2020 2020 2020  amespace.       
+0004dda0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+0004ddb0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+0004ddc0: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+0004ddd0: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+0004dde0: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+0004ddf0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0004de00: 2827 4153 4d47 6174 6577 6179 4e61 6d65  ('ASMGatewayName
+0004de10: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0004de20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0004de30: 2e61 736d 6761 7465 7761 795f 6e61 6d65  .asmgateway_name
+0004de40: 203d 206d 2e67 6574 2827 4153 4d47 6174   = m.get('ASMGat
+0004de50: 6577 6179 4e61 6d65 2729 0a20 2020 2020  ewayName').     
+0004de60: 2020 2069 6620 6d2e 6765 7428 2753 6572     if m.get('Ser
+0004de70: 7669 6365 4d65 7368 4964 2729 2069 7320  viceMeshId') is 
+0004de80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0004de90: 2020 2020 2020 7365 6c66 2e73 6572 7669        self.servi
+0004dea0: 6365 5f6d 6573 685f 6964 203d 206d 2e67  ce_mesh_id = m.g
+0004deb0: 6574 2827 5365 7276 6963 654d 6573 6849  et('ServiceMeshI
+0004dec0: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
+0004ded0: 2e67 6574 2827 5365 7276 6963 654e 616d  .get('ServiceNam
+0004dee0: 6573 2729 2069 7320 6e6f 7420 4e6f 6e65  es') is not None
+0004def0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0004df00: 6c66 2e73 6572 7669 6365 5f6e 616d 6573  lf.service_names
+0004df10: 203d 206d 2e67 6574 2827 5365 7276 6963   = m.get('Servic
+0004df20: 654e 616d 6573 2729 0a20 2020 2020 2020  eNames').       
+0004df30: 2069 6620 6d2e 6765 7428 2753 6572 7669   if m.get('Servi
+0004df40: 6365 4e61 6d65 7370 6163 6527 2920 6973  ceNamespace') is
+0004df50: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0004df60: 2020 2020 2020 2073 656c 662e 7365 7276         self.serv
+0004df70: 6963 655f 6e61 6d65 7370 6163 6520 3d20  ice_namespace = 
+0004df80: 6d2e 6765 7428 2753 6572 7669 6365 4e61  m.get('ServiceNa
+0004df90: 6d65 7370 6163 6527 290a 2020 2020 2020  mespace').      
+0004dfa0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+0004dfb0: 636c 6173 7320 5570 6461 7465 4153 4d47  class UpdateASMG
+0004dfc0: 6174 6577 6179 496d 706f 7274 6564 5365  atewayImportedSe
+0004dfd0: 7276 6963 6573 5265 7370 6f6e 7365 426f  rvicesResponseBo
+0004dfe0: 6479 2854 6561 4d6f 6465 6c29 3a0a 2020  dy(TeaModel):.  
+0004dff0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+0004e000: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0004e010: 2020 2020 2020 7265 7175 6573 745f 6964        request_id
+0004e020: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+0004e030: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+0004e040: 662e 7265 7175 6573 745f 6964 203d 2072  f.request_id = r
+0004e050: 6571 7565 7374 5f69 640a 0a20 2020 2064  equest_id..    d
+0004e060: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+0004e070: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+0004e080: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+0004e090: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+0004e0a0: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+0004e0b0: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+0004e0c0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+0004e0d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0004e0e0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+0004e0f0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+0004e100: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0004e110: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+0004e120: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0004e130: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0004e140: 2752 6571 7565 7374 4964 275d 203d 2073  'RequestId'] = s
+0004e150: 656c 662e 7265 7175 6573 745f 6964 0a20  elf.request_id. 
+0004e160: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0004e170: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+0004e180: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+0004e190: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+0004e1a0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+0004e1b0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+0004e1c0: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
+0004e1d0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+0004e1e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0004e1f0: 662e 7265 7175 6573 745f 6964 203d 206d  f.request_id = m
+0004e200: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
+0004e210: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0004e220: 2073 656c 660a 0a0a 636c 6173 7320 5570   self...class Up
+0004e230: 6461 7465 4153 4d47 6174 6577 6179 496d  dateASMGatewayIm
+0004e240: 706f 7274 6564 5365 7276 6963 6573 5265  portedServicesRe
+0004e250: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
+0004e260: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+0004e270: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+0004e280: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
+0004e290: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
+0004e2a0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0004e2b0: 2020 626f 6479 3a20 5570 6461 7465 4153    body: UpdateAS
+0004e2c0: 4d47 6174 6577 6179 496d 706f 7274 6564  MGatewayImported
+0004e2d0: 5365 7276 6963 6573 5265 7370 6f6e 7365  ServicesResponse
+0004e2e0: 426f 6479 203d 204e 6f6e 652c 0a20 2020  Body = None,.   
+0004e2f0: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
+0004e300: 2e68 6561 6465 7273 203d 2068 6561 6465  .headers = heade
+0004e310: 7273 0a20 2020 2020 2020 2073 656c 662e  rs.        self.
+0004e320: 626f 6479 203d 2062 6f64 790a 0a20 2020  body = body..   
+0004e330: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+0004e340: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
+0004e350: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+0004e360: 7265 6428 7365 6c66 2e68 6561 6465 7273  red(self.headers
+0004e370: 2c20 2768 6561 6465 7273 2729 0a20 2020  , 'headers').   
+0004e380: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
+0004e390: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
+0004e3a0: 2e62 6f64 792c 2027 626f 6479 2729 0a20  .body, 'body'). 
+0004e3b0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+0004e3c0: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
+0004e3d0: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
+0004e3e0: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
+0004e3f0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+0004e400: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+0004e410: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+0004e420: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+0004e430: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0004e440: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+0004e450: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+0004e460: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+0004e470: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
+0004e480: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
+0004e490: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0004e4a0: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
+0004e4b0: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
+0004e4c0: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+0004e4d0: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+0004e4e0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0004e4f0: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
+0004e500: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
+0004e510: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0004e520: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+0004e530: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+0004e540: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+0004e550: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+0004e560: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+0004e570: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+0004e580: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0004e590: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0004e5a0: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
+0004e5b0: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
+0004e5c0: 2020 2069 6620 6d2e 6765 7428 2762 6f64     if m.get('bod
+0004e5d0: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
+0004e5e0: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+0004e5f0: 705f 6d6f 6465 6c20 3d20 5570 6461 7465  p_model = Update
+0004e600: 4153 4d47 6174 6577 6179 496d 706f 7274  ASMGatewayImport
+0004e610: 6564 5365 7276 6963 6573 5265 7370 6f6e  edServicesRespon
+0004e620: 7365 426f 6479 2829 0a20 2020 2020 2020  seBody().       
+0004e630: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+0004e640: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
+0004e650: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
+0004e660: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0004e670: 656c 660a 0a0a 636c 6173 7320 5570 6461  elf...class Upda
+0004e680: 7465 4d65 7368 4665 6174 7572 6552 6571  teMeshFeatureReq
+0004e690: 7565 7374 2854 6561 4d6f 6465 6c29 3a0a  uest(TeaModel):.
+0004e6a0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0004e6b0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0004e6c0: 2020 2020 2020 2020 6163 6365 7373 5f6c          access_l
+0004e6d0: 6f67 5f65 6e61 626c 6564 3a20 626f 6f6c  og_enabled: bool
+0004e6e0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0004e6f0: 2061 6363 6573 735f 6c6f 675f 6669 6c65   access_log_file
+0004e700: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+0004e710: 2020 2020 2020 6163 6365 7373 5f6c 6f67        access_log
+0004e720: 5f66 6f72 6d61 743a 2073 7472 203d 204e  _format: str = N
+0004e730: 6f6e 652c 0a20 2020 2020 2020 2061 6363  one,.        acc
+0004e740: 6573 735f 6c6f 675f 7072 6f6a 6563 743a  ess_log_project:
+0004e750: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+0004e760: 2020 2020 2061 6363 6573 735f 6c6f 675f       access_log_
+0004e770: 7365 7276 6963 655f 656e 6162 6c65 643a  service_enabled:
+0004e780: 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020   bool = None,.  
+0004e790: 2020 2020 2020 6163 6365 7373 5f6c 6f67        access_log
+0004e7a0: 5f73 6572 7669 6365 5f68 6f73 743a 2073  _service_host: s
+0004e7b0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0004e7c0: 2020 2061 6363 6573 735f 6c6f 675f 7365     access_log_se
+0004e7d0: 7276 6963 655f 706f 7274 3a20 696e 7420  rvice_port: int 
+0004e7e0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0004e7f0: 6175 6469 745f 7072 6f6a 6563 743a 2073  audit_project: s
+0004e800: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0004e810: 2020 2061 7574 6f5f 696e 6a65 6374 696f     auto_injectio
+0004e820: 6e5f 706f 6c69 6379 5f65 6e61 626c 6564  n_policy_enabled
+0004e830: 3a20 626f 6f6c 203d 204e 6f6e 652c 0a20  : bool = None,. 
+0004e840: 2020 2020 2020 2063 7261 6767 7265 6761         craggrega
+0004e850: 7469 6f6e 5f65 6e61 626c 6564 3a20 626f  tion_enabled: bo
+0004e860: 6f6c 203d 204e 6f6e 652c 0a20 2020 2020  ol = None,.     
+0004e870: 2020 2063 6c75 7374 6572 5f73 7065 633a     cluster_spec:
+0004e880: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+0004e890: 2020 2020 2063 6e69 5f65 6e61 626c 6564       cni_enabled
+0004e8a0: 3a20 626f 6f6c 203d 204e 6f6e 652c 0a20  : bool = None,. 
+0004e8b0: 2020 2020 2020 2063 6e69 5f65 7863 6c75         cni_exclu
+0004e8c0: 6465 5f6e 616d 6573 7061 6365 733a 2073  de_namespaces: s
+0004e8d0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0004e8e0: 2020 2063 6f6e 6669 675f 736f 7572 6365     config_source
+0004e8f0: 5f65 6e61 626c 6564 3a20 626f 6f6c 203d  _enabled: bool =
+0004e900: 204e 6f6e 652c 0a20 2020 2020 2020 2063   None,.        c
+0004e910: 6f6e 6669 675f 736f 7572 6365 5f6e 6163  onfig_source_nac
+0004e920: 6f73 5f69 643a 2073 7472 203d 204e 6f6e  os_id: str = Non
+0004e930: 652c 0a20 2020 2020 2020 2063 7573 746f  e,.        custo
+0004e940: 6d69 7a65 645f 7072 6f6d 6574 6865 7573  mized_prometheus
+0004e950: 3a20 626f 6f6c 203d 204e 6f6e 652c 0a20  : bool = None,. 
+0004e960: 2020 2020 2020 2063 7573 746f 6d69 7a65         customize
+0004e970: 645f 7a69 706b 696e 3a20 626f 6f6c 203d  d_zipkin: bool =
+0004e980: 204e 6f6e 652c 0a20 2020 2020 2020 2064   None,.        d
+0004e990: 6e73 7072 6f78 7969 6e67 5f65 6e61 626c  nsproxying_enabl
+0004e9a0: 6564 3a20 626f 6f6c 203d 204e 6f6e 652c  ed: bool = None,
+0004e9b0: 0a20 2020 2020 2020 2064 6973 636f 7665  .        discove
+0004e9c0: 7279 5f73 656c 6563 746f 7273 3a20 7374  ry_selectors: st
+0004e9d0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+0004e9e0: 2020 6475 6262 6f5f 6669 6c74 6572 5f65    dubbo_filter_e
+0004e9f0: 6e61 626c 6564 3a20 626f 6f6c 203d 204e  nabled: bool = N
+0004ea00: 6f6e 652c 0a20 2020 2020 2020 2065 6e61  one,.        ena
+0004ea10: 626c 655f 6175 6469 743a 2062 6f6f 6c20  ble_audit: bool 
+0004ea20: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0004ea30: 656e 6162 6c65 5f63 7268 6973 746f 7279  enable_crhistory
+0004ea40: 3a20 626f 6f6c 203d 204e 6f6e 652c 0a20  : bool = None,. 
+0004ea50: 2020 2020 2020 2065 6e61 626c 655f 6e61         enable_na
+0004ea60: 6d65 7370 6163 6573 5f62 795f 6465 6661  mespaces_by_defa
+0004ea70: 756c 743a 2062 6f6f 6c20 3d20 4e6f 6e65  ult: bool = None
+0004ea80: 2c0a 2020 2020 2020 2020 656e 6162 6c65  ,.        enable
+0004ea90: 5f73 6473 7365 7276 6572 3a20 626f 6f6c  _sdsserver: bool
+0004eaa0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0004eab0: 2065 7863 6c75 6465 5f69 7072 616e 6765   exclude_iprange
+0004eac0: 733a 2073 7472 203d 204e 6f6e 652c 0a20  s: str = None,. 
+0004ead0: 2020 2020 2020 2065 7863 6c75 6465 5f69         exclude_i
+0004eae0: 6e62 6f75 6e64 5f70 6f72 7473 3a20 7374  nbound_ports: st
+0004eaf0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+0004eb00: 2020 6578 636c 7564 655f 6f75 7462 6f75    exclude_outbou
+0004eb10: 6e64 5f70 6f72 7473 3a20 7374 7220 3d20  nd_ports: str = 
+0004eb20: 4e6f 6e65 2c0a 2020 2020 2020 2020 6669  None,.        fi
+0004eb30: 6c74 6572 5f67 6174 6577 6179 5f63 6c75  lter_gateway_clu
+0004eb40: 7374 6572 5f63 6f6e 6669 673a 2062 6f6f  ster_config: boo
+0004eb50: 6c20 3d20 4e6f 6e65 2c0a 2020 2020 2020  l = None,.      
+0004eb60: 2020 6761 7465 7761 795f 6170 6965 6e61    gateway_apiena
+0004eb70: 626c 6564 3a20 626f 6f6c 203d 204e 6f6e  bled: bool = Non
+0004eb80: 652c 0a20 2020 2020 2020 2067 6c6f 6261  e,.        globa
+0004eb90: 6c5f 7261 7465 5f6c 696d 6974 5f65 6e61  l_rate_limit_ena
+0004eba0: 626c 6564 3a20 626f 6f6c 203d 204e 6f6e  bled: bool = Non
+0004ebb0: 652c 0a20 2020 2020 2020 2068 7474 705f  e,.        http_
+0004ebc0: 3130 656e 6162 6c65 643a 2062 6f6f 6c20  10enabled: bool 
+0004ebd0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0004ebe0: 696e 636c 7564 655f 6970 7261 6e67 6573  include_ipranges
+0004ebf0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+0004ec00: 2020 2020 2020 696e 636c 7564 655f 696e        include_in
+0004ec10: 626f 756e 645f 706f 7274 733a 2073 7472  bound_ports: str
+0004ec20: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0004ec30: 206b 6961 6c69 5f65 6e61 626c 6564 3a20   kiali_enabled: 
+0004ec40: 626f 6f6c 203d 204e 6f6e 652c 0a20 2020  bool = None,.   
+0004ec50: 2020 2020 206c 6966 6563 7963 6c65 3a20       lifecycle: 
+0004ec60: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+0004ec70: 2020 2020 6c6f 6361 6c69 7479 5f6c 6263      locality_lbc
+0004ec80: 6f6e 663a 2073 7472 203d 204e 6f6e 652c  onf: str = None,
+0004ec90: 0a20 2020 2020 2020 206c 6f63 616c 6974  .        localit
+0004eca0: 795f 6c6f 6164 5f62 616c 616e 6369 6e67  y_load_balancing
+0004ecb0: 3a20 626f 6f6c 203d 204e 6f6e 652c 0a20  : bool = None,. 
+0004ecc0: 2020 2020 2020 206d 7365 656e 6162 6c65         mseenable
+0004ecd0: 643a 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a  d: bool = None,.
+0004ece0: 2020 2020 2020 2020 6d75 6c74 695f 6275          multi_bu
+0004ecf0: 6666 6572 5f65 6e61 626c 6564 3a20 626f  ffer_enabled: bo
+0004ed00: 6f6c 203d 204e 6f6e 652c 0a20 2020 2020  ol = None,.     
+0004ed10: 2020 206d 756c 7469 5f62 7566 6665 725f     multi_buffer_
+0004ed20: 706f 6c6c 5f64 656c 6179 3a20 7374 7220  poll_delay: str 
+0004ed30: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0004ed40: 6d79 7371 6c5f 6669 6c74 6572 5f65 6e61  mysql_filter_ena
+0004ed50: 626c 6564 3a20 626f 6f6c 203d 204e 6f6e  bled: bool = Non
+0004ed60: 652c 0a20 2020 2020 2020 206f 7061 6c69  e,.        opali
+0004ed70: 6d69 745f 6370 753a 2073 7472 203d 204e  mit_cpu: str = N
+0004ed80: 6f6e 652c 0a20 2020 2020 2020 206f 7061  one,.        opa
+0004ed90: 6c69 6d69 745f 6d65 6d6f 7279 3a20 7374  limit_memory: st
+0004eda0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+0004edb0: 2020 6f70 616c 6f67 5f6c 6576 656c 3a20    opalog_level: 
+0004edc0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+0004edd0: 2020 2020 6f70 6172 6571 7565 7374 5f63      oparequest_c
+0004ede0: 7075 3a20 7374 7220 3d20 4e6f 6e65 2c0a  pu: str = None,.
+0004edf0: 2020 2020 2020 2020 6f70 6172 6571 7565          opareque
+0004ee00: 7374 5f6d 656d 6f72 793a 2073 7472 203d  st_memory: str =
+0004ee10: 204e 6f6e 652c 0a20 2020 2020 2020 206f   None,.        o
+0004ee20: 7061 5f65 6e61 626c 6564 3a20 626f 6f6c  pa_enabled: bool
+0004ee30: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0004ee40: 206f 7065 6e5f 6167 656e 745f 706f 6c69   open_agent_poli
+0004ee50: 6379 3a20 626f 6f6c 203d 204e 6f6e 652c  cy: bool = None,
+0004ee60: 0a20 2020 2020 2020 206f 7574 626f 756e  .        outboun
+0004ee70: 645f 7472 6166 6669 635f 706f 6c69 6379  d_traffic_policy
+0004ee80: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+0004ee90: 2020 2020 2020 7072 6f6d 6574 6865 7573        prometheus
+0004eea0: 5f75 726c 3a20 7374 7220 3d20 4e6f 6e65  _url: str = None
+0004eeb0: 2c0a 2020 2020 2020 2020 7072 6f78 795f  ,.        proxy_
+0004eec0: 696e 6974 5f63 7075 7265 736f 7572 6365  init_cpuresource
+0004eed0: 5f6c 696d 6974 3a20 7374 7220 3d20 4e6f  _limit: str = No
+0004eee0: 6e65 2c0a 2020 2020 2020 2020 7072 6f78  ne,.        prox
+0004eef0: 795f 696e 6974 5f63 7075 7265 736f 7572  y_init_cpuresour
+0004ef00: 6365 5f72 6571 7565 7374 3a20 7374 7220  ce_request: str 
+0004ef10: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0004ef20: 7072 6f78 795f 696e 6974 5f6d 656d 6f72  proxy_init_memor
+0004ef30: 795f 7265 736f 7572 6365 5f6c 696d 6974  y_resource_limit
+0004ef40: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+0004ef50: 2020 2020 2020 7072 6f78 795f 696e 6974        proxy_init
+0004ef60: 5f6d 656d 6f72 795f 7265 736f 7572 6365  _memory_resource
+0004ef70: 5f72 6571 7565 7374 3a20 7374 7220 3d20  _request: str = 
+0004ef80: 4e6f 6e65 2c0a 2020 2020 2020 2020 7072  None,.        pr
+0004ef90: 6f78 795f 6c69 6d69 745f 6370 753a 2073  oxy_limit_cpu: s
+0004efa0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0004efb0: 2020 2070 726f 7879 5f6c 696d 6974 5f6d     proxy_limit_m
+0004efc0: 656d 6f72 793a 2073 7472 203d 204e 6f6e  emory: str = Non
+0004efd0: 652c 0a20 2020 2020 2020 2070 726f 7879  e,.        proxy
+0004efe0: 5f72 6571 7565 7374 5f63 7075 3a20 7374  _request_cpu: st
+0004eff0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+0004f000: 2020 7072 6f78 795f 7265 7175 6573 745f    proxy_request_
+0004f010: 6d65 6d6f 7279 3a20 7374 7220 3d20 4e6f  memory: str = No
+0004f020: 6e65 2c0a 2020 2020 2020 2020 7265 6469  ne,.        redi
+0004f030: 735f 6669 6c74 6572 5f65 6e61 626c 6564  s_filter_enabled
+0004f040: 3a20 626f 6f6c 203d 204e 6f6e 652c 0a20  : bool = None,. 
+0004f050: 2020 2020 2020 2073 6572 7669 6365 5f6d         service_m
+0004f060: 6573 685f 6964 3a20 7374 7220 3d20 4e6f  esh_id: str = No
+0004f070: 6e65 2c0a 2020 2020 2020 2020 7369 6465  ne,.        side
+0004f080: 6361 725f 696e 6a65 6374 6f72 5f6c 696d  car_injector_lim
+0004f090: 6974 5f63 7075 3a20 7374 7220 3d20 4e6f  it_cpu: str = No
+0004f0a0: 6e65 2c0a 2020 2020 2020 2020 7369 6465  ne,.        side
+0004f0b0: 6361 725f 696e 6a65 6374 6f72 5f6c 696d  car_injector_lim
+0004f0c0: 6974 5f6d 656d 6f72 793a 2073 7472 203d  it_memory: str =
+0004f0d0: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
+0004f0e0: 6964 6563 6172 5f69 6e6a 6563 746f 725f  idecar_injector_
+0004f0f0: 7265 7175 6573 745f 6370 753a 2073 7472  request_cpu: str
+0004f100: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0004f110: 2073 6964 6563 6172 5f69 6e6a 6563 746f   sidecar_injecto
+0004f120: 725f 7265 7175 6573 745f 6d65 6d6f 7279  r_request_memory
+0004f130: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+0004f140: 2020 2020 2020 7369 6465 6361 725f 696e        sidecar_in
+0004f150: 6a65 6374 6f72 5f77 6562 686f 6f6b 5f61  jector_webhook_a
+0004f160: 735f 7961 6d6c 3a20 7374 7220 3d20 4e6f  s_yaml: str = No
+0004f170: 6e65 2c0a 2020 2020 2020 2020 7465 6c65  ne,.        tele
+0004f180: 6d65 7472 793a 2062 6f6f 6c20 3d20 4e6f  metry: bool = No
+0004f190: 6e65 2c0a 2020 2020 2020 2020 7465 726d  ne,.        term
+0004f1a0: 696e 6174 696f 6e5f 6472 6169 6e5f 6475  ination_drain_du
+0004f1b0: 7261 7469 6f6e 3a20 7374 7220 3d20 4e6f  ration: str = No
+0004f1c0: 6e65 2c0a 2020 2020 2020 2020 7468 7269  ne,.        thri
+0004f1d0: 6674 5f66 696c 7465 725f 656e 6162 6c65  ft_filter_enable
+0004f1e0: 643a 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a  d: bool = None,.
+0004f1f0: 2020 2020 2020 2020 7472 6163 655f 7361          trace_sa
+0004f200: 6d70 6c69 6e67 3a20 666c 6f61 7420 3d20  mpling: float = 
+0004f210: 4e6f 6e65 2c0a 2020 2020 2020 2020 7472  None,.        tr
+0004f220: 6163 696e 673a 2062 6f6f 6c20 3d20 4e6f  acing: bool = No
+0004f230: 6e65 2c0a 2020 2020 2020 2020 7765 625f  ne,.        web_
+0004f240: 6173 7365 6d62 6c79 5f66 696c 7465 725f  assembly_filter_
+0004f250: 656e 6162 6c65 643a 2062 6f6f 6c20 3d20  enabled: bool = 
+0004f260: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+0004f270: 2020 2020 2073 656c 662e 6163 6365 7373       self.access
+0004f280: 5f6c 6f67 5f65 6e61 626c 6564 203d 2061  _log_enabled = a
+0004f290: 6363 6573 735f 6c6f 675f 656e 6162 6c65  ccess_log_enable
+0004f2a0: 640a 2020 2020 2020 2020 7365 6c66 2e61  d.        self.a
+0004f2b0: 6363 6573 735f 6c6f 675f 6669 6c65 203d  ccess_log_file =
+0004f2c0: 2061 6363 6573 735f 6c6f 675f 6669 6c65   access_log_file
+0004f2d0: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
+0004f2e0: 6365 7373 5f6c 6f67 5f66 6f72 6d61 7420  cess_log_format 
+0004f2f0: 3d20 6163 6365 7373 5f6c 6f67 5f66 6f72  = access_log_for
+0004f300: 6d61 740a 2020 2020 2020 2020 7365 6c66  mat.        self
+0004f310: 2e61 6363 6573 735f 6c6f 675f 7072 6f6a  .access_log_proj
+0004f320: 6563 7420 3d20 6163 6365 7373 5f6c 6f67  ect = access_log
+0004f330: 5f70 726f 6a65 6374 0a20 2020 2020 2020  _project.       
+0004f340: 2073 656c 662e 6163 6365 7373 5f6c 6f67   self.access_log
+0004f350: 5f73 6572 7669 6365 5f65 6e61 626c 6564  _service_enabled
+0004f360: 203d 2061 6363 6573 735f 6c6f 675f 7365   = access_log_se
+0004f370: 7276 6963 655f 656e 6162 6c65 640a 2020  rvice_enabled.  
+0004f380: 2020 2020 2020 7365 6c66 2e61 6363 6573        self.acces
+0004f390: 735f 6c6f 675f 7365 7276 6963 655f 686f  s_log_service_ho
+0004f3a0: 7374 203d 2061 6363 6573 735f 6c6f 675f  st = access_log_
+0004f3b0: 7365 7276 6963 655f 686f 7374 0a20 2020  service_host.   
+0004f3c0: 2020 2020 2073 656c 662e 6163 6365 7373       self.access
+0004f3d0: 5f6c 6f67 5f73 6572 7669 6365 5f70 6f72  _log_service_por
+0004f3e0: 7420 3d20 6163 6365 7373 5f6c 6f67 5f73  t = access_log_s
+0004f3f0: 6572 7669 6365 5f70 6f72 740a 2020 2020  ervice_port.    
+0004f400: 2020 2020 7365 6c66 2e61 7564 6974 5f70      self.audit_p
+0004f410: 726f 6a65 6374 203d 2061 7564 6974 5f70  roject = audit_p
+0004f420: 726f 6a65 6374 0a20 2020 2020 2020 2073  roject.        s
+0004f430: 656c 662e 6175 746f 5f69 6e6a 6563 7469  elf.auto_injecti
+0004f440: 6f6e 5f70 6f6c 6963 795f 656e 6162 6c65  on_policy_enable
+0004f450: 6420 3d20 6175 746f 5f69 6e6a 6563 7469  d = auto_injecti
+0004f460: 6f6e 5f70 6f6c 6963 795f 656e 6162 6c65  on_policy_enable
+0004f470: 640a 2020 2020 2020 2020 7365 6c66 2e63  d.        self.c
+0004f480: 7261 6767 7265 6761 7469 6f6e 5f65 6e61  raggregation_ena
+0004f490: 626c 6564 203d 2063 7261 6767 7265 6761  bled = craggrega
+0004f4a0: 7469 6f6e 5f65 6e61 626c 6564 0a20 2020  tion_enabled.   
+0004f4b0: 2020 2020 2073 656c 662e 636c 7573 7465       self.cluste
+0004f4c0: 725f 7370 6563 203d 2063 6c75 7374 6572  r_spec = cluster
+0004f4d0: 5f73 7065 630a 2020 2020 2020 2020 7365  _spec.        se
+0004f4e0: 6c66 2e63 6e69 5f65 6e61 626c 6564 203d  lf.cni_enabled =
+0004f4f0: 2063 6e69 5f65 6e61 626c 6564 0a20 2020   cni_enabled.   
+0004f500: 2020 2020 2073 656c 662e 636e 695f 6578       self.cni_ex
+0004f510: 636c 7564 655f 6e61 6d65 7370 6163 6573  clude_namespaces
+0004f520: 203d 2063 6e69 5f65 7863 6c75 6465 5f6e   = cni_exclude_n
+0004f530: 616d 6573 7061 6365 730a 2020 2020 2020  amespaces.      
+0004f540: 2020 7365 6c66 2e63 6f6e 6669 675f 736f    self.config_so
+0004f550: 7572 6365 5f65 6e61 626c 6564 203d 2063  urce_enabled = c
+0004f560: 6f6e 6669 675f 736f 7572 6365 5f65 6e61  onfig_source_ena
+0004f570: 626c 6564 0a20 2020 2020 2020 2073 656c  bled.        sel
+0004f580: 662e 636f 6e66 6967 5f73 6f75 7263 655f  f.config_source_
+0004f590: 6e61 636f 735f 6964 203d 2063 6f6e 6669  nacos_id = confi
+0004f5a0: 675f 736f 7572 6365 5f6e 6163 6f73 5f69  g_source_nacos_i
+0004f5b0: 640a 2020 2020 2020 2020 7365 6c66 2e63  d.        self.c
+0004f5c0: 7573 746f 6d69 7a65 645f 7072 6f6d 6574  ustomized_promet
+0004f5d0: 6865 7573 203d 2063 7573 746f 6d69 7a65  heus = customize
+0004f5e0: 645f 7072 6f6d 6574 6865 7573 0a20 2020  d_prometheus.   
+0004f5f0: 2020 2020 2073 656c 662e 6375 7374 6f6d       self.custom
+0004f600: 697a 6564 5f7a 6970 6b69 6e20 3d20 6375  ized_zipkin = cu
+0004f610: 7374 6f6d 697a 6564 5f7a 6970 6b69 6e0a  stomized_zipkin.
+0004f620: 2020 2020 2020 2020 7365 6c66 2e64 6e73          self.dns
+0004f630: 7072 6f78 7969 6e67 5f65 6e61 626c 6564  proxying_enabled
+0004f640: 203d 2064 6e73 7072 6f78 7969 6e67 5f65   = dnsproxying_e
+0004f650: 6e61 626c 6564 0a20 2020 2020 2020 2073  nabled.        s
+0004f660: 656c 662e 6469 7363 6f76 6572 795f 7365  elf.discovery_se
+0004f670: 6c65 6374 6f72 7320 3d20 6469 7363 6f76  lectors = discov
+0004f680: 6572 795f 7365 6c65 6374 6f72 730a 2020  ery_selectors.  
+0004f690: 2020 2020 2020 7365 6c66 2e64 7562 626f        self.dubbo
+0004f6a0: 5f66 696c 7465 725f 656e 6162 6c65 6420  _filter_enabled 
+0004f6b0: 3d20 6475 6262 6f5f 6669 6c74 6572 5f65  = dubbo_filter_e
+0004f6c0: 6e61 626c 6564 0a20 2020 2020 2020 2073  nabled.        s
+0004f6d0: 656c 662e 656e 6162 6c65 5f61 7564 6974  elf.enable_audit
+0004f6e0: 203d 2065 6e61 626c 655f 6175 6469 740a   = enable_audit.
+0004f6f0: 2020 2020 2020 2020 7365 6c66 2e65 6e61          self.ena
+0004f700: 626c 655f 6372 6869 7374 6f72 7920 3d20  ble_crhistory = 
+0004f710: 656e 6162 6c65 5f63 7268 6973 746f 7279  enable_crhistory
+0004f720: 0a20 2020 2020 2020 2073 656c 662e 656e  .        self.en
+0004f730: 6162 6c65 5f6e 616d 6573 7061 6365 735f  able_namespaces_
+0004f740: 6279 5f64 6566 6175 6c74 203d 2065 6e61  by_default = ena
+0004f750: 626c 655f 6e61 6d65 7370 6163 6573 5f62  ble_namespaces_b
+0004f760: 795f 6465 6661 756c 740a 2020 2020 2020  y_default.      
+0004f770: 2020 7365 6c66 2e65 6e61 626c 655f 7364    self.enable_sd
+0004f780: 7373 6572 7665 7220 3d20 656e 6162 6c65  sserver = enable
+0004f790: 5f73 6473 7365 7276 6572 0a20 2020 2020  _sdsserver.     
+0004f7a0: 2020 2073 656c 662e 6578 636c 7564 655f     self.exclude_
+0004f7b0: 6970 7261 6e67 6573 203d 2065 7863 6c75  ipranges = exclu
+0004f7c0: 6465 5f69 7072 616e 6765 730a 2020 2020  de_ipranges.    
+0004f7d0: 2020 2020 7365 6c66 2e65 7863 6c75 6465      self.exclude
+0004f7e0: 5f69 6e62 6f75 6e64 5f70 6f72 7473 203d  _inbound_ports =
+0004f7f0: 2065 7863 6c75 6465 5f69 6e62 6f75 6e64   exclude_inbound
+0004f800: 5f70 6f72 7473 0a20 2020 2020 2020 2073  _ports.        s
+0004f810: 656c 662e 6578 636c 7564 655f 6f75 7462  elf.exclude_outb
+0004f820: 6f75 6e64 5f70 6f72 7473 203d 2065 7863  ound_ports = exc
+0004f830: 6c75 6465 5f6f 7574 626f 756e 645f 706f  lude_outbound_po
+0004f840: 7274 730a 2020 2020 2020 2020 7365 6c66  rts.        self
+0004f850: 2e66 696c 7465 725f 6761 7465 7761 795f  .filter_gateway_
+0004f860: 636c 7573 7465 725f 636f 6e66 6967 203d  cluster_config =
+0004f870: 2066 696c 7465 725f 6761 7465 7761 795f   filter_gateway_
+0004f880: 636c 7573 7465 725f 636f 6e66 6967 0a20  cluster_config. 
+0004f890: 2020 2020 2020 2073 656c 662e 6761 7465         self.gate
+0004f8a0: 7761 795f 6170 6965 6e61 626c 6564 203d  way_apienabled =
+0004f8b0: 2067 6174 6577 6179 5f61 7069 656e 6162   gateway_apienab
+0004f8c0: 6c65 640a 2020 2020 2020 2020 7365 6c66  led.        self
+0004f8d0: 2e67 6c6f 6261 6c5f 7261 7465 5f6c 696d  .global_rate_lim
+0004f8e0: 6974 5f65 6e61 626c 6564 203d 2067 6c6f  it_enabled = glo
+0004f8f0: 6261 6c5f 7261 7465 5f6c 696d 6974 5f65  bal_rate_limit_e
+0004f900: 6e61 626c 6564 0a20 2020 2020 2020 2073  nabled.        s
+0004f910: 656c 662e 6874 7470 5f31 3065 6e61 626c  elf.http_10enabl
+0004f920: 6564 203d 2068 7474 705f 3130 656e 6162  ed = http_10enab
+0004f930: 6c65 640a 2020 2020 2020 2020 7365 6c66  led.        self
+0004f940: 2e69 6e63 6c75 6465 5f69 7072 616e 6765  .include_iprange
+0004f950: 7320 3d20 696e 636c 7564 655f 6970 7261  s = include_ipra
+0004f960: 6e67 6573 0a20 2020 2020 2020 2073 656c  nges.        sel
+0004f970: 662e 696e 636c 7564 655f 696e 626f 756e  f.include_inboun
+0004f980: 645f 706f 7274 7320 3d20 696e 636c 7564  d_ports = includ
+0004f990: 655f 696e 626f 756e 645f 706f 7274 730a  e_inbound_ports.
+0004f9a0: 2020 2020 2020 2020 7365 6c66 2e6b 6961          self.kia
+0004f9b0: 6c69 5f65 6e61 626c 6564 203d 206b 6961  li_enabled = kia
+0004f9c0: 6c69 5f65 6e61 626c 6564 0a20 2020 2020  li_enabled.     
+0004f9d0: 2020 2073 656c 662e 6c69 6665 6379 636c     self.lifecycl
+0004f9e0: 6520 3d20 6c69 6665 6379 636c 650a 2020  e = lifecycle.  
+0004f9f0: 2020 2020 2020 7365 6c66 2e6c 6f63 616c        self.local
+0004fa00: 6974 795f 6c62 636f 6e66 203d 206c 6f63  ity_lbconf = loc
+0004fa10: 616c 6974 795f 6c62 636f 6e66 0a20 2020  ality_lbconf.   
+0004fa20: 2020 2020 2073 656c 662e 6c6f 6361 6c69       self.locali
+0004fa30: 7479 5f6c 6f61 645f 6261 6c61 6e63 696e  ty_load_balancin
+0004fa40: 6720 3d20 6c6f 6361 6c69 7479 5f6c 6f61  g = locality_loa
+0004fa50: 645f 6261 6c61 6e63 696e 670a 2020 2020  d_balancing.    
+0004fa60: 2020 2020 7365 6c66 2e6d 7365 656e 6162      self.mseenab
+0004fa70: 6c65 6420 3d20 6d73 6565 6e61 626c 6564  led = mseenabled
+0004fa80: 0a20 2020 2020 2020 2073 656c 662e 6d75  .        self.mu
+0004fa90: 6c74 695f 6275 6666 6572 5f65 6e61 626c  lti_buffer_enabl
+0004faa0: 6564 203d 206d 756c 7469 5f62 7566 6665  ed = multi_buffe
+0004fab0: 725f 656e 6162 6c65 640a 2020 2020 2020  r_enabled.      
+0004fac0: 2020 7365 6c66 2e6d 756c 7469 5f62 7566    self.multi_buf
+0004fad0: 6665 725f 706f 6c6c 5f64 656c 6179 203d  fer_poll_delay =
+0004fae0: 206d 756c 7469 5f62 7566 6665 725f 706f   multi_buffer_po
+0004faf0: 6c6c 5f64 656c 6179 0a20 2020 2020 2020  ll_delay.       
+0004fb00: 2073 656c 662e 6d79 7371 6c5f 6669 6c74   self.mysql_filt
+0004fb10: 6572 5f65 6e61 626c 6564 203d 206d 7973  er_enabled = mys
+0004fb20: 716c 5f66 696c 7465 725f 656e 6162 6c65  ql_filter_enable
+0004fb30: 640a 2020 2020 2020 2020 7365 6c66 2e6f  d.        self.o
+0004fb40: 7061 6c69 6d69 745f 6370 7520 3d20 6f70  palimit_cpu = op
+0004fb50: 616c 696d 6974 5f63 7075 0a20 2020 2020  alimit_cpu.     
+0004fb60: 2020 2073 656c 662e 6f70 616c 696d 6974     self.opalimit
+0004fb70: 5f6d 656d 6f72 7920 3d20 6f70 616c 696d  _memory = opalim
+0004fb80: 6974 5f6d 656d 6f72 790a 2020 2020 2020  it_memory.      
+0004fb90: 2020 7365 6c66 2e6f 7061 6c6f 675f 6c65    self.opalog_le
+0004fba0: 7665 6c20 3d20 6f70 616c 6f67 5f6c 6576  vel = opalog_lev
+0004fbb0: 656c 0a20 2020 2020 2020 2073 656c 662e  el.        self.
+0004fbc0: 6f70 6172 6571 7565 7374 5f63 7075 203d  oparequest_cpu =
+0004fbd0: 206f 7061 7265 7175 6573 745f 6370 750a   oparequest_cpu.
+0004fbe0: 2020 2020 2020 2020 7365 6c66 2e6f 7061          self.opa
+0004fbf0: 7265 7175 6573 745f 6d65 6d6f 7279 203d  request_memory =
+0004fc00: 206f 7061 7265 7175 6573 745f 6d65 6d6f   oparequest_memo
+0004fc10: 7279 0a20 2020 2020 2020 2073 656c 662e  ry.        self.
+0004fc20: 6f70 615f 656e 6162 6c65 6420 3d20 6f70  opa_enabled = op
+0004fc30: 615f 656e 6162 6c65 640a 2020 2020 2020  a_enabled.      
+0004fc40: 2020 7365 6c66 2e6f 7065 6e5f 6167 656e    self.open_agen
+0004fc50: 745f 706f 6c69 6379 203d 206f 7065 6e5f  t_policy = open_
+0004fc60: 6167 656e 745f 706f 6c69 6379 0a20 2020  agent_policy.   
+0004fc70: 2020 2020 2073 656c 662e 6f75 7462 6f75       self.outbou
+0004fc80: 6e64 5f74 7261 6666 6963 5f70 6f6c 6963  nd_traffic_polic
+0004fc90: 7920 3d20 6f75 7462 6f75 6e64 5f74 7261  y = outbound_tra
+0004fca0: 6666 6963 5f70 6f6c 6963 790a 2020 2020  ffic_policy.    
+0004fcb0: 2020 2020 7365 6c66 2e70 726f 6d65 7468      self.prometh
+0004fcc0: 6575 735f 7572 6c20 3d20 7072 6f6d 6574  eus_url = promet
+0004fcd0: 6865 7573 5f75 726c 0a20 2020 2020 2020  heus_url.       
+0004fce0: 2073 656c 662e 7072 6f78 795f 696e 6974   self.proxy_init
+0004fcf0: 5f63 7075 7265 736f 7572 6365 5f6c 696d  _cpuresource_lim
+0004fd00: 6974 203d 2070 726f 7879 5f69 6e69 745f  it = proxy_init_
+0004fd10: 6370 7572 6573 6f75 7263 655f 6c69 6d69  cpuresource_limi
+0004fd20: 740a 2020 2020 2020 2020 7365 6c66 2e70  t.        self.p
+0004fd30: 726f 7879 5f69 6e69 745f 6370 7572 6573  roxy_init_cpures
+0004fd40: 6f75 7263 655f 7265 7175 6573 7420 3d20  ource_request = 
+0004fd50: 7072 6f78 795f 696e 6974 5f63 7075 7265  proxy_init_cpure
+0004fd60: 736f 7572 6365 5f72 6571 7565 7374 0a20  source_request. 
+0004fd70: 2020 2020 2020 2073 656c 662e 7072 6f78         self.prox
+0004fd80: 795f 696e 6974 5f6d 656d 6f72 795f 7265  y_init_memory_re
+0004fd90: 736f 7572 6365 5f6c 696d 6974 203d 2070  source_limit = p
+0004fda0: 726f 7879 5f69 6e69 745f 6d65 6d6f 7279  roxy_init_memory
+0004fdb0: 5f72 6573 6f75 7263 655f 6c69 6d69 740a  _resource_limit.
+0004fdc0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+0004fdd0: 7879 5f69 6e69 745f 6d65 6d6f 7279 5f72  xy_init_memory_r
+0004fde0: 6573 6f75 7263 655f 7265 7175 6573 7420  esource_request 
+0004fdf0: 3d20 7072 6f78 795f 696e 6974 5f6d 656d  = proxy_init_mem
+0004fe00: 6f72 795f 7265 736f 7572 6365 5f72 6571  ory_resource_req
+0004fe10: 7565 7374 0a20 2020 2020 2020 2073 656c  uest.        sel
+0004fe20: 662e 7072 6f78 795f 6c69 6d69 745f 6370  f.proxy_limit_cp
+0004fe30: 7520 3d20 7072 6f78 795f 6c69 6d69 745f  u = proxy_limit_
+0004fe40: 6370 750a 2020 2020 2020 2020 7365 6c66  cpu.        self
+0004fe50: 2e70 726f 7879 5f6c 696d 6974 5f6d 656d  .proxy_limit_mem
+0004fe60: 6f72 7920 3d20 7072 6f78 795f 6c69 6d69  ory = proxy_limi
+0004fe70: 745f 6d65 6d6f 7279 0a20 2020 2020 2020  t_memory.       
+0004fe80: 2073 656c 662e 7072 6f78 795f 7265 7175   self.proxy_requ
+0004fe90: 6573 745f 6370 7520 3d20 7072 6f78 795f  est_cpu = proxy_
+0004fea0: 7265 7175 6573 745f 6370 750a 2020 2020  request_cpu.    
+0004feb0: 2020 2020 7365 6c66 2e70 726f 7879 5f72      self.proxy_r
+0004fec0: 6571 7565 7374 5f6d 656d 6f72 7920 3d20  equest_memory = 
+0004fed0: 7072 6f78 795f 7265 7175 6573 745f 6d65  proxy_request_me
+0004fee0: 6d6f 7279 0a20 2020 2020 2020 2073 656c  mory.        sel
+0004fef0: 662e 7265 6469 735f 6669 6c74 6572 5f65  f.redis_filter_e
+0004ff00: 6e61 626c 6564 203d 2072 6564 6973 5f66  nabled = redis_f
+0004ff10: 696c 7465 725f 656e 6162 6c65 640a 2020  ilter_enabled.  
+0004ff20: 2020 2020 2020 7365 6c66 2e73 6572 7669        self.servi
+0004ff30: 6365 5f6d 6573 685f 6964 203d 2073 6572  ce_mesh_id = ser
+0004ff40: 7669 6365 5f6d 6573 685f 6964 0a20 2020  vice_mesh_id.   
+0004ff50: 2020 2020 2073 656c 662e 7369 6465 6361       self.sideca
+0004ff60: 725f 696e 6a65 6374 6f72 5f6c 696d 6974  r_injector_limit
+0004ff70: 5f63 7075 203d 2073 6964 6563 6172 5f69  _cpu = sidecar_i
+0004ff80: 6e6a 6563 746f 725f 6c69 6d69 745f 6370  njector_limit_cp
+0004ff90: 750a 2020 2020 2020 2020 7365 6c66 2e73  u.        self.s
+0004ffa0: 6964 6563 6172 5f69 6e6a 6563 746f 725f  idecar_injector_
+0004ffb0: 6c69 6d69 745f 6d65 6d6f 7279 203d 2073  limit_memory = s
+0004ffc0: 6964 6563 6172 5f69 6e6a 6563 746f 725f  idecar_injector_
+0004ffd0: 6c69 6d69 745f 6d65 6d6f 7279 0a20 2020  limit_memory.   
+0004ffe0: 2020 2020 2073 656c 662e 7369 6465 6361       self.sideca
+0004fff0: 725f 696e 6a65 6374 6f72 5f72 6571 7565  r_injector_reque
+00050000: 7374 5f63 7075 203d 2073 6964 6563 6172  st_cpu = sidecar
+00050010: 5f69 6e6a 6563 746f 725f 7265 7175 6573  _injector_reques
+00050020: 745f 6370 750a 2020 2020 2020 2020 7365  t_cpu.        se
+00050030: 6c66 2e73 6964 6563 6172 5f69 6e6a 6563  lf.sidecar_injec
+00050040: 746f 725f 7265 7175 6573 745f 6d65 6d6f  tor_request_memo
+00050050: 7279 203d 2073 6964 6563 6172 5f69 6e6a  ry = sidecar_inj
+00050060: 6563 746f 725f 7265 7175 6573 745f 6d65  ector_request_me
+00050070: 6d6f 7279 0a20 2020 2020 2020 2073 656c  mory.        sel
+00050080: 662e 7369 6465 6361 725f 696e 6a65 6374  f.sidecar_inject
+00050090: 6f72 5f77 6562 686f 6f6b 5f61 735f 7961  or_webhook_as_ya
+000500a0: 6d6c 203d 2073 6964 6563 6172 5f69 6e6a  ml = sidecar_inj
+000500b0: 6563 746f 725f 7765 6268 6f6f 6b5f 6173  ector_webhook_as
+000500c0: 5f79 616d 6c0a 2020 2020 2020 2020 7365  _yaml.        se
+000500d0: 6c66 2e74 656c 656d 6574 7279 203d 2074  lf.telemetry = t
+000500e0: 656c 656d 6574 7279 0a20 2020 2020 2020  elemetry.       
+000500f0: 2073 656c 662e 7465 726d 696e 6174 696f   self.terminatio
+00050100: 6e5f 6472 6169 6e5f 6475 7261 7469 6f6e  n_drain_duration
+00050110: 203d 2074 6572 6d69 6e61 7469 6f6e 5f64   = termination_d
+00050120: 7261 696e 5f64 7572 6174 696f 6e0a 2020  rain_duration.  
+00050130: 2020 2020 2020 7365 6c66 2e74 6872 6966        self.thrif
+00050140: 745f 6669 6c74 6572 5f65 6e61 626c 6564  t_filter_enabled
+00050150: 203d 2074 6872 6966 745f 6669 6c74 6572   = thrift_filter
+00050160: 5f65 6e61 626c 6564 0a20 2020 2020 2020  _enabled.       
+00050170: 2073 656c 662e 7472 6163 655f 7361 6d70   self.trace_samp
+00050180: 6c69 6e67 203d 2074 7261 6365 5f73 616d  ling = trace_sam
+00050190: 706c 696e 670a 2020 2020 2020 2020 7365  pling.        se
+000501a0: 6c66 2e74 7261 6369 6e67 203d 2074 7261  lf.tracing = tra
+000501b0: 6369 6e67 0a20 2020 2020 2020 2073 656c  cing.        sel
+000501c0: 662e 7765 625f 6173 7365 6d62 6c79 5f66  f.web_assembly_f
+000501d0: 696c 7465 725f 656e 6162 6c65 6420 3d20  ilter_enabled = 
+000501e0: 7765 625f 6173 7365 6d62 6c79 5f66 696c  web_assembly_fil
+000501f0: 7465 725f 656e 6162 6c65 640a 0a20 2020  ter_enabled..   
+00050200: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+00050210: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+00050220: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
+00050230: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+00050240: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+00050250: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00050260: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+00050270: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00050280: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+00050290: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+000502a0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+000502b0: 6620 7365 6c66 2e61 6363 6573 735f 6c6f  f self.access_lo
+000502c0: 675f 656e 6162 6c65 6420 6973 206e 6f74  g_enabled is not
+000502d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000502e0: 2020 2072 6573 756c 745b 2741 6363 6573     result['Acces
+000502f0: 734c 6f67 456e 6162 6c65 6427 5d20 3d20  sLogEnabled'] = 
+00050300: 7365 6c66 2e61 6363 6573 735f 6c6f 675f  self.access_log_
+00050310: 656e 6162 6c65 640a 2020 2020 2020 2020  enabled.        
+00050320: 6966 2073 656c 662e 6163 6365 7373 5f6c  if self.access_l
+00050330: 6f67 5f66 696c 6520 6973 206e 6f74 204e  og_file is not N
+00050340: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00050350: 2072 6573 756c 745b 2741 6363 6573 734c   result['AccessL
+00050360: 6f67 4669 6c65 275d 203d 2073 656c 662e  ogFile'] = self.
+00050370: 6163 6365 7373 5f6c 6f67 5f66 696c 650a  access_log_file.
+00050380: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00050390: 6163 6365 7373 5f6c 6f67 5f66 6f72 6d61  access_log_forma
+000503a0: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
+000503b0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000503c0: 745b 2741 6363 6573 734c 6f67 466f 726d  t['AccessLogForm
+000503d0: 6174 275d 203d 2073 656c 662e 6163 6365  at'] = self.acce
+000503e0: 7373 5f6c 6f67 5f66 6f72 6d61 740a 2020  ss_log_format.  
+000503f0: 2020 2020 2020 6966 2073 656c 662e 6163        if self.ac
+00050400: 6365 7373 5f6c 6f67 5f70 726f 6a65 6374  cess_log_project
+00050410: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00050420: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00050430: 5b27 4163 6365 7373 4c6f 6750 726f 6a65  ['AccessLogProje
+00050440: 6374 275d 203d 2073 656c 662e 6163 6365  ct'] = self.acce
+00050450: 7373 5f6c 6f67 5f70 726f 6a65 6374 0a20  ss_log_project. 
+00050460: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
+00050470: 6363 6573 735f 6c6f 675f 7365 7276 6963  ccess_log_servic
+00050480: 655f 656e 6162 6c65 6420 6973 206e 6f74  e_enabled is not
+00050490: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000504a0: 2020 2072 6573 756c 745b 2741 6363 6573     result['Acces
+000504b0: 734c 6f67 5365 7276 6963 6545 6e61 626c  sLogServiceEnabl
+000504c0: 6564 275d 203d 2073 656c 662e 6163 6365  ed'] = self.acce
+000504d0: 7373 5f6c 6f67 5f73 6572 7669 6365 5f65  ss_log_service_e
+000504e0: 6e61 626c 6564 0a20 2020 2020 2020 2069  nabled.        i
+000504f0: 6620 7365 6c66 2e61 6363 6573 735f 6c6f  f self.access_lo
+00050500: 675f 7365 7276 6963 655f 686f 7374 2069  g_service_host i
+00050510: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00050520: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00050530: 4163 6365 7373 4c6f 6753 6572 7669 6365  AccessLogService
+00050540: 486f 7374 275d 203d 2073 656c 662e 6163  Host'] = self.ac
+00050550: 6365 7373 5f6c 6f67 5f73 6572 7669 6365  cess_log_service
+00050560: 5f68 6f73 740a 2020 2020 2020 2020 6966  _host.        if
+00050570: 2073 656c 662e 6163 6365 7373 5f6c 6f67   self.access_log
+00050580: 5f73 6572 7669 6365 5f70 6f72 7420 6973  _service_port is
+00050590: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000505a0: 2020 2020 2020 2072 6573 756c 745b 2741         result['A
+000505b0: 6363 6573 734c 6f67 5365 7276 6963 6550  ccessLogServiceP
+000505c0: 6f72 7427 5d20 3d20 7365 6c66 2e61 6363  ort'] = self.acc
+000505d0: 6573 735f 6c6f 675f 7365 7276 6963 655f  ess_log_service_
+000505e0: 706f 7274 0a20 2020 2020 2020 2069 6620  port.        if 
+000505f0: 7365 6c66 2e61 7564 6974 5f70 726f 6a65  self.audit_proje
+00050600: 6374 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ct is not None:.
+00050610: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00050620: 6c74 5b27 4175 6469 7450 726f 6a65 6374  lt['AuditProject
+00050630: 275d 203d 2073 656c 662e 6175 6469 745f  '] = self.audit_
+00050640: 7072 6f6a 6563 740a 2020 2020 2020 2020  project.        
+00050650: 6966 2073 656c 662e 6175 746f 5f69 6e6a  if self.auto_inj
+00050660: 6563 7469 6f6e 5f70 6f6c 6963 795f 656e  ection_policy_en
+00050670: 6162 6c65 6420 6973 206e 6f74 204e 6f6e  abled is not Non
+00050680: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00050690: 6573 756c 745b 2741 7574 6f49 6e6a 6563  esult['AutoInjec
+000506a0: 7469 6f6e 506f 6c69 6379 456e 6162 6c65  tionPolicyEnable
+000506b0: 6427 5d20 3d20 7365 6c66 2e61 7574 6f5f  d'] = self.auto_
+000506c0: 696e 6a65 6374 696f 6e5f 706f 6c69 6379  injection_policy
+000506d0: 5f65 6e61 626c 6564 0a20 2020 2020 2020  _enabled.       
+000506e0: 2069 6620 7365 6c66 2e63 7261 6767 7265   if self.craggre
+000506f0: 6761 7469 6f6e 5f65 6e61 626c 6564 2069  gation_enabled i
+00050700: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00050710: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00050720: 4352 4167 6772 6567 6174 696f 6e45 6e61  CRAggregationEna
+00050730: 626c 6564 275d 203d 2073 656c 662e 6372  bled'] = self.cr
+00050740: 6167 6772 6567 6174 696f 6e5f 656e 6162  aggregation_enab
+00050750: 6c65 640a 2020 2020 2020 2020 6966 2073  led.        if s
+00050760: 656c 662e 636c 7573 7465 725f 7370 6563  elf.cluster_spec
+00050770: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00050780: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00050790: 5b27 436c 7573 7465 7253 7065 6327 5d20  ['ClusterSpec'] 
+000507a0: 3d20 7365 6c66 2e63 6c75 7374 6572 5f73  = self.cluster_s
+000507b0: 7065 630a 2020 2020 2020 2020 6966 2073  pec.        if s
+000507c0: 656c 662e 636e 695f 656e 6162 6c65 6420  elf.cni_enabled 
+000507d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000507e0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000507f0: 2743 6e69 456e 6162 6c65 6427 5d20 3d20  'CniEnabled'] = 
+00050800: 7365 6c66 2e63 6e69 5f65 6e61 626c 6564  self.cni_enabled
+00050810: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00050820: 2e63 6e69 5f65 7863 6c75 6465 5f6e 616d  .cni_exclude_nam
+00050830: 6573 7061 6365 7320 6973 206e 6f74 204e  espaces is not N
+00050840: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00050850: 2072 6573 756c 745b 2743 6e69 4578 636c   result['CniExcl
+00050860: 7564 654e 616d 6573 7061 6365 7327 5d20  udeNamespaces'] 
+00050870: 3d20 7365 6c66 2e63 6e69 5f65 7863 6c75  = self.cni_exclu
+00050880: 6465 5f6e 616d 6573 7061 6365 730a 2020  de_namespaces.  
+00050890: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+000508a0: 6e66 6967 5f73 6f75 7263 655f 656e 6162  nfig_source_enab
+000508b0: 6c65 6420 6973 206e 6f74 204e 6f6e 653a  led is not None:
+000508c0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000508d0: 756c 745b 2743 6f6e 6669 6753 6f75 7263  ult['ConfigSourc
+000508e0: 6545 6e61 626c 6564 275d 203d 2073 656c  eEnabled'] = sel
+000508f0: 662e 636f 6e66 6967 5f73 6f75 7263 655f  f.config_source_
+00050900: 656e 6162 6c65 640a 2020 2020 2020 2020  enabled.        
+00050910: 6966 2073 656c 662e 636f 6e66 6967 5f73  if self.config_s
+00050920: 6f75 7263 655f 6e61 636f 735f 6964 2069  ource_nacos_id i
+00050930: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00050940: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00050950: 436f 6e66 6967 536f 7572 6365 4e61 636f  ConfigSourceNaco
+00050960: 7349 4427 5d20 3d20 7365 6c66 2e63 6f6e  sID'] = self.con
+00050970: 6669 675f 736f 7572 6365 5f6e 6163 6f73  fig_source_nacos
+00050980: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
+00050990: 656c 662e 6375 7374 6f6d 697a 6564 5f70  elf.customized_p
+000509a0: 726f 6d65 7468 6575 7320 6973 206e 6f74  rometheus is not
+000509b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000509c0: 2020 2072 6573 756c 745b 2743 7573 746f     result['Custo
+000509d0: 6d69 7a65 6450 726f 6d65 7468 6575 7327  mizedPrometheus'
+000509e0: 5d20 3d20 7365 6c66 2e63 7573 746f 6d69  ] = self.customi
+000509f0: 7a65 645f 7072 6f6d 6574 6865 7573 0a20  zed_prometheus. 
+00050a00: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+00050a10: 7573 746f 6d69 7a65 645f 7a69 706b 696e  ustomized_zipkin
+00050a20: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00050a30: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00050a40: 5b27 4375 7374 6f6d 697a 6564 5a69 706b  ['CustomizedZipk
+00050a50: 696e 275d 203d 2073 656c 662e 6375 7374  in'] = self.cust
+00050a60: 6f6d 697a 6564 5f7a 6970 6b69 6e0a 2020  omized_zipkin.  
+00050a70: 2020 2020 2020 6966 2073 656c 662e 646e        if self.dn
+00050a80: 7370 726f 7879 696e 675f 656e 6162 6c65  sproxying_enable
+00050a90: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+00050aa0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00050ab0: 745b 2744 4e53 5072 6f78 7969 6e67 456e  t['DNSProxyingEn
+00050ac0: 6162 6c65 6427 5d20 3d20 7365 6c66 2e64  abled'] = self.d
+00050ad0: 6e73 7072 6f78 7969 6e67 5f65 6e61 626c  nsproxying_enabl
+00050ae0: 6564 0a20 2020 2020 2020 2069 6620 7365  ed.        if se
+00050af0: 6c66 2e64 6973 636f 7665 7279 5f73 656c  lf.discovery_sel
+00050b00: 6563 746f 7273 2069 7320 6e6f 7420 4e6f  ectors is not No
+00050b10: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00050b20: 7265 7375 6c74 5b27 4469 7363 6f76 6572  result['Discover
+00050b30: 7953 656c 6563 746f 7273 275d 203d 2073  ySelectors'] = s
+00050b40: 656c 662e 6469 7363 6f76 6572 795f 7365  elf.discovery_se
+00050b50: 6c65 6374 6f72 730a 2020 2020 2020 2020  lectors.        
+00050b60: 6966 2073 656c 662e 6475 6262 6f5f 6669  if self.dubbo_fi
+00050b70: 6c74 6572 5f65 6e61 626c 6564 2069 7320  lter_enabled is 
+00050b80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00050b90: 2020 2020 2020 7265 7375 6c74 5b27 4475        result['Du
+00050ba0: 6262 6f46 696c 7465 7245 6e61 626c 6564  bboFilterEnabled
+00050bb0: 275d 203d 2073 656c 662e 6475 6262 6f5f  '] = self.dubbo_
+00050bc0: 6669 6c74 6572 5f65 6e61 626c 6564 0a20  filter_enabled. 
+00050bd0: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
+00050be0: 6e61 626c 655f 6175 6469 7420 6973 206e  nable_audit is n
+00050bf0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00050c00: 2020 2020 2072 6573 756c 745b 2745 6e61       result['Ena
+00050c10: 626c 6541 7564 6974 275d 203d 2073 656c  bleAudit'] = sel
+00050c20: 662e 656e 6162 6c65 5f61 7564 6974 0a20  f.enable_audit. 
+00050c30: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
+00050c40: 6e61 626c 655f 6372 6869 7374 6f72 7920  nable_crhistory 
+00050c50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00050c60: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00050c70: 2745 6e61 626c 6543 5248 6973 746f 7279  'EnableCRHistory
+00050c80: 275d 203d 2073 656c 662e 656e 6162 6c65  '] = self.enable
+00050c90: 5f63 7268 6973 746f 7279 0a20 2020 2020  _crhistory.     
+00050ca0: 2020 2069 6620 7365 6c66 2e65 6e61 626c     if self.enabl
+00050cb0: 655f 6e61 6d65 7370 6163 6573 5f62 795f  e_namespaces_by_
+00050cc0: 6465 6661 756c 7420 6973 206e 6f74 204e  default is not N
+00050cd0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00050ce0: 2072 6573 756c 745b 2745 6e61 626c 654e   result['EnableN
+00050cf0: 616d 6573 7061 6365 7342 7944 6566 6175  amespacesByDefau
+00050d00: 6c74 275d 203d 2073 656c 662e 656e 6162  lt'] = self.enab
+00050d10: 6c65 5f6e 616d 6573 7061 6365 735f 6279  le_namespaces_by
+00050d20: 5f64 6566 6175 6c74 0a20 2020 2020 2020  _default.       
+00050d30: 2069 6620 7365 6c66 2e65 6e61 626c 655f   if self.enable_
+00050d40: 7364 7373 6572 7665 7220 6973 206e 6f74  sdsserver is not
+00050d50: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00050d60: 2020 2072 6573 756c 745b 2745 6e61 626c     result['Enabl
+00050d70: 6553 4453 5365 7276 6572 275d 203d 2073  eSDSServer'] = s
+00050d80: 656c 662e 656e 6162 6c65 5f73 6473 7365  elf.enable_sdsse
+00050d90: 7276 6572 0a20 2020 2020 2020 2069 6620  rver.        if 
+00050da0: 7365 6c66 2e65 7863 6c75 6465 5f69 7072  self.exclude_ipr
+00050db0: 616e 6765 7320 6973 206e 6f74 204e 6f6e  anges is not Non
+00050dc0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00050dd0: 6573 756c 745b 2745 7863 6c75 6465 4950  esult['ExcludeIP
+00050de0: 5261 6e67 6573 275d 203d 2073 656c 662e  Ranges'] = self.
+00050df0: 6578 636c 7564 655f 6970 7261 6e67 6573  exclude_ipranges
+00050e00: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00050e10: 2e65 7863 6c75 6465 5f69 6e62 6f75 6e64  .exclude_inbound
+00050e20: 5f70 6f72 7473 2069 7320 6e6f 7420 4e6f  _ports is not No
+00050e30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00050e40: 7265 7375 6c74 5b27 4578 636c 7564 6549  result['ExcludeI
+00050e50: 6e62 6f75 6e64 506f 7274 7327 5d20 3d20  nboundPorts'] = 
+00050e60: 7365 6c66 2e65 7863 6c75 6465 5f69 6e62  self.exclude_inb
+00050e70: 6f75 6e64 5f70 6f72 7473 0a20 2020 2020  ound_ports.     
+00050e80: 2020 2069 6620 7365 6c66 2e65 7863 6c75     if self.exclu
+00050e90: 6465 5f6f 7574 626f 756e 645f 706f 7274  de_outbound_port
+00050ea0: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+00050eb0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00050ec0: 745b 2745 7863 6c75 6465 4f75 7462 6f75  t['ExcludeOutbou
+00050ed0: 6e64 506f 7274 7327 5d20 3d20 7365 6c66  ndPorts'] = self
+00050ee0: 2e65 7863 6c75 6465 5f6f 7574 626f 756e  .exclude_outboun
+00050ef0: 645f 706f 7274 730a 2020 2020 2020 2020  d_ports.        
+00050f00: 6966 2073 656c 662e 6669 6c74 6572 5f67  if self.filter_g
+00050f10: 6174 6577 6179 5f63 6c75 7374 6572 5f63  ateway_cluster_c
+00050f20: 6f6e 6669 6720 6973 206e 6f74 204e 6f6e  onfig is not Non
+00050f30: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00050f40: 6573 756c 745b 2746 696c 7465 7247 6174  esult['FilterGat
+00050f50: 6577 6179 436c 7573 7465 7243 6f6e 6669  ewayClusterConfi
+00050f60: 6727 5d20 3d20 7365 6c66 2e66 696c 7465  g'] = self.filte
+00050f70: 725f 6761 7465 7761 795f 636c 7573 7465  r_gateway_cluste
+00050f80: 725f 636f 6e66 6967 0a20 2020 2020 2020  r_config.       
+00050f90: 2069 6620 7365 6c66 2e67 6174 6577 6179   if self.gateway
+00050fa0: 5f61 7069 656e 6162 6c65 6420 6973 206e  _apienabled is n
+00050fb0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00050fc0: 2020 2020 2072 6573 756c 745b 2747 6174       result['Gat
+00050fd0: 6577 6179 4150 4945 6e61 626c 6564 275d  ewayAPIEnabled']
+00050fe0: 203d 2073 656c 662e 6761 7465 7761 795f   = self.gateway_
+00050ff0: 6170 6965 6e61 626c 6564 0a20 2020 2020  apienabled.     
+00051000: 2020 2069 6620 7365 6c66 2e67 6c6f 6261     if self.globa
+00051010: 6c5f 7261 7465 5f6c 696d 6974 5f65 6e61  l_rate_limit_ena
+00051020: 626c 6564 2069 7320 6e6f 7420 4e6f 6e65  bled is not None
+00051030: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00051040: 7375 6c74 5b27 476c 6f62 616c 5261 7465  sult['GlobalRate
+00051050: 4c69 6d69 7445 6e61 626c 6564 275d 203d  LimitEnabled'] =
+00051060: 2073 656c 662e 676c 6f62 616c 5f72 6174   self.global_rat
+00051070: 655f 6c69 6d69 745f 656e 6162 6c65 640a  e_limit_enabled.
+00051080: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00051090: 6874 7470 5f31 3065 6e61 626c 6564 2069  http_10enabled i
+000510a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000510b0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000510c0: 4874 7470 3130 456e 6162 6c65 6427 5d20  Http10Enabled'] 
+000510d0: 3d20 7365 6c66 2e68 7474 705f 3130 656e  = self.http_10en
+000510e0: 6162 6c65 640a 2020 2020 2020 2020 6966  abled.        if
+000510f0: 2073 656c 662e 696e 636c 7564 655f 6970   self.include_ip
+00051100: 7261 6e67 6573 2069 7320 6e6f 7420 4e6f  ranges is not No
+00051110: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00051120: 7265 7375 6c74 5b27 496e 636c 7564 6549  result['IncludeI
+00051130: 5052 616e 6765 7327 5d20 3d20 7365 6c66  PRanges'] = self
+00051140: 2e69 6e63 6c75 6465 5f69 7072 616e 6765  .include_iprange
+00051150: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
+00051160: 662e 696e 636c 7564 655f 696e 626f 756e  f.include_inboun
+00051170: 645f 706f 7274 7320 6973 206e 6f74 204e  d_ports is not N
+00051180: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00051190: 2072 6573 756c 745b 2749 6e63 6c75 6465   result['Include
+000511a0: 496e 626f 756e 6450 6f72 7473 275d 203d  InboundPorts'] =
+000511b0: 2073 656c 662e 696e 636c 7564 655f 696e   self.include_in
+000511c0: 626f 756e 645f 706f 7274 730a 2020 2020  bound_ports.    
+000511d0: 2020 2020 6966 2073 656c 662e 6b69 616c      if self.kial
+000511e0: 695f 656e 6162 6c65 6420 6973 206e 6f74  i_enabled is not
+000511f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00051200: 2020 2072 6573 756c 745b 274b 6961 6c69     result['Kiali
+00051210: 456e 6162 6c65 6427 5d20 3d20 7365 6c66  Enabled'] = self
+00051220: 2e6b 6961 6c69 5f65 6e61 626c 6564 0a20  .kiali_enabled. 
+00051230: 2020 2020 2020 2069 6620 7365 6c66 2e6c         if self.l
+00051240: 6966 6563 7963 6c65 2069 7320 6e6f 7420  ifecycle is not 
+00051250: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00051260: 2020 7265 7375 6c74 5b27 4c69 6665 6379    result['Lifecy
+00051270: 636c 6527 5d20 3d20 7365 6c66 2e6c 6966  cle'] = self.lif
+00051280: 6563 7963 6c65 0a20 2020 2020 2020 2069  ecycle.        i
+00051290: 6620 7365 6c66 2e6c 6f63 616c 6974 795f  f self.locality_
+000512a0: 6c62 636f 6e66 2069 7320 6e6f 7420 4e6f  lbconf is not No
+000512b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000512c0: 7265 7375 6c74 5b27 4c6f 6361 6c69 7479  result['Locality
+000512d0: 4c42 436f 6e66 275d 203d 2073 656c 662e  LBConf'] = self.
+000512e0: 6c6f 6361 6c69 7479 5f6c 6263 6f6e 660a  locality_lbconf.
+000512f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00051300: 6c6f 6361 6c69 7479 5f6c 6f61 645f 6261  locality_load_ba
+00051310: 6c61 6e63 696e 6720 6973 206e 6f74 204e  lancing is not N
+00051320: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00051330: 2072 6573 756c 745b 274c 6f63 616c 6974   result['Localit
+00051340: 794c 6f61 6442 616c 616e 6369 6e67 275d  yLoadBalancing']
+00051350: 203d 2073 656c 662e 6c6f 6361 6c69 7479   = self.locality
+00051360: 5f6c 6f61 645f 6261 6c61 6e63 696e 670a  _load_balancing.
+00051370: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00051380: 6d73 6565 6e61 626c 6564 2069 7320 6e6f  mseenabled is no
+00051390: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000513a0: 2020 2020 7265 7375 6c74 5b27 4d53 4545      result['MSEE
+000513b0: 6e61 626c 6564 275d 203d 2073 656c 662e  nabled'] = self.
+000513c0: 6d73 6565 6e61 626c 6564 0a20 2020 2020  mseenabled.     
+000513d0: 2020 2069 6620 7365 6c66 2e6d 756c 7469     if self.multi
+000513e0: 5f62 7566 6665 725f 656e 6162 6c65 6420  _buffer_enabled 
+000513f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00051400: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00051410: 274d 756c 7469 4275 6666 6572 456e 6162  'MultiBufferEnab
+00051420: 6c65 6427 5d20 3d20 7365 6c66 2e6d 756c  led'] = self.mul
+00051430: 7469 5f62 7566 6665 725f 656e 6162 6c65  ti_buffer_enable
+00051440: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
+00051450: 662e 6d75 6c74 695f 6275 6666 6572 5f70  f.multi_buffer_p
+00051460: 6f6c 6c5f 6465 6c61 7920 6973 206e 6f74  oll_delay is not
+00051470: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00051480: 2020 2072 6573 756c 745b 274d 756c 7469     result['Multi
+00051490: 4275 6666 6572 506f 6c6c 4465 6c61 7927  BufferPollDelay'
+000514a0: 5d20 3d20 7365 6c66 2e6d 756c 7469 5f62  ] = self.multi_b
+000514b0: 7566 6665 725f 706f 6c6c 5f64 656c 6179  uffer_poll_delay
+000514c0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000514d0: 2e6d 7973 716c 5f66 696c 7465 725f 656e  .mysql_filter_en
+000514e0: 6162 6c65 6420 6973 206e 6f74 204e 6f6e  abled is not Non
+000514f0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00051500: 6573 756c 745b 274d 7973 716c 4669 6c74  esult['MysqlFilt
+00051510: 6572 456e 6162 6c65 6427 5d20 3d20 7365  erEnabled'] = se
+00051520: 6c66 2e6d 7973 716c 5f66 696c 7465 725f  lf.mysql_filter_
+00051530: 656e 6162 6c65 640a 2020 2020 2020 2020  enabled.        
+00051540: 6966 2073 656c 662e 6f70 616c 696d 6974  if self.opalimit
+00051550: 5f63 7075 2069 7320 6e6f 7420 4e6f 6e65  _cpu is not None
+00051560: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00051570: 7375 6c74 5b27 4f50 414c 696d 6974 4350  sult['OPALimitCP
+00051580: 5527 5d20 3d20 7365 6c66 2e6f 7061 6c69  U'] = self.opali
+00051590: 6d69 745f 6370 750a 2020 2020 2020 2020  mit_cpu.        
+000515a0: 6966 2073 656c 662e 6f70 616c 696d 6974  if self.opalimit
+000515b0: 5f6d 656d 6f72 7920 6973 206e 6f74 204e  _memory is not N
+000515c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000515d0: 2072 6573 756c 745b 274f 5041 4c69 6d69   result['OPALimi
+000515e0: 744d 656d 6f72 7927 5d20 3d20 7365 6c66  tMemory'] = self
+000515f0: 2e6f 7061 6c69 6d69 745f 6d65 6d6f 7279  .opalimit_memory
+00051600: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00051610: 2e6f 7061 6c6f 675f 6c65 7665 6c20 6973  .opalog_level is
+00051620: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00051630: 2020 2020 2020 2072 6573 756c 745b 274f         result['O
+00051640: 5041 4c6f 674c 6576 656c 275d 203d 2073  PALogLevel'] = s
+00051650: 656c 662e 6f70 616c 6f67 5f6c 6576 656c  elf.opalog_level
+00051660: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00051670: 2e6f 7061 7265 7175 6573 745f 6370 7520  .oparequest_cpu 
+00051680: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00051690: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000516a0: 274f 5041 5265 7175 6573 7443 5055 275d  'OPARequestCPU']
+000516b0: 203d 2073 656c 662e 6f70 6172 6571 7565   = self.opareque
+000516c0: 7374 5f63 7075 0a20 2020 2020 2020 2069  st_cpu.        i
+000516d0: 6620 7365 6c66 2e6f 7061 7265 7175 6573  f self.opareques
+000516e0: 745f 6d65 6d6f 7279 2069 7320 6e6f 7420  t_memory is not 
+000516f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00051700: 2020 7265 7375 6c74 5b27 4f50 4152 6571    result['OPAReq
+00051710: 7565 7374 4d65 6d6f 7279 275d 203d 2073  uestMemory'] = s
+00051720: 656c 662e 6f70 6172 6571 7565 7374 5f6d  elf.oparequest_m
+00051730: 656d 6f72 790a 2020 2020 2020 2020 6966  emory.        if
+00051740: 2073 656c 662e 6f70 615f 656e 6162 6c65   self.opa_enable
+00051750: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+00051760: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00051770: 745b 274f 7061 456e 6162 6c65 6427 5d20  t['OpaEnabled'] 
+00051780: 3d20 7365 6c66 2e6f 7061 5f65 6e61 626c  = self.opa_enabl
+00051790: 6564 0a20 2020 2020 2020 2069 6620 7365  ed.        if se
+000517a0: 6c66 2e6f 7065 6e5f 6167 656e 745f 706f  lf.open_agent_po
+000517b0: 6c69 6379 2069 7320 6e6f 7420 4e6f 6e65  licy is not None
+000517c0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000517d0: 7375 6c74 5b27 4f70 656e 4167 656e 7450  sult['OpenAgentP
+000517e0: 6f6c 6963 7927 5d20 3d20 7365 6c66 2e6f  olicy'] = self.o
+000517f0: 7065 6e5f 6167 656e 745f 706f 6c69 6379  pen_agent_policy
+00051800: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00051810: 2e6f 7574 626f 756e 645f 7472 6166 6669  .outbound_traffi
+00051820: 635f 706f 6c69 6379 2069 7320 6e6f 7420  c_policy is not 
+00051830: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00051840: 2020 7265 7375 6c74 5b27 4f75 7462 6f75    result['Outbou
+00051850: 6e64 5472 6166 6669 6350 6f6c 6963 7927  ndTrafficPolicy'
+00051860: 5d20 3d20 7365 6c66 2e6f 7574 626f 756e  ] = self.outboun
+00051870: 645f 7472 6166 6669 635f 706f 6c69 6379  d_traffic_policy
+00051880: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00051890: 2e70 726f 6d65 7468 6575 735f 7572 6c20  .prometheus_url 
+000518a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000518b0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000518c0: 2750 726f 6d65 7468 6575 7355 726c 275d  'PrometheusUrl']
+000518d0: 203d 2073 656c 662e 7072 6f6d 6574 6865   = self.promethe
+000518e0: 7573 5f75 726c 0a20 2020 2020 2020 2069  us_url.        i
+000518f0: 6620 7365 6c66 2e70 726f 7879 5f69 6e69  f self.proxy_ini
+00051900: 745f 6370 7572 6573 6f75 7263 655f 6c69  t_cpuresource_li
+00051910: 6d69 7420 6973 206e 6f74 204e 6f6e 653a  mit is not None:
+00051920: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00051930: 756c 745b 2750 726f 7879 496e 6974 4350  ult['ProxyInitCP
+00051940: 5552 6573 6f75 7263 654c 696d 6974 275d  UResourceLimit']
+00051950: 203d 2073 656c 662e 7072 6f78 795f 696e   = self.proxy_in
+00051960: 6974 5f63 7075 7265 736f 7572 6365 5f6c  it_cpuresource_l
+00051970: 696d 6974 0a20 2020 2020 2020 2069 6620  imit.        if 
+00051980: 7365 6c66 2e70 726f 7879 5f69 6e69 745f  self.proxy_init_
+00051990: 6370 7572 6573 6f75 7263 655f 7265 7175  cpuresource_requ
+000519a0: 6573 7420 6973 206e 6f74 204e 6f6e 653a  est is not None:
+000519b0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000519c0: 756c 745b 2750 726f 7879 496e 6974 4350  ult['ProxyInitCP
+000519d0: 5552 6573 6f75 7263 6552 6571 7565 7374  UResourceRequest
+000519e0: 275d 203d 2073 656c 662e 7072 6f78 795f  '] = self.proxy_
+000519f0: 696e 6974 5f63 7075 7265 736f 7572 6365  init_cpuresource
+00051a00: 5f72 6571 7565 7374 0a20 2020 2020 2020  _request.       
+00051a10: 2069 6620 7365 6c66 2e70 726f 7879 5f69   if self.proxy_i
+00051a20: 6e69 745f 6d65 6d6f 7279 5f72 6573 6f75  nit_memory_resou
+00051a30: 7263 655f 6c69 6d69 7420 6973 206e 6f74  rce_limit is not
+00051a40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00051a50: 2020 2072 6573 756c 745b 2750 726f 7879     result['Proxy
+00051a60: 496e 6974 4d65 6d6f 7279 5265 736f 7572  InitMemoryResour
+00051a70: 6365 4c69 6d69 7427 5d20 3d20 7365 6c66  ceLimit'] = self
+00051a80: 2e70 726f 7879 5f69 6e69 745f 6d65 6d6f  .proxy_init_memo
+00051a90: 7279 5f72 6573 6f75 7263 655f 6c69 6d69  ry_resource_limi
+00051aa0: 740a 2020 2020 2020 2020 6966 2073 656c  t.        if sel
+00051ab0: 662e 7072 6f78 795f 696e 6974 5f6d 656d  f.proxy_init_mem
+00051ac0: 6f72 795f 7265 736f 7572 6365 5f72 6571  ory_resource_req
+00051ad0: 7565 7374 2069 7320 6e6f 7420 4e6f 6e65  uest is not None
+00051ae0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00051af0: 7375 6c74 5b27 5072 6f78 7949 6e69 744d  sult['ProxyInitM
+00051b00: 656d 6f72 7952 6573 6f75 7263 6552 6571  emoryResourceReq
+00051b10: 7565 7374 275d 203d 2073 656c 662e 7072  uest'] = self.pr
+00051b20: 6f78 795f 696e 6974 5f6d 656d 6f72 795f  oxy_init_memory_
+00051b30: 7265 736f 7572 6365 5f72 6571 7565 7374  resource_request
+00051b40: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00051b50: 2e70 726f 7879 5f6c 696d 6974 5f63 7075  .proxy_limit_cpu
+00051b60: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00051b70: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00051b80: 5b27 5072 6f78 794c 696d 6974 4350 5527  ['ProxyLimitCPU'
+00051b90: 5d20 3d20 7365 6c66 2e70 726f 7879 5f6c  ] = self.proxy_l
+00051ba0: 696d 6974 5f63 7075 0a20 2020 2020 2020  imit_cpu.       
+00051bb0: 2069 6620 7365 6c66 2e70 726f 7879 5f6c   if self.proxy_l
+00051bc0: 696d 6974 5f6d 656d 6f72 7920 6973 206e  imit_memory is n
+00051bd0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00051be0: 2020 2020 2072 6573 756c 745b 2750 726f       result['Pro
+00051bf0: 7879 4c69 6d69 744d 656d 6f72 7927 5d20  xyLimitMemory'] 
+00051c00: 3d20 7365 6c66 2e70 726f 7879 5f6c 696d  = self.proxy_lim
+00051c10: 6974 5f6d 656d 6f72 790a 2020 2020 2020  it_memory.      
+00051c20: 2020 6966 2073 656c 662e 7072 6f78 795f    if self.proxy_
+00051c30: 7265 7175 6573 745f 6370 7520 6973 206e  request_cpu is n
+00051c40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00051c50: 2020 2020 2072 6573 756c 745b 2750 726f       result['Pro
+00051c60: 7879 5265 7175 6573 7443 5055 275d 203d  xyRequestCPU'] =
+00051c70: 2073 656c 662e 7072 6f78 795f 7265 7175   self.proxy_requ
+00051c80: 6573 745f 6370 750a 2020 2020 2020 2020  est_cpu.        
+00051c90: 6966 2073 656c 662e 7072 6f78 795f 7265  if self.proxy_re
+00051ca0: 7175 6573 745f 6d65 6d6f 7279 2069 7320  quest_memory is 
+00051cb0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00051cc0: 2020 2020 2020 7265 7375 6c74 5b27 5072        result['Pr
+00051cd0: 6f78 7952 6571 7565 7374 4d65 6d6f 7279  oxyRequestMemory
+00051ce0: 275d 203d 2073 656c 662e 7072 6f78 795f  '] = self.proxy_
+00051cf0: 7265 7175 6573 745f 6d65 6d6f 7279 0a20  request_memory. 
+00051d00: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+00051d10: 6564 6973 5f66 696c 7465 725f 656e 6162  edis_filter_enab
+00051d20: 6c65 6420 6973 206e 6f74 204e 6f6e 653a  led is not None:
+00051d30: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00051d40: 756c 745b 2752 6564 6973 4669 6c74 6572  ult['RedisFilter
+00051d50: 456e 6162 6c65 6427 5d20 3d20 7365 6c66  Enabled'] = self
+00051d60: 2e72 6564 6973 5f66 696c 7465 725f 656e  .redis_filter_en
+00051d70: 6162 6c65 640a 2020 2020 2020 2020 6966  abled.        if
+00051d80: 2073 656c 662e 7365 7276 6963 655f 6d65   self.service_me
+00051d90: 7368 5f69 6420 6973 206e 6f74 204e 6f6e  sh_id is not Non
+00051da0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00051db0: 6573 756c 745b 2753 6572 7669 6365 4d65  esult['ServiceMe
+00051dc0: 7368 4964 275d 203d 2073 656c 662e 7365  shId'] = self.se
+00051dd0: 7276 6963 655f 6d65 7368 5f69 640a 2020  rvice_mesh_id.  
+00051de0: 2020 2020 2020 6966 2073 656c 662e 7369        if self.si
+00051df0: 6465 6361 725f 696e 6a65 6374 6f72 5f6c  decar_injector_l
+00051e00: 696d 6974 5f63 7075 2069 7320 6e6f 7420  imit_cpu is not 
+00051e10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00051e20: 2020 7265 7375 6c74 5b27 5369 6465 6361    result['Sideca
+00051e30: 7249 6e6a 6563 746f 724c 696d 6974 4350  rInjectorLimitCP
+00051e40: 5527 5d20 3d20 7365 6c66 2e73 6964 6563  U'] = self.sidec
+00051e50: 6172 5f69 6e6a 6563 746f 725f 6c69 6d69  ar_injector_limi
+00051e60: 745f 6370 750a 2020 2020 2020 2020 6966  t_cpu.        if
+00051e70: 2073 656c 662e 7369 6465 6361 725f 696e   self.sidecar_in
+00051e80: 6a65 6374 6f72 5f6c 696d 6974 5f6d 656d  jector_limit_mem
+00051e90: 6f72 7920 6973 206e 6f74 204e 6f6e 653a  ory is not None:
+00051ea0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00051eb0: 756c 745b 2753 6964 6563 6172 496e 6a65  ult['SidecarInje
+00051ec0: 6374 6f72 4c69 6d69 744d 656d 6f72 7927  ctorLimitMemory'
+00051ed0: 5d20 3d20 7365 6c66 2e73 6964 6563 6172  ] = self.sidecar
+00051ee0: 5f69 6e6a 6563 746f 725f 6c69 6d69 745f  _injector_limit_
+00051ef0: 6d65 6d6f 7279 0a20 2020 2020 2020 2069  memory.        i
+00051f00: 6620 7365 6c66 2e73 6964 6563 6172 5f69  f self.sidecar_i
+00051f10: 6e6a 6563 746f 725f 7265 7175 6573 745f  njector_request_
+00051f20: 6370 7520 6973 206e 6f74 204e 6f6e 653a  cpu is not None:
+00051f30: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00051f40: 756c 745b 2753 6964 6563 6172 496e 6a65  ult['SidecarInje
+00051f50: 6374 6f72 5265 7175 6573 7443 5055 275d  ctorRequestCPU']
+00051f60: 203d 2073 656c 662e 7369 6465 6361 725f   = self.sidecar_
+00051f70: 696e 6a65 6374 6f72 5f72 6571 7565 7374  injector_request
+00051f80: 5f63 7075 0a20 2020 2020 2020 2069 6620  _cpu.        if 
+00051f90: 7365 6c66 2e73 6964 6563 6172 5f69 6e6a  self.sidecar_inj
+00051fa0: 6563 746f 725f 7265 7175 6573 745f 6d65  ector_request_me
+00051fb0: 6d6f 7279 2069 7320 6e6f 7420 4e6f 6e65  mory is not None
+00051fc0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00051fd0: 7375 6c74 5b27 5369 6465 6361 7249 6e6a  sult['SidecarInj
+00051fe0: 6563 746f 7252 6571 7565 7374 4d65 6d6f  ectorRequestMemo
+00051ff0: 7279 275d 203d 2073 656c 662e 7369 6465  ry'] = self.side
+00052000: 6361 725f 696e 6a65 6374 6f72 5f72 6571  car_injector_req
+00052010: 7565 7374 5f6d 656d 6f72 790a 2020 2020  uest_memory.    
+00052020: 2020 2020 6966 2073 656c 662e 7369 6465      if self.side
+00052030: 6361 725f 696e 6a65 6374 6f72 5f77 6562  car_injector_web
+00052040: 686f 6f6b 5f61 735f 7961 6d6c 2069 7320  hook_as_yaml is 
+00052050: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00052060: 2020 2020 2020 7265 7375 6c74 5b27 5369        result['Si
+00052070: 6465 6361 7249 6e6a 6563 746f 7257 6562  decarInjectorWeb
+00052080: 686f 6f6b 4173 5961 6d6c 275d 203d 2073  hookAsYaml'] = s
+00052090: 656c 662e 7369 6465 6361 725f 696e 6a65  elf.sidecar_inje
+000520a0: 6374 6f72 5f77 6562 686f 6f6b 5f61 735f  ctor_webhook_as_
+000520b0: 7961 6d6c 0a20 2020 2020 2020 2069 6620  yaml.        if 
+000520c0: 7365 6c66 2e74 656c 656d 6574 7279 2069  self.telemetry i
+000520d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000520e0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000520f0: 5465 6c65 6d65 7472 7927 5d20 3d20 7365  Telemetry'] = se
+00052100: 6c66 2e74 656c 656d 6574 7279 0a20 2020  lf.telemetry.   
+00052110: 2020 2020 2069 6620 7365 6c66 2e74 6572       if self.ter
+00052120: 6d69 6e61 7469 6f6e 5f64 7261 696e 5f64  mination_drain_d
+00052130: 7572 6174 696f 6e20 6973 206e 6f74 204e  uration is not N
+00052140: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00052150: 2072 6573 756c 745b 2754 6572 6d69 6e61   result['Termina
+00052160: 7469 6f6e 4472 6169 6e44 7572 6174 696f  tionDrainDuratio
+00052170: 6e27 5d20 3d20 7365 6c66 2e74 6572 6d69  n'] = self.termi
+00052180: 6e61 7469 6f6e 5f64 7261 696e 5f64 7572  nation_drain_dur
+00052190: 6174 696f 6e0a 2020 2020 2020 2020 6966  ation.        if
+000521a0: 2073 656c 662e 7468 7269 6674 5f66 696c   self.thrift_fil
+000521b0: 7465 725f 656e 6162 6c65 6420 6973 206e  ter_enabled is n
+000521c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000521d0: 2020 2020 2072 6573 756c 745b 2754 6872       result['Thr
+000521e0: 6966 7446 696c 7465 7245 6e61 626c 6564  iftFilterEnabled
+000521f0: 275d 203d 2073 656c 662e 7468 7269 6674  '] = self.thrift
+00052200: 5f66 696c 7465 725f 656e 6162 6c65 640a  _filter_enabled.
+00052210: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00052220: 7472 6163 655f 7361 6d70 6c69 6e67 2069  trace_sampling i
+00052230: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00052240: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00052250: 5472 6163 6553 616d 706c 696e 6727 5d20  TraceSampling'] 
+00052260: 3d20 7365 6c66 2e74 7261 6365 5f73 616d  = self.trace_sam
+00052270: 706c 696e 670a 2020 2020 2020 2020 6966  pling.        if
+00052280: 2073 656c 662e 7472 6163 696e 6720 6973   self.tracing is
+00052290: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000522a0: 2020 2020 2020 2072 6573 756c 745b 2754         result['T
+000522b0: 7261 6369 6e67 275d 203d 2073 656c 662e  racing'] = self.
+000522c0: 7472 6163 696e 670a 2020 2020 2020 2020  tracing.        
+000522d0: 6966 2073 656c 662e 7765 625f 6173 7365  if self.web_asse
+000522e0: 6d62 6c79 5f66 696c 7465 725f 656e 6162  mbly_filter_enab
+000522f0: 6c65 6420 6973 206e 6f74 204e 6f6e 653a  led is not None:
+00052300: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00052310: 756c 745b 2757 6562 4173 7365 6d62 6c79  ult['WebAssembly
+00052320: 4669 6c74 6572 456e 6162 6c65 6427 5d20  FilterEnabled'] 
+00052330: 3d20 7365 6c66 2e77 6562 5f61 7373 656d  = self.web_assem
+00052340: 626c 795f 6669 6c74 6572 5f65 6e61 626c  bly_filter_enabl
+00052350: 6564 0a20 2020 2020 2020 2072 6574 7572  ed.        retur
+00052360: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+00052370: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+00052380: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+00052390: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+000523a0: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+000523b0: 2020 6966 206d 2e67 6574 2827 4163 6365    if m.get('Acce
+000523c0: 7373 4c6f 6745 6e61 626c 6564 2729 2069  ssLogEnabled') i
+000523d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000523e0: 2020 2020 2020 2020 7365 6c66 2e61 6363          self.acc
+000523f0: 6573 735f 6c6f 675f 656e 6162 6c65 6420  ess_log_enabled 
+00052400: 3d20 6d2e 6765 7428 2741 6363 6573 734c  = m.get('AccessL
+00052410: 6f67 456e 6162 6c65 6427 290a 2020 2020  ogEnabled').    
+00052420: 2020 2020 6966 206d 2e67 6574 2827 4163      if m.get('Ac
+00052430: 6365 7373 4c6f 6746 696c 6527 2920 6973  cessLogFile') is
+00052440: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00052450: 2020 2020 2020 2073 656c 662e 6163 6365         self.acce
+00052460: 7373 5f6c 6f67 5f66 696c 6520 3d20 6d2e  ss_log_file = m.
+00052470: 6765 7428 2741 6363 6573 734c 6f67 4669  get('AccessLogFi
+00052480: 6c65 2729 0a20 2020 2020 2020 2069 6620  le').        if 
+00052490: 6d2e 6765 7428 2741 6363 6573 734c 6f67  m.get('AccessLog
+000524a0: 466f 726d 6174 2729 2069 7320 6e6f 7420  Format') is not 
+000524b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000524c0: 2020 7365 6c66 2e61 6363 6573 735f 6c6f    self.access_lo
+000524d0: 675f 666f 726d 6174 203d 206d 2e67 6574  g_format = m.get
+000524e0: 2827 4163 6365 7373 4c6f 6746 6f72 6d61  ('AccessLogForma
+000524f0: 7427 290a 2020 2020 2020 2020 6966 206d  t').        if m
+00052500: 2e67 6574 2827 4163 6365 7373 4c6f 6750  .get('AccessLogP
+00052510: 726f 6a65 6374 2729 2069 7320 6e6f 7420  roject') is not 
+00052520: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00052530: 2020 7365 6c66 2e61 6363 6573 735f 6c6f    self.access_lo
+00052540: 675f 7072 6f6a 6563 7420 3d20 6d2e 6765  g_project = m.ge
+00052550: 7428 2741 6363 6573 734c 6f67 5072 6f6a  t('AccessLogProj
+00052560: 6563 7427 290a 2020 2020 2020 2020 6966  ect').        if
+00052570: 206d 2e67 6574 2827 4163 6365 7373 4c6f   m.get('AccessLo
+00052580: 6753 6572 7669 6365 456e 6162 6c65 6427  gServiceEnabled'
+00052590: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000525a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000525b0: 6163 6365 7373 5f6c 6f67 5f73 6572 7669  access_log_servi
+000525c0: 6365 5f65 6e61 626c 6564 203d 206d 2e67  ce_enabled = m.g
+000525d0: 6574 2827 4163 6365 7373 4c6f 6753 6572  et('AccessLogSer
+000525e0: 7669 6365 456e 6162 6c65 6427 290a 2020  viceEnabled').  
+000525f0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00052600: 4163 6365 7373 4c6f 6753 6572 7669 6365  AccessLogService
+00052610: 486f 7374 2729 2069 7320 6e6f 7420 4e6f  Host') is not No
+00052620: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00052630: 7365 6c66 2e61 6363 6573 735f 6c6f 675f  self.access_log_
+00052640: 7365 7276 6963 655f 686f 7374 203d 206d  service_host = m
+00052650: 2e67 6574 2827 4163 6365 7373 4c6f 6753  .get('AccessLogS
+00052660: 6572 7669 6365 486f 7374 2729 0a20 2020  erviceHost').   
+00052670: 2020 2020 2069 6620 6d2e 6765 7428 2741       if m.get('A
+00052680: 6363 6573 734c 6f67 5365 7276 6963 6550  ccessLogServiceP
+00052690: 6f72 7427 2920 6973 206e 6f74 204e 6f6e  ort') is not Non
+000526a0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000526b0: 656c 662e 6163 6365 7373 5f6c 6f67 5f73  elf.access_log_s
+000526c0: 6572 7669 6365 5f70 6f72 7420 3d20 6d2e  ervice_port = m.
+000526d0: 6765 7428 2741 6363 6573 734c 6f67 5365  get('AccessLogSe
+000526e0: 7276 6963 6550 6f72 7427 290a 2020 2020  rvicePort').    
+000526f0: 2020 2020 6966 206d 2e67 6574 2827 4175      if m.get('Au
+00052700: 6469 7450 726f 6a65 6374 2729 2069 7320  ditProject') is 
+00052710: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00052720: 2020 2020 2020 7365 6c66 2e61 7564 6974        self.audit
+00052730: 5f70 726f 6a65 6374 203d 206d 2e67 6574  _project = m.get
+00052740: 2827 4175 6469 7450 726f 6a65 6374 2729  ('AuditProject')
+00052750: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00052760: 7428 2741 7574 6f49 6e6a 6563 7469 6f6e  t('AutoInjection
+00052770: 506f 6c69 6379 456e 6162 6c65 6427 2920  PolicyEnabled') 
+00052780: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00052790: 2020 2020 2020 2020 2073 656c 662e 6175           self.au
+000527a0: 746f 5f69 6e6a 6563 7469 6f6e 5f70 6f6c  to_injection_pol
+000527b0: 6963 795f 656e 6162 6c65 6420 3d20 6d2e  icy_enabled = m.
+000527c0: 6765 7428 2741 7574 6f49 6e6a 6563 7469  get('AutoInjecti
+000527d0: 6f6e 506f 6c69 6379 456e 6162 6c65 6427  onPolicyEnabled'
+000527e0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000527f0: 6574 2827 4352 4167 6772 6567 6174 696f  et('CRAggregatio
+00052800: 6e45 6e61 626c 6564 2729 2069 7320 6e6f  nEnabled') is no
+00052810: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00052820: 2020 2020 7365 6c66 2e63 7261 6767 7265      self.craggre
+00052830: 6761 7469 6f6e 5f65 6e61 626c 6564 203d  gation_enabled =
+00052840: 206d 2e67 6574 2827 4352 4167 6772 6567   m.get('CRAggreg
+00052850: 6174 696f 6e45 6e61 626c 6564 2729 0a20  ationEnabled'). 
+00052860: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00052870: 2743 6c75 7374 6572 5370 6563 2729 2069  'ClusterSpec') i
+00052880: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00052890: 2020 2020 2020 2020 7365 6c66 2e63 6c75          self.clu
+000528a0: 7374 6572 5f73 7065 6320 3d20 6d2e 6765  ster_spec = m.ge
+000528b0: 7428 2743 6c75 7374 6572 5370 6563 2729  t('ClusterSpec')
+000528c0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000528d0: 7428 2743 6e69 456e 6162 6c65 6427 2920  t('CniEnabled') 
+000528e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000528f0: 2020 2020 2020 2020 2073 656c 662e 636e           self.cn
+00052900: 695f 656e 6162 6c65 6420 3d20 6d2e 6765  i_enabled = m.ge
+00052910: 7428 2743 6e69 456e 6162 6c65 6427 290a  t('CniEnabled').
+00052920: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00052930: 2827 436e 6945 7863 6c75 6465 4e61 6d65  ('CniExcludeName
+00052940: 7370 6163 6573 2729 2069 7320 6e6f 7420  spaces') is not 
+00052950: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00052960: 2020 7365 6c66 2e63 6e69 5f65 7863 6c75    self.cni_exclu
+00052970: 6465 5f6e 616d 6573 7061 6365 7320 3d20  de_namespaces = 
+00052980: 6d2e 6765 7428 2743 6e69 4578 636c 7564  m.get('CniExclud
+00052990: 654e 616d 6573 7061 6365 7327 290a 2020  eNamespaces').  
+000529a0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000529b0: 436f 6e66 6967 536f 7572 6365 456e 6162  ConfigSourceEnab
+000529c0: 6c65 6427 2920 6973 206e 6f74 204e 6f6e  led') is not Non
+000529d0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000529e0: 656c 662e 636f 6e66 6967 5f73 6f75 7263  elf.config_sourc
+000529f0: 655f 656e 6162 6c65 6420 3d20 6d2e 6765  e_enabled = m.ge
+00052a00: 7428 2743 6f6e 6669 6753 6f75 7263 6545  t('ConfigSourceE
+00052a10: 6e61 626c 6564 2729 0a20 2020 2020 2020  nabled').       
+00052a20: 2069 6620 6d2e 6765 7428 2743 6f6e 6669   if m.get('Confi
+00052a30: 6753 6f75 7263 654e 6163 6f73 4944 2729  gSourceNacosID')
+00052a40: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00052a50: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00052a60: 6f6e 6669 675f 736f 7572 6365 5f6e 6163  onfig_source_nac
+00052a70: 6f73 5f69 6420 3d20 6d2e 6765 7428 2743  os_id = m.get('C
+00052a80: 6f6e 6669 6753 6f75 7263 654e 6163 6f73  onfigSourceNacos
+00052a90: 4944 2729 0a20 2020 2020 2020 2069 6620  ID').        if 
+00052aa0: 6d2e 6765 7428 2743 7573 746f 6d69 7a65  m.get('Customize
+00052ab0: 6450 726f 6d65 7468 6575 7327 2920 6973  dPrometheus') is
+00052ac0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00052ad0: 2020 2020 2020 2073 656c 662e 6375 7374         self.cust
+00052ae0: 6f6d 697a 6564 5f70 726f 6d65 7468 6575  omized_prometheu
+00052af0: 7320 3d20 6d2e 6765 7428 2743 7573 746f  s = m.get('Custo
+00052b00: 6d69 7a65 6450 726f 6d65 7468 6575 7327  mizedPrometheus'
+00052b10: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00052b20: 6574 2827 4375 7374 6f6d 697a 6564 5a69  et('CustomizedZi
+00052b30: 706b 696e 2729 2069 7320 6e6f 7420 4e6f  pkin') is not No
+00052b40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00052b50: 7365 6c66 2e63 7573 746f 6d69 7a65 645f  self.customized_
+00052b60: 7a69 706b 696e 203d 206d 2e67 6574 2827  zipkin = m.get('
+00052b70: 4375 7374 6f6d 697a 6564 5a69 706b 696e  CustomizedZipkin
+00052b80: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00052b90: 6765 7428 2744 4e53 5072 6f78 7969 6e67  get('DNSProxying
+00052ba0: 456e 6162 6c65 6427 2920 6973 206e 6f74  Enabled') is not
+00052bb0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00052bc0: 2020 2073 656c 662e 646e 7370 726f 7879     self.dnsproxy
+00052bd0: 696e 675f 656e 6162 6c65 6420 3d20 6d2e  ing_enabled = m.
+00052be0: 6765 7428 2744 4e53 5072 6f78 7969 6e67  get('DNSProxying
+00052bf0: 456e 6162 6c65 6427 290a 2020 2020 2020  Enabled').      
+00052c00: 2020 6966 206d 2e67 6574 2827 4469 7363    if m.get('Disc
+00052c10: 6f76 6572 7953 656c 6563 746f 7273 2729  overySelectors')
+00052c20: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00052c30: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00052c40: 6973 636f 7665 7279 5f73 656c 6563 746f  iscovery_selecto
+00052c50: 7273 203d 206d 2e67 6574 2827 4469 7363  rs = m.get('Disc
+00052c60: 6f76 6572 7953 656c 6563 746f 7273 2729  overySelectors')
+00052c70: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00052c80: 7428 2744 7562 626f 4669 6c74 6572 456e  t('DubboFilterEn
+00052c90: 6162 6c65 6427 2920 6973 206e 6f74 204e  abled') is not N
+00052ca0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00052cb0: 2073 656c 662e 6475 6262 6f5f 6669 6c74   self.dubbo_filt
+00052cc0: 6572 5f65 6e61 626c 6564 203d 206d 2e67  er_enabled = m.g
+00052cd0: 6574 2827 4475 6262 6f46 696c 7465 7245  et('DubboFilterE
+00052ce0: 6e61 626c 6564 2729 0a20 2020 2020 2020  nabled').       
+00052cf0: 2069 6620 6d2e 6765 7428 2745 6e61 626c   if m.get('Enabl
+00052d00: 6541 7564 6974 2729 2069 7320 6e6f 7420  eAudit') is not 
+00052d10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00052d20: 2020 7365 6c66 2e65 6e61 626c 655f 6175    self.enable_au
+00052d30: 6469 7420 3d20 6d2e 6765 7428 2745 6e61  dit = m.get('Ena
+00052d40: 626c 6541 7564 6974 2729 0a20 2020 2020  bleAudit').     
+00052d50: 2020 2069 6620 6d2e 6765 7428 2745 6e61     if m.get('Ena
+00052d60: 626c 6543 5248 6973 746f 7279 2729 2069  bleCRHistory') i
+00052d70: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00052d80: 2020 2020 2020 2020 7365 6c66 2e65 6e61          self.ena
+00052d90: 626c 655f 6372 6869 7374 6f72 7920 3d20  ble_crhistory = 
+00052da0: 6d2e 6765 7428 2745 6e61 626c 6543 5248  m.get('EnableCRH
+00052db0: 6973 746f 7279 2729 0a20 2020 2020 2020  istory').       
+00052dc0: 2069 6620 6d2e 6765 7428 2745 6e61 626c   if m.get('Enabl
+00052dd0: 654e 616d 6573 7061 6365 7342 7944 6566  eNamespacesByDef
+00052de0: 6175 6c74 2729 2069 7320 6e6f 7420 4e6f  ault') is not No
+00052df0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00052e00: 7365 6c66 2e65 6e61 626c 655f 6e61 6d65  self.enable_name
+00052e10: 7370 6163 6573 5f62 795f 6465 6661 756c  spaces_by_defaul
+00052e20: 7420 3d20 6d2e 6765 7428 2745 6e61 626c  t = m.get('Enabl
+00052e30: 654e 616d 6573 7061 6365 7342 7944 6566  eNamespacesByDef
+00052e40: 6175 6c74 2729 0a20 2020 2020 2020 2069  ault').        i
+00052e50: 6620 6d2e 6765 7428 2745 6e61 626c 6553  f m.get('EnableS
+00052e60: 4453 5365 7276 6572 2729 2069 7320 6e6f  DSServer') is no
+00052e70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00052e80: 2020 2020 7365 6c66 2e65 6e61 626c 655f      self.enable_
+00052e90: 7364 7373 6572 7665 7220 3d20 6d2e 6765  sdsserver = m.ge
+00052ea0: 7428 2745 6e61 626c 6553 4453 5365 7276  t('EnableSDSServ
+00052eb0: 6572 2729 0a20 2020 2020 2020 2069 6620  er').        if 
+00052ec0: 6d2e 6765 7428 2745 7863 6c75 6465 4950  m.get('ExcludeIP
+00052ed0: 5261 6e67 6573 2729 2069 7320 6e6f 7420  Ranges') is not 
+00052ee0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00052ef0: 2020 7365 6c66 2e65 7863 6c75 6465 5f69    self.exclude_i
+00052f00: 7072 616e 6765 7320 3d20 6d2e 6765 7428  pranges = m.get(
+00052f10: 2745 7863 6c75 6465 4950 5261 6e67 6573  'ExcludeIPRanges
+00052f20: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00052f30: 6765 7428 2745 7863 6c75 6465 496e 626f  get('ExcludeInbo
+00052f40: 756e 6450 6f72 7473 2729 2069 7320 6e6f  undPorts') is no
+00052f50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00052f60: 2020 2020 7365 6c66 2e65 7863 6c75 6465      self.exclude
+00052f70: 5f69 6e62 6f75 6e64 5f70 6f72 7473 203d  _inbound_ports =
+00052f80: 206d 2e67 6574 2827 4578 636c 7564 6549   m.get('ExcludeI
+00052f90: 6e62 6f75 6e64 506f 7274 7327 290a 2020  nboundPorts').  
+00052fa0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00052fb0: 4578 636c 7564 654f 7574 626f 756e 6450  ExcludeOutboundP
+00052fc0: 6f72 7473 2729 2069 7320 6e6f 7420 4e6f  orts') is not No
+00052fd0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00052fe0: 7365 6c66 2e65 7863 6c75 6465 5f6f 7574  self.exclude_out
+00052ff0: 626f 756e 645f 706f 7274 7320 3d20 6d2e  bound_ports = m.
+00053000: 6765 7428 2745 7863 6c75 6465 4f75 7462  get('ExcludeOutb
+00053010: 6f75 6e64 506f 7274 7327 290a 2020 2020  oundPorts').    
+00053020: 2020 2020 6966 206d 2e67 6574 2827 4669      if m.get('Fi
+00053030: 6c74 6572 4761 7465 7761 7943 6c75 7374  lterGatewayClust
+00053040: 6572 436f 6e66 6967 2729 2069 7320 6e6f  erConfig') is no
+00053050: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00053060: 2020 2020 7365 6c66 2e66 696c 7465 725f      self.filter_
+00053070: 6761 7465 7761 795f 636c 7573 7465 725f  gateway_cluster_
+00053080: 636f 6e66 6967 203d 206d 2e67 6574 2827  config = m.get('
+00053090: 4669 6c74 6572 4761 7465 7761 7943 6c75  FilterGatewayClu
+000530a0: 7374 6572 436f 6e66 6967 2729 0a20 2020  sterConfig').   
+000530b0: 2020 2020 2069 6620 6d2e 6765 7428 2747       if m.get('G
+000530c0: 6174 6577 6179 4150 4945 6e61 626c 6564  atewayAPIEnabled
+000530d0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000530e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000530f0: 2e67 6174 6577 6179 5f61 7069 656e 6162  .gateway_apienab
+00053100: 6c65 6420 3d20 6d2e 6765 7428 2747 6174  led = m.get('Gat
+00053110: 6577 6179 4150 4945 6e61 626c 6564 2729  ewayAPIEnabled')
+00053120: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00053130: 7428 2747 6c6f 6261 6c52 6174 654c 696d  t('GlobalRateLim
+00053140: 6974 456e 6162 6c65 6427 2920 6973 206e  itEnabled') is n
+00053150: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00053160: 2020 2020 2073 656c 662e 676c 6f62 616c       self.global
+00053170: 5f72 6174 655f 6c69 6d69 745f 656e 6162  _rate_limit_enab
+00053180: 6c65 6420 3d20 6d2e 6765 7428 2747 6c6f  led = m.get('Glo
+00053190: 6261 6c52 6174 654c 696d 6974 456e 6162  balRateLimitEnab
+000531a0: 6c65 6427 290a 2020 2020 2020 2020 6966  led').        if
+000531b0: 206d 2e67 6574 2827 4874 7470 3130 456e   m.get('Http10En
+000531c0: 6162 6c65 6427 2920 6973 206e 6f74 204e  abled') is not N
+000531d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000531e0: 2073 656c 662e 6874 7470 5f31 3065 6e61   self.http_10ena
+000531f0: 626c 6564 203d 206d 2e67 6574 2827 4874  bled = m.get('Ht
+00053200: 7470 3130 456e 6162 6c65 6427 290a 2020  tp10Enabled').  
+00053210: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00053220: 496e 636c 7564 6549 5052 616e 6765 7327  IncludeIPRanges'
+00053230: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00053240: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00053250: 696e 636c 7564 655f 6970 7261 6e67 6573  include_ipranges
+00053260: 203d 206d 2e67 6574 2827 496e 636c 7564   = m.get('Includ
+00053270: 6549 5052 616e 6765 7327 290a 2020 2020  eIPRanges').    
+00053280: 2020 2020 6966 206d 2e67 6574 2827 496e      if m.get('In
+00053290: 636c 7564 6549 6e62 6f75 6e64 506f 7274  cludeInboundPort
+000532a0: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+000532b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000532c0: 662e 696e 636c 7564 655f 696e 626f 756e  f.include_inboun
+000532d0: 645f 706f 7274 7320 3d20 6d2e 6765 7428  d_ports = m.get(
+000532e0: 2749 6e63 6c75 6465 496e 626f 756e 6450  'IncludeInboundP
+000532f0: 6f72 7473 2729 0a20 2020 2020 2020 2069  orts').        i
+00053300: 6620 6d2e 6765 7428 274b 6961 6c69 456e  f m.get('KialiEn
+00053310: 6162 6c65 6427 2920 6973 206e 6f74 204e  abled') is not N
+00053320: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00053330: 2073 656c 662e 6b69 616c 695f 656e 6162   self.kiali_enab
+00053340: 6c65 6420 3d20 6d2e 6765 7428 274b 6961  led = m.get('Kia
+00053350: 6c69 456e 6162 6c65 6427 290a 2020 2020  liEnabled').    
+00053360: 2020 2020 6966 206d 2e67 6574 2827 4c69      if m.get('Li
+00053370: 6665 6379 636c 6527 2920 6973 206e 6f74  fecycle') is not
+00053380: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00053390: 2020 2073 656c 662e 6c69 6665 6379 636c     self.lifecycl
+000533a0: 6520 3d20 6d2e 6765 7428 274c 6966 6563  e = m.get('Lifec
+000533b0: 7963 6c65 2729 0a20 2020 2020 2020 2069  ycle').        i
+000533c0: 6620 6d2e 6765 7428 274c 6f63 616c 6974  f m.get('Localit
+000533d0: 794c 4243 6f6e 6627 2920 6973 206e 6f74  yLBConf') is not
+000533e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000533f0: 2020 2073 656c 662e 6c6f 6361 6c69 7479     self.locality
+00053400: 5f6c 6263 6f6e 6620 3d20 6d2e 6765 7428  _lbconf = m.get(
+00053410: 274c 6f63 616c 6974 794c 4243 6f6e 6627  'LocalityLBConf'
+00053420: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00053430: 6574 2827 4c6f 6361 6c69 7479 4c6f 6164  et('LocalityLoad
+00053440: 4261 6c61 6e63 696e 6727 2920 6973 206e  Balancing') is n
+00053450: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00053460: 2020 2020 2073 656c 662e 6c6f 6361 6c69       self.locali
+00053470: 7479 5f6c 6f61 645f 6261 6c61 6e63 696e  ty_load_balancin
+00053480: 6720 3d20 6d2e 6765 7428 274c 6f63 616c  g = m.get('Local
+00053490: 6974 794c 6f61 6442 616c 616e 6369 6e67  ityLoadBalancing
+000534a0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+000534b0: 6765 7428 274d 5345 456e 6162 6c65 6427  get('MSEEnabled'
+000534c0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000534d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000534e0: 6d73 6565 6e61 626c 6564 203d 206d 2e67  mseenabled = m.g
+000534f0: 6574 2827 4d53 4545 6e61 626c 6564 2729  et('MSEEnabled')
+00053500: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00053510: 7428 274d 756c 7469 4275 6666 6572 456e  t('MultiBufferEn
+00053520: 6162 6c65 6427 2920 6973 206e 6f74 204e  abled') is not N
+00053530: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00053540: 2073 656c 662e 6d75 6c74 695f 6275 6666   self.multi_buff
+00053550: 6572 5f65 6e61 626c 6564 203d 206d 2e67  er_enabled = m.g
+00053560: 6574 2827 4d75 6c74 6942 7566 6665 7245  et('MultiBufferE
+00053570: 6e61 626c 6564 2729 0a20 2020 2020 2020  nabled').       
+00053580: 2069 6620 6d2e 6765 7428 274d 756c 7469   if m.get('Multi
+00053590: 4275 6666 6572 506f 6c6c 4465 6c61 7927  BufferPollDelay'
+000535a0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000535b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000535c0: 6d75 6c74 695f 6275 6666 6572 5f70 6f6c  multi_buffer_pol
+000535d0: 6c5f 6465 6c61 7920 3d20 6d2e 6765 7428  l_delay = m.get(
+000535e0: 274d 756c 7469 4275 6666 6572 506f 6c6c  'MultiBufferPoll
+000535f0: 4465 6c61 7927 290a 2020 2020 2020 2020  Delay').        
+00053600: 6966 206d 2e67 6574 2827 4d79 7371 6c46  if m.get('MysqlF
+00053610: 696c 7465 7245 6e61 626c 6564 2729 2069  ilterEnabled') i
+00053620: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00053630: 2020 2020 2020 2020 7365 6c66 2e6d 7973          self.mys
+00053640: 716c 5f66 696c 7465 725f 656e 6162 6c65  ql_filter_enable
+00053650: 6420 3d20 6d2e 6765 7428 274d 7973 716c  d = m.get('Mysql
+00053660: 4669 6c74 6572 456e 6162 6c65 6427 290a  FilterEnabled').
+00053670: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00053680: 2827 4f50 414c 696d 6974 4350 5527 2920  ('OPALimitCPU') 
+00053690: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000536a0: 2020 2020 2020 2020 2073 656c 662e 6f70           self.op
+000536b0: 616c 696d 6974 5f63 7075 203d 206d 2e67  alimit_cpu = m.g
+000536c0: 6574 2827 4f50 414c 696d 6974 4350 5527  et('OPALimitCPU'
+000536d0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000536e0: 6574 2827 4f50 414c 696d 6974 4d65 6d6f  et('OPALimitMemo
+000536f0: 7279 2729 2069 7320 6e6f 7420 4e6f 6e65  ry') is not None
+00053700: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00053710: 6c66 2e6f 7061 6c69 6d69 745f 6d65 6d6f  lf.opalimit_memo
+00053720: 7279 203d 206d 2e67 6574 2827 4f50 414c  ry = m.get('OPAL
+00053730: 696d 6974 4d65 6d6f 7279 2729 0a20 2020  imitMemory').   
+00053740: 2020 2020 2069 6620 6d2e 6765 7428 274f       if m.get('O
+00053750: 5041 4c6f 674c 6576 656c 2729 2069 7320  PALogLevel') is 
+00053760: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00053770: 2020 2020 2020 7365 6c66 2e6f 7061 6c6f        self.opalo
+00053780: 675f 6c65 7665 6c20 3d20 6d2e 6765 7428  g_level = m.get(
+00053790: 274f 5041 4c6f 674c 6576 656c 2729 0a20  'OPALogLevel'). 
+000537a0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000537b0: 274f 5041 5265 7175 6573 7443 5055 2729  'OPARequestCPU')
+000537c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000537d0: 2020 2020 2020 2020 2020 7365 6c66 2e6f            self.o
+000537e0: 7061 7265 7175 6573 745f 6370 7520 3d20  parequest_cpu = 
+000537f0: 6d2e 6765 7428 274f 5041 5265 7175 6573  m.get('OPAReques
+00053800: 7443 5055 2729 0a20 2020 2020 2020 2069  tCPU').        i
+00053810: 6620 6d2e 6765 7428 274f 5041 5265 7175  f m.get('OPARequ
+00053820: 6573 744d 656d 6f72 7927 2920 6973 206e  estMemory') is n
+00053830: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00053840: 2020 2020 2073 656c 662e 6f70 6172 6571       self.opareq
+00053850: 7565 7374 5f6d 656d 6f72 7920 3d20 6d2e  uest_memory = m.
+00053860: 6765 7428 274f 5041 5265 7175 6573 744d  get('OPARequestM
+00053870: 656d 6f72 7927 290a 2020 2020 2020 2020  emory').        
+00053880: 6966 206d 2e67 6574 2827 4f70 6145 6e61  if m.get('OpaEna
+00053890: 626c 6564 2729 2069 7320 6e6f 7420 4e6f  bled') is not No
+000538a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000538b0: 7365 6c66 2e6f 7061 5f65 6e61 626c 6564  self.opa_enabled
+000538c0: 203d 206d 2e67 6574 2827 4f70 6145 6e61   = m.get('OpaEna
+000538d0: 626c 6564 2729 0a20 2020 2020 2020 2069  bled').        i
+000538e0: 6620 6d2e 6765 7428 274f 7065 6e41 6765  f m.get('OpenAge
+000538f0: 6e74 506f 6c69 6379 2729 2069 7320 6e6f  ntPolicy') is no
+00053900: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00053910: 2020 2020 7365 6c66 2e6f 7065 6e5f 6167      self.open_ag
+00053920: 656e 745f 706f 6c69 6379 203d 206d 2e67  ent_policy = m.g
+00053930: 6574 2827 4f70 656e 4167 656e 7450 6f6c  et('OpenAgentPol
+00053940: 6963 7927 290a 2020 2020 2020 2020 6966  icy').        if
+00053950: 206d 2e67 6574 2827 4f75 7462 6f75 6e64   m.get('Outbound
+00053960: 5472 6166 6669 6350 6f6c 6963 7927 2920  TrafficPolicy') 
+00053970: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00053980: 2020 2020 2020 2020 2073 656c 662e 6f75           self.ou
+00053990: 7462 6f75 6e64 5f74 7261 6666 6963 5f70  tbound_traffic_p
+000539a0: 6f6c 6963 7920 3d20 6d2e 6765 7428 274f  olicy = m.get('O
+000539b0: 7574 626f 756e 6454 7261 6666 6963 506f  utboundTrafficPo
+000539c0: 6c69 6379 2729 0a20 2020 2020 2020 2069  licy').        i
+000539d0: 6620 6d2e 6765 7428 2750 726f 6d65 7468  f m.get('Prometh
+000539e0: 6575 7355 726c 2729 2069 7320 6e6f 7420  eusUrl') is not 
+000539f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00053a00: 2020 7365 6c66 2e70 726f 6d65 7468 6575    self.prometheu
+00053a10: 735f 7572 6c20 3d20 6d2e 6765 7428 2750  s_url = m.get('P
+00053a20: 726f 6d65 7468 6575 7355 726c 2729 0a20  rometheusUrl'). 
+00053a30: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00053a40: 2750 726f 7879 496e 6974 4350 5552 6573  'ProxyInitCPURes
+00053a50: 6f75 7263 654c 696d 6974 2729 2069 7320  ourceLimit') is 
+00053a60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00053a70: 2020 2020 2020 7365 6c66 2e70 726f 7879        self.proxy
+00053a80: 5f69 6e69 745f 6370 7572 6573 6f75 7263  _init_cpuresourc
+00053a90: 655f 6c69 6d69 7420 3d20 6d2e 6765 7428  e_limit = m.get(
+00053aa0: 2750 726f 7879 496e 6974 4350 5552 6573  'ProxyInitCPURes
+00053ab0: 6f75 7263 654c 696d 6974 2729 0a20 2020  ourceLimit').   
+00053ac0: 2020 2020 2069 6620 6d2e 6765 7428 2750       if m.get('P
+00053ad0: 726f 7879 496e 6974 4350 5552 6573 6f75  roxyInitCPUResou
+00053ae0: 7263 6552 6571 7565 7374 2729 2069 7320  rceRequest') is 
+00053af0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00053b00: 2020 2020 2020 7365 6c66 2e70 726f 7879        self.proxy
+00053b10: 5f69 6e69 745f 6370 7572 6573 6f75 7263  _init_cpuresourc
+00053b20: 655f 7265 7175 6573 7420 3d20 6d2e 6765  e_request = m.ge
+00053b30: 7428 2750 726f 7879 496e 6974 4350 5552  t('ProxyInitCPUR
+00053b40: 6573 6f75 7263 6552 6571 7565 7374 2729  esourceRequest')
+00053b50: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00053b60: 7428 2750 726f 7879 496e 6974 4d65 6d6f  t('ProxyInitMemo
+00053b70: 7279 5265 736f 7572 6365 4c69 6d69 7427  ryResourceLimit'
+00053b80: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00053b90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00053ba0: 7072 6f78 795f 696e 6974 5f6d 656d 6f72  proxy_init_memor
+00053bb0: 795f 7265 736f 7572 6365 5f6c 696d 6974  y_resource_limit
+00053bc0: 203d 206d 2e67 6574 2827 5072 6f78 7949   = m.get('ProxyI
+00053bd0: 6e69 744d 656d 6f72 7952 6573 6f75 7263  nitMemoryResourc
+00053be0: 654c 696d 6974 2729 0a20 2020 2020 2020  eLimit').       
+00053bf0: 2069 6620 6d2e 6765 7428 2750 726f 7879   if m.get('Proxy
+00053c00: 496e 6974 4d65 6d6f 7279 5265 736f 7572  InitMemoryResour
+00053c10: 6365 5265 7175 6573 7427 2920 6973 206e  ceRequest') is n
+00053c20: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00053c30: 2020 2020 2073 656c 662e 7072 6f78 795f       self.proxy_
+00053c40: 696e 6974 5f6d 656d 6f72 795f 7265 736f  init_memory_reso
+00053c50: 7572 6365 5f72 6571 7565 7374 203d 206d  urce_request = m
+00053c60: 2e67 6574 2827 5072 6f78 7949 6e69 744d  .get('ProxyInitM
+00053c70: 656d 6f72 7952 6573 6f75 7263 6552 6571  emoryResourceReq
+00053c80: 7565 7374 2729 0a20 2020 2020 2020 2069  uest').        i
+00053c90: 6620 6d2e 6765 7428 2750 726f 7879 4c69  f m.get('ProxyLi
+00053ca0: 6d69 7443 5055 2729 2069 7320 6e6f 7420  mitCPU') is not 
+00053cb0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00053cc0: 2020 7365 6c66 2e70 726f 7879 5f6c 696d    self.proxy_lim
+00053cd0: 6974 5f63 7075 203d 206d 2e67 6574 2827  it_cpu = m.get('
+00053ce0: 5072 6f78 794c 696d 6974 4350 5527 290a  ProxyLimitCPU').
+00053cf0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00053d00: 2827 5072 6f78 794c 696d 6974 4d65 6d6f  ('ProxyLimitMemo
+00053d10: 7279 2729 2069 7320 6e6f 7420 4e6f 6e65  ry') is not None
+00053d20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00053d30: 6c66 2e70 726f 7879 5f6c 696d 6974 5f6d  lf.proxy_limit_m
+00053d40: 656d 6f72 7920 3d20 6d2e 6765 7428 2750  emory = m.get('P
+00053d50: 726f 7879 4c69 6d69 744d 656d 6f72 7927  roxyLimitMemory'
+00053d60: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00053d70: 6574 2827 5072 6f78 7952 6571 7565 7374  et('ProxyRequest
+00053d80: 4350 5527 2920 6973 206e 6f74 204e 6f6e  CPU') is not Non
+00053d90: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00053da0: 656c 662e 7072 6f78 795f 7265 7175 6573  elf.proxy_reques
+00053db0: 745f 6370 7520 3d20 6d2e 6765 7428 2750  t_cpu = m.get('P
+00053dc0: 726f 7879 5265 7175 6573 7443 5055 2729  roxyRequestCPU')
+00053dd0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00053de0: 7428 2750 726f 7879 5265 7175 6573 744d  t('ProxyRequestM
+00053df0: 656d 6f72 7927 2920 6973 206e 6f74 204e  emory') is not N
+00053e00: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00053e10: 2073 656c 662e 7072 6f78 795f 7265 7175   self.proxy_requ
+00053e20: 6573 745f 6d65 6d6f 7279 203d 206d 2e67  est_memory = m.g
+00053e30: 6574 2827 5072 6f78 7952 6571 7565 7374  et('ProxyRequest
+00053e40: 4d65 6d6f 7279 2729 0a20 2020 2020 2020  Memory').       
+00053e50: 2069 6620 6d2e 6765 7428 2752 6564 6973   if m.get('Redis
+00053e60: 4669 6c74 6572 456e 6162 6c65 6427 2920  FilterEnabled') 
+00053e70: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00053e80: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+00053e90: 6469 735f 6669 6c74 6572 5f65 6e61 626c  dis_filter_enabl
+00053ea0: 6564 203d 206d 2e67 6574 2827 5265 6469  ed = m.get('Redi
+00053eb0: 7346 696c 7465 7245 6e61 626c 6564 2729  sFilterEnabled')
+00053ec0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00053ed0: 7428 2753 6572 7669 6365 4d65 7368 4964  t('ServiceMeshId
+00053ee0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00053ef0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00053f00: 2e73 6572 7669 6365 5f6d 6573 685f 6964  .service_mesh_id
+00053f10: 203d 206d 2e67 6574 2827 5365 7276 6963   = m.get('Servic
+00053f20: 654d 6573 6849 6427 290a 2020 2020 2020  eMeshId').      
+00053f30: 2020 6966 206d 2e67 6574 2827 5369 6465    if m.get('Side
+00053f40: 6361 7249 6e6a 6563 746f 724c 696d 6974  carInjectorLimit
+00053f50: 4350 5527 2920 6973 206e 6f74 204e 6f6e  CPU') is not Non
+00053f60: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00053f70: 656c 662e 7369 6465 6361 725f 696e 6a65  elf.sidecar_inje
+00053f80: 6374 6f72 5f6c 696d 6974 5f63 7075 203d  ctor_limit_cpu =
+00053f90: 206d 2e67 6574 2827 5369 6465 6361 7249   m.get('SidecarI
+00053fa0: 6e6a 6563 746f 724c 696d 6974 4350 5527  njectorLimitCPU'
+00053fb0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00053fc0: 6574 2827 5369 6465 6361 7249 6e6a 6563  et('SidecarInjec
+00053fd0: 746f 724c 696d 6974 4d65 6d6f 7279 2729  torLimitMemory')
+00053fe0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00053ff0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00054000: 6964 6563 6172 5f69 6e6a 6563 746f 725f  idecar_injector_
+00054010: 6c69 6d69 745f 6d65 6d6f 7279 203d 206d  limit_memory = m
+00054020: 2e67 6574 2827 5369 6465 6361 7249 6e6a  .get('SidecarInj
+00054030: 6563 746f 724c 696d 6974 4d65 6d6f 7279  ectorLimitMemory
+00054040: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00054050: 6765 7428 2753 6964 6563 6172 496e 6a65  get('SidecarInje
+00054060: 6374 6f72 5265 7175 6573 7443 5055 2729  ctorRequestCPU')
+00054070: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00054080: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00054090: 6964 6563 6172 5f69 6e6a 6563 746f 725f  idecar_injector_
+000540a0: 7265 7175 6573 745f 6370 7520 3d20 6d2e  request_cpu = m.
+000540b0: 6765 7428 2753 6964 6563 6172 496e 6a65  get('SidecarInje
+000540c0: 6374 6f72 5265 7175 6573 7443 5055 2729  ctorRequestCPU')
+000540d0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000540e0: 7428 2753 6964 6563 6172 496e 6a65 6374  t('SidecarInject
+000540f0: 6f72 5265 7175 6573 744d 656d 6f72 7927  orRequestMemory'
+00054100: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00054110: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00054120: 7369 6465 6361 725f 696e 6a65 6374 6f72  sidecar_injector
+00054130: 5f72 6571 7565 7374 5f6d 656d 6f72 7920  _request_memory 
+00054140: 3d20 6d2e 6765 7428 2753 6964 6563 6172  = m.get('Sidecar
+00054150: 496e 6a65 6374 6f72 5265 7175 6573 744d  InjectorRequestM
+00054160: 656d 6f72 7927 290a 2020 2020 2020 2020  emory').        
+00054170: 6966 206d 2e67 6574 2827 5369 6465 6361  if m.get('Sideca
+00054180: 7249 6e6a 6563 746f 7257 6562 686f 6f6b  rInjectorWebhook
+00054190: 4173 5961 6d6c 2729 2069 7320 6e6f 7420  AsYaml') is not 
+000541a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000541b0: 2020 7365 6c66 2e73 6964 6563 6172 5f69    self.sidecar_i
+000541c0: 6e6a 6563 746f 725f 7765 6268 6f6f 6b5f  njector_webhook_
+000541d0: 6173 5f79 616d 6c20 3d20 6d2e 6765 7428  as_yaml = m.get(
+000541e0: 2753 6964 6563 6172 496e 6a65 6374 6f72  'SidecarInjector
+000541f0: 5765 6268 6f6f 6b41 7359 616d 6c27 290a  WebhookAsYaml').
+00054200: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00054210: 2827 5465 6c65 6d65 7472 7927 2920 6973  ('Telemetry') is
+00054220: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00054230: 2020 2020 2020 2073 656c 662e 7465 6c65         self.tele
+00054240: 6d65 7472 7920 3d20 6d2e 6765 7428 2754  metry = m.get('T
+00054250: 656c 656d 6574 7279 2729 0a20 2020 2020  elemetry').     
+00054260: 2020 2069 6620 6d2e 6765 7428 2754 6572     if m.get('Ter
+00054270: 6d69 6e61 7469 6f6e 4472 6169 6e44 7572  minationDrainDur
+00054280: 6174 696f 6e27 2920 6973 206e 6f74 204e  ation') is not N
+00054290: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000542a0: 2073 656c 662e 7465 726d 696e 6174 696f   self.terminatio
+000542b0: 6e5f 6472 6169 6e5f 6475 7261 7469 6f6e  n_drain_duration
+000542c0: 203d 206d 2e67 6574 2827 5465 726d 696e   = m.get('Termin
+000542d0: 6174 696f 6e44 7261 696e 4475 7261 7469  ationDrainDurati
+000542e0: 6f6e 2729 0a20 2020 2020 2020 2069 6620  on').        if 
+000542f0: 6d2e 6765 7428 2754 6872 6966 7446 696c  m.get('ThriftFil
+00054300: 7465 7245 6e61 626c 6564 2729 2069 7320  terEnabled') is 
+00054310: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00054320: 2020 2020 2020 7365 6c66 2e74 6872 6966        self.thrif
+00054330: 745f 6669 6c74 6572 5f65 6e61 626c 6564  t_filter_enabled
+00054340: 203d 206d 2e67 6574 2827 5468 7269 6674   = m.get('Thrift
+00054350: 4669 6c74 6572 456e 6162 6c65 6427 290a  FilterEnabled').
+00054360: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00054370: 2827 5472 6163 6553 616d 706c 696e 6727  ('TraceSampling'
+00054380: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00054390: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000543a0: 7472 6163 655f 7361 6d70 6c69 6e67 203d  trace_sampling =
+000543b0: 206d 2e67 6574 2827 5472 6163 6553 616d   m.get('TraceSam
+000543c0: 706c 696e 6727 290a 2020 2020 2020 2020  pling').        
+000543d0: 6966 206d 2e67 6574 2827 5472 6163 696e  if m.get('Tracin
+000543e0: 6727 2920 6973 206e 6f74 204e 6f6e 653a  g') is not None:
+000543f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00054400: 662e 7472 6163 696e 6720 3d20 6d2e 6765  f.tracing = m.ge
+00054410: 7428 2754 7261 6369 6e67 2729 0a20 2020  t('Tracing').   
+00054420: 2020 2020 2069 6620 6d2e 6765 7428 2757       if m.get('W
+00054430: 6562 4173 7365 6d62 6c79 4669 6c74 6572  ebAssemblyFilter
+00054440: 456e 6162 6c65 6427 2920 6973 206e 6f74  Enabled') is not
+00054450: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00054460: 2020 2073 656c 662e 7765 625f 6173 7365     self.web_asse
+00054470: 6d62 6c79 5f66 696c 7465 725f 656e 6162  mbly_filter_enab
+00054480: 6c65 6420 3d20 6d2e 6765 7428 2757 6562  led = m.get('Web
+00054490: 4173 7365 6d62 6c79 4669 6c74 6572 456e  AssemblyFilterEn
+000544a0: 6162 6c65 6427 290a 2020 2020 2020 2020  abled').        
+000544b0: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+000544c0: 6173 7320 5570 6461 7465 4d65 7368 4665  ass UpdateMeshFe
+000544d0: 6174 7572 6552 6573 706f 6e73 6542 6f64  atureResponseBod
+000544e0: 7928 5465 614d 6f64 656c 293a 0a20 2020  y(TeaModel):.   
+000544f0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00054500: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00054510: 2020 2020 2072 6571 7565 7374 5f69 643a       request_id:
+00054520: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+00054530: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
+00054540: 2e72 6571 7565 7374 5f69 6420 3d20 7265  .request_id = re
+00054550: 7175 6573 745f 6964 0a0a 2020 2020 6465  quest_id..    de
+00054560: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+00054570: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+00054580: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+00054590: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+000545a0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+000545b0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+000545c0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+000545d0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000545e0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+000545f0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+00054600: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+00054610: 656c 662e 7265 7175 6573 745f 6964 2069  elf.request_id i
+00054620: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00054630: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00054640: 5265 7175 6573 7449 6427 5d20 3d20 7365  RequestId'] = se
+00054650: 6c66 2e72 6571 7565 7374 5f69 640a 2020  lf.request_id.  
+00054660: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00054670: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00054680: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+00054690: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+000546a0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+000546b0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000546c0: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
+000546d0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000546e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000546f0: 2e72 6571 7565 7374 5f69 6420 3d20 6d2e  .request_id = m.
+00054700: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
+00054710: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00054720: 7365 6c66 0a0a 0a63 6c61 7373 2055 7064  self...class Upd
+00054730: 6174 654d 6573 6846 6561 7475 7265 5265  ateMeshFeatureRe
+00054740: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
+00054750: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00054760: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00054770: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
+00054780: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
+00054790: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+000547a0: 2020 626f 6479 3a20 5570 6461 7465 4d65    body: UpdateMe
+000547b0: 7368 4665 6174 7572 6552 6573 706f 6e73  shFeatureRespons
+000547c0: 6542 6f64 7920 3d20 4e6f 6e65 2c0a 2020  eBody = None,.  
+000547d0: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+000547e0: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+000547f0: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
+00054800: 2e62 6f64 7920 3d20 626f 6479 0a0a 2020  .body = body..  
+00054810: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+00054820: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+00054830: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
+00054840: 6972 6564 2873 656c 662e 6865 6164 6572  ired(self.header
+00054850: 732c 2027 6865 6164 6572 7327 290a 2020  s, 'headers').  
+00054860: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
+00054870: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
+00054880: 662e 626f 6479 2c20 2762 6f64 7927 290a  f.body, 'body').
+00054890: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000548a0: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
+000548b0: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
+000548c0: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
+000548d0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+000548e0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+000548f0: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
+00054900: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+00054910: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00054920: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+00054930: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+00054940: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+00054950: 2020 2020 6966 2073 656c 662e 6865 6164      if self.head
+00054960: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
+00054970: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00054980: 756c 745b 2768 6561 6465 7273 275d 203d  ult['headers'] =
+00054990: 2073 656c 662e 6865 6164 6572 730a 2020   self.headers.  
+000549a0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+000549b0: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
+000549c0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000549d0: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
+000549e0: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
+000549f0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00054a00: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+00054a10: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+00054a20: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+00054a30: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+00054a40: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00054a50: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
+00054a60: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00054a70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00054a80: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
+00054a90: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
+00054aa0: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
+00054ab0: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
+00054ac0: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+00054ad0: 6d70 5f6d 6f64 656c 203d 2055 7064 6174  mp_model = Updat
+00054ae0: 654d 6573 6846 6561 7475 7265 5265 7370  eMeshFeatureResp
+00054af0: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
+00054b00: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+00054b10: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+00054b20: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+00054b30: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00054b40: 2073 656c 660a 0a0a 636c 6173 7320 5570   self...class Up
+00054b50: 6461 7465 4e61 6d65 7370 6163 6553 636f  dateNamespaceSco
+00054b60: 7065 5369 6465 6361 7243 6f6e 6669 6752  peSidecarConfigR
+00054b70: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
+00054b80: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00054b90: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00054ba0: 2c0a 2020 2020 2020 2020 6578 636c 7564  ,.        exclud
+00054bb0: 655f 6970 7261 6e67 6573 3a20 7374 7220  e_ipranges: str 
+00054bc0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00054bd0: 6578 636c 7564 655f 696e 626f 756e 645f  exclude_inbound_
+00054be0: 706f 7274 733a 2073 7472 203d 204e 6f6e  ports: str = Non
+00054bf0: 652c 0a20 2020 2020 2020 2065 7863 6c75  e,.        exclu
+00054c00: 6465 5f6f 7574 626f 756e 645f 706f 7274  de_outbound_port
+00054c10: 733a 2073 7472 203d 204e 6f6e 652c 0a20  s: str = None,. 
+00054c20: 2020 2020 2020 2069 6e63 6c75 6465 5f69         include_i
+00054c30: 7072 616e 6765 733a 2073 7472 203d 204e  pranges: str = N
+00054c40: 6f6e 652c 0a20 2020 2020 2020 2069 6e63  one,.        inc
+00054c50: 6c75 6465 5f69 6e62 6f75 6e64 5f70 6f72  lude_inbound_por
+00054c60: 7473 3a20 7374 7220 3d20 4e6f 6e65 2c0a  ts: str = None,.
+00054c70: 2020 2020 2020 2020 696e 636c 7564 655f          include_
+00054c80: 6f75 7462 6f75 6e64 5f70 6f72 7473 3a20  outbound_ports: 
+00054c90: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00054ca0: 2020 2020 6973 7469 6f5f 646e 7370 726f      istio_dnspro
+00054cb0: 7879 5f65 6e61 626c 6564 3a20 626f 6f6c  xy_enabled: bool
+00054cc0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00054cd0: 206c 6966 6563 7963 6c65 3a20 7374 7220   lifecycle: str 
+00054ce0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00054cf0: 6e61 6d65 7370 6163 653a 2073 7472 203d  namespace: str =
+00054d00: 204e 6f6e 652c 0a20 2020 2020 2020 2070   None,.        p
+00054d10: 726f 7879 5f69 6e69 745f 6370 7572 6573  roxy_init_cpures
+00054d20: 6f75 7263 655f 6c69 6d69 743a 2073 7472  ource_limit: str
+00054d30: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00054d40: 2070 726f 7879 5f69 6e69 745f 6370 7572   proxy_init_cpur
+00054d50: 6573 6f75 7263 655f 7265 7175 6573 743a  esource_request:
+00054d60: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+00054d70: 2020 2020 2070 726f 7879 5f69 6e69 745f       proxy_init_
+00054d80: 6d65 6d6f 7279 5f72 6573 6f75 7263 655f  memory_resource_
+00054d90: 6c69 6d69 743a 2073 7472 203d 204e 6f6e  limit: str = Non
+00054da0: 652c 0a20 2020 2020 2020 2070 726f 7879  e,.        proxy
+00054db0: 5f69 6e69 745f 6d65 6d6f 7279 5f72 6573  _init_memory_res
+00054dc0: 6f75 7263 655f 7265 7175 6573 743a 2073  ource_request: s
+00054dd0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+00054de0: 2020 2073 6572 7669 6365 5f6d 6573 685f     service_mesh_
+00054df0: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+00054e00: 2020 2020 2020 2020 7369 6465 6361 725f          sidecar_
+00054e10: 7072 6f78 795f 6370 7572 6573 6f75 7263  proxy_cpuresourc
+00054e20: 655f 6c69 6d69 743a 2073 7472 203d 204e  e_limit: str = N
+00054e30: 6f6e 652c 0a20 2020 2020 2020 2073 6964  one,.        sid
+00054e40: 6563 6172 5f70 726f 7879 5f63 7075 7265  ecar_proxy_cpure
+00054e50: 736f 7572 6365 5f72 6571 7565 7374 3a20  source_request: 
+00054e60: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00054e70: 2020 2020 7369 6465 6361 725f 7072 6f78      sidecar_prox
+00054e80: 795f 6d65 6d6f 7279 5f72 6573 6f75 7263  y_memory_resourc
+00054e90: 655f 6c69 6d69 743a 2073 7472 203d 204e  e_limit: str = N
+00054ea0: 6f6e 652c 0a20 2020 2020 2020 2073 6964  one,.        sid
+00054eb0: 6563 6172 5f70 726f 7879 5f6d 656d 6f72  ecar_proxy_memor
+00054ec0: 795f 7265 736f 7572 6365 5f72 6571 7565  y_resource_reque
+00054ed0: 7374 3a20 7374 7220 3d20 4e6f 6e65 2c0a  st: str = None,.
+00054ee0: 2020 2020 2020 2020 7465 726d 696e 6174          terminat
+00054ef0: 696f 6e5f 6472 6169 6e5f 6475 7261 7469  ion_drain_durati
+00054f00: 6f6e 3a20 7374 7220 3d20 4e6f 6e65 2c0a  on: str = None,.
+00054f10: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+00054f20: 656c 662e 6578 636c 7564 655f 6970 7261  elf.exclude_ipra
+00054f30: 6e67 6573 203d 2065 7863 6c75 6465 5f69  nges = exclude_i
+00054f40: 7072 616e 6765 730a 2020 2020 2020 2020  pranges.        
+00054f50: 7365 6c66 2e65 7863 6c75 6465 5f69 6e62  self.exclude_inb
+00054f60: 6f75 6e64 5f70 6f72 7473 203d 2065 7863  ound_ports = exc
+00054f70: 6c75 6465 5f69 6e62 6f75 6e64 5f70 6f72  lude_inbound_por
+00054f80: 7473 0a20 2020 2020 2020 2073 656c 662e  ts.        self.
+00054f90: 6578 636c 7564 655f 6f75 7462 6f75 6e64  exclude_outbound
+00054fa0: 5f70 6f72 7473 203d 2065 7863 6c75 6465  _ports = exclude
+00054fb0: 5f6f 7574 626f 756e 645f 706f 7274 730a  _outbound_ports.
+00054fc0: 2020 2020 2020 2020 7365 6c66 2e69 6e63          self.inc
+00054fd0: 6c75 6465 5f69 7072 616e 6765 7320 3d20  lude_ipranges = 
+00054fe0: 696e 636c 7564 655f 6970 7261 6e67 6573  include_ipranges
+00054ff0: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
+00055000: 636c 7564 655f 696e 626f 756e 645f 706f  clude_inbound_po
+00055010: 7274 7320 3d20 696e 636c 7564 655f 696e  rts = include_in
+00055020: 626f 756e 645f 706f 7274 730a 2020 2020  bound_ports.    
+00055030: 2020 2020 7365 6c66 2e69 6e63 6c75 6465      self.include
+00055040: 5f6f 7574 626f 756e 645f 706f 7274 7320  _outbound_ports 
+00055050: 3d20 696e 636c 7564 655f 6f75 7462 6f75  = include_outbou
+00055060: 6e64 5f70 6f72 7473 0a20 2020 2020 2020  nd_ports.       
+00055070: 2073 656c 662e 6973 7469 6f5f 646e 7370   self.istio_dnsp
+00055080: 726f 7879 5f65 6e61 626c 6564 203d 2069  roxy_enabled = i
+00055090: 7374 696f 5f64 6e73 7072 6f78 795f 656e  stio_dnsproxy_en
+000550a0: 6162 6c65 640a 2020 2020 2020 2020 7365  abled.        se
+000550b0: 6c66 2e6c 6966 6563 7963 6c65 203d 206c  lf.lifecycle = l
+000550c0: 6966 6563 7963 6c65 0a20 2020 2020 2020  ifecycle.       
+000550d0: 2073 656c 662e 6e61 6d65 7370 6163 6520   self.namespace 
+000550e0: 3d20 6e61 6d65 7370 6163 650a 2020 2020  = namespace.    
+000550f0: 2020 2020 7365 6c66 2e70 726f 7879 5f69      self.proxy_i
+00055100: 6e69 745f 6370 7572 6573 6f75 7263 655f  nit_cpuresource_
+00055110: 6c69 6d69 7420 3d20 7072 6f78 795f 696e  limit = proxy_in
+00055120: 6974 5f63 7075 7265 736f 7572 6365 5f6c  it_cpuresource_l
+00055130: 696d 6974 0a20 2020 2020 2020 2073 656c  imit.        sel
+00055140: 662e 7072 6f78 795f 696e 6974 5f63 7075  f.proxy_init_cpu
+00055150: 7265 736f 7572 6365 5f72 6571 7565 7374  resource_request
+00055160: 203d 2070 726f 7879 5f69 6e69 745f 6370   = proxy_init_cp
+00055170: 7572 6573 6f75 7263 655f 7265 7175 6573  uresource_reques
+00055180: 740a 2020 2020 2020 2020 7365 6c66 2e70  t.        self.p
+00055190: 726f 7879 5f69 6e69 745f 6d65 6d6f 7279  roxy_init_memory
+000551a0: 5f72 6573 6f75 7263 655f 6c69 6d69 7420  _resource_limit 
+000551b0: 3d20 7072 6f78 795f 696e 6974 5f6d 656d  = proxy_init_mem
+000551c0: 6f72 795f 7265 736f 7572 6365 5f6c 696d  ory_resource_lim
+000551d0: 6974 0a20 2020 2020 2020 2073 656c 662e  it.        self.
+000551e0: 7072 6f78 795f 696e 6974 5f6d 656d 6f72  proxy_init_memor
+000551f0: 795f 7265 736f 7572 6365 5f72 6571 7565  y_resource_reque
+00055200: 7374 203d 2070 726f 7879 5f69 6e69 745f  st = proxy_init_
+00055210: 6d65 6d6f 7279 5f72 6573 6f75 7263 655f  memory_resource_
+00055220: 7265 7175 6573 740a 2020 2020 2020 2020  request.        
+00055230: 7365 6c66 2e73 6572 7669 6365 5f6d 6573  self.service_mes
+00055240: 685f 6964 203d 2073 6572 7669 6365 5f6d  h_id = service_m
+00055250: 6573 685f 6964 0a20 2020 2020 2020 2073  esh_id.        s
+00055260: 656c 662e 7369 6465 6361 725f 7072 6f78  elf.sidecar_prox
+00055270: 795f 6370 7572 6573 6f75 7263 655f 6c69  y_cpuresource_li
+00055280: 6d69 7420 3d20 7369 6465 6361 725f 7072  mit = sidecar_pr
+00055290: 6f78 795f 6370 7572 6573 6f75 7263 655f  oxy_cpuresource_
+000552a0: 6c69 6d69 740a 2020 2020 2020 2020 7365  limit.        se
+000552b0: 6c66 2e73 6964 6563 6172 5f70 726f 7879  lf.sidecar_proxy
+000552c0: 5f63 7075 7265 736f 7572 6365 5f72 6571  _cpuresource_req
+000552d0: 7565 7374 203d 2073 6964 6563 6172 5f70  uest = sidecar_p
+000552e0: 726f 7879 5f63 7075 7265 736f 7572 6365  roxy_cpuresource
+000552f0: 5f72 6571 7565 7374 0a20 2020 2020 2020  _request.       
+00055300: 2073 656c 662e 7369 6465 6361 725f 7072   self.sidecar_pr
+00055310: 6f78 795f 6d65 6d6f 7279 5f72 6573 6f75  oxy_memory_resou
+00055320: 7263 655f 6c69 6d69 7420 3d20 7369 6465  rce_limit = side
+00055330: 6361 725f 7072 6f78 795f 6d65 6d6f 7279  car_proxy_memory
+00055340: 5f72 6573 6f75 7263 655f 6c69 6d69 740a  _resource_limit.
+00055350: 2020 2020 2020 2020 7365 6c66 2e73 6964          self.sid
+00055360: 6563 6172 5f70 726f 7879 5f6d 656d 6f72  ecar_proxy_memor
+00055370: 795f 7265 736f 7572 6365 5f72 6571 7565  y_resource_reque
+00055380: 7374 203d 2073 6964 6563 6172 5f70 726f  st = sidecar_pro
+00055390: 7879 5f6d 656d 6f72 795f 7265 736f 7572  xy_memory_resour
+000553a0: 6365 5f72 6571 7565 7374 0a20 2020 2020  ce_request.     
+000553b0: 2020 2073 656c 662e 7465 726d 696e 6174     self.terminat
+000553c0: 696f 6e5f 6472 6169 6e5f 6475 7261 7469  ion_drain_durati
+000553d0: 6f6e 203d 2074 6572 6d69 6e61 7469 6f6e  on = termination
+000553e0: 5f64 7261 696e 5f64 7572 6174 696f 6e0a  _drain_duration.
+000553f0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00055400: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00055410: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+00055420: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+00055430: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+00055440: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+00055450: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+00055460: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00055470: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+00055480: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+00055490: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+000554a0: 2020 2069 6620 7365 6c66 2e65 7863 6c75     if self.exclu
+000554b0: 6465 5f69 7072 616e 6765 7320 6973 206e  de_ipranges is n
+000554c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000554d0: 2020 2020 2072 6573 756c 745b 2745 7863       result['Exc
+000554e0: 6c75 6465 4950 5261 6e67 6573 275d 203d  ludeIPRanges'] =
+000554f0: 2073 656c 662e 6578 636c 7564 655f 6970   self.exclude_ip
+00055500: 7261 6e67 6573 0a20 2020 2020 2020 2069  ranges.        i
+00055510: 6620 7365 6c66 2e65 7863 6c75 6465 5f69  f self.exclude_i
+00055520: 6e62 6f75 6e64 5f70 6f72 7473 2069 7320  nbound_ports is 
+00055530: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00055540: 2020 2020 2020 7265 7375 6c74 5b27 4578        result['Ex
+00055550: 636c 7564 6549 6e62 6f75 6e64 506f 7274  cludeInboundPort
+00055560: 7327 5d20 3d20 7365 6c66 2e65 7863 6c75  s'] = self.exclu
+00055570: 6465 5f69 6e62 6f75 6e64 5f70 6f72 7473  de_inbound_ports
+00055580: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00055590: 2e65 7863 6c75 6465 5f6f 7574 626f 756e  .exclude_outboun
+000555a0: 645f 706f 7274 7320 6973 206e 6f74 204e  d_ports is not N
+000555b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000555c0: 2072 6573 756c 745b 2745 7863 6c75 6465   result['Exclude
+000555d0: 4f75 7462 6f75 6e64 506f 7274 7327 5d20  OutboundPorts'] 
+000555e0: 3d20 7365 6c66 2e65 7863 6c75 6465 5f6f  = self.exclude_o
+000555f0: 7574 626f 756e 645f 706f 7274 730a 2020  utbound_ports.  
+00055600: 2020 2020 2020 6966 2073 656c 662e 696e        if self.in
+00055610: 636c 7564 655f 6970 7261 6e67 6573 2069  clude_ipranges i
+00055620: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00055630: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00055640: 496e 636c 7564 6549 5052 616e 6765 7327  IncludeIPRanges'
+00055650: 5d20 3d20 7365 6c66 2e69 6e63 6c75 6465  ] = self.include
+00055660: 5f69 7072 616e 6765 730a 2020 2020 2020  _ipranges.      
+00055670: 2020 6966 2073 656c 662e 696e 636c 7564    if self.includ
+00055680: 655f 696e 626f 756e 645f 706f 7274 7320  e_inbound_ports 
+00055690: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000556a0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000556b0: 2749 6e63 6c75 6465 496e 626f 756e 6450  'IncludeInboundP
+000556c0: 6f72 7473 275d 203d 2073 656c 662e 696e  orts'] = self.in
+000556d0: 636c 7564 655f 696e 626f 756e 645f 706f  clude_inbound_po
+000556e0: 7274 730a 2020 2020 2020 2020 6966 2073  rts.        if s
+000556f0: 656c 662e 696e 636c 7564 655f 6f75 7462  elf.include_outb
+00055700: 6f75 6e64 5f70 6f72 7473 2069 7320 6e6f  ound_ports is no
+00055710: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00055720: 2020 2020 7265 7375 6c74 5b27 496e 636c      result['Incl
+00055730: 7564 654f 7574 626f 756e 6450 6f72 7473  udeOutboundPorts
+00055740: 275d 203d 2073 656c 662e 696e 636c 7564  '] = self.includ
+00055750: 655f 6f75 7462 6f75 6e64 5f70 6f72 7473  e_outbound_ports
+00055760: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00055770: 2e69 7374 696f 5f64 6e73 7072 6f78 795f  .istio_dnsproxy_
+00055780: 656e 6162 6c65 6420 6973 206e 6f74 204e  enabled is not N
+00055790: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000557a0: 2072 6573 756c 745b 2749 7374 696f 444e   result['IstioDN
+000557b0: 5350 726f 7879 456e 6162 6c65 6427 5d20  SProxyEnabled'] 
+000557c0: 3d20 7365 6c66 2e69 7374 696f 5f64 6e73  = self.istio_dns
+000557d0: 7072 6f78 795f 656e 6162 6c65 640a 2020  proxy_enabled.  
+000557e0: 2020 2020 2020 6966 2073 656c 662e 6c69        if self.li
+000557f0: 6665 6379 636c 6520 6973 206e 6f74 204e  fecycle is not N
+00055800: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00055810: 2072 6573 756c 745b 274c 6966 6563 7963   result['Lifecyc
+00055820: 6c65 275d 203d 2073 656c 662e 6c69 6665  le'] = self.life
+00055830: 6379 636c 650a 2020 2020 2020 2020 6966  cycle.        if
+00055840: 2073 656c 662e 6e61 6d65 7370 6163 6520   self.namespace 
+00055850: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00055860: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00055870: 274e 616d 6573 7061 6365 275d 203d 2073  'Namespace'] = s
+00055880: 656c 662e 6e61 6d65 7370 6163 650a 2020  elf.namespace.  
+00055890: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+000558a0: 6f78 795f 696e 6974 5f63 7075 7265 736f  oxy_init_cpureso
+000558b0: 7572 6365 5f6c 696d 6974 2069 7320 6e6f  urce_limit is no
+000558c0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000558d0: 2020 2020 7265 7375 6c74 5b27 5072 6f78      result['Prox
+000558e0: 7949 6e69 7443 5055 5265 736f 7572 6365  yInitCPUResource
+000558f0: 4c69 6d69 7427 5d20 3d20 7365 6c66 2e70  Limit'] = self.p
+00055900: 726f 7879 5f69 6e69 745f 6370 7572 6573  roxy_init_cpures
+00055910: 6f75 7263 655f 6c69 6d69 740a 2020 2020  ource_limit.    
+00055920: 2020 2020 6966 2073 656c 662e 7072 6f78      if self.prox
+00055930: 795f 696e 6974 5f63 7075 7265 736f 7572  y_init_cpuresour
+00055940: 6365 5f72 6571 7565 7374 2069 7320 6e6f  ce_request is no
+00055950: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00055960: 2020 2020 7265 7375 6c74 5b27 5072 6f78      result['Prox
+00055970: 7949 6e69 7443 5055 5265 736f 7572 6365  yInitCPUResource
+00055980: 5265 7175 6573 7427 5d20 3d20 7365 6c66  Request'] = self
+00055990: 2e70 726f 7879 5f69 6e69 745f 6370 7572  .proxy_init_cpur
+000559a0: 6573 6f75 7263 655f 7265 7175 6573 740a  esource_request.
+000559b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000559c0: 7072 6f78 795f 696e 6974 5f6d 656d 6f72  proxy_init_memor
+000559d0: 795f 7265 736f 7572 6365 5f6c 696d 6974  y_resource_limit
+000559e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000559f0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00055a00: 5b27 5072 6f78 7949 6e69 744d 656d 6f72  ['ProxyInitMemor
+00055a10: 7952 6573 6f75 7263 654c 696d 6974 275d  yResourceLimit']
+00055a20: 203d 2073 656c 662e 7072 6f78 795f 696e   = self.proxy_in
+00055a30: 6974 5f6d 656d 6f72 795f 7265 736f 7572  it_memory_resour
+00055a40: 6365 5f6c 696d 6974 0a20 2020 2020 2020  ce_limit.       
+00055a50: 2069 6620 7365 6c66 2e70 726f 7879 5f69   if self.proxy_i
+00055a60: 6e69 745f 6d65 6d6f 7279 5f72 6573 6f75  nit_memory_resou
+00055a70: 7263 655f 7265 7175 6573 7420 6973 206e  rce_request is n
+00055a80: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00055a90: 2020 2020 2072 6573 756c 745b 2750 726f       result['Pro
+00055aa0: 7879 496e 6974 4d65 6d6f 7279 5265 736f  xyInitMemoryReso
+00055ab0: 7572 6365 5265 7175 6573 7427 5d20 3d20  urceRequest'] = 
+00055ac0: 7365 6c66 2e70 726f 7879 5f69 6e69 745f  self.proxy_init_
+00055ad0: 6d65 6d6f 7279 5f72 6573 6f75 7263 655f  memory_resource_
+00055ae0: 7265 7175 6573 740a 2020 2020 2020 2020  request.        
+00055af0: 6966 2073 656c 662e 7365 7276 6963 655f  if self.service_
+00055b00: 6d65 7368 5f69 6420 6973 206e 6f74 204e  mesh_id is not N
+00055b10: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00055b20: 2072 6573 756c 745b 2753 6572 7669 6365   result['Service
+00055b30: 4d65 7368 4964 275d 203d 2073 656c 662e  MeshId'] = self.
+00055b40: 7365 7276 6963 655f 6d65 7368 5f69 640a  service_mesh_id.
+00055b50: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00055b60: 7369 6465 6361 725f 7072 6f78 795f 6370  sidecar_proxy_cp
+00055b70: 7572 6573 6f75 7263 655f 6c69 6d69 7420  uresource_limit 
+00055b80: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00055b90: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00055ba0: 2753 6964 6563 6172 5072 6f78 7943 5055  'SidecarProxyCPU
+00055bb0: 5265 736f 7572 6365 4c69 6d69 7427 5d20  ResourceLimit'] 
+00055bc0: 3d20 7365 6c66 2e73 6964 6563 6172 5f70  = self.sidecar_p
+00055bd0: 726f 7879 5f63 7075 7265 736f 7572 6365  roxy_cpuresource
+00055be0: 5f6c 696d 6974 0a20 2020 2020 2020 2069  _limit.        i
+00055bf0: 6620 7365 6c66 2e73 6964 6563 6172 5f70  f self.sidecar_p
+00055c00: 726f 7879 5f63 7075 7265 736f 7572 6365  roxy_cpuresource
+00055c10: 5f72 6571 7565 7374 2069 7320 6e6f 7420  _request is not 
+00055c20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00055c30: 2020 7265 7375 6c74 5b27 5369 6465 6361    result['Sideca
+00055c40: 7250 726f 7879 4350 5552 6573 6f75 7263  rProxyCPUResourc
+00055c50: 6552 6571 7565 7374 275d 203d 2073 656c  eRequest'] = sel
+00055c60: 662e 7369 6465 6361 725f 7072 6f78 795f  f.sidecar_proxy_
+00055c70: 6370 7572 6573 6f75 7263 655f 7265 7175  cpuresource_requ
+00055c80: 6573 740a 2020 2020 2020 2020 6966 2073  est.        if s
+00055c90: 656c 662e 7369 6465 6361 725f 7072 6f78  elf.sidecar_prox
+00055ca0: 795f 6d65 6d6f 7279 5f72 6573 6f75 7263  y_memory_resourc
+00055cb0: 655f 6c69 6d69 7420 6973 206e 6f74 204e  e_limit is not N
+00055cc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00055cd0: 2072 6573 756c 745b 2753 6964 6563 6172   result['Sidecar
+00055ce0: 5072 6f78 794d 656d 6f72 7952 6573 6f75  ProxyMemoryResou
+00055cf0: 7263 654c 696d 6974 275d 203d 2073 656c  rceLimit'] = sel
+00055d00: 662e 7369 6465 6361 725f 7072 6f78 795f  f.sidecar_proxy_
+00055d10: 6d65 6d6f 7279 5f72 6573 6f75 7263 655f  memory_resource_
+00055d20: 6c69 6d69 740a 2020 2020 2020 2020 6966  limit.        if
 00055d30: 2073 656c 662e 7369 6465 6361 725f 7072   self.sidecar_pr
 00055d40: 6f78 795f 6d65 6d6f 7279 5f72 6573 6f75  oxy_memory_resou
-00055d50: 7263 655f 7265 7175 6573 7420 3d20 7369  rce_request = si
-00055d60: 6465 6361 725f 7072 6f78 795f 6d65 6d6f  decar_proxy_memo
-00055d70: 7279 5f72 6573 6f75 7263 655f 7265 7175  ry_resource_requ
-00055d80: 6573 740a 2020 2020 2020 2020 7365 6c66  est.        self
-00055d90: 2e74 6572 6d69 6e61 7469 6f6e 5f64 7261  .termination_dra
-00055da0: 696e 5f64 7572 6174 696f 6e20 3d20 7465  in_duration = te
-00055db0: 726d 696e 6174 696f 6e5f 6472 6169 6e5f  rmination_drain_
-00055dc0: 6475 7261 7469 6f6e 0a0a 2020 2020 6465  duration..    de
-00055dd0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-00055de0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-00055df0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-00055e00: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-00055e10: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-00055e20: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-00055e30: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-00055e40: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00055e50: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-00055e60: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-00055e70: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-00055e80: 656c 662e 6578 636c 7564 655f 6970 7261  elf.exclude_ipra
-00055e90: 6e67 6573 2069 7320 6e6f 7420 4e6f 6e65  nges is not None
-00055ea0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00055eb0: 7375 6c74 5b27 4578 636c 7564 6549 5052  sult['ExcludeIPR
-00055ec0: 616e 6765 7327 5d20 3d20 7365 6c66 2e65  anges'] = self.e
-00055ed0: 7863 6c75 6465 5f69 7072 616e 6765 730a  xclude_ipranges.
-00055ee0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00055ef0: 6578 636c 7564 655f 696e 626f 756e 645f  exclude_inbound_
-00055f00: 706f 7274 7320 6973 206e 6f74 204e 6f6e  ports is not Non
-00055f10: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00055f20: 6573 756c 745b 2745 7863 6c75 6465 496e  esult['ExcludeIn
-00055f30: 626f 756e 6450 6f72 7473 275d 203d 2073  boundPorts'] = s
-00055f40: 656c 662e 6578 636c 7564 655f 696e 626f  elf.exclude_inbo
-00055f50: 756e 645f 706f 7274 730a 2020 2020 2020  und_ports.      
-00055f60: 2020 6966 2073 656c 662e 6578 636c 7564    if self.exclud
-00055f70: 655f 6f75 7462 6f75 6e64 5f70 6f72 7473  e_outbound_ports
-00055f80: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00055f90: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00055fa0: 5b27 4578 636c 7564 654f 7574 626f 756e  ['ExcludeOutboun
-00055fb0: 6450 6f72 7473 275d 203d 2073 656c 662e  dPorts'] = self.
-00055fc0: 6578 636c 7564 655f 6f75 7462 6f75 6e64  exclude_outbound
-00055fd0: 5f70 6f72 7473 0a20 2020 2020 2020 2069  _ports.        i
-00055fe0: 6620 7365 6c66 2e69 6e63 6c75 6465 5f69  f self.include_i
-00055ff0: 7072 616e 6765 7320 6973 206e 6f74 204e  pranges is not N
-00056000: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00056010: 2072 6573 756c 745b 2749 6e63 6c75 6465   result['Include
-00056020: 4950 5261 6e67 6573 275d 203d 2073 656c  IPRanges'] = sel
-00056030: 662e 696e 636c 7564 655f 6970 7261 6e67  f.include_iprang
-00056040: 6573 0a20 2020 2020 2020 2069 6620 7365  es.        if se
-00056050: 6c66 2e69 6e63 6c75 6465 5f69 6e62 6f75  lf.include_inbou
-00056060: 6e64 5f70 6f72 7473 2069 7320 6e6f 7420  nd_ports is not 
-00056070: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00056080: 2020 7265 7375 6c74 5b27 496e 636c 7564    result['Includ
-00056090: 6549 6e62 6f75 6e64 506f 7274 7327 5d20  eInboundPorts'] 
-000560a0: 3d20 7365 6c66 2e69 6e63 6c75 6465 5f69  = self.include_i
-000560b0: 6e62 6f75 6e64 5f70 6f72 7473 0a20 2020  nbound_ports.   
-000560c0: 2020 2020 2069 6620 7365 6c66 2e69 6e63       if self.inc
-000560d0: 6c75 6465 5f6f 7574 626f 756e 645f 706f  lude_outbound_po
-000560e0: 7274 7320 6973 206e 6f74 204e 6f6e 653a  rts is not None:
-000560f0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00056100: 756c 745b 2749 6e63 6c75 6465 4f75 7462  ult['IncludeOutb
-00056110: 6f75 6e64 506f 7274 7327 5d20 3d20 7365  oundPorts'] = se
-00056120: 6c66 2e69 6e63 6c75 6465 5f6f 7574 626f  lf.include_outbo
-00056130: 756e 645f 706f 7274 730a 2020 2020 2020  und_ports.      
-00056140: 2020 6966 2073 656c 662e 6973 7469 6f5f    if self.istio_
-00056150: 646e 7370 726f 7879 5f65 6e61 626c 6564  dnsproxy_enabled
-00056160: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00056170: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00056180: 5b27 4973 7469 6f44 4e53 5072 6f78 7945  ['IstioDNSProxyE
-00056190: 6e61 626c 6564 275d 203d 2073 656c 662e  nabled'] = self.
-000561a0: 6973 7469 6f5f 646e 7370 726f 7879 5f65  istio_dnsproxy_e
-000561b0: 6e61 626c 6564 0a20 2020 2020 2020 2069  nabled.        i
-000561c0: 6620 7365 6c66 2e6c 6966 6563 7963 6c65  f self.lifecycle
-000561d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000561e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000561f0: 5b27 4c69 6665 6379 636c 6527 5d20 3d20  ['Lifecycle'] = 
-00056200: 7365 6c66 2e6c 6966 6563 7963 6c65 0a20  self.lifecycle. 
-00056210: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
-00056220: 616d 6573 7061 6365 2069 7320 6e6f 7420  amespace is not 
-00056230: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00056240: 2020 7265 7375 6c74 5b27 4e61 6d65 7370    result['Namesp
-00056250: 6163 6527 5d20 3d20 7365 6c66 2e6e 616d  ace'] = self.nam
-00056260: 6573 7061 6365 0a20 2020 2020 2020 2069  espace.        i
-00056270: 6620 7365 6c66 2e70 726f 7879 5f69 6e69  f self.proxy_ini
-00056280: 745f 6370 7572 6573 6f75 7263 655f 6c69  t_cpuresource_li
-00056290: 6d69 7420 6973 206e 6f74 204e 6f6e 653a  mit is not None:
-000562a0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000562b0: 756c 745b 2750 726f 7879 496e 6974 4350  ult['ProxyInitCP
-000562c0: 5552 6573 6f75 7263 654c 696d 6974 275d  UResourceLimit']
-000562d0: 203d 2073 656c 662e 7072 6f78 795f 696e   = self.proxy_in
-000562e0: 6974 5f63 7075 7265 736f 7572 6365 5f6c  it_cpuresource_l
-000562f0: 696d 6974 0a20 2020 2020 2020 2069 6620  imit.        if 
-00056300: 7365 6c66 2e70 726f 7879 5f69 6e69 745f  self.proxy_init_
-00056310: 6370 7572 6573 6f75 7263 655f 7265 7175  cpuresource_requ
-00056320: 6573 7420 6973 206e 6f74 204e 6f6e 653a  est is not None:
-00056330: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00056340: 756c 745b 2750 726f 7879 496e 6974 4350  ult['ProxyInitCP
-00056350: 5552 6573 6f75 7263 6552 6571 7565 7374  UResourceRequest
-00056360: 275d 203d 2073 656c 662e 7072 6f78 795f  '] = self.proxy_
-00056370: 696e 6974 5f63 7075 7265 736f 7572 6365  init_cpuresource
-00056380: 5f72 6571 7565 7374 0a20 2020 2020 2020  _request.       
-00056390: 2069 6620 7365 6c66 2e70 726f 7879 5f69   if self.proxy_i
-000563a0: 6e69 745f 6d65 6d6f 7279 5f72 6573 6f75  nit_memory_resou
-000563b0: 7263 655f 6c69 6d69 7420 6973 206e 6f74  rce_limit is not
-000563c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000563d0: 2020 2072 6573 756c 745b 2750 726f 7879     result['Proxy
-000563e0: 496e 6974 4d65 6d6f 7279 5265 736f 7572  InitMemoryResour
-000563f0: 6365 4c69 6d69 7427 5d20 3d20 7365 6c66  ceLimit'] = self
-00056400: 2e70 726f 7879 5f69 6e69 745f 6d65 6d6f  .proxy_init_memo
-00056410: 7279 5f72 6573 6f75 7263 655f 6c69 6d69  ry_resource_limi
-00056420: 740a 2020 2020 2020 2020 6966 2073 656c  t.        if sel
-00056430: 662e 7072 6f78 795f 696e 6974 5f6d 656d  f.proxy_init_mem
-00056440: 6f72 795f 7265 736f 7572 6365 5f72 6571  ory_resource_req
-00056450: 7565 7374 2069 7320 6e6f 7420 4e6f 6e65  uest is not None
-00056460: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00056470: 7375 6c74 5b27 5072 6f78 7949 6e69 744d  sult['ProxyInitM
-00056480: 656d 6f72 7952 6573 6f75 7263 6552 6571  emoryResourceReq
-00056490: 7565 7374 275d 203d 2073 656c 662e 7072  uest'] = self.pr
-000564a0: 6f78 795f 696e 6974 5f6d 656d 6f72 795f  oxy_init_memory_
-000564b0: 7265 736f 7572 6365 5f72 6571 7565 7374  resource_request
-000564c0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000564d0: 2e73 6572 7669 6365 5f6d 6573 685f 6964  .service_mesh_id
-000564e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000564f0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00056500: 5b27 5365 7276 6963 654d 6573 6849 6427  ['ServiceMeshId'
-00056510: 5d20 3d20 7365 6c66 2e73 6572 7669 6365  ] = self.service
-00056520: 5f6d 6573 685f 6964 0a20 2020 2020 2020  _mesh_id.       
-00056530: 2069 6620 7365 6c66 2e73 6964 6563 6172   if self.sidecar
-00056540: 5f70 726f 7879 5f63 7075 7265 736f 7572  _proxy_cpuresour
-00056550: 6365 5f6c 696d 6974 2069 7320 6e6f 7420  ce_limit is not 
-00056560: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00056570: 2020 7265 7375 6c74 5b27 5369 6465 6361    result['Sideca
-00056580: 7250 726f 7879 4350 5552 6573 6f75 7263  rProxyCPUResourc
-00056590: 654c 696d 6974 275d 203d 2073 656c 662e  eLimit'] = self.
-000565a0: 7369 6465 6361 725f 7072 6f78 795f 6370  sidecar_proxy_cp
-000565b0: 7572 6573 6f75 7263 655f 6c69 6d69 740a  uresource_limit.
-000565c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000565d0: 7369 6465 6361 725f 7072 6f78 795f 6370  sidecar_proxy_cp
-000565e0: 7572 6573 6f75 7263 655f 7265 7175 6573  uresource_reques
-000565f0: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
-00056600: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00056610: 745b 2753 6964 6563 6172 5072 6f78 7943  t['SidecarProxyC
-00056620: 5055 5265 736f 7572 6365 5265 7175 6573  PUResourceReques
-00056630: 7427 5d20 3d20 7365 6c66 2e73 6964 6563  t'] = self.sidec
-00056640: 6172 5f70 726f 7879 5f63 7075 7265 736f  ar_proxy_cpureso
-00056650: 7572 6365 5f72 6571 7565 7374 0a20 2020  urce_request.   
-00056660: 2020 2020 2069 6620 7365 6c66 2e73 6964       if self.sid
-00056670: 6563 6172 5f70 726f 7879 5f6d 656d 6f72  ecar_proxy_memor
-00056680: 795f 7265 736f 7572 6365 5f6c 696d 6974  y_resource_limit
-00056690: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000566a0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000566b0: 5b27 5369 6465 6361 7250 726f 7879 4d65  ['SidecarProxyMe
-000566c0: 6d6f 7279 5265 736f 7572 6365 4c69 6d69  moryResourceLimi
-000566d0: 7427 5d20 3d20 7365 6c66 2e73 6964 6563  t'] = self.sidec
-000566e0: 6172 5f70 726f 7879 5f6d 656d 6f72 795f  ar_proxy_memory_
-000566f0: 7265 736f 7572 6365 5f6c 696d 6974 0a20  resource_limit. 
-00056700: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00056710: 6964 6563 6172 5f70 726f 7879 5f6d 656d  idecar_proxy_mem
-00056720: 6f72 795f 7265 736f 7572 6365 5f72 6571  ory_resource_req
-00056730: 7565 7374 2069 7320 6e6f 7420 4e6f 6e65  uest is not None
-00056740: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00056750: 7375 6c74 5b27 5369 6465 6361 7250 726f  sult['SidecarPro
-00056760: 7879 4d65 6d6f 7279 5265 736f 7572 6365  xyMemoryResource
-00056770: 5265 7175 6573 7427 5d20 3d20 7365 6c66  Request'] = self
-00056780: 2e73 6964 6563 6172 5f70 726f 7879 5f6d  .sidecar_proxy_m
-00056790: 656d 6f72 795f 7265 736f 7572 6365 5f72  emory_resource_r
-000567a0: 6571 7565 7374 0a20 2020 2020 2020 2069  equest.        i
-000567b0: 6620 7365 6c66 2e74 6572 6d69 6e61 7469  f self.terminati
-000567c0: 6f6e 5f64 7261 696e 5f64 7572 6174 696f  on_drain_duratio
-000567d0: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
-000567e0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000567f0: 745b 2754 6572 6d69 6e61 7469 6f6e 4472  t['TerminationDr
-00056800: 6169 6e44 7572 6174 696f 6e27 5d20 3d20  ainDuration'] = 
-00056810: 7365 6c66 2e74 6572 6d69 6e61 7469 6f6e  self.termination
-00056820: 5f64 7261 696e 5f64 7572 6174 696f 6e0a  _drain_duration.
-00056830: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00056840: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-00056850: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
-00056860: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
-00056870: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-00056880: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00056890: 6620 6d2e 6765 7428 2745 7863 6c75 6465  f m.get('Exclude
-000568a0: 4950 5261 6e67 6573 2729 2069 7320 6e6f  IPRanges') is no
-000568b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000568c0: 2020 2020 7365 6c66 2e65 7863 6c75 6465      self.exclude
-000568d0: 5f69 7072 616e 6765 7320 3d20 6d2e 6765  _ipranges = m.ge
-000568e0: 7428 2745 7863 6c75 6465 4950 5261 6e67  t('ExcludeIPRang
-000568f0: 6573 2729 0a20 2020 2020 2020 2069 6620  es').        if 
-00056900: 6d2e 6765 7428 2745 7863 6c75 6465 496e  m.get('ExcludeIn
-00056910: 626f 756e 6450 6f72 7473 2729 2069 7320  boundPorts') is 
-00056920: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00056930: 2020 2020 2020 7365 6c66 2e65 7863 6c75        self.exclu
-00056940: 6465 5f69 6e62 6f75 6e64 5f70 6f72 7473  de_inbound_ports
-00056950: 203d 206d 2e67 6574 2827 4578 636c 7564   = m.get('Exclud
-00056960: 6549 6e62 6f75 6e64 506f 7274 7327 290a  eInboundPorts').
-00056970: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00056980: 2827 4578 636c 7564 654f 7574 626f 756e  ('ExcludeOutboun
-00056990: 6450 6f72 7473 2729 2069 7320 6e6f 7420  dPorts') is not 
-000569a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000569b0: 2020 7365 6c66 2e65 7863 6c75 6465 5f6f    self.exclude_o
-000569c0: 7574 626f 756e 645f 706f 7274 7320 3d20  utbound_ports = 
-000569d0: 6d2e 6765 7428 2745 7863 6c75 6465 4f75  m.get('ExcludeOu
-000569e0: 7462 6f75 6e64 506f 7274 7327 290a 2020  tboundPorts').  
-000569f0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00056a00: 496e 636c 7564 6549 5052 616e 6765 7327  IncludeIPRanges'
-00056a10: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00056a20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00056a30: 696e 636c 7564 655f 6970 7261 6e67 6573  include_ipranges
-00056a40: 203d 206d 2e67 6574 2827 496e 636c 7564   = m.get('Includ
-00056a50: 6549 5052 616e 6765 7327 290a 2020 2020  eIPRanges').    
-00056a60: 2020 2020 6966 206d 2e67 6574 2827 496e      if m.get('In
-00056a70: 636c 7564 6549 6e62 6f75 6e64 506f 7274  cludeInboundPort
-00056a80: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
-00056a90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00056aa0: 662e 696e 636c 7564 655f 696e 626f 756e  f.include_inboun
-00056ab0: 645f 706f 7274 7320 3d20 6d2e 6765 7428  d_ports = m.get(
-00056ac0: 2749 6e63 6c75 6465 496e 626f 756e 6450  'IncludeInboundP
-00056ad0: 6f72 7473 2729 0a20 2020 2020 2020 2069  orts').        i
-00056ae0: 6620 6d2e 6765 7428 2749 6e63 6c75 6465  f m.get('Include
-00056af0: 4f75 7462 6f75 6e64 506f 7274 7327 2920  OutboundPorts') 
-00056b00: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00056b10: 2020 2020 2020 2020 2073 656c 662e 696e           self.in
-00056b20: 636c 7564 655f 6f75 7462 6f75 6e64 5f70  clude_outbound_p
-00056b30: 6f72 7473 203d 206d 2e67 6574 2827 496e  orts = m.get('In
-00056b40: 636c 7564 654f 7574 626f 756e 6450 6f72  cludeOutboundPor
-00056b50: 7473 2729 0a20 2020 2020 2020 2069 6620  ts').        if 
-00056b60: 6d2e 6765 7428 2749 7374 696f 444e 5350  m.get('IstioDNSP
-00056b70: 726f 7879 456e 6162 6c65 6427 2920 6973  roxyEnabled') is
-00056b80: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00056b90: 2020 2020 2020 2073 656c 662e 6973 7469         self.isti
-00056ba0: 6f5f 646e 7370 726f 7879 5f65 6e61 626c  o_dnsproxy_enabl
-00056bb0: 6564 203d 206d 2e67 6574 2827 4973 7469  ed = m.get('Isti
-00056bc0: 6f44 4e53 5072 6f78 7945 6e61 626c 6564  oDNSProxyEnabled
-00056bd0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00056be0: 6765 7428 274c 6966 6563 7963 6c65 2729  get('Lifecycle')
-00056bf0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00056c00: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
-00056c10: 6966 6563 7963 6c65 203d 206d 2e67 6574  ifecycle = m.get
-00056c20: 2827 4c69 6665 6379 636c 6527 290a 2020  ('Lifecycle').  
-00056c30: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00056c40: 4e61 6d65 7370 6163 6527 2920 6973 206e  Namespace') is n
-00056c50: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00056c60: 2020 2020 2073 656c 662e 6e61 6d65 7370       self.namesp
-00056c70: 6163 6520 3d20 6d2e 6765 7428 274e 616d  ace = m.get('Nam
-00056c80: 6573 7061 6365 2729 0a20 2020 2020 2020  espace').       
-00056c90: 2069 6620 6d2e 6765 7428 2750 726f 7879   if m.get('Proxy
-00056ca0: 496e 6974 4350 5552 6573 6f75 7263 654c  InitCPUResourceL
-00056cb0: 696d 6974 2729 2069 7320 6e6f 7420 4e6f  imit') is not No
-00056cc0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00056cd0: 7365 6c66 2e70 726f 7879 5f69 6e69 745f  self.proxy_init_
-00056ce0: 6370 7572 6573 6f75 7263 655f 6c69 6d69  cpuresource_limi
-00056cf0: 7420 3d20 6d2e 6765 7428 2750 726f 7879  t = m.get('Proxy
-00056d00: 496e 6974 4350 5552 6573 6f75 7263 654c  InitCPUResourceL
-00056d10: 696d 6974 2729 0a20 2020 2020 2020 2069  imit').        i
-00056d20: 6620 6d2e 6765 7428 2750 726f 7879 496e  f m.get('ProxyIn
-00056d30: 6974 4350 5552 6573 6f75 7263 6552 6571  itCPUResourceReq
-00056d40: 7565 7374 2729 2069 7320 6e6f 7420 4e6f  uest') is not No
-00056d50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00056d60: 7365 6c66 2e70 726f 7879 5f69 6e69 745f  self.proxy_init_
-00056d70: 6370 7572 6573 6f75 7263 655f 7265 7175  cpuresource_requ
-00056d80: 6573 7420 3d20 6d2e 6765 7428 2750 726f  est = m.get('Pro
-00056d90: 7879 496e 6974 4350 5552 6573 6f75 7263  xyInitCPUResourc
-00056da0: 6552 6571 7565 7374 2729 0a20 2020 2020  eRequest').     
-00056db0: 2020 2069 6620 6d2e 6765 7428 2750 726f     if m.get('Pro
-00056dc0: 7879 496e 6974 4d65 6d6f 7279 5265 736f  xyInitMemoryReso
-00056dd0: 7572 6365 4c69 6d69 7427 2920 6973 206e  urceLimit') is n
-00056de0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00056df0: 2020 2020 2073 656c 662e 7072 6f78 795f       self.proxy_
-00056e00: 696e 6974 5f6d 656d 6f72 795f 7265 736f  init_memory_reso
-00056e10: 7572 6365 5f6c 696d 6974 203d 206d 2e67  urce_limit = m.g
-00056e20: 6574 2827 5072 6f78 7949 6e69 744d 656d  et('ProxyInitMem
-00056e30: 6f72 7952 6573 6f75 7263 654c 696d 6974  oryResourceLimit
-00056e40: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00056e50: 6765 7428 2750 726f 7879 496e 6974 4d65  get('ProxyInitMe
-00056e60: 6d6f 7279 5265 736f 7572 6365 5265 7175  moryResourceRequ
-00056e70: 6573 7427 2920 6973 206e 6f74 204e 6f6e  est') is not Non
-00056e80: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00056e90: 656c 662e 7072 6f78 795f 696e 6974 5f6d  elf.proxy_init_m
-00056ea0: 656d 6f72 795f 7265 736f 7572 6365 5f72  emory_resource_r
-00056eb0: 6571 7565 7374 203d 206d 2e67 6574 2827  equest = m.get('
-00056ec0: 5072 6f78 7949 6e69 744d 656d 6f72 7952  ProxyInitMemoryR
-00056ed0: 6573 6f75 7263 6552 6571 7565 7374 2729  esourceRequest')
-00056ee0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00056ef0: 7428 2753 6572 7669 6365 4d65 7368 4964  t('ServiceMeshId
-00056f00: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00056f10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00056f20: 2e73 6572 7669 6365 5f6d 6573 685f 6964  .service_mesh_id
-00056f30: 203d 206d 2e67 6574 2827 5365 7276 6963   = m.get('Servic
-00056f40: 654d 6573 6849 6427 290a 2020 2020 2020  eMeshId').      
-00056f50: 2020 6966 206d 2e67 6574 2827 5369 6465    if m.get('Side
-00056f60: 6361 7250 726f 7879 4350 5552 6573 6f75  carProxyCPUResou
-00056f70: 7263 654c 696d 6974 2729 2069 7320 6e6f  rceLimit') is no
-00056f80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00056f90: 2020 2020 7365 6c66 2e73 6964 6563 6172      self.sidecar
-00056fa0: 5f70 726f 7879 5f63 7075 7265 736f 7572  _proxy_cpuresour
-00056fb0: 6365 5f6c 696d 6974 203d 206d 2e67 6574  ce_limit = m.get
-00056fc0: 2827 5369 6465 6361 7250 726f 7879 4350  ('SidecarProxyCP
-00056fd0: 5552 6573 6f75 7263 654c 696d 6974 2729  UResourceLimit')
-00056fe0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00056ff0: 7428 2753 6964 6563 6172 5072 6f78 7943  t('SidecarProxyC
-00057000: 5055 5265 736f 7572 6365 5265 7175 6573  PUResourceReques
-00057010: 7427 2920 6973 206e 6f74 204e 6f6e 653a  t') is not None:
-00057020: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00057030: 662e 7369 6465 6361 725f 7072 6f78 795f  f.sidecar_proxy_
-00057040: 6370 7572 6573 6f75 7263 655f 7265 7175  cpuresource_requ
-00057050: 6573 7420 3d20 6d2e 6765 7428 2753 6964  est = m.get('Sid
-00057060: 6563 6172 5072 6f78 7943 5055 5265 736f  ecarProxyCPUReso
-00057070: 7572 6365 5265 7175 6573 7427 290a 2020  urceRequest').  
-00057080: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00057090: 5369 6465 6361 7250 726f 7879 4d65 6d6f  SidecarProxyMemo
-000570a0: 7279 5265 736f 7572 6365 4c69 6d69 7427  ryResourceLimit'
-000570b0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000570c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000570d0: 7369 6465 6361 725f 7072 6f78 795f 6d65  sidecar_proxy_me
-000570e0: 6d6f 7279 5f72 6573 6f75 7263 655f 6c69  mory_resource_li
-000570f0: 6d69 7420 3d20 6d2e 6765 7428 2753 6964  mit = m.get('Sid
-00057100: 6563 6172 5072 6f78 794d 656d 6f72 7952  ecarProxyMemoryR
-00057110: 6573 6f75 7263 654c 696d 6974 2729 0a20  esourceLimit'). 
-00057120: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00057130: 2753 6964 6563 6172 5072 6f78 794d 656d  'SidecarProxyMem
-00057140: 6f72 7952 6573 6f75 7263 6552 6571 7565  oryResourceReque
-00057150: 7374 2729 2069 7320 6e6f 7420 4e6f 6e65  st') is not None
-00057160: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00057170: 6c66 2e73 6964 6563 6172 5f70 726f 7879  lf.sidecar_proxy
-00057180: 5f6d 656d 6f72 795f 7265 736f 7572 6365  _memory_resource
-00057190: 5f72 6571 7565 7374 203d 206d 2e67 6574  _request = m.get
-000571a0: 2827 5369 6465 6361 7250 726f 7879 4d65  ('SidecarProxyMe
-000571b0: 6d6f 7279 5265 736f 7572 6365 5265 7175  moryResourceRequ
-000571c0: 6573 7427 290a 2020 2020 2020 2020 6966  est').        if
-000571d0: 206d 2e67 6574 2827 5465 726d 696e 6174   m.get('Terminat
-000571e0: 696f 6e44 7261 696e 4475 7261 7469 6f6e  ionDrainDuration
-000571f0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00057200: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00057210: 2e74 6572 6d69 6e61 7469 6f6e 5f64 7261  .termination_dra
-00057220: 696e 5f64 7572 6174 696f 6e20 3d20 6d2e  in_duration = m.
-00057230: 6765 7428 2754 6572 6d69 6e61 7469 6f6e  get('Termination
-00057240: 4472 6169 6e44 7572 6174 696f 6e27 290a  DrainDuration').
-00057250: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00057260: 656c 660a 0a0a 636c 6173 7320 5570 6461  elf...class Upda
-00057270: 7465 4e61 6d65 7370 6163 6553 636f 7065  teNamespaceScope
-00057280: 5369 6465 6361 7243 6f6e 6669 6752 6573  SidecarConfigRes
-00057290: 706f 6e73 6542 6f64 7928 5465 614d 6f64  ponseBody(TeaMod
-000572a0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-000572b0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-000572c0: 656c 662c 0a20 2020 2020 2020 2072 6571  elf,.        req
-000572d0: 7565 7374 5f69 643a 2073 7472 203d 204e  uest_id: str = N
-000572e0: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-000572f0: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
-00057300: 5f69 6420 3d20 7265 7175 6573 745f 6964  _id = request_id
-00057310: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-00057320: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-00057330: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00057340: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-00057350: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-00057360: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
-00057370: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-00057380: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00057390: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-000573a0: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-000573b0: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-000573c0: 2020 2020 6966 2073 656c 662e 7265 7175      if self.requ
-000573d0: 6573 745f 6964 2069 7320 6e6f 7420 4e6f  est_id is not No
-000573e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000573f0: 7265 7375 6c74 5b27 5265 7175 6573 7449  result['RequestI
-00057400: 6427 5d20 3d20 7365 6c66 2e72 6571 7565  d'] = self.reque
-00057410: 7374 5f69 640a 2020 2020 2020 2020 7265  st_id.        re
-00057420: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-00057430: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-00057440: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
-00057450: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-00057460: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-00057470: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
-00057480: 6571 7565 7374 4964 2729 2069 7320 6e6f  equestId') is no
-00057490: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000574a0: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
-000574b0: 5f69 6420 3d20 6d2e 6765 7428 2752 6571  _id = m.get('Req
-000574c0: 7565 7374 4964 2729 0a20 2020 2020 2020  uestId').       
-000574d0: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-000574e0: 6c61 7373 2055 7064 6174 654e 616d 6573  lass UpdateNames
-000574f0: 7061 6365 5363 6f70 6553 6964 6563 6172  paceScopeSidecar
-00057500: 436f 6e66 6967 5265 7370 6f6e 7365 2854  ConfigResponse(T
-00057510: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-00057520: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-00057530: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00057540: 2020 6865 6164 6572 733a 2044 6963 745b    headers: Dict[
-00057550: 7374 722c 2073 7472 5d20 3d20 4e6f 6e65  str, str] = None
-00057560: 2c0a 2020 2020 2020 2020 626f 6479 3a20  ,.        body: 
-00057570: 5570 6461 7465 4e61 6d65 7370 6163 6553  UpdateNamespaceS
-00057580: 636f 7065 5369 6465 6361 7243 6f6e 6669  copeSidecarConfi
-00057590: 6752 6573 706f 6e73 6542 6f64 7920 3d20  gResponseBody = 
-000575a0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-000575b0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-000575c0: 7320 3d20 6865 6164 6572 730a 2020 2020  s = headers.    
-000575d0: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-000575e0: 626f 6479 0a0a 2020 2020 6465 6620 7661  body..    def va
-000575f0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-00057600: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
-00057610: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
-00057620: 662e 6865 6164 6572 732c 2027 6865 6164  f.headers, 'head
-00057630: 6572 7327 290a 2020 2020 2020 2020 7365  ers').        se
-00057640: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
-00057650: 6972 6564 2873 656c 662e 626f 6479 2c20  ired(self.body, 
-00057660: 2762 6f64 7927 290a 2020 2020 2020 2020  'body').        
-00057670: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
-00057680: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-00057690: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
-000576a0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-000576b0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-000576c0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-000576d0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-000576e0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-000576f0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00057700: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-00057710: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-00057720: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-00057730: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
-00057740: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00057750: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
-00057760: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
-00057770: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
-00057780: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
-00057790: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000577a0: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
-000577b0: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
-000577c0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-000577d0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-000577e0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-000577f0: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-00057800: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-00057810: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-00057820: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00057830: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
-00057840: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00057850: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-00057860: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
-00057870: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
-00057880: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
-00057890: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000578a0: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
-000578b0: 203d 2055 7064 6174 654e 616d 6573 7061   = UpdateNamespa
-000578c0: 6365 5363 6f70 6553 6964 6563 6172 436f  ceScopeSidecarCo
-000578d0: 6e66 6967 5265 7370 6f6e 7365 426f 6479  nfigResponseBody
-000578e0: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-000578f0: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
-00057900: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
-00057910: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
-00057920: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-00057930: 636c 6173 7320 5570 6772 6164 654d 6573  class UpgradeMes
-00057940: 6845 6469 7469 6f6e 5061 7274 6961 6c6c  hEditionPartiall
-00057950: 7952 6571 7565 7374 2854 6561 4d6f 6465  yRequest(TeaMode
-00057960: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-00057970: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-00057980: 6c66 2c0a 2020 2020 2020 2020 6173 6d67  lf,.        asmg
-00057990: 6174 6577 6179 5f63 6f6e 7469 6e75 653a  ateway_continue:
-000579a0: 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020   bool = None,.  
-000579b0: 2020 2020 2020 7365 7276 6963 655f 6d65        service_me
-000579c0: 7368 5f69 643a 2073 7472 203d 204e 6f6e  sh_id: str = Non
-000579d0: 652c 0a20 2020 2020 2020 2073 7769 7463  e,.        switc
-000579e0: 685f 746f 5f70 726f 3a20 626f 6f6c 203d  h_to_pro: bool =
-000579f0: 204e 6f6e 652c 0a20 2020 2020 2020 2075   None,.        u
-00057a00: 7067 7261 6465 5f67 6174 6577 6179 5f72  pgrade_gateway_r
-00057a10: 6563 6f72 6473 3a20 7374 7220 3d20 4e6f  ecords: str = No
-00057a20: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-00057a30: 2020 2073 656c 662e 6173 6d67 6174 6577     self.asmgatew
-00057a40: 6179 5f63 6f6e 7469 6e75 6520 3d20 6173  ay_continue = as
-00057a50: 6d67 6174 6577 6179 5f63 6f6e 7469 6e75  mgateway_continu
-00057a60: 650a 2020 2020 2020 2020 7365 6c66 2e73  e.        self.s
-00057a70: 6572 7669 6365 5f6d 6573 685f 6964 203d  ervice_mesh_id =
-00057a80: 2073 6572 7669 6365 5f6d 6573 685f 6964   service_mesh_id
-00057a90: 0a20 2020 2020 2020 2073 656c 662e 7377  .        self.sw
-00057aa0: 6974 6368 5f74 6f5f 7072 6f20 3d20 7377  itch_to_pro = sw
-00057ab0: 6974 6368 5f74 6f5f 7072 6f0a 2020 2020  itch_to_pro.    
-00057ac0: 2020 2020 7365 6c66 2e75 7067 7261 6465      self.upgrade
-00057ad0: 5f67 6174 6577 6179 5f72 6563 6f72 6473  _gateway_records
-00057ae0: 203d 2075 7067 7261 6465 5f67 6174 6577   = upgrade_gatew
-00057af0: 6179 5f72 6563 6f72 6473 0a0a 2020 2020  ay_records..    
-00057b00: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-00057b10: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-00057b20: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-00057b30: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00057b40: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-00057b50: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-00057b60: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-00057b70: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00057b80: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-00057b90: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-00057ba0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00057bb0: 2073 656c 662e 6173 6d67 6174 6577 6179   self.asmgateway
-00057bc0: 5f63 6f6e 7469 6e75 6520 6973 206e 6f74  _continue is not
-00057bd0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00057be0: 2020 2072 6573 756c 745b 2741 534d 4761     result['ASMGa
-00057bf0: 7465 7761 7943 6f6e 7469 6e75 6527 5d20  tewayContinue'] 
-00057c00: 3d20 7365 6c66 2e61 736d 6761 7465 7761  = self.asmgatewa
-00057c10: 795f 636f 6e74 696e 7565 0a20 2020 2020  y_continue.     
-00057c20: 2020 2069 6620 7365 6c66 2e73 6572 7669     if self.servi
-00057c30: 6365 5f6d 6573 685f 6964 2069 7320 6e6f  ce_mesh_id is no
-00057c40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00057c50: 2020 2020 7265 7375 6c74 5b27 5365 7276      result['Serv
-00057c60: 6963 654d 6573 6849 6427 5d20 3d20 7365  iceMeshId'] = se
-00057c70: 6c66 2e73 6572 7669 6365 5f6d 6573 685f  lf.service_mesh_
-00057c80: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
-00057c90: 6c66 2e73 7769 7463 685f 746f 5f70 726f  lf.switch_to_pro
-00057ca0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00057cb0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00057cc0: 5b27 5377 6974 6368 546f 5072 6f27 5d20  ['SwitchToPro'] 
-00057cd0: 3d20 7365 6c66 2e73 7769 7463 685f 746f  = self.switch_to
-00057ce0: 5f70 726f 0a20 2020 2020 2020 2069 6620  _pro.        if 
-00057cf0: 7365 6c66 2e75 7067 7261 6465 5f67 6174  self.upgrade_gat
-00057d00: 6577 6179 5f72 6563 6f72 6473 2069 7320  eway_records is 
-00057d10: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00057d20: 2020 2020 2020 7265 7375 6c74 5b27 5570        result['Up
-00057d30: 6772 6164 6547 6174 6577 6179 5265 636f  gradeGatewayReco
-00057d40: 7264 7327 5d20 3d20 7365 6c66 2e75 7067  rds'] = self.upg
-00057d50: 7261 6465 5f67 6174 6577 6179 5f72 6563  rade_gateway_rec
-00057d60: 6f72 6473 0a20 2020 2020 2020 2072 6574  ords.        ret
-00057d70: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-00057d80: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-00057d90: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-00057da0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-00057db0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-00057dc0: 2020 2020 6966 206d 2e67 6574 2827 4153      if m.get('AS
-00057dd0: 4d47 6174 6577 6179 436f 6e74 696e 7565  MGatewayContinue
-00057de0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00057df0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00057e00: 2e61 736d 6761 7465 7761 795f 636f 6e74  .asmgateway_cont
-00057e10: 696e 7565 203d 206d 2e67 6574 2827 4153  inue = m.get('AS
-00057e20: 4d47 6174 6577 6179 436f 6e74 696e 7565  MGatewayContinue
-00057e30: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00057e40: 6765 7428 2753 6572 7669 6365 4d65 7368  get('ServiceMesh
-00057e50: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-00057e60: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00057e70: 6c66 2e73 6572 7669 6365 5f6d 6573 685f  lf.service_mesh_
-00057e80: 6964 203d 206d 2e67 6574 2827 5365 7276  id = m.get('Serv
-00057e90: 6963 654d 6573 6849 6427 290a 2020 2020  iceMeshId').    
-00057ea0: 2020 2020 6966 206d 2e67 6574 2827 5377      if m.get('Sw
-00057eb0: 6974 6368 546f 5072 6f27 2920 6973 206e  itchToPro') is n
-00057ec0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00057ed0: 2020 2020 2073 656c 662e 7377 6974 6368       self.switch
-00057ee0: 5f74 6f5f 7072 6f20 3d20 6d2e 6765 7428  _to_pro = m.get(
-00057ef0: 2753 7769 7463 6854 6f50 726f 2729 0a20  'SwitchToPro'). 
-00057f00: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00057f10: 2755 7067 7261 6465 4761 7465 7761 7952  'UpgradeGatewayR
-00057f20: 6563 6f72 6473 2729 2069 7320 6e6f 7420  ecords') is not 
-00057f30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00057f40: 2020 7365 6c66 2e75 7067 7261 6465 5f67    self.upgrade_g
-00057f50: 6174 6577 6179 5f72 6563 6f72 6473 203d  ateway_records =
-00057f60: 206d 2e67 6574 2827 5570 6772 6164 6547   m.get('UpgradeG
-00057f70: 6174 6577 6179 5265 636f 7264 7327 290a  atewayRecords').
-00057f80: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00057f90: 656c 660a 0a0a 636c 6173 7320 5570 6772  elf...class Upgr
-00057fa0: 6164 654d 6573 6845 6469 7469 6f6e 5061  adeMeshEditionPa
-00057fb0: 7274 6961 6c6c 7952 6573 706f 6e73 6542  rtiallyResponseB
-00057fc0: 6f64 7928 5465 614d 6f64 656c 293a 0a20  ody(TeaModel):. 
-00057fd0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00057fe0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00057ff0: 2020 2020 2020 2072 6571 7565 7374 5f69         request_i
-00058000: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-00058010: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-00058020: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-00058030: 7265 7175 6573 745f 6964 0a0a 2020 2020  request_id..    
-00058040: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-00058050: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-00058060: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-00058070: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00058080: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-00058090: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-000580a0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-000580b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000580c0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-000580d0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-000580e0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000580f0: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
-00058100: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00058110: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00058120: 5b27 5265 7175 6573 7449 6427 5d20 3d20  ['RequestId'] = 
-00058130: 7365 6c66 2e72 6571 7565 7374 5f69 640a  self.request_id.
-00058140: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00058150: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-00058160: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
-00058170: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
-00058180: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-00058190: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-000581a0: 6620 6d2e 6765 7428 2752 6571 7565 7374  f m.get('Request
-000581b0: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-000581c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000581d0: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-000581e0: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
-000581f0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-00058200: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2055  n self...class U
-00058210: 7067 7261 6465 4d65 7368 4564 6974 696f  pgradeMeshEditio
-00058220: 6e50 6172 7469 616c 6c79 5265 7370 6f6e  nPartiallyRespon
-00058230: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
-00058240: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-00058250: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00058260: 2020 2020 2020 6865 6164 6572 733a 2044        headers: D
-00058270: 6963 745b 7374 722c 2073 7472 5d20 3d20  ict[str, str] = 
-00058280: 4e6f 6e65 2c0a 2020 2020 2020 2020 626f  None,.        bo
-00058290: 6479 3a20 5570 6772 6164 654d 6573 6845  dy: UpgradeMeshE
-000582a0: 6469 7469 6f6e 5061 7274 6961 6c6c 7952  ditionPartiallyR
-000582b0: 6573 706f 6e73 6542 6f64 7920 3d20 4e6f  esponseBody = No
-000582c0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-000582d0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-000582e0: 3d20 6865 6164 6572 730a 2020 2020 2020  = headers.      
-000582f0: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
-00058300: 6479 0a0a 2020 2020 6465 6620 7661 6c69  dy..    def vali
-00058310: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-00058320: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
-00058330: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
-00058340: 6865 6164 6572 732c 2027 6865 6164 6572  headers, 'header
-00058350: 7327 290a 2020 2020 2020 2020 7365 6c66  s').        self
-00058360: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
-00058370: 6564 2873 656c 662e 626f 6479 2c20 2762  ed(self.body, 'b
-00058380: 6f64 7927 290a 2020 2020 2020 2020 6966  ody').        if
-00058390: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
-000583a0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-000583b0: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
-000583c0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-000583d0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-000583e0: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-000583f0: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-00058400: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-00058410: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00058420: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-00058430: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-00058440: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00058450: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
-00058460: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00058470: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
-00058480: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
-00058490: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
-000584a0: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
-000584b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000584c0: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
-000584d0: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
-000584e0: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
-000584f0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-00058500: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-00058510: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
-00058520: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-00058530: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-00058540: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
-00058550: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
-00058560: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00058570: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
-00058580: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-00058590: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000585a0: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
-000585b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000585c0: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
-000585d0: 2055 7067 7261 6465 4d65 7368 4564 6974   UpgradeMeshEdit
-000585e0: 696f 6e50 6172 7469 616c 6c79 5265 7370  ionPartiallyResp
-000585f0: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
-00058600: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-00058610: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
-00058620: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
-00058630: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00058640: 2073 656c 660a 0a0a 636c 6173 7320 5570   self...class Up
-00058650: 6772 6164 654d 6573 6856 6572 7369 6f6e  gradeMeshVersion
-00058660: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
-00058670: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-00058680: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-00058690: 662c 0a20 2020 2020 2020 2073 6572 7669  f,.        servi
-000586a0: 6365 5f6d 6573 685f 6964 3a20 7374 7220  ce_mesh_id: str 
-000586b0: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-000586c0: 2020 2020 2020 2073 656c 662e 7365 7276         self.serv
-000586d0: 6963 655f 6d65 7368 5f69 6420 3d20 7365  ice_mesh_id = se
-000586e0: 7276 6963 655f 6d65 7368 5f69 640a 0a20  rvice_mesh_id.. 
-000586f0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-00058700: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-00058710: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
-00058720: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-00058730: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-00058740: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00058750: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-00058760: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00058770: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-00058780: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00058790: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-000587a0: 2069 6620 7365 6c66 2e73 6572 7669 6365   if self.service
-000587b0: 5f6d 6573 685f 6964 2069 7320 6e6f 7420  _mesh_id is not 
-000587c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000587d0: 2020 7265 7375 6c74 5b27 5365 7276 6963    result['Servic
-000587e0: 654d 6573 6849 6427 5d20 3d20 7365 6c66  eMeshId'] = self
-000587f0: 2e73 6572 7669 6365 5f6d 6573 685f 6964  .service_mesh_id
-00058800: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00058810: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-00058820: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-00058830: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
-00058840: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-00058850: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00058860: 6966 206d 2e67 6574 2827 5365 7276 6963  if m.get('Servic
-00058870: 654d 6573 6849 6427 2920 6973 206e 6f74  eMeshId') is not
-00058880: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00058890: 2020 2073 656c 662e 7365 7276 6963 655f     self.service_
-000588a0: 6d65 7368 5f69 6420 3d20 6d2e 6765 7428  mesh_id = m.get(
-000588b0: 2753 6572 7669 6365 4d65 7368 4964 2729  'ServiceMeshId')
-000588c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000588d0: 7365 6c66 0a0a 0a63 6c61 7373 2055 7067  self...class Upg
-000588e0: 7261 6465 4d65 7368 5665 7273 696f 6e52  radeMeshVersionR
-000588f0: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
-00058900: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-00058910: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-00058920: 2073 656c 662c 0a20 2020 2020 2020 2072   self,.        r
-00058930: 6571 7565 7374 5f69 643a 2073 7472 203d  equest_id: str =
-00058940: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-00058950: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
-00058960: 7374 5f69 6420 3d20 7265 7175 6573 745f  st_id = request_
-00058970: 6964 0a0a 2020 2020 6465 6620 7661 6c69  id..    def vali
-00058980: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-00058990: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-000589a0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-000589b0: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-000589c0: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
-000589d0: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-000589e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000589f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00058a00: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-00058a10: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-00058a20: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
-00058a30: 7175 6573 745f 6964 2069 7320 6e6f 7420  quest_id is not 
-00058a40: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00058a50: 2020 7265 7375 6c74 5b27 5265 7175 6573    result['Reques
-00058a60: 7449 6427 5d20 3d20 7365 6c66 2e72 6571  tId'] = self.req
-00058a70: 7565 7374 5f69 640a 2020 2020 2020 2020  uest_id.        
-00058a80: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-00058a90: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-00058aa0: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-00058ab0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-00058ac0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-00058ad0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00058ae0: 2752 6571 7565 7374 4964 2729 2069 7320  'RequestId') is 
-00058af0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00058b00: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
-00058b10: 7374 5f69 6420 3d20 6d2e 6765 7428 2752  st_id = m.get('R
-00058b20: 6571 7565 7374 4964 2729 0a20 2020 2020  equestId').     
-00058b30: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-00058b40: 0a63 6c61 7373 2055 7067 7261 6465 4d65  .class UpgradeMe
-00058b50: 7368 5665 7273 696f 6e52 6573 706f 6e73  shVersionRespons
-00058b60: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
-00058b70: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-00058b80: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00058b90: 2020 2020 2068 6561 6465 7273 3a20 4469       headers: Di
-00058ba0: 6374 5b73 7472 2c20 7374 725d 203d 204e  ct[str, str] = N
-00058bb0: 6f6e 652c 0a20 2020 2020 2020 2062 6f64  one,.        bod
-00058bc0: 793a 2055 7067 7261 6465 4d65 7368 5665  y: UpgradeMeshVe
-00058bd0: 7273 696f 6e52 6573 706f 6e73 6542 6f64  rsionResponseBod
-00058be0: 7920 3d20 4e6f 6e65 2c0a 2020 2020 293a  y = None,.    ):
-00058bf0: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
-00058c00: 6164 6572 7320 3d20 6865 6164 6572 730a  aders = headers.
-00058c10: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-00058c20: 7920 3d20 626f 6479 0a0a 2020 2020 6465  y = body..    de
-00058c30: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-00058c40: 3a0a 2020 2020 2020 2020 7365 6c66 2e76  :.        self.v
-00058c50: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
-00058c60: 2873 656c 662e 6865 6164 6572 732c 2027  (self.headers, '
-00058c70: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
-00058c80: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
-00058c90: 7265 7175 6972 6564 2873 656c 662e 626f  required(self.bo
-00058ca0: 6479 2c20 2762 6f64 7927 290a 2020 2020  dy, 'body').    
-00058cb0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
-00058cc0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00058cd0: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
-00058ce0: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
-00058cf0: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-00058d00: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
-00058d10: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00058d20: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-00058d30: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00058d40: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-00058d50: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00058d60: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00058d70: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
-00058d80: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00058d90: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00058da0: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
-00058db0: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
-00058dc0: 2020 6966 2073 656c 662e 626f 6479 2069    if self.body i
-00058dd0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00058de0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00058df0: 626f 6479 275d 203d 2073 656c 662e 626f  body'] = self.bo
-00058e00: 6479 2e74 6f5f 6d61 7028 290a 2020 2020  dy.to_map().    
-00058e10: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00058e20: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-00058e30: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-00058e40: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-00058e50: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-00058e60: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-00058e70: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
-00058e80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00058e90: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-00058ea0: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
-00058eb0: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
-00058ec0: 6966 206d 2e67 6574 2827 626f 6479 2729  if m.get('body')
-00058ed0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00058ee0: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
-00058ef0: 6f64 656c 203d 2055 7067 7261 6465 4d65  odel = UpgradeMe
-00058f00: 7368 5665 7273 696f 6e52 6573 706f 6e73  shVersionRespons
-00058f10: 6542 6f64 7928 290a 2020 2020 2020 2020  eBody().        
-00058f20: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-00058f30: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
-00058f40: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
-00058f50: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00058f60: 6c66 0a0a 0a63 6c61 7373 2043 6c75 7374  lf...class Clust
-00058f70: 6572 5374 6174 7573 4c6f 6774 6169 6c53  erStatusLogtailS
-00058f80: 7461 7475 7352 6563 6f72 6456 616c 7565  tatusRecordValue
-00058f90: 5661 6c75 6528 5465 614d 6f64 656c 293a  Value(TeaModel):
-00058fa0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00058fb0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-00058fc0: 0a20 2020 2020 2020 2074 6974 6c65 3a20  .        title: 
-00058fd0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-00058fe0: 2020 2020 7572 6c3a 2073 7472 203d 204e      url: str = N
-00058ff0: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-00059000: 2020 2020 7365 6c66 2e74 6974 6c65 203d      self.title =
-00059010: 2074 6974 6c65 0a20 2020 2020 2020 2073   title.        s
-00059020: 656c 662e 7572 6c20 3d20 7572 6c0a 0a20  elf.url = url.. 
-00059030: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-00059040: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-00059050: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
-00059060: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-00059070: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-00059080: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00059090: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-000590a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000590b0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-000590c0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-000590d0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-000590e0: 2069 6620 7365 6c66 2e74 6974 6c65 2069   if self.title i
-000590f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00059100: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00059110: 5469 746c 6527 5d20 3d20 7365 6c66 2e74  Title'] = self.t
-00059120: 6974 6c65 0a20 2020 2020 2020 2069 6620  itle.        if 
-00059130: 7365 6c66 2e75 726c 2069 7320 6e6f 7420  self.url is not 
-00059140: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00059150: 2020 7265 7375 6c74 5b27 5572 6c27 5d20    result['Url'] 
-00059160: 3d20 7365 6c66 2e75 726c 0a20 2020 2020  = self.url.     
-00059170: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00059180: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-00059190: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
-000591a0: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
-000591b0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-000591c0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000591d0: 6574 2827 5469 746c 6527 2920 6973 206e  et('Title') is n
-000591e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000591f0: 2020 2020 2073 656c 662e 7469 746c 6520       self.title 
-00059200: 3d20 6d2e 6765 7428 2754 6974 6c65 2729  = m.get('Title')
-00059210: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00059220: 7428 2755 726c 2729 2069 7320 6e6f 7420  t('Url') is not 
-00059230: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00059240: 2020 7365 6c66 2e75 726c 203d 206d 2e67    self.url = m.g
-00059250: 6574 2827 5572 6c27 290a 2020 2020 2020  et('Url').      
-00059260: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+00055d50: 7263 655f 7265 7175 6573 7420 6973 206e  rce_request is n
+00055d60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00055d70: 2020 2020 2072 6573 756c 745b 2753 6964       result['Sid
+00055d80: 6563 6172 5072 6f78 794d 656d 6f72 7952  ecarProxyMemoryR
+00055d90: 6573 6f75 7263 6552 6571 7565 7374 275d  esourceRequest']
+00055da0: 203d 2073 656c 662e 7369 6465 6361 725f   = self.sidecar_
+00055db0: 7072 6f78 795f 6d65 6d6f 7279 5f72 6573  proxy_memory_res
+00055dc0: 6f75 7263 655f 7265 7175 6573 740a 2020  ource_request.  
+00055dd0: 2020 2020 2020 6966 2073 656c 662e 7465        if self.te
+00055de0: 726d 696e 6174 696f 6e5f 6472 6169 6e5f  rmination_drain_
+00055df0: 6475 7261 7469 6f6e 2069 7320 6e6f 7420  duration is not 
+00055e00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00055e10: 2020 7265 7375 6c74 5b27 5465 726d 696e    result['Termin
+00055e20: 6174 696f 6e44 7261 696e 4475 7261 7469  ationDrainDurati
+00055e30: 6f6e 275d 203d 2073 656c 662e 7465 726d  on'] = self.term
+00055e40: 696e 6174 696f 6e5f 6472 6169 6e5f 6475  ination_drain_du
+00055e50: 7261 7469 6f6e 0a20 2020 2020 2020 2072  ration.        r
+00055e60: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+00055e70: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+00055e80: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
+00055e90: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+00055ea0: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+00055eb0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00055ec0: 4578 636c 7564 6549 5052 616e 6765 7327  ExcludeIPRanges'
+00055ed0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00055ee0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00055ef0: 6578 636c 7564 655f 6970 7261 6e67 6573  exclude_ipranges
+00055f00: 203d 206d 2e67 6574 2827 4578 636c 7564   = m.get('Exclud
+00055f10: 6549 5052 616e 6765 7327 290a 2020 2020  eIPRanges').    
+00055f20: 2020 2020 6966 206d 2e67 6574 2827 4578      if m.get('Ex
+00055f30: 636c 7564 6549 6e62 6f75 6e64 506f 7274  cludeInboundPort
+00055f40: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+00055f50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00055f60: 662e 6578 636c 7564 655f 696e 626f 756e  f.exclude_inboun
+00055f70: 645f 706f 7274 7320 3d20 6d2e 6765 7428  d_ports = m.get(
+00055f80: 2745 7863 6c75 6465 496e 626f 756e 6450  'ExcludeInboundP
+00055f90: 6f72 7473 2729 0a20 2020 2020 2020 2069  orts').        i
+00055fa0: 6620 6d2e 6765 7428 2745 7863 6c75 6465  f m.get('Exclude
+00055fb0: 4f75 7462 6f75 6e64 506f 7274 7327 2920  OutboundPorts') 
+00055fc0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00055fd0: 2020 2020 2020 2020 2073 656c 662e 6578           self.ex
+00055fe0: 636c 7564 655f 6f75 7462 6f75 6e64 5f70  clude_outbound_p
+00055ff0: 6f72 7473 203d 206d 2e67 6574 2827 4578  orts = m.get('Ex
+00056000: 636c 7564 654f 7574 626f 756e 6450 6f72  cludeOutboundPor
+00056010: 7473 2729 0a20 2020 2020 2020 2069 6620  ts').        if 
+00056020: 6d2e 6765 7428 2749 6e63 6c75 6465 4950  m.get('IncludeIP
+00056030: 5261 6e67 6573 2729 2069 7320 6e6f 7420  Ranges') is not 
+00056040: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00056050: 2020 7365 6c66 2e69 6e63 6c75 6465 5f69    self.include_i
+00056060: 7072 616e 6765 7320 3d20 6d2e 6765 7428  pranges = m.get(
+00056070: 2749 6e63 6c75 6465 4950 5261 6e67 6573  'IncludeIPRanges
+00056080: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00056090: 6765 7428 2749 6e63 6c75 6465 496e 626f  get('IncludeInbo
+000560a0: 756e 6450 6f72 7473 2729 2069 7320 6e6f  undPorts') is no
+000560b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000560c0: 2020 2020 7365 6c66 2e69 6e63 6c75 6465      self.include
+000560d0: 5f69 6e62 6f75 6e64 5f70 6f72 7473 203d  _inbound_ports =
+000560e0: 206d 2e67 6574 2827 496e 636c 7564 6549   m.get('IncludeI
+000560f0: 6e62 6f75 6e64 506f 7274 7327 290a 2020  nboundPorts').  
+00056100: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00056110: 496e 636c 7564 654f 7574 626f 756e 6450  IncludeOutboundP
+00056120: 6f72 7473 2729 2069 7320 6e6f 7420 4e6f  orts') is not No
+00056130: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00056140: 7365 6c66 2e69 6e63 6c75 6465 5f6f 7574  self.include_out
+00056150: 626f 756e 645f 706f 7274 7320 3d20 6d2e  bound_ports = m.
+00056160: 6765 7428 2749 6e63 6c75 6465 4f75 7462  get('IncludeOutb
+00056170: 6f75 6e64 506f 7274 7327 290a 2020 2020  oundPorts').    
+00056180: 2020 2020 6966 206d 2e67 6574 2827 4973      if m.get('Is
+00056190: 7469 6f44 4e53 5072 6f78 7945 6e61 626c  tioDNSProxyEnabl
+000561a0: 6564 2729 2069 7320 6e6f 7420 4e6f 6e65  ed') is not None
+000561b0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000561c0: 6c66 2e69 7374 696f 5f64 6e73 7072 6f78  lf.istio_dnsprox
+000561d0: 795f 656e 6162 6c65 6420 3d20 6d2e 6765  y_enabled = m.ge
+000561e0: 7428 2749 7374 696f 444e 5350 726f 7879  t('IstioDNSProxy
+000561f0: 456e 6162 6c65 6427 290a 2020 2020 2020  Enabled').      
+00056200: 2020 6966 206d 2e67 6574 2827 4c69 6665    if m.get('Life
+00056210: 6379 636c 6527 2920 6973 206e 6f74 204e  cycle') is not N
+00056220: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00056230: 2073 656c 662e 6c69 6665 6379 636c 6520   self.lifecycle 
+00056240: 3d20 6d2e 6765 7428 274c 6966 6563 7963  = m.get('Lifecyc
+00056250: 6c65 2729 0a20 2020 2020 2020 2069 6620  le').        if 
+00056260: 6d2e 6765 7428 274e 616d 6573 7061 6365  m.get('Namespace
+00056270: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00056280: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00056290: 2e6e 616d 6573 7061 6365 203d 206d 2e67  .namespace = m.g
+000562a0: 6574 2827 4e61 6d65 7370 6163 6527 290a  et('Namespace').
+000562b0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000562c0: 2827 5072 6f78 7949 6e69 7443 5055 5265  ('ProxyInitCPURe
+000562d0: 736f 7572 6365 4c69 6d69 7427 2920 6973  sourceLimit') is
+000562e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000562f0: 2020 2020 2020 2073 656c 662e 7072 6f78         self.prox
+00056300: 795f 696e 6974 5f63 7075 7265 736f 7572  y_init_cpuresour
+00056310: 6365 5f6c 696d 6974 203d 206d 2e67 6574  ce_limit = m.get
+00056320: 2827 5072 6f78 7949 6e69 7443 5055 5265  ('ProxyInitCPURe
+00056330: 736f 7572 6365 4c69 6d69 7427 290a 2020  sourceLimit').  
+00056340: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00056350: 5072 6f78 7949 6e69 7443 5055 5265 736f  ProxyInitCPUReso
+00056360: 7572 6365 5265 7175 6573 7427 2920 6973  urceRequest') is
+00056370: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00056380: 2020 2020 2020 2073 656c 662e 7072 6f78         self.prox
+00056390: 795f 696e 6974 5f63 7075 7265 736f 7572  y_init_cpuresour
+000563a0: 6365 5f72 6571 7565 7374 203d 206d 2e67  ce_request = m.g
+000563b0: 6574 2827 5072 6f78 7949 6e69 7443 5055  et('ProxyInitCPU
+000563c0: 5265 736f 7572 6365 5265 7175 6573 7427  ResourceRequest'
+000563d0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000563e0: 6574 2827 5072 6f78 7949 6e69 744d 656d  et('ProxyInitMem
+000563f0: 6f72 7952 6573 6f75 7263 654c 696d 6974  oryResourceLimit
+00056400: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00056410: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00056420: 2e70 726f 7879 5f69 6e69 745f 6d65 6d6f  .proxy_init_memo
+00056430: 7279 5f72 6573 6f75 7263 655f 6c69 6d69  ry_resource_limi
+00056440: 7420 3d20 6d2e 6765 7428 2750 726f 7879  t = m.get('Proxy
+00056450: 496e 6974 4d65 6d6f 7279 5265 736f 7572  InitMemoryResour
+00056460: 6365 4c69 6d69 7427 290a 2020 2020 2020  ceLimit').      
+00056470: 2020 6966 206d 2e67 6574 2827 5072 6f78    if m.get('Prox
+00056480: 7949 6e69 744d 656d 6f72 7952 6573 6f75  yInitMemoryResou
+00056490: 7263 6552 6571 7565 7374 2729 2069 7320  rceRequest') is 
+000564a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000564b0: 2020 2020 2020 7365 6c66 2e70 726f 7879        self.proxy
+000564c0: 5f69 6e69 745f 6d65 6d6f 7279 5f72 6573  _init_memory_res
+000564d0: 6f75 7263 655f 7265 7175 6573 7420 3d20  ource_request = 
+000564e0: 6d2e 6765 7428 2750 726f 7879 496e 6974  m.get('ProxyInit
+000564f0: 4d65 6d6f 7279 5265 736f 7572 6365 5265  MemoryResourceRe
+00056500: 7175 6573 7427 290a 2020 2020 2020 2020  quest').        
+00056510: 6966 206d 2e67 6574 2827 5365 7276 6963  if m.get('Servic
+00056520: 654d 6573 6849 6427 2920 6973 206e 6f74  eMeshId') is not
+00056530: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00056540: 2020 2073 656c 662e 7365 7276 6963 655f     self.service_
+00056550: 6d65 7368 5f69 6420 3d20 6d2e 6765 7428  mesh_id = m.get(
+00056560: 2753 6572 7669 6365 4d65 7368 4964 2729  'ServiceMeshId')
+00056570: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00056580: 7428 2753 6964 6563 6172 5072 6f78 7943  t('SidecarProxyC
+00056590: 5055 5265 736f 7572 6365 4c69 6d69 7427  PUResourceLimit'
+000565a0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000565b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000565c0: 7369 6465 6361 725f 7072 6f78 795f 6370  sidecar_proxy_cp
+000565d0: 7572 6573 6f75 7263 655f 6c69 6d69 7420  uresource_limit 
+000565e0: 3d20 6d2e 6765 7428 2753 6964 6563 6172  = m.get('Sidecar
+000565f0: 5072 6f78 7943 5055 5265 736f 7572 6365  ProxyCPUResource
+00056600: 4c69 6d69 7427 290a 2020 2020 2020 2020  Limit').        
+00056610: 6966 206d 2e67 6574 2827 5369 6465 6361  if m.get('Sideca
+00056620: 7250 726f 7879 4350 5552 6573 6f75 7263  rProxyCPUResourc
+00056630: 6552 6571 7565 7374 2729 2069 7320 6e6f  eRequest') is no
+00056640: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00056650: 2020 2020 7365 6c66 2e73 6964 6563 6172      self.sidecar
+00056660: 5f70 726f 7879 5f63 7075 7265 736f 7572  _proxy_cpuresour
+00056670: 6365 5f72 6571 7565 7374 203d 206d 2e67  ce_request = m.g
+00056680: 6574 2827 5369 6465 6361 7250 726f 7879  et('SidecarProxy
+00056690: 4350 5552 6573 6f75 7263 6552 6571 7565  CPUResourceReque
+000566a0: 7374 2729 0a20 2020 2020 2020 2069 6620  st').        if 
+000566b0: 6d2e 6765 7428 2753 6964 6563 6172 5072  m.get('SidecarPr
+000566c0: 6f78 794d 656d 6f72 7952 6573 6f75 7263  oxyMemoryResourc
+000566d0: 654c 696d 6974 2729 2069 7320 6e6f 7420  eLimit') is not 
+000566e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000566f0: 2020 7365 6c66 2e73 6964 6563 6172 5f70    self.sidecar_p
+00056700: 726f 7879 5f6d 656d 6f72 795f 7265 736f  roxy_memory_reso
+00056710: 7572 6365 5f6c 696d 6974 203d 206d 2e67  urce_limit = m.g
+00056720: 6574 2827 5369 6465 6361 7250 726f 7879  et('SidecarProxy
+00056730: 4d65 6d6f 7279 5265 736f 7572 6365 4c69  MemoryResourceLi
+00056740: 6d69 7427 290a 2020 2020 2020 2020 6966  mit').        if
+00056750: 206d 2e67 6574 2827 5369 6465 6361 7250   m.get('SidecarP
+00056760: 726f 7879 4d65 6d6f 7279 5265 736f 7572  roxyMemoryResour
+00056770: 6365 5265 7175 6573 7427 2920 6973 206e  ceRequest') is n
+00056780: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00056790: 2020 2020 2073 656c 662e 7369 6465 6361       self.sideca
+000567a0: 725f 7072 6f78 795f 6d65 6d6f 7279 5f72  r_proxy_memory_r
+000567b0: 6573 6f75 7263 655f 7265 7175 6573 7420  esource_request 
+000567c0: 3d20 6d2e 6765 7428 2753 6964 6563 6172  = m.get('Sidecar
+000567d0: 5072 6f78 794d 656d 6f72 7952 6573 6f75  ProxyMemoryResou
+000567e0: 7263 6552 6571 7565 7374 2729 0a20 2020  rceRequest').   
+000567f0: 2020 2020 2069 6620 6d2e 6765 7428 2754       if m.get('T
+00056800: 6572 6d69 6e61 7469 6f6e 4472 6169 6e44  erminationDrainD
+00056810: 7572 6174 696f 6e27 2920 6973 206e 6f74  uration') is not
+00056820: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00056830: 2020 2073 656c 662e 7465 726d 696e 6174     self.terminat
+00056840: 696f 6e5f 6472 6169 6e5f 6475 7261 7469  ion_drain_durati
+00056850: 6f6e 203d 206d 2e67 6574 2827 5465 726d  on = m.get('Term
+00056860: 696e 6174 696f 6e44 7261 696e 4475 7261  inationDrainDura
+00056870: 7469 6f6e 2729 0a20 2020 2020 2020 2072  tion').        r
+00056880: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+00056890: 7373 2055 7064 6174 654e 616d 6573 7061  ss UpdateNamespa
+000568a0: 6365 5363 6f70 6553 6964 6563 6172 436f  ceScopeSidecarCo
+000568b0: 6e66 6967 5265 7370 6f6e 7365 426f 6479  nfigResponseBody
+000568c0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+000568d0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+000568e0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000568f0: 2020 2020 7265 7175 6573 745f 6964 3a20      request_id: 
+00056900: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00056910: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00056920: 7265 7175 6573 745f 6964 203d 2072 6571  request_id = req
+00056930: 7565 7374 5f69 640a 0a20 2020 2064 6566  uest_id..    def
+00056940: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+00056950: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00056960: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+00056970: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+00056980: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
+00056990: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+000569a0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+000569b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000569c0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+000569d0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+000569e0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+000569f0: 6c66 2e72 6571 7565 7374 5f69 6420 6973  lf.request_id is
+00056a00: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00056a10: 2020 2020 2020 2072 6573 756c 745b 2752         result['R
+00056a20: 6571 7565 7374 4964 275d 203d 2073 656c  equestId'] = sel
+00056a30: 662e 7265 7175 6573 745f 6964 0a20 2020  f.request_id.   
+00056a40: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00056a50: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+00056a60: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
+00056a70: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
+00056a80: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+00056a90: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+00056aa0: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
+00056ab0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00056ac0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00056ad0: 7265 7175 6573 745f 6964 203d 206d 2e67  request_id = m.g
+00056ae0: 6574 2827 5265 7175 6573 7449 6427 290a  et('RequestId').
+00056af0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00056b00: 656c 660a 0a0a 636c 6173 7320 5570 6461  elf...class Upda
+00056b10: 7465 4e61 6d65 7370 6163 6553 636f 7065  teNamespaceScope
+00056b20: 5369 6465 6361 7243 6f6e 6669 6752 6573  SidecarConfigRes
+00056b30: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
+00056b40: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00056b50: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+00056b60: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
+00056b70: 3a20 4469 6374 5b73 7472 2c20 7374 725d  : Dict[str, str]
+00056b80: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00056b90: 2062 6f64 793a 2055 7064 6174 654e 616d   body: UpdateNam
+00056ba0: 6573 7061 6365 5363 6f70 6553 6964 6563  espaceScopeSidec
+00056bb0: 6172 436f 6e66 6967 5265 7370 6f6e 7365  arConfigResponse
+00056bc0: 426f 6479 203d 204e 6f6e 652c 0a20 2020  Body = None,.   
+00056bd0: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
+00056be0: 2e68 6561 6465 7273 203d 2068 6561 6465  .headers = heade
+00056bf0: 7273 0a20 2020 2020 2020 2073 656c 662e  rs.        self.
+00056c00: 626f 6479 203d 2062 6f64 790a 0a20 2020  body = body..   
+00056c10: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+00056c20: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
+00056c30: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+00056c40: 7265 6428 7365 6c66 2e68 6561 6465 7273  red(self.headers
+00056c50: 2c20 2768 6561 6465 7273 2729 0a20 2020  , 'headers').   
+00056c60: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
+00056c70: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
+00056c80: 2e62 6f64 792c 2027 626f 6479 2729 0a20  .body, 'body'). 
+00056c90: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+00056ca0: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
+00056cb0: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
+00056cc0: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
+00056cd0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+00056ce0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+00056cf0: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+00056d00: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+00056d10: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00056d20: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+00056d30: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+00056d40: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+00056d50: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
+00056d60: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
+00056d70: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00056d80: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
+00056d90: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
+00056da0: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+00056db0: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+00056dc0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00056dd0: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
+00056de0: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
+00056df0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00056e00: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+00056e10: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+00056e20: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+00056e30: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+00056e40: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00056e50: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+00056e60: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00056e70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00056e80: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
+00056e90: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
+00056ea0: 2020 2069 6620 6d2e 6765 7428 2762 6f64     if m.get('bod
+00056eb0: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
+00056ec0: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+00056ed0: 705f 6d6f 6465 6c20 3d20 5570 6461 7465  p_model = Update
+00056ee0: 4e61 6d65 7370 6163 6553 636f 7065 5369  NamespaceScopeSi
+00056ef0: 6465 6361 7243 6f6e 6669 6752 6573 706f  decarConfigRespo
+00056f00: 6e73 6542 6f64 7928 290a 2020 2020 2020  nseBody().      
+00056f10: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+00056f20: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
+00056f30: 6d5f 6d61 7028 6d5b 2762 6f64 7927 5d29  m_map(m['body'])
+00056f40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00056f50: 7365 6c66 0a0a 0a63 6c61 7373 2055 7067  self...class Upg
+00056f60: 7261 6465 4d65 7368 4564 6974 696f 6e50  radeMeshEditionP
+00056f70: 6172 7469 616c 6c79 5265 7175 6573 7428  artiallyRequest(
+00056f80: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+00056f90: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+00056fa0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00056fb0: 2020 2061 736d 6761 7465 7761 795f 636f     asmgateway_co
+00056fc0: 6e74 696e 7565 3a20 626f 6f6c 203d 204e  ntinue: bool = N
+00056fd0: 6f6e 652c 0a20 2020 2020 2020 2073 6572  one,.        ser
+00056fe0: 7669 6365 5f6d 6573 685f 6964 3a20 7374  vice_mesh_id: st
+00056ff0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+00057000: 2020 7377 6974 6368 5f74 6f5f 7072 6f3a    switch_to_pro:
+00057010: 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020   bool = None,.  
+00057020: 2020 2020 2020 7570 6772 6164 655f 6761        upgrade_ga
+00057030: 7465 7761 795f 7265 636f 7264 733a 2073  teway_records: s
+00057040: 7472 203d 204e 6f6e 652c 0a20 2020 2029  tr = None,.    )
+00057050: 3a0a 2020 2020 2020 2020 7365 6c66 2e61  :.        self.a
+00057060: 736d 6761 7465 7761 795f 636f 6e74 696e  smgateway_contin
+00057070: 7565 203d 2061 736d 6761 7465 7761 795f  ue = asmgateway_
+00057080: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
+00057090: 2073 656c 662e 7365 7276 6963 655f 6d65   self.service_me
+000570a0: 7368 5f69 6420 3d20 7365 7276 6963 655f  sh_id = service_
+000570b0: 6d65 7368 5f69 640a 2020 2020 2020 2020  mesh_id.        
+000570c0: 7365 6c66 2e73 7769 7463 685f 746f 5f70  self.switch_to_p
+000570d0: 726f 203d 2073 7769 7463 685f 746f 5f70  ro = switch_to_p
+000570e0: 726f 0a20 2020 2020 2020 2073 656c 662e  ro.        self.
+000570f0: 7570 6772 6164 655f 6761 7465 7761 795f  upgrade_gateway_
+00057100: 7265 636f 7264 7320 3d20 7570 6772 6164  records = upgrad
+00057110: 655f 6761 7465 7761 795f 7265 636f 7264  e_gateway_record
+00057120: 730a 0a20 2020 2064 6566 2076 616c 6964  s..    def valid
+00057130: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+00057140: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00057150: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+00057160: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+00057170: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+00057180: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+00057190: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000571a0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+000571b0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+000571c0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+000571d0: 2020 2020 2069 6620 7365 6c66 2e61 736d       if self.asm
+000571e0: 6761 7465 7761 795f 636f 6e74 696e 7565  gateway_continue
+000571f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00057200: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00057210: 5b27 4153 4d47 6174 6577 6179 436f 6e74  ['ASMGatewayCont
+00057220: 696e 7565 275d 203d 2073 656c 662e 6173  inue'] = self.as
+00057230: 6d67 6174 6577 6179 5f63 6f6e 7469 6e75  mgateway_continu
+00057240: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+00057250: 662e 7365 7276 6963 655f 6d65 7368 5f69  f.service_mesh_i
+00057260: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+00057270: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00057280: 745b 2753 6572 7669 6365 4d65 7368 4964  t['ServiceMeshId
+00057290: 275d 203d 2073 656c 662e 7365 7276 6963  '] = self.servic
+000572a0: 655f 6d65 7368 5f69 640a 2020 2020 2020  e_mesh_id.      
+000572b0: 2020 6966 2073 656c 662e 7377 6974 6368    if self.switch
+000572c0: 5f74 6f5f 7072 6f20 6973 206e 6f74 204e  _to_pro is not N
+000572d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000572e0: 2072 6573 756c 745b 2753 7769 7463 6854   result['SwitchT
+000572f0: 6f50 726f 275d 203d 2073 656c 662e 7377  oPro'] = self.sw
+00057300: 6974 6368 5f74 6f5f 7072 6f0a 2020 2020  itch_to_pro.    
+00057310: 2020 2020 6966 2073 656c 662e 7570 6772      if self.upgr
+00057320: 6164 655f 6761 7465 7761 795f 7265 636f  ade_gateway_reco
+00057330: 7264 7320 6973 206e 6f74 204e 6f6e 653a  rds is not None:
+00057340: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00057350: 756c 745b 2755 7067 7261 6465 4761 7465  ult['UpgradeGate
+00057360: 7761 7952 6563 6f72 6473 275d 203d 2073  wayRecords'] = s
+00057370: 656c 662e 7570 6772 6164 655f 6761 7465  elf.upgrade_gate
+00057380: 7761 795f 7265 636f 7264 730a 2020 2020  way_records.    
+00057390: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+000573a0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+000573b0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
+000573c0: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
+000573d0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+000573e0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+000573f0: 6765 7428 2741 534d 4761 7465 7761 7943  get('ASMGatewayC
+00057400: 6f6e 7469 6e75 6527 2920 6973 206e 6f74  ontinue') is not
+00057410: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00057420: 2020 2073 656c 662e 6173 6d67 6174 6577     self.asmgatew
+00057430: 6179 5f63 6f6e 7469 6e75 6520 3d20 6d2e  ay_continue = m.
+00057440: 6765 7428 2741 534d 4761 7465 7761 7943  get('ASMGatewayC
+00057450: 6f6e 7469 6e75 6527 290a 2020 2020 2020  ontinue').      
+00057460: 2020 6966 206d 2e67 6574 2827 5365 7276    if m.get('Serv
+00057470: 6963 654d 6573 6849 6427 2920 6973 206e  iceMeshId') is n
+00057480: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00057490: 2020 2020 2073 656c 662e 7365 7276 6963       self.servic
+000574a0: 655f 6d65 7368 5f69 6420 3d20 6d2e 6765  e_mesh_id = m.ge
+000574b0: 7428 2753 6572 7669 6365 4d65 7368 4964  t('ServiceMeshId
+000574c0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+000574d0: 6765 7428 2753 7769 7463 6854 6f50 726f  get('SwitchToPro
+000574e0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000574f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00057500: 2e73 7769 7463 685f 746f 5f70 726f 203d  .switch_to_pro =
+00057510: 206d 2e67 6574 2827 5377 6974 6368 546f   m.get('SwitchTo
+00057520: 5072 6f27 290a 2020 2020 2020 2020 6966  Pro').        if
+00057530: 206d 2e67 6574 2827 5570 6772 6164 6547   m.get('UpgradeG
+00057540: 6174 6577 6179 5265 636f 7264 7327 2920  atewayRecords') 
+00057550: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00057560: 2020 2020 2020 2020 2073 656c 662e 7570           self.up
+00057570: 6772 6164 655f 6761 7465 7761 795f 7265  grade_gateway_re
+00057580: 636f 7264 7320 3d20 6d2e 6765 7428 2755  cords = m.get('U
+00057590: 7067 7261 6465 4761 7465 7761 7952 6563  pgradeGatewayRec
+000575a0: 6f72 6473 2729 0a20 2020 2020 2020 2072  ords').        r
+000575b0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+000575c0: 7373 2055 7067 7261 6465 4d65 7368 4564  ss UpgradeMeshEd
+000575d0: 6974 696f 6e50 6172 7469 616c 6c79 5265  itionPartiallyRe
+000575e0: 7370 6f6e 7365 426f 6479 2854 6561 4d6f  sponseBody(TeaMo
+000575f0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+00057600: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+00057610: 7365 6c66 2c0a 2020 2020 2020 2020 7265  self,.        re
+00057620: 7175 6573 745f 6964 3a20 7374 7220 3d20  quest_id: str = 
+00057630: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+00057640: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
+00057650: 745f 6964 203d 2072 6571 7565 7374 5f69  t_id = request_i
+00057660: 640a 0a20 2020 2064 6566 2076 616c 6964  d..    def valid
+00057670: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+00057680: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00057690: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+000576a0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+000576b0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+000576c0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+000576d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000576e0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+000576f0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+00057700: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+00057710: 2020 2020 2069 6620 7365 6c66 2e72 6571       if self.req
+00057720: 7565 7374 5f69 6420 6973 206e 6f74 204e  uest_id is not N
+00057730: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00057740: 2072 6573 756c 745b 2752 6571 7565 7374   result['Request
+00057750: 4964 275d 203d 2073 656c 662e 7265 7175  Id'] = self.requ
+00057760: 6573 745f 6964 0a20 2020 2020 2020 2072  est_id.        r
+00057770: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+00057780: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+00057790: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
+000577a0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+000577b0: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+000577c0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000577d0: 5265 7175 6573 7449 6427 2920 6973 206e  RequestId') is n
+000577e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000577f0: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
+00057800: 745f 6964 203d 206d 2e67 6574 2827 5265  t_id = m.get('Re
+00057810: 7175 6573 7449 6427 290a 2020 2020 2020  questId').      
+00057820: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+00057830: 636c 6173 7320 5570 6772 6164 654d 6573  class UpgradeMes
+00057840: 6845 6469 7469 6f6e 5061 7274 6961 6c6c  hEditionPartiall
+00057850: 7952 6573 706f 6e73 6528 5465 614d 6f64  yResponse(TeaMod
+00057860: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+00057870: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+00057880: 656c 662c 0a20 2020 2020 2020 2068 6561  elf,.        hea
+00057890: 6465 7273 3a20 4469 6374 5b73 7472 2c20  ders: Dict[str, 
+000578a0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+000578b0: 2020 2020 2062 6f64 793a 2055 7067 7261       body: Upgra
+000578c0: 6465 4d65 7368 4564 6974 696f 6e50 6172  deMeshEditionPar
+000578d0: 7469 616c 6c79 5265 7370 6f6e 7365 426f  tiallyResponseBo
+000578e0: 6479 203d 204e 6f6e 652c 0a20 2020 2029  dy = None,.    )
+000578f0: 3a0a 2020 2020 2020 2020 7365 6c66 2e68  :.        self.h
+00057900: 6561 6465 7273 203d 2068 6561 6465 7273  eaders = headers
+00057910: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
+00057920: 6479 203d 2062 6f64 790a 0a20 2020 2064  dy = body..    d
+00057930: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+00057940: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00057950: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
+00057960: 6428 7365 6c66 2e68 6561 6465 7273 2c20  d(self.headers, 
+00057970: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
+00057980: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
+00057990: 5f72 6571 7569 7265 6428 7365 6c66 2e62  _required(self.b
+000579a0: 6f64 792c 2027 626f 6479 2729 0a20 2020  ody, 'body').   
+000579b0: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+000579c0: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+000579d0: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
+000579e0: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+000579f0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00057a00: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00057a10: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00057a20: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00057a30: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00057a40: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+00057a50: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00057a60: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+00057a70: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
+00057a80: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00057a90: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00057aa0: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
+00057ab0: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
+00057ac0: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
+00057ad0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00057ae0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00057af0: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
+00057b00: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
+00057b10: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00057b20: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+00057b30: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
+00057b40: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
+00057b50: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+00057b60: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+00057b70: 2e67 6574 2827 6865 6164 6572 7327 2920  .get('headers') 
+00057b80: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00057b90: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
+00057ba0: 6164 6572 7320 3d20 6d2e 6765 7428 2768  aders = m.get('h
+00057bb0: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
+00057bc0: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
+00057bd0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00057be0: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+00057bf0: 6d6f 6465 6c20 3d20 5570 6772 6164 654d  model = UpgradeM
+00057c00: 6573 6845 6469 7469 6f6e 5061 7274 6961  eshEditionPartia
+00057c10: 6c6c 7952 6573 706f 6e73 6542 6f64 7928  llyResponseBody(
+00057c20: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00057c30: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
+00057c40: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
+00057c50: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
+00057c60: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+00057c70: 6c61 7373 2055 7067 7261 6465 4d65 7368  lass UpgradeMesh
+00057c80: 5665 7273 696f 6e52 6571 7565 7374 2854  VersionRequest(T
+00057c90: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+00057ca0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+00057cb0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00057cc0: 2020 7365 7276 6963 655f 6d65 7368 5f69    service_mesh_i
+00057cd0: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
+00057ce0: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
+00057cf0: 6c66 2e73 6572 7669 6365 5f6d 6573 685f  lf.service_mesh_
+00057d00: 6964 203d 2073 6572 7669 6365 5f6d 6573  id = service_mes
+00057d10: 685f 6964 0a0a 2020 2020 6465 6620 7661  h_id..    def va
+00057d20: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+00057d30: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00057d40: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00057d50: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+00057d60: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+00057d70: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00057d80: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00057d90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00057da0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+00057db0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+00057dc0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00057dd0: 7365 7276 6963 655f 6d65 7368 5f69 6420  service_mesh_id 
+00057de0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00057df0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00057e00: 2753 6572 7669 6365 4d65 7368 4964 275d  'ServiceMeshId']
+00057e10: 203d 2073 656c 662e 7365 7276 6963 655f   = self.service_
+00057e20: 6d65 7368 5f69 640a 2020 2020 2020 2020  mesh_id.        
+00057e30: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+00057e40: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+00057e50: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+00057e60: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+00057e70: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+00057e80: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00057e90: 2753 6572 7669 6365 4d65 7368 4964 2729  'ServiceMeshId')
+00057ea0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00057eb0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00057ec0: 6572 7669 6365 5f6d 6573 685f 6964 203d  ervice_mesh_id =
+00057ed0: 206d 2e67 6574 2827 5365 7276 6963 654d   m.get('ServiceM
+00057ee0: 6573 6849 6427 290a 2020 2020 2020 2020  eshId').        
+00057ef0: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00057f00: 6173 7320 5570 6772 6164 654d 6573 6856  ass UpgradeMeshV
+00057f10: 6572 7369 6f6e 5265 7370 6f6e 7365 426f  ersionResponseBo
+00057f20: 6479 2854 6561 4d6f 6465 6c29 3a0a 2020  dy(TeaModel):.  
+00057f30: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00057f40: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00057f50: 2020 2020 2020 7265 7175 6573 745f 6964        request_id
+00057f60: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00057f70: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+00057f80: 662e 7265 7175 6573 745f 6964 203d 2072  f.request_id = r
+00057f90: 6571 7565 7374 5f69 640a 0a20 2020 2064  equest_id..    d
+00057fa0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+00057fb0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+00057fc0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+00057fd0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+00057fe0: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+00057ff0: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+00058000: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+00058010: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00058020: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+00058030: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+00058040: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00058050: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+00058060: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00058070: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00058080: 2752 6571 7565 7374 4964 275d 203d 2073  'RequestId'] = s
+00058090: 656c 662e 7265 7175 6573 745f 6964 0a20  elf.request_id. 
+000580a0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000580b0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+000580c0: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+000580d0: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+000580e0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+000580f0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00058100: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
+00058110: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+00058120: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00058130: 662e 7265 7175 6573 745f 6964 203d 206d  f.request_id = m
+00058140: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
+00058150: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00058160: 2073 656c 660a 0a0a 636c 6173 7320 5570   self...class Up
+00058170: 6772 6164 654d 6573 6856 6572 7369 6f6e  gradeMeshVersion
+00058180: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
+00058190: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+000581a0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+000581b0: 6c66 2c0a 2020 2020 2020 2020 6865 6164  lf,.        head
+000581c0: 6572 733a 2044 6963 745b 7374 722c 2073  ers: Dict[str, s
+000581d0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+000581e0: 2020 2020 626f 6479 3a20 5570 6772 6164      body: Upgrad
+000581f0: 654d 6573 6856 6572 7369 6f6e 5265 7370  eMeshVersionResp
+00058200: 6f6e 7365 426f 6479 203d 204e 6f6e 652c  onseBody = None,
+00058210: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00058220: 7365 6c66 2e68 6561 6465 7273 203d 2068  self.headers = h
+00058230: 6561 6465 7273 0a20 2020 2020 2020 2073  eaders.        s
+00058240: 656c 662e 626f 6479 203d 2062 6f64 790a  elf.body = body.
+00058250: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00058260: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00058270: 2073 656c 662e 7661 6c69 6461 7465 5f72   self.validate_r
+00058280: 6571 7569 7265 6428 7365 6c66 2e68 6561  equired(self.hea
+00058290: 6465 7273 2c20 2768 6561 6465 7273 2729  ders, 'headers')
+000582a0: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
+000582b0: 6c69 6461 7465 5f72 6571 7569 7265 6428  lidate_required(
+000582c0: 7365 6c66 2e62 6f64 792c 2027 626f 6479  self.body, 'body
+000582d0: 2729 0a20 2020 2020 2020 2069 6620 7365  ').        if se
+000582e0: 6c66 2e62 6f64 793a 0a20 2020 2020 2020  lf.body:.       
+000582f0: 2020 2020 2073 656c 662e 626f 6479 2e76       self.body.v
+00058300: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
+00058310: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+00058320: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+00058330: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+00058340: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+00058350: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00058360: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00058370: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+00058380: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+00058390: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+000583a0: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
+000583b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000583c0: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
+000583d0: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
+000583e0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000583f0: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
+00058400: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00058410: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
+00058420: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
+00058430: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+00058440: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+00058450: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+00058460: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+00058470: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+00058480: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+00058490: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
+000584a0: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
+000584b0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000584c0: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
+000584d0: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
+000584e0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000584f0: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
+00058500: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00058510: 2074 656d 705f 6d6f 6465 6c20 3d20 5570   temp_model = Up
+00058520: 6772 6164 654d 6573 6856 6572 7369 6f6e  gradeMeshVersion
+00058530: 5265 7370 6f6e 7365 426f 6479 2829 0a20  ResponseBody(). 
+00058540: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00058550: 626f 6479 203d 2074 656d 705f 6d6f 6465  body = temp_mode
+00058560: 6c2e 6672 6f6d 5f6d 6170 286d 5b27 626f  l.from_map(m['bo
+00058570: 6479 275d 290a 2020 2020 2020 2020 7265  dy']).        re
+00058580: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+00058590: 7320 436c 7573 7465 7253 7461 7475 734c  s ClusterStatusL
+000585a0: 6f67 7461 696c 5374 6174 7573 5265 636f  ogtailStatusReco
+000585b0: 7264 5661 6c75 6556 616c 7565 2854 6561  rdValueValue(Tea
+000585c0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+000585d0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+000585e0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+000585f0: 7469 746c 653a 2073 7472 203d 204e 6f6e  title: str = Non
+00058600: 652c 0a20 2020 2020 2020 2075 726c 3a20  e,.        url: 
+00058610: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00058620: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00058630: 7469 746c 6520 3d20 7469 746c 650a 2020  title = title.  
+00058640: 2020 2020 2020 7365 6c66 2e75 726c 203d        self.url =
+00058650: 2075 726c 0a0a 2020 2020 6465 6620 7661   url..    def va
+00058660: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+00058670: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00058680: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00058690: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+000586a0: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+000586b0: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+000586c0: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+000586d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000586e0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+000586f0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+00058700: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00058710: 7469 746c 6520 6973 206e 6f74 204e 6f6e  title is not Non
+00058720: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00058730: 6573 756c 745b 2754 6974 6c65 275d 203d  esult['Title'] =
+00058740: 2073 656c 662e 7469 746c 650a 2020 2020   self.title.    
+00058750: 2020 2020 6966 2073 656c 662e 7572 6c20      if self.url 
+00058760: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00058770: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00058780: 2755 726c 275d 203d 2073 656c 662e 7572  'Url'] = self.ur
+00058790: 6c0a 2020 2020 2020 2020 7265 7475 726e  l.        return
+000587a0: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+000587b0: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+000587c0: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
+000587d0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+000587e0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+000587f0: 2069 6620 6d2e 6765 7428 2754 6974 6c65   if m.get('Title
+00058800: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00058810: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00058820: 2e74 6974 6c65 203d 206d 2e67 6574 2827  .title = m.get('
+00058830: 5469 746c 6527 290a 2020 2020 2020 2020  Title').        
+00058840: 6966 206d 2e67 6574 2827 5572 6c27 2920  if m.get('Url') 
+00058850: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00058860: 2020 2020 2020 2020 2073 656c 662e 7572           self.ur
+00058870: 6c20 3d20 6d2e 6765 7428 2755 726c 2729  l = m.get('Url')
+00058880: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00058890: 7365 6c66 0a0a 0a                        self...
```

### Comparing `alibabacloud_servicemesh20200111-2.0.8/alibabacloud_servicemesh20200111.egg-info/PKG-INFO` & `alibabacloud_servicemesh20200111-2.0.9/alibabacloud_servicemesh20200111.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-servicemesh20200111
-Version: 2.0.8
+Version: 2.0.9
 Summary: Alibaba Cloud Alibaba Cloud Service Mesh (20200111) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_servicemesh20200111-2.0.8/setup.py` & `alibabacloud_servicemesh20200111-2.0.9/setup.py`

 * *Files identical despite different names*

