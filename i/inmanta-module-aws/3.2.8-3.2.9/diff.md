# Comparing `tmp/inmanta_module_aws-3.2.8-py3-none-any.whl.zip` & `tmp/inmanta_module_aws-3.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 19349 bytes, number of entries: 10
--rw-rw-r--  2.0 unx    62068 b- defN 23-Feb-07 09:30 inmanta_plugins/aws/__init__.py
--rw-rw-r--  2.0 unx      814 b- defN 23-Feb-07 09:30 inmanta_plugins/aws/setup.cfg
--rw-rw-r--  2.0 unx     9165 b- defN 23-Feb-07 09:30 inmanta_plugins/aws/model/_init.cf
--rw-rw-r--  2.0 unx     1403 b- defN 23-Feb-07 09:30 inmanta_plugins/aws/model/analytics.cf
--rw-rw-r--  2.0 unx     1223 b- defN 23-Feb-07 09:30 inmanta_plugins/aws/model/database.cf
--rw-rw-r--  2.0 unx      826 b- defN 23-Feb-07 09:30 inmanta_plugins/aws/model/os.cf
--rw-rw-r--  2.0 unx      327 b- defN 23-Feb-07 09:30 inmanta_module_aws-3.2.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Feb-07 09:30 inmanta_module_aws-3.2.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 23-Feb-07 09:30 inmanta_module_aws-3.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      882 b- defN 23-Feb-07 09:30 inmanta_module_aws-3.2.8.dist-info/RECORD
-10 files, 76816 bytes uncompressed, 17823 bytes compressed:  76.8%
+Zip file size: 19345 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx    62068 b- defN 23-Apr-04 12:33 inmanta_plugins/aws/__init__.py
+-rw-rw-r--  2.0 unx      811 b- defN 23-Apr-04 12:33 inmanta_plugins/aws/setup.cfg
+-rw-rw-r--  2.0 unx     9165 b- defN 23-Apr-04 12:33 inmanta_plugins/aws/model/_init.cf
+-rw-rw-r--  2.0 unx     1403 b- defN 23-Apr-04 12:33 inmanta_plugins/aws/model/analytics.cf
+-rw-rw-r--  2.0 unx     1223 b- defN 23-Apr-04 12:33 inmanta_plugins/aws/model/database.cf
+-rw-rw-r--  2.0 unx      826 b- defN 23-Apr-04 12:33 inmanta_plugins/aws/model/os.cf
+-rw-rw-r--  2.0 unx      324 b- defN 23-Apr-04 12:33 inmanta_module_aws-3.2.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-04 12:33 inmanta_module_aws-3.2.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 23-Apr-04 12:33 inmanta_module_aws-3.2.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      882 b- defN 23-Apr-04 12:33 inmanta_module_aws-3.2.9.dist-info/RECORD
+10 files, 76810 bytes uncompressed, 17819 bytes compressed:  76.8%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: inmanta_plugins/aws/model/database.cf
 Comment: 
 
 Filename: inmanta_plugins/aws/model/os.cf
 Comment: 
 
-Filename: inmanta_module_aws-3.2.8.dist-info/METADATA
+Filename: inmanta_module_aws-3.2.9.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_aws-3.2.8.dist-info/WHEEL
+Filename: inmanta_module_aws-3.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_aws-3.2.8.dist-info/top_level.txt
+Filename: inmanta_module_aws-3.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_aws-3.2.8.dist-info/RECORD
+Filename: inmanta_module_aws-3.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/aws/setup.cfg

```diff
@@ -17,26 +17,26 @@
 line-length = 128
 target-version = 'py36', 'py37', 'py38'
 
 [metadata]
 name = inmanta-module-aws
 freeze_recursive = False
 freeze_operator = ~=
-version = 3.2.8
+version = 3.2.9
 license = Apache 2.0
 version_tag = 
 
 [options]
 install_requires = inmanta-module-ip
 	inmanta-module-platform
 	inmanta-module-redhat
 	inmanta-module-ssh
 	inmanta-module-std
 	inmanta-module-web
-	boto3==1.26.65
+	boto3~=1.26
 zip_safe = False
 include_package_data = True
 packages = find_namespace:
 
 [options.packages.find]
 include = inmanta_plugins*
```

## Comparing `inmanta_module_aws-3.2.8.dist-info/RECORD` & `inmanta_module_aws-3.2.9.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 inmanta_plugins/aws/__init__.py,sha256=-yYIXcktEcEMc_IjmG1NQFywm8GMhmdYmzE7CKDCT_o,62068
-inmanta_plugins/aws/setup.cfg,sha256=a57YCVCaNLvb7EIgPW0nY4NO2XwxtbC_2BOe17XYd9c,814
+inmanta_plugins/aws/setup.cfg,sha256=kjVgdJpu_IGB2OFkPMzgzo9Yb_57oKEdbYD-Sy-IUA4,811
 inmanta_plugins/aws/model/_init.cf,sha256=KFs4t-NQLjG0dkdz4MWgQbkwhFlYyn9B63FDXHBdVJs,9165
 inmanta_plugins/aws/model/analytics.cf,sha256=40VyZ7T2ZM_E6u4mq9TrXob2sZn-4QqY0hFRsuCA0ok,1403
 inmanta_plugins/aws/model/database.cf,sha256=E56lWdoKpB4z4_CwgAe6LKEDpg8w1JSyScM8PMrqC2s,1223
 inmanta_plugins/aws/model/os.cf,sha256=da_HY9UNA6I5h8UiV-T0Vd9gN_xX08NEcujTvbIiYSE,826
-inmanta_module_aws-3.2.8.dist-info/METADATA,sha256=f4DI7QJislFOeltjyUrniHsp1fO6B6c0RiwLClu9jcw,327
-inmanta_module_aws-3.2.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-inmanta_module_aws-3.2.8.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
-inmanta_module_aws-3.2.8.dist-info/RECORD,,
+inmanta_module_aws-3.2.9.dist-info/METADATA,sha256=hkUTE4_vkkMgycAG40eFtOTYkhdJQImy2Nhk-8fU0cs,324
+inmanta_module_aws-3.2.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+inmanta_module_aws-3.2.9.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
+inmanta_module_aws-3.2.9.dist-info/RECORD,,
```

