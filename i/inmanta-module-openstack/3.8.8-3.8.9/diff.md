# Comparing `tmp/inmanta_module_openstack-3.8.8-py3-none-any.whl.zip` & `tmp/inmanta_module_openstack-3.8.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 26411 bytes, number of entries: 7
--rw-rw-r--  2.0 unx   101502 b- defN 23-Apr-04 12:39 inmanta_plugins/openstack/__init__.py
--rw-rw-r--  2.0 unx      931 b- defN 23-Apr-04 12:39 inmanta_plugins/openstack/setup.cfg
--rw-rw-r--  2.0 unx    17095 b- defN 23-Apr-04 12:39 inmanta_plugins/openstack/model/_init.cf
--rw-rw-r--  2.0 unx      475 b- defN 23-Apr-04 12:39 inmanta_module_openstack-3.8.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-04 12:39 inmanta_module_openstack-3.8.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 23-Apr-04 12:39 inmanta_module_openstack-3.8.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      650 b- defN 23-Apr-04 12:39 inmanta_module_openstack-3.8.8.dist-info/RECORD
+-rw-rw-r--  2.0 unx   101502 b- defN 23-Apr-04 12:55 inmanta_plugins/openstack/__init__.py
+-rw-rw-r--  2.0 unx      931 b- defN 23-Apr-04 12:55 inmanta_plugins/openstack/setup.cfg
+-rw-rw-r--  2.0 unx    17095 b- defN 23-Apr-04 12:55 inmanta_plugins/openstack/model/_init.cf
+-rw-rw-r--  2.0 unx      475 b- defN 23-Apr-04 12:55 inmanta_module_openstack-3.8.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-04 12:55 inmanta_module_openstack-3.8.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 23-Apr-04 12:55 inmanta_module_openstack-3.8.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      650 b- defN 23-Apr-04 12:55 inmanta_module_openstack-3.8.9.dist-info/RECORD
 7 files, 120761 bytes uncompressed, 25241 bytes compressed:  79.1%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: inmanta_plugins/openstack/setup.cfg
 Comment: 
 
 Filename: inmanta_plugins/openstack/model/_init.cf
 Comment: 
 
-Filename: inmanta_module_openstack-3.8.8.dist-info/METADATA
+Filename: inmanta_module_openstack-3.8.9.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_openstack-3.8.8.dist-info/WHEEL
+Filename: inmanta_module_openstack-3.8.9.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_openstack-3.8.8.dist-info/top_level.txt
+Filename: inmanta_module_openstack-3.8.9.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_openstack-3.8.8.dist-info/RECORD
+Filename: inmanta_module_openstack-3.8.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/openstack/setup.cfg

```diff
@@ -18,15 +18,15 @@
 line-length = 128
 target-version = 'py36', 'py37', 'py38'
 
 [metadata]
 name = inmanta-module-openstack
 freeze_recursive = False
 freeze_operator = ~=
-version = 3.8.8
+version = 3.8.9
 license = Apache 2.0
 version_tag = 
 
 [options]
 install_requires = inmanta-module-ip
 	inmanta-module-net
 	inmanta-module-platform
```

## Comparing `inmanta_module_openstack-3.8.8.dist-info/RECORD` & `inmanta_module_openstack-3.8.9.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 inmanta_plugins/openstack/__init__.py,sha256=-fAsPo-sVsZbZ5IfbDDXNY7P0i-n-ruBdseVUIMkMmE,101502
-inmanta_plugins/openstack/setup.cfg,sha256=w_FHyXXsgayV8H8vpTWh0imX5B9dTEodYfZ72j8-0T4,931
+inmanta_plugins/openstack/setup.cfg,sha256=ua57gbRxQnuXHC-vjhOPo6SwwszYngswJI9l0fnar5s,931
 inmanta_plugins/openstack/model/_init.cf,sha256=t1-ce1wu9vAfdEu9iL37_v3E0pr9KFsJA0VQRM2TZfs,17095
-inmanta_module_openstack-3.8.8.dist-info/METADATA,sha256=6BbhnIa4ZYlq8m67kqiPeQw6HBkyiMF92tHgsT-hU8w,475
-inmanta_module_openstack-3.8.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-inmanta_module_openstack-3.8.8.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
-inmanta_module_openstack-3.8.8.dist-info/RECORD,,
+inmanta_module_openstack-3.8.9.dist-info/METADATA,sha256=p2g98XfIXcqCGmkKVEdhPJZLCfQKHRw8Xq10i8BRwp0,475
+inmanta_module_openstack-3.8.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+inmanta_module_openstack-3.8.9.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
+inmanta_module_openstack-3.8.9.dist-info/RECORD,,
```

