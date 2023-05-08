# Comparing `tmp/rcsb.utils.targets-0.69.tar.gz` & `tmp/rcsb.utils.targets-0.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.targets-0.69.tar", last modified: Wed May  3 20:18:38 2023, max compression
+gzip compressed data, was "rcsb.utils.targets-0.70.tar", last modified: Mon May  8 17:44:53 2023, max compression
```

## Comparing `rcsb.utils.targets-0.69.tar` & `rcsb.utils.targets-0.70.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 20:18:38.238499 rcsb.utils.targets-0.69/
--rw-r--r--   0 vsts      (1001) docker     (122)     5885 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-05-03 20:18:38.238499 rcsb.utils.targets-0.69/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      952 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 20:18:38.234499 rcsb.utils.targets-0.69/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 20:18:38.234499 rcsb.utils.targets-0.69/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 20:18:38.238499 rcsb.utils.targets-0.69/rcsb/utils/targets/
--rw-r--r--   0 vsts      (1001) docker     (122)     9301 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/CARDTargetAnnotationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7017 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/CARDTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8021 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/CARDTargetOntologyProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10102 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/CARDTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19228 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/ChEMBLTargetActivityProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13181 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5330 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8904 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/ChEMBLTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9171 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/DrugBankTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12661 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/DrugBankTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9505 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/IMGTTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    20738 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/IMGTTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10451 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/PharosTargetActivityProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12770 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/PharosTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8841 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/PharosTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8898 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/SAbDabTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9689 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/SAbDabTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 20:18:38.234499 rcsb.utils.targets-0.69/rcsb.utils.targets.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-05-03 20:18:38.000000 rcsb.utils.targets-0.69/rcsb.utils.targets.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1209 2023-05-03 20:18:38.000000 rcsb.utils.targets-0.69/rcsb.utils.targets.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-03 20:18:38.000000 rcsb.utils.targets-0.69/rcsb.utils.targets.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-03 20:03:55.000000 rcsb.utils.targets-0.69/rcsb.utils.targets.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      216 2023-05-03 20:18:38.000000 rcsb.utils.targets-0.69/rcsb.utils.targets.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-03 20:18:38.000000 rcsb.utils.targets-0.69/rcsb.utils.targets.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-05-03 20:18:38.238499 rcsb.utils.targets-0.69/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     2273 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-08 17:44:53.818546 rcsb.utils.targets-0.70/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5977 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1645 2023-05-08 17:44:53.818546 rcsb.utils.targets-0.70/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      953 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-08 17:44:53.814546 rcsb.utils.targets-0.70/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-08 17:44:53.818546 rcsb.utils.targets-0.70/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-08 17:44:53.818546 rcsb.utils.targets-0.70/rcsb/utils/targets/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9301 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/CARDTargetAnnotationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7017 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/CARDTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8021 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/CARDTargetOntologyProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10102 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/CARDTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19228 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/ChEMBLTargetActivityProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13181 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5330 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8904 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/ChEMBLTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9171 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/DrugBankTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12661 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/DrugBankTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9505 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/IMGTTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    20738 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/IMGTTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10451 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/PharosTargetActivityProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12770 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/PharosTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9154 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/PharosTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8898 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/SAbDabTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9689 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/SAbDabTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-08 17:44:53.818546 rcsb.utils.targets-0.70/rcsb.utils.targets.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1645 2023-05-08 17:44:53.000000 rcsb.utils.targets-0.70/rcsb.utils.targets.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1209 2023-05-08 17:44:53.000000 rcsb.utils.targets-0.70/rcsb.utils.targets.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-08 17:44:53.000000 rcsb.utils.targets-0.70/rcsb.utils.targets.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-08 17:32:15.000000 rcsb.utils.targets-0.70/rcsb.utils.targets.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      216 2023-05-08 17:44:53.000000 rcsb.utils.targets-0.70/rcsb.utils.targets.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-08 17:44:53.000000 rcsb.utils.targets-0.70/rcsb.utils.targets.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-05-08 17:44:53.818546 rcsb.utils.targets-0.70/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     2273 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/setup.py
```

### Comparing `rcsb.utils.targets-0.69/HISTORY.txt` & `rcsb.utils.targets-0.70/HISTORY.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,7 +55,8 @@
    3-Mar-2023  - V0.63 Fix typo and handle missing activityType in PharosTargetCofactorProvider()
   13-Mar-2023  - V0.64 Add CARDTargetAnnotationProvider (to replace CARDTargetFeatureProvider)
   22-Mar-2023  - V0.65 Add timeout to IMGT data file fetch, and update py-rcsb_exdb_assets locators
   24-Mar-2023  - V0.66 In PharosTargetProvider(), download sql file to separate dir
   11-Apr-2023  - V0.67 Fix issue with CARD lineage tree building--handle cases with two parents at same depth; Add treeNodeList building and exporting
   27-Apr-2023  - V0.68 Update CARD treeNodeList building
    2-May-2023  - V0.69 Remove depth field from CARD lineage tree
