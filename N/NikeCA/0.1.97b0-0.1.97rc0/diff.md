# Comparing `tmp/NikeCA-0.1.97b0.tar.gz` & `tmp/NikeCA-0.1.97rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.97b0.tar", last modified: Sun May  7 22:01:22 2023, max compression
+gzip compressed data, was "NikeCA-0.1.97rc0.tar", last modified: Sun May  7 22:08:03 2023, max compression
```

## Comparing `NikeCA-0.1.97b0.tar` & `NikeCA-0.1.97rc0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-07 22:01:22.145433 NikeCA-0.1.97b0/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.97b0/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18014 2023-05-07 22:01:22.145021 NikeCA-0.1.97b0/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.97b0/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-07 22:01:22.145542 NikeCA-0.1.97b0/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2504 2023-05-07 22:01:15.000000 NikeCA-0.1.97b0/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-07 22:01:22.138343 NikeCA-0.1.97b0/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-07 22:01:22.139802 NikeCA-0.1.97b0/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     3966 2023-05-07 20:32:52.000000 NikeCA-0.1.97b0/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-07 22:01:22.140830 NikeCA-0.1.97b0/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-07 20:33:10.000000 NikeCA-0.1.97b0/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.97b0/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-07 22:01:22.142588 NikeCA-0.1.97b0/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.1.97b0/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     6138 2023-05-07 21:58:42.000000 NikeCA-0.1.97b0/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.1.97b0/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.97b0/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-07 22:01:22.144476 NikeCA-0.1.97b0/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18014 2023-05-07 22:01:21.000000 NikeCA-0.1.97b0/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-07 22:01:21.000000 NikeCA-0.1.97b0/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-07 22:01:21.000000 NikeCA-0.1.97b0/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-07 22:01:21.000000 NikeCA-0.1.97b0/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-07 22:01:21.000000 NikeCA-0.1.97b0/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      428 2023-05-07 22:01:04.000000 NikeCA-0.1.97b0/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.1.97b0/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    23787 2023-05-07 21:48:03.000000 NikeCA-0.1.97b0/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.1.97b0/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.1.97b0/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.1.97b0/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.1.97b0/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-05-04 17:11:39.000000 NikeCA-0.1.97b0/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-04 17:07:22.000000 NikeCA-0.1.97b0/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7134 2023-05-07 19:42:02.000000 NikeCA-0.1.97b0/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.1.97b0/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-07 22:08:03.268187 NikeCA-0.1.97rc0/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.97rc0/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18015 2023-05-07 22:08:03.267512 NikeCA-0.1.97rc0/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.97rc0/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-07 22:08:03.268410 NikeCA-0.1.97rc0/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2504 2023-05-07 22:07:51.000000 NikeCA-0.1.97rc0/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-07 22:08:03.257793 NikeCA-0.1.97rc0/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-07 22:08:03.259127 NikeCA-0.1.97rc0/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4020 2023-05-07 22:07:42.000000 NikeCA-0.1.97rc0/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-07 22:08:03.260466 NikeCA-0.1.97rc0/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-07 20:33:10.000000 NikeCA-0.1.97rc0/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.97rc0/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-07 22:08:03.262692 NikeCA-0.1.97rc0/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.1.97rc0/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6138 2023-05-07 21:58:42.000000 NikeCA-0.1.97rc0/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.1.97rc0/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.97rc0/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-07 22:08:03.266462 NikeCA-0.1.97rc0/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18015 2023-05-07 22:08:03.000000 NikeCA-0.1.97rc0/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-07 22:08:03.000000 NikeCA-0.1.97rc0/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-07 22:08:03.000000 NikeCA-0.1.97rc0/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-07 22:08:03.000000 NikeCA-0.1.97rc0/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-07 22:08:03.000000 NikeCA-0.1.97rc0/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      428 2023-05-07 22:01:04.000000 NikeCA-0.1.97rc0/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.1.97rc0/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    23787 2023-05-07 21:48:03.000000 NikeCA-0.1.97rc0/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.1.97rc0/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.1.97rc0/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.1.97rc0/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.1.97rc0/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-05-04 17:11:39.000000 NikeCA-0.1.97rc0/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-04 17:07:22.000000 NikeCA-0.1.97rc0/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7134 2023-05-07 19:42:02.000000 NikeCA-0.1.97rc0/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.1.97rc0/src/__init__.py
```

### Comparing `NikeCA-0.1.97b0/LICENSE` & `NikeCA-0.1.97rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.97b0/PKG-INFO` & `NikeCA-0.1.97rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.97b0
+Version: 0.1.97rc0
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.97b0/README.md` & `NikeCA-0.1.97rc0/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.97b0/setup.py` & `NikeCA-0.1.97rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.97b',
+	version='0.1.97c',
 	description='Standardize and Automate processes',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"Dashboards/__init__",
```

### Comparing `NikeCA-0.1.97b0/src/Dashboards/Dashboards.py` & `NikeCA-0.1.97rc0/src/Dashboards/Dashboards.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .Telemetry.Telemetry import Telemetry
 from .InclusionExclusion.InclusionExclusion import InclusionExclusion
 
 
 class Dashboards(Telemetry, InclusionExclusion):
 
     Telemetry = Telemetry()
+    Telemetry.ProductUsage = Telemetry.ProductUsage()
     InclusionExclusion = InclusionExclusion()
 
     def imp_summary_dashboard(self
                               , username: str
                               , warehouse: str
                               , database: str
                               , role: str
```

### Comparing `NikeCA-0.1.97b0/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.1.97rc0/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.97b0/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.1.97rc0/src/Dashboards/Telemetry/ProductUsage.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.97b0/src/Dashboards/Telemetry/Telemetry.py` & `NikeCA-0.1.97rc0/src/Dashboards/Telemetry/Telemetry.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.97b0/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.97rc0/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.97b0
+Version: 0.1.97rc0
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.97b0/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.1.97rc0/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.97b0/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.97rc0/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.97b0/src/NikeQA.py` & `NikeCA-0.1.97rc0/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.97b0/src/NikeSF.py` & `NikeCA-0.1.97rc0/src/NikeSF.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.97b0/src/_BuildSearchQuery.py` & `NikeCA-0.1.97rc0/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.97b0/src/_GitHub.py` & `NikeCA-0.1.97rc0/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.97b0/src/_QA.py` & `NikeCA-0.1.97rc0/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.97b0/src/_SearchFiles.py` & `NikeCA-0.1.97rc0/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.97b0/src/_SnowflakeData.py` & `NikeCA-0.1.97rc0/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.97b0/src/_SnowflakeDependencies.py` & `NikeCA-0.1.97rc0/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.97b0/src/_SnowflakePull.py` & `NikeCA-0.1.97rc0/src/_SnowflakePull.py`

 * *Files identical despite different names*

