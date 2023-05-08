# Comparing `tmp/odoo14_addon_crm_rest_api-14.0.1.0.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_crm_rest_api-14.0.1.0.1.dev1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 3571 bytes, number of entries: 10
+Zip file size: 3637 bytes, number of entries: 10
 -rw-r--r--  2.0 unx       96 b- defN 23-May-03 12:41 odoo/addons/crm_rest_api/README.rst
 -rw-r--r--  2.0 unx       23 b- defN 23-May-03 12:41 odoo/addons/crm_rest_api/__init__.py
 -rw-r--r--  2.0 unx      516 b- defN 23-May-03 13:36 odoo/addons/crm_rest_api/__manifest__.py
 -rw-r--r--  2.0 unx       32 b- defN 23-May-03 12:41 odoo/addons/crm_rest_api/services/__init__.py
 -rw-r--r--  2.0 unx      952 b- defN 23-May-03 12:41 odoo/addons/crm_rest_api/services/crm_lead_services.py
--rw-r--r--  2.0 unx      162 b- defN 23-May-03 12:41 odoo/addons/crm_rest_api/services/schemas.py
--rw-r--r--  2.0 unx      600 b- defN 23-May-03 14:11 odoo14_addon_crm_rest_api-14.0.1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-03 14:11 odoo14_addon_crm_rest_api-14.0.1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-May-03 14:11 odoo14_addon_crm_rest_api-14.0.1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      975 b- defN 23-May-03 14:11 odoo14_addon_crm_rest_api-14.0.1.0.0.dist-info/RECORD
-10 files, 3453 bytes uncompressed, 1841 bytes compressed:  46.7%
+-rw-r--r--  2.0 unx      235 b- defN 23-May-08 14:04 odoo/addons/crm_rest_api/services/schemas.py
+-rw-r--r--  2.0 unx      605 b- defN 23-May-08 14:10 odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-08 14:10 odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-May-08 14:10 odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      995 b- defN 23-May-08 14:10 odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/RECORD
+10 files, 3551 bytes uncompressed, 1867 bytes compressed:  47.4%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: odoo/addons/crm_rest_api/services/crm_lead_services.py
 Comment: 
 
 Filename: odoo/addons/crm_rest_api/services/schemas.py
 Comment: 
 
-Filename: odoo14_addon_crm_rest_api-14.0.1.0.0.dist-info/METADATA
+Filename: odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_crm_rest_api-14.0.1.0.0.dist-info/WHEEL
+Filename: odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_crm_rest_api-14.0.1.0.0.dist-info/top_level.txt
+Filename: odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_crm_rest_api-14.0.1.0.0.dist-info/RECORD
+Filename: odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/crm_rest_api/services/schemas.py

```diff
@@ -1,4 +1,5 @@
 S_CRM_LEAD_CREATE = {
     "name": {"type": "string", "required": True, "empty": False},
-    "email_from": {"type": "string", "required": False, "empty": False}
+    "email_from": {"type": "string", "required": False, "empty": False},
+    "company_id": {"type": "integer", "required": True, "empty": False}
 }
```

## Comparing `odoo14_addon_crm_rest_api-14.0.1.0.0.dist-info/METADATA` & `odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-crm-rest-api
-Version: 14.0.1.0.0
+Version: 14.0.1.0.1.dev1
 Summary: Expose CRM Lead on the Rest API
 Home-page: UNKNOWN
 Author: Coopdevs Treball SCCL
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
```

## Comparing `odoo14_addon_crm_rest_api-14.0.1.0.0.dist-info/RECORD` & `odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 odoo/addons/crm_rest_api/README.rst,sha256=PNgi4-SbJwOD445Gn_oNPQvrgB5v7OprI92qr8Ctmsw,96
 odoo/addons/crm_rest_api/__init__.py,sha256=qksdRxAxHhEXpY0NZlTEolhxFILjRI5o7J0O4UrAE04,23
 odoo/addons/crm_rest_api/__manifest__.py,sha256=sbRDSV3rSGeEn-gf7HKlCMZBQiP28iv8z4JamUFBRTY,516
 odoo/addons/crm_rest_api/services/__init__.py,sha256=gyXaE_NlVgF1KawzsiRb0DeYYTT13kmL4Ya1LgcRg5c,32
 odoo/addons/crm_rest_api/services/crm_lead_services.py,sha256=IeoJAFjcXUVJbwxGZqaYiVBsFLmz_dDmxyUq-wWGU18,952
-odoo/addons/crm_rest_api/services/schemas.py,sha256=4H1w38NBA82yoZg65IPkcNcWn7xP0juAA9y8LPhzL0k,162
-odoo14_addon_crm_rest_api-14.0.1.0.0.dist-info/METADATA,sha256=vPN4DwsfDwU-bYKvsvEqV_vSNLlkpMx9Tg_ZhGgCnGI,600
-odoo14_addon_crm_rest_api-14.0.1.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-odoo14_addon_crm_rest_api-14.0.1.0.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_crm_rest_api-14.0.1.0.0.dist-info/RECORD,,
+odoo/addons/crm_rest_api/services/schemas.py,sha256=ePXpp9hilOM7h4JjvAelE7hDzuax10WAN1CU1WlWaeE,235
+odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/METADATA,sha256=yEJj1ZI1weOWimpncJ3X7aWJx7YWaIO-JBjWX9SQDUQ,605
+odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/RECORD,,
```