+   5-May-2023  - V0.70 Actually check cache files exist in PharosTargetProvider testCache()
```

### Comparing `rcsb.utils.targets-0.69/LICENSE` & `rcsb.utils.targets-0.70/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.69/PKG-INFO` & `rcsb.utils.targets-0.70/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.targets
-Version: 0.69
+Version: 0.70
 Summary: RCSB Python Wrapper Module for Target Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_targets
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # RCSB Python Target Data Management Utilities
 
-[![Build Status](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_apis/build/status/rcsb.py-rcsb_utils_targets?branchName=master)](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_build/latest?definitionId=1&branchName=master)
+[![Build Status](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_apis/build/status/rcsb.py-rcsb_utils_targets?branchName=master)](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_build/latest?definitionId=29&branchName=master)
 
 ## Introduction
 
 This module contains methods for target data management.
 
 ### Installation
```

### Comparing `rcsb.utils.targets-0.69/README.md` & `rcsb.utils.targets-0.70/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RCSB Python Target Data Management Utilities
 
-[![Build Status](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_apis/build/status/rcsb.py-rcsb_utils_targets?branchName=master)](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_build/latest?definitionId=1&branchName=master)
+[![Build Status](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_apis/build/status/rcsb.py-rcsb_utils_targets?branchName=master)](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_build/latest?definitionId=29&branchName=master)
 
 ## Introduction
 
 This module contains methods for target data management.
 
 ### Installation
```

### Comparing `rcsb.utils.targets-0.69/rcsb/utils/targets/CARDTargetAnnotationProvider.py` & `rcsb.utils.targets-0.70/rcsb/utils/targets/CARDTargetAnnotationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.69/rcsb/utils/targets/CARDTargetFeatureProvider.py` & `rcsb.utils.targets-0.70/rcsb/utils/targets/CARDTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.69/rcsb/utils/targets/CARDTargetOntologyProvider.py` & `rcsb.utils.targets-0.70/rcsb/utils/targets/CARDTargetOntologyProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.69/rcsb/utils/targets/CARDTargetProvider.py` & `rcsb.utils.targets-0.70/rcsb/utils/targets/CARDTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.69/rcsb/utils/targets/ChEMBLTargetActivityProvider.py` & `rcsb.utils.targets-0.70/rcsb/utils/targets/ChEMBLTargetActivityProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.69/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py` & `rcsb.utils.targets-0.70/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.69/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py` & `rcsb.utils.targets-0.70/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.69/rcsb/utils/targets/ChEMBLTargetProvider.py` & `rcsb.utils.targets-0.70/rcsb/utils/targets/ChEMBLTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.69/rcsb/utils/targets/DrugBankTargetCofactorProvider.py` & `rcsb.utils.targets-0.70/rcsb/utils/targets/DrugBankTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.69/rcsb/utils/targets/DrugBankTargetProvider.py` & `rcsb.utils.targets-0.70/rcsb/utils/targets/DrugBankTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.69/rcsb/utils/targets/IMGTTargetFeatureProvider.py` & `rcsb.utils.targets-0.70/rcsb/utils/targets/IMGTTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.69/rcsb/utils/targets/IMGTTargetProvider.py` & `rcsb.utils.targets-0.70/rcsb/utils/targets/IMGTTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.69/rcsb/utils/targets/PharosTargetActivityProvider.py` & `rcsb.utils.targets-0.70/rcsb/utils/targets/PharosTargetActivityProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.69/rcsb/utils/targets/PharosTargetCofactorProvider.py` & `rcsb.utils.targets-0.70/rcsb/utils/targets/PharosTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.69/rcsb/utils/targets/PharosTargetProvider.py` & `rcsb.utils.targets-0.70/rcsb/utils/targets/PharosTargetProvider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ##
 #  File:           PharosTargetProvider.py
 #  Date:           11-Jun-2021 jdw
 #
 #  Updates:
 #   27-Feb-2023 dwp Update mysql loading command
 #   23-Mar-2023 aae Download sql file to separate dir
+#    5-May-2023 aae Check cache files exist in testCache()
 ##
 """
 Accessors for Pharos target assignments.
 """
 
 import logging
 import os.path
@@ -34,14 +35,15 @@
         self.__dirPath = os.path.join(self.__cachePath, self.__dirName)
         #
         # Folder for SQL dump
         self.__sqlDumpDirName = "Pharos-targets-sqldump"
         self.__sqlDumpDirPath = os.path.join(self.__cachePath, self.__sqlDumpDirName)
         #
         self.__mU = MarshalUtil(workPath=self.__dirPath)
+        self.__pharosSelectedTables = ["drug_activity", "cmpd_activity", "target", "protein", "t2tc"]
         reloadDb = kwargs.get("reloadDb", False)
         fromDb = kwargs.get("fromDb", False)
         useCache = kwargs.get("useCache", False)
         pharosDumpUrl = kwargs.get("pharosDumpUrl", None)
         mysqlUser = kwargs.get("mysqlUser", None)
         mysqlPassword = kwargs.get("mysqlPassword", None)
         self.__version = None
