# Comparing `tmp/inmanta_module_rest-0.2.8-py3-none-any.whl.zip` & `tmp/inmanta_module_rest-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,9 @@
-Zip file size: 4751 bytes, number of entries: 8
--rw-rw-r--  2.0 unx     2888 b- defN 22-Apr-05 15:02 inmanta_plugins/rest/__init__.py
--rw-rw-r--  2.0 unx      268 b- defN 22-Apr-05 15:03 inmanta_plugins/rest/setup.cfg
--rw-rw-r--  2.0 unx     2148 b- defN 22-Apr-05 15:02 inmanta_plugins/rest/model/_init.cf
--rw-rw-r--  2.0 unx     1001 b- defN 22-Apr-05 15:02 tests/test_rest.py
--rw-rw-r--  2.0 unx      221 b- defN 22-Apr-05 15:03 inmanta_module_rest-0.2.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Apr-05 15:03 inmanta_module_rest-0.2.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       26 b- defN 22-Apr-05 15:03 inmanta_module_rest-0.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      687 b- defN 22-Apr-05 15:03 inmanta_module_rest-0.2.8.dist-info/RECORD
-8 files, 7331 bytes uncompressed, 3539 bytes compressed:  51.7%
+Zip file size: 4021 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx     2888 b- defN 22-Apr-25 06:30 inmanta_plugins/rest/__init__.py
+-rw-rw-r--  2.0 unx      320 b- defN 22-Apr-25 06:31 inmanta_plugins/rest/setup.cfg
+-rw-rw-r--  2.0 unx     2148 b- defN 22-Apr-25 06:30 inmanta_plugins/rest/model/_init.cf
+-rw-rw-r--  2.0 unx      221 b- defN 22-Apr-25 06:31 inmanta_module_rest-0.2.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Apr-25 06:31 inmanta_module_rest-0.2.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 22-Apr-25 06:31 inmanta_module_rest-0.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      612 b- defN 22-Apr-25 06:31 inmanta_module_rest-0.2.9.dist-info/RECORD
+7 files, 6297 bytes uncompressed, 2921 bytes compressed:  53.6%
```

## zipnote {}

```diff
@@ -3,23 +3,20 @@
 
 Filename: inmanta_plugins/rest/setup.cfg
 Comment: 
 
 Filename: inmanta_plugins/rest/model/_init.cf
 Comment: 
 
-Filename: tests/test_rest.py
+Filename: inmanta_module_rest-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_rest-0.2.8.dist-info/METADATA
+Filename: inmanta_module_rest-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_rest-0.2.8.dist-info/WHEEL
+Filename: inmanta_module_rest-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_rest-0.2.8.dist-info/top_level.txt
-Comment: 
-
-Filename: inmanta_module_rest-0.2.8.dist-info/RECORD
+Filename: inmanta_module_rest-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/rest/setup.cfg

```diff
@@ -1,15 +1,18 @@
 [metadata]
 name = inmanta-module-rest
 freeze_recursive = False
 freeze_operator = ~=
-version = 0.2.8
+version = 0.2.9
 license = Apache 2.0
 
 [options]
 install_requires = inmanta-module-std
 	requests~=2.25
 	jq~=1.2
 zip_safe = False
 include_package_data = True
 packages = find_namespace:
 
+[options.packages.find]
+include = inmanta_plugins*
+
```