@@ -55,22 +57,27 @@
                 pharosDumpUrl=pharosDumpUrl,
                 mysqlUser=mysqlUser,
                 mysqlPassword=mysqlPassword
             )
         #
 
     def testCache(self):
-        return True
+        ok = True
+        for tbl in self.__pharosSelectedTables:
+            outPath = os.path.join(self.__dirPath, "%s.tdd" % tbl)
+            ok = self.__mU.exists(outPath) and ok
+            if not ok:
+                break
+        return ok
 
     def getVersion(self):
         return self.__version
 
     def __reload(self, targetsPath, sqlPath, reloadDb=False, fromDb=False, useCache=False, pharosDumpUrl=None, mysqlUser=None, mysqlPassword=None):
         startTime = time.time()
-        pharosSelectedTables = ["drug_activity", "cmpd_activity", "target", "protein", "t2tc"]
         pharosDumpUrl = pharosDumpUrl if pharosDumpUrl else "http://juniper.health.unm.edu/tcrd/download/latest.sql.gz"
         pharosReadmeUrl = "http://juniper.health.unm.edu/tcrd/download/latest.README"
         ok = False
         fU = FileUtil()
         pharosDumpFileName = fU.getFileName(pharosDumpUrl)
         pharosDumpPath = os.path.join(sqlPath, pharosDumpFileName)
         pharosUpdatePath = os.path.join(sqlPath, "pharos-update.sql")
@@ -92,22 +99,22 @@
                 ok1 = fU.get(pharosDumpUrl, pharosDumpPath)
                 ok2 = fU.get(pharosReadmeUrl, pharosReadmePath)
                 logger.info("Completed fetch (%r) at %s (%.4f seconds)", ok1 and ok2, time.strftime("%Y %m %d %H:%M:%S", time.localtime()), time.time() - startTime)
             # ---
             readmeLines = self.__mU.doImport(pharosReadmePath, fmt="list")
             self.__version = readmeLines[0].split(" ")[1][1:] if readmeLines else "6"
             # ---
-            logger.info("Filtering SQL dump %r for selected tables %r", pharosDumpFileName, pharosSelectedTables)
+            logger.info("Filtering SQL dump %r for selected tables %r", pharosDumpFileName, self.__pharosSelectedTables)
             doWrite = True
             # Note: the pharos dump file latest.sql.gz is not gzipped
             with open(pharosDumpPath, "r", encoding="utf-8") as ifh, open(pharosUpdatePath, "w", encoding="utf-8") as ofh:
                 for line in ifh:
                     if line.startswith("-- Table structure for table"):
                         tN = line.split(" ")[-1][1:-2]
-                        doWrite = True if tN in pharosSelectedTables else False
+                        doWrite = True if tN in self.__pharosSelectedTables else False
                     if doWrite:
                         ofh.write(line)
             # ---
             ok = exU.run(
                 "mysql",
                 execArgList=["-v", "-u", mysqlUser, "--password=%s" % mysqlPassword, "-e", "create database if not exists tcrd6;"],
                 outPath=logPath,
@@ -133,15 +140,15 @@
                 inpPath=None,
                 outAppend=True,
                 timeOut=None,
             )
             logger.info("SQL dump restore status %r", ok)
         # --
         if fromDb:
-            for tbl in pharosSelectedTables:
+            for tbl in self.__pharosSelectedTables:
                 outPath = os.path.join(targetsPath, "%s.tdd" % tbl)
                 # if useCache and self.__mU.exists(outPath):
                 #   continue
                 ok = exU.run(
                     "mysql",
                     execArgList=["-u", mysqlUser, "--password=%s" % mysqlPassword, "-e", "use tcrd6; select * from %s;" % tbl],
                     outPath=outPath,
```

### Comparing `rcsb.utils.targets-0.69/rcsb/utils/targets/SAbDabTargetFeatureProvider.py` & `rcsb.utils.targets-0.70/rcsb/utils/targets/SAbDabTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.69/rcsb/utils/targets/SAbDabTargetProvider.py` & `rcsb.utils.targets-0.70/rcsb/utils/targets/SAbDabTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.69/rcsb.utils.targets.egg-info/PKG-INFO` & `rcsb.utils.targets-0.70/rcsb.utils.targets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.targets
-Version: 0.69
+Version: 0.70
 Summary: RCSB Python Wrapper Module for Target Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_targets
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # RCSB Python Target Data Management Utilities
 
-[![Build Status](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_apis/build/status/rcsb.py-rcsb_utils_targets?branchName=master)](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_build/latest?definitionId=1&branchName=master)
+[![Build Status](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_apis/build/status/rcsb.py-rcsb_utils_targets?branchName=master)](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_build/latest?definitionId=29&branchName=master)
 
 ## Introduction
 
 This module contains methods for target data management.
 
 ### Installation
```

### Comparing `rcsb.utils.targets-0.69/rcsb.utils.targets.egg-info/SOURCES.txt` & `rcsb.utils.targets-0.70/rcsb.utils.targets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.69/setup.py` & `rcsb.utils.targets-0.70/setup.py`

 * *Files identical despite different names*

