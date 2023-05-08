# Comparing `tmp/warrenapp-0.1.0.tar.gz` & `tmp/warrenapp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warrenapp-0.1.0.tar", last modified: Fri May  5 00:05:11 2023, max compression
+gzip compressed data, was "warrenapp-0.1.1.tar", last modified: Mon May  8 18:57:45 2023, max compression
```

## Comparing `warrenapp-0.1.0.tar` & `warrenapp-0.1.1.tar`

### file list

```diff
@@ -1,51 +1,56 @@
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-05 00:05:11.195687 warrenapp-0.1.0/
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1521 2023-05-04 23:55:17.000000 warrenapp-0.1.0/LICENSE
--rw-rw-r--   0 sweav     (1001) sweav     (1001)     3615 2023-05-05 00:05:11.195687 warrenapp-0.1.0/PKG-INFO
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1405 2023-05-05 00:01:10.000000 warrenapp-0.1.0/README.md
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1351 2023-05-05 00:04:08.000000 warrenapp-0.1.0/pyproject.toml
--rw-rw-r--   0 sweav     (1001) sweav     (1001)       38 2023-05-05 00:05:11.195687 warrenapp-0.1.0/setup.cfg
--rw-r--r--   0 sweav     (1001) sweav     (1001)      245 2023-05-04 23:55:17.000000 warrenapp-0.1.0/setup.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-05 00:05:11.191687 warrenapp-0.1.0/src/
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-05 00:05:11.191687 warrenapp-0.1.0/src/warrenapp/
--rw-r--r--   0 sweav     (1001) sweav     (1001)       24 2023-05-04 23:55:17.000000 warrenapp-0.1.0/src/warrenapp/__init__.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      281 2023-05-04 23:55:17.000000 warrenapp-0.1.0/src/warrenapp/apps.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-05 00:05:11.191687 warrenapp-0.1.0/src/warrenapp/badelf_tools/
--rw-r--r--   0 sweav     (1001) sweav     (1001)    20158 2023-05-04 23:55:17.000000 warrenapp-0.1.0/src/warrenapp/badelf_tools/badelf_algorithm_functions.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)    13829 2023-05-05 00:03:13.000000 warrenapp-0.1.0/src/warrenapp/badelf_tools/utilities.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)     5179 2023-05-04 23:55:17.000000 warrenapp-0.1.0/src/warrenapp/models.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-05 00:05:11.191687 warrenapp-0.1.0/src/warrenapp/workflows/
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1099 2023-05-05 00:03:13.000000 warrenapp-0.1.0/src/warrenapp/workflows/__init__.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-05 00:05:11.195687 warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/
--rw-r--r--   0 sweav     (1001) sweav     (1001)      829 2023-05-05 00:03:13.000000 warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/__init__.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1391 2023-05-05 00:03:13.000000 warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/badelf_hse.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1387 2023-05-05 00:03:13.000000 warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/badelf_pbe.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1357 2023-05-05 00:03:13.000000 warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/bader_badelf_hse.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1459 2023-05-05 00:03:13.000000 warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/bader_badelf_pbe.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1327 2023-05-05 00:03:13.000000 warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/bader_hse.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1401 2023-05-05 00:03:13.000000 warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/bader_pbe.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)    15458 2023-05-05 00:03:13.000000 warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/base.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      903 2023-05-04 23:55:17.000000 warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/elf_hse.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      903 2023-05-04 23:55:17.000000 warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/elf_pbe.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)    13893 2023-05-05 00:03:13.000000 warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/warren_badelf_v3_7.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-05 00:05:11.195687 warrenapp-0.1.0/src/warrenapp/workflows/relaxation/
--rw-r--r--   0 sweav     (1001) sweav     (1001)      296 2023-05-04 23:55:17.000000 warrenapp-0.1.0/src/warrenapp/workflows/relaxation/__init__.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      624 2023-05-04 23:55:17.000000 warrenapp-0.1.0/src/warrenapp/workflows/relaxation/hse.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      545 2023-05-04 23:55:17.000000 warrenapp-0.1.0/src/warrenapp/workflows/relaxation/hsesol.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)     4621 2023-05-05 00:03:13.000000 warrenapp-0.1.0/src/warrenapp/workflows/relaxation/pbe.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      503 2023-05-04 23:55:17.000000 warrenapp-0.1.0/src/warrenapp/workflows/relaxation/pbe_metal.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      443 2023-05-04 23:55:17.000000 warrenapp-0.1.0/src/warrenapp/workflows/relaxation/pbesol.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      702 2023-05-04 23:55:17.000000 warrenapp-0.1.0/src/warrenapp/workflows/relaxation/scan.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-05 00:05:11.195687 warrenapp-0.1.0/src/warrenapp/workflows/static_energy/
--rw-r--r--   0 sweav     (1001) sweav     (1001)      308 2023-05-04 23:55:17.000000 warrenapp-0.1.0/src/warrenapp/workflows/static_energy/__init__.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      431 2023-05-04 23:55:17.000000 warrenapp-0.1.0/src/warrenapp/workflows/static_energy/hse.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      449 2023-05-04 23:55:17.000000 warrenapp-0.1.0/src/warrenapp/workflows/static_energy/hsesol.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      765 2023-05-04 23:55:17.000000 warrenapp-0.1.0/src/warrenapp/workflows/static_energy/pbe.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      474 2023-05-04 23:55:17.000000 warrenapp-0.1.0/src/warrenapp/workflows/static_energy/pbe_metal.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      449 2023-05-04 23:55:17.000000 warrenapp-0.1.0/src/warrenapp/workflows/static_energy/pbesol.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      437 2023-05-04 23:55:17.000000 warrenapp-0.1.0/src/warrenapp/workflows/static_energy/scan.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-05 00:05:11.191687 warrenapp-0.1.0/src/warrenapp.egg-info/
--rw-rw-r--   0 sweav     (1001) sweav     (1001)     3615 2023-05-05 00:05:11.000000 warrenapp-0.1.0/src/warrenapp.egg-info/PKG-INFO
--rw-rw-r--   0 sweav     (1001) sweav     (1001)     1717 2023-05-05 00:05:11.000000 warrenapp-0.1.0/src/warrenapp.egg-info/SOURCES.txt
--rw-rw-r--   0 sweav     (1001) sweav     (1001)        1 2023-05-05 00:05:11.000000 warrenapp-0.1.0/src/warrenapp.egg-info/dependency_links.txt
--rw-rw-r--   0 sweav     (1001) sweav     (1001)        8 2023-05-05 00:05:11.000000 warrenapp-0.1.0/src/warrenapp.egg-info/requires.txt
--rw-rw-r--   0 sweav     (1001) sweav     (1001)       10 2023-05-05 00:05:11.000000 warrenapp-0.1.0/src/warrenapp.egg-info/top_level.txt
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-08 18:57:45.562255 warrenapp-0.1.1/
+-rw-r--r--   0 sweav     (1001) sweav     (1001)     1521 2023-05-04 20:41:15.000000 warrenapp-0.1.1/LICENSE
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     3615 2023-05-08 18:57:45.558255 warrenapp-0.1.1/PKG-INFO
+-rw-r--r--   0 sweav     (1001) sweav     (1001)     1405 2023-05-05 00:01:17.000000 warrenapp-0.1.1/README.md
+-rw-r--r--   0 sweav     (1001) sweav     (1001)     1351 2023-05-08 18:35:34.000000 warrenapp-0.1.1/pyproject.toml
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)       38 2023-05-08 18:57:45.562255 warrenapp-0.1.1/setup.cfg
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      245 2023-05-04 23:54:39.000000 warrenapp-0.1.1/setup.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-08 18:57:45.554255 warrenapp-0.1.1/src/
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-08 18:57:45.554255 warrenapp-0.1.1/src/warrenapp/
+-rw-r--r--   0 sweav     (1001) sweav     (1001)       24 2023-05-04 20:41:15.000000 warrenapp-0.1.1/src/warrenapp/__init__.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      281 2023-05-04 23:54:00.000000 warrenapp-0.1.1/src/warrenapp/apps.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-08 18:57:45.554255 warrenapp-0.1.1/src/warrenapp/badelf_tools/
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     4776 2023-05-08 18:36:02.000000 warrenapp-0.1.1/src/warrenapp/badelf_tools/acf.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)    20158 2023-05-04 20:41:15.000000 warrenapp-0.1.1/src/warrenapp/badelf_tools/badelf_algorithm_functions.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)    13809 2023-05-08 16:36:29.000000 warrenapp-0.1.1/src/warrenapp/badelf_tools/utilities.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)     5179 2023-05-08 18:36:04.000000 warrenapp-0.1.1/src/warrenapp/models.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-08 18:57:45.554255 warrenapp-0.1.1/src/warrenapp/workflows/
+-rw-r--r--   0 sweav     (1001) sweav     (1001)     1394 2023-05-08 18:36:04.000000 warrenapp-0.1.1/src/warrenapp/workflows/__init__.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-08 18:57:45.558255 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/
+-rw-r--r--   0 sweav     (1001) sweav     (1001)     1177 2023-05-08 18:36:04.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/__init__.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)     1703 2023-05-08 18:36:02.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/badelf_hse.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)     1387 2023-05-05 00:04:23.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/badelf_pbe.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)     1712 2023-05-08 18:36:04.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/bader_badelf_hse.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)     1350 2023-05-08 15:51:16.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/bader_badelf_pbe.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      931 2023-05-08 18:36:04.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/bader_badelf_relaxation_hse.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      874 2023-05-08 18:36:04.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/bader_badelf_relaxation_pbe.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)     1595 2023-05-08 18:36:02.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/bader_hse.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)     1401 2023-05-05 00:04:23.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/bader_pbe.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)    15457 2023-05-08 15:20:27.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/base.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      903 2023-05-04 23:50:58.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/elf_hse.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      903 2023-05-04 23:50:58.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/elf_pbe.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     2171 2023-05-08 18:36:04.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/relaxation_base.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)    13893 2023-05-05 00:04:23.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/warren_badelf_v3_7.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-08 18:57:45.558255 warrenapp-0.1.1/src/warrenapp/workflows/relaxation/
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      296 2023-05-04 20:41:15.000000 warrenapp-0.1.1/src/warrenapp/workflows/relaxation/__init__.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      624 2023-05-04 23:52:02.000000 warrenapp-0.1.1/src/warrenapp/workflows/relaxation/hse.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      545 2023-05-04 23:52:02.000000 warrenapp-0.1.1/src/warrenapp/workflows/relaxation/hsesol.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)     4621 2023-05-05 00:04:23.000000 warrenapp-0.1.1/src/warrenapp/workflows/relaxation/pbe.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      503 2023-05-04 23:52:02.000000 warrenapp-0.1.1/src/warrenapp/workflows/relaxation/pbe_metal.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      443 2023-05-04 23:52:02.000000 warrenapp-0.1.1/src/warrenapp/workflows/relaxation/pbesol.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      702 2023-05-04 23:52:02.000000 warrenapp-0.1.1/src/warrenapp/workflows/relaxation/scan.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-08 18:57:45.558255 warrenapp-0.1.1/src/warrenapp/workflows/static_energy/
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      364 2023-05-08 17:14:12.000000 warrenapp-0.1.1/src/warrenapp/workflows/static_energy/__init__.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      431 2023-05-04 23:53:18.000000 warrenapp-0.1.1/src/warrenapp/workflows/static_energy/hse.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      449 2023-05-04 23:53:18.000000 warrenapp-0.1.1/src/warrenapp/workflows/static_energy/hsesol.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      764 2023-05-08 17:18:15.000000 warrenapp-0.1.1/src/warrenapp/workflows/static_energy/pbe.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      474 2023-05-04 23:53:18.000000 warrenapp-0.1.1/src/warrenapp/workflows/static_energy/pbe_metal.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      567 2023-05-08 18:34:55.000000 warrenapp-0.1.1/src/warrenapp/workflows/static_energy/pbesol.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      437 2023-05-04 23:53:18.000000 warrenapp-0.1.1/src/warrenapp/workflows/static_energy/scan.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     2137 2023-05-08 18:36:04.000000 warrenapp-0.1.1/src/warrenapp/workflows/static_energy/seeded_hse.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-08 18:57:45.554255 warrenapp-0.1.1/src/warrenapp.egg-info/
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     3615 2023-05-08 18:57:45.000000 warrenapp-0.1.1/src/warrenapp.egg-info/PKG-INFO
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     2016 2023-05-08 18:57:45.000000 warrenapp-0.1.1/src/warrenapp.egg-info/SOURCES.txt
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)        1 2023-05-08 18:57:45.000000 warrenapp-0.1.1/src/warrenapp.egg-info/dependency_links.txt
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)        8 2023-05-08 18:57:45.000000 warrenapp-0.1.1/src/warrenapp.egg-info/requires.txt
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)       10 2023-05-08 18:57:45.000000 warrenapp-0.1.1/src/warrenapp.egg-info/top_level.txt
```

### Comparing `warrenapp-0.1.0/LICENSE` & `warrenapp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.0/PKG-INFO` & `warrenapp-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warrenapp
-Version: 0.1.0
+Version: 0.1.1
 Summary: The Warrenapp is an extension of the Simulated Materials Ecosystem (Simmate), a package designed to ease computational materials research. The WarrenApp adds several custom workflows and settings.
 Author-email: Sam Weaver <sweav@unc.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Sam M. Weaver
         All rights reserved.
```

### Comparing `warrenapp-0.1.0/README.md` & `warrenapp-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.0/pyproject.toml` & `warrenapp-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend= "setuptools.build_meta"
 
 [project]
 name = "warrenapp"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = ["simmate"]
 description = "The Warrenapp is an extension of the Simulated Materials Ecosystem (Simmate), a package designed to ease computational materials research. The WarrenApp adds several custom workflows and settings."
 readme = "README.md"
 requires-python=">=3.10"
 authors = [{ name = "Sam Weaver", email = "sweav@unc.edu" }]
 license = { file = "LICENSE" }
```

### Comparing `warrenapp-0.1.0/src/warrenapp/badelf_tools/badelf_algorithm_functions.py` & `warrenapp-0.1.1/src/warrenapp/badelf_tools/badelf_algorithm_functions.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.0/src/warrenapp/badelf_tools/utilities.py` & `warrenapp-0.1.1/src/warrenapp/badelf_tools/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,15 +289,14 @@
     check_required_files(directory=directory, required_files=required_files)
     # Get number of lines to replace in teh ELFCAR
     lines_to_replace = structure.num_sites + 8
     # Run for each file
     for density_file in density_files:
         # Open CHGCAR or ELFCAR and add all of the lines past the structure info
         # to a list.
-        print("hi")
         file = open(directory / f"{density_file}", "r")
         early_lines_to_keep = []
         later_lines_to_keep = []
         for i, line in enumerate(file):
             if i < 5:
                 early_lines_to_keep.append(line)
             elif i > lines_to_replace:
```

### Comparing `warrenapp-0.1.0/src/warrenapp/models.py` & `warrenapp-0.1.1/src/warrenapp/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
 from pandas import DataFrame
-from simmate.apps.bader.outputs import ACF
 from simmate.database.base_data_types import StaticEnergy, table_column
 
+from warrenapp.badelf_tools.acf import ACF
 from warrenapp.badelf_tools.utilities import get_electride_num
 
 
 class WarrenPopulationAnalysis(StaticEnergy):
     """
     This table combines results from a static energy calculation and the follow-up
     oxidation analysis on the charge density.
```

### Comparing `warrenapp-0.1.0/src/warrenapp/workflows/__init__.py` & `warrenapp-0.1.1/src/warrenapp/workflows/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # -*- coding: utf-8 -*-
 
 from .population_analysis import (
     PopulationAnalysis__Warren__BadelfHse,
     PopulationAnalysis__Warren__BadelfPbe,
     PopulationAnalysis__Warren__BaderBadelfHse,
     PopulationAnalysis__Warren__BaderBadelfPbe,
+    PopulationAnalysis__Warren__BaderBadelfRelaxationHse,
+    PopulationAnalysis__Warren__BaderBadelfRelaxationPbe,
     PopulationAnalysis__Warren__BaderHse,
     PopulationAnalysis__Warren__BaderPbe,
     PopulationAnalysis__Warren__ElfHse,
     PopulationAnalysis__Warren__ElfPbe,
     StaticEnergy__Warren__PrebadelfHse,
     StaticEnergy__Warren__PrebadelfPbe,
+    StaticEnergy__Warren__PrebadelfSeededHse,
     StaticEnergy__Warren__PrebaderbadelfHse,
     StaticEnergy__Warren__PrebaderbadelfPbe,
+    StaticEnergy__Warren__PrebaderbadelfSeededHse,
     StaticEnergy__Warren__PrebaderHse,
     StaticEnergy__Warren__PrebaderPbe,
+    StaticEnergy__Warren__PrebaderSeededHse,
 )
 from .relaxation import (
     Relaxation__Warren__Hse,
     Relaxation__Warren__Hsesol,
     Relaxation__Warren__Pbe,
     Relaxation__Warren__PbeMetal,
     Relaxation__Warren__Pbesol,
@@ -27,8 +32,9 @@
 from .static_energy import (
     StaticEnergy__Warren__Hse,
     StaticEnergy__Warren__Hsesol,
     StaticEnergy__Warren__Pbe,
     StaticEnergy__Warren__PbeMetal,
     StaticEnergy__Warren__Pbesol,
     StaticEnergy__Warren__Scan,
+    StaticEnergy__Warren__SeededHse,
 )
```

### Comparing `warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/__init__.py` & `warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 # -*- coding: utf-8 -*-
 
 from .badelf_hse import (
     PopulationAnalysis__Warren__BadelfHse,
     StaticEnergy__Warren__PrebadelfHse,
+    StaticEnergy__Warren__PrebadelfSeededHse,
 )
 from .badelf_pbe import (
     PopulationAnalysis__Warren__BadelfPbe,
     StaticEnergy__Warren__PrebadelfPbe,
 )
 from .bader_badelf_hse import (
     PopulationAnalysis__Warren__BaderBadelfHse,
     StaticEnergy__Warren__PrebaderbadelfHse,
+    StaticEnergy__Warren__PrebaderbadelfSeededHse,
 )
 from .bader_badelf_pbe import (
     PopulationAnalysis__Warren__BaderBadelfPbe,
     StaticEnergy__Warren__PrebaderbadelfPbe,
 )
+from .bader_badelf_relaxation_hse import (
+    PopulationAnalysis__Warren__BaderBadelfRelaxationHse,
+)
+from .bader_badelf_relaxation_pbe import (
+    PopulationAnalysis__Warren__BaderBadelfRelaxationPbe,
+)
 from .bader_hse import (
     PopulationAnalysis__Warren__BaderHse,
     StaticEnergy__Warren__PrebaderHse,
+    StaticEnergy__Warren__PrebaderSeededHse,
 )
 from .bader_pbe import (
     PopulationAnalysis__Warren__BaderPbe,
     StaticEnergy__Warren__PrebaderPbe,
 )
 from .elf_hse import PopulationAnalysis__Warren__ElfHse
 from .elf_pbe import PopulationAnalysis__Warren__ElfPbe
```

### Comparing `warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/badelf_hse.py` & `warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/badelf_pbe.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # -*- coding: utf-8 -*-
 
 from warrenapp.workflows.population_analysis.base import (
     VaspBadElfBase,
     prebadelf_incar_settings,
 )
-from warrenapp.workflows.static_energy.hse import StaticEnergy__Warren__Hse
+from warrenapp.workflows.static_energy.pbe import StaticEnergy__Warren__Pbe
 
 
-class StaticEnergy__Warren__PrebadelfHse(StaticEnergy__Warren__Hse):
+class StaticEnergy__Warren__PrebadelfPbe(StaticEnergy__Warren__Pbe):
     """
-    Runs a static energy calculation with a high-density FFT grid under HSE
-    settings from the Warren Lab. Results can be used for Bader analysis where
+    Runs a static energy calculation with a high-density FFT grid under settings
+    from the Warren Lab. Results can be used for Bader analysis where
     the ELF is used as the reference instead of the CHGCAR.
 
     We do NOT recommend running this calculation on its own. Instead, you should
     use the full workflow, which runs this calculation AND the following bader
     analysis for you. This S3Task is only the first step of that workflow.
     """
 
     # The key thing for bader analysis is that we need a very fine FFT mesh. Other
     # than that, it's the same as a static energy calculation.
-    incar = StaticEnergy__Warren__Hse.incar.copy()
+    incar = StaticEnergy__Warren__Pbe.incar.copy()
     incar.update(prebadelf_incar_settings)
 
 
-class PopulationAnalysis__Warren__BadelfHse(VaspBadElfBase):
+class PopulationAnalysis__Warren__BadelfPbe(VaspBadElfBase):
     """
     Runs a static energy calculation using an extra-fine FFT grid and then
     carries out Bader analysis on the resulting charge density using the ELFCAR
-    as a reference when partitioning. Uses the HSE functional and settings from
+    as a reference when partitioning. Uses the PBE functional and settings from
     the Warren Lab.
     """
 
-    static_energy_prebadelf = StaticEnergy__Warren__PrebadelfHse
+    static_energy_prebadelf = StaticEnergy__Warren__PrebadelfPbe
```

### Comparing `warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/badelf_pbe.py` & `warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/badelf_hse.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 # -*- coding: utf-8 -*-
 
 from warrenapp.workflows.population_analysis.base import (
     VaspBadElfBase,
     prebadelf_incar_settings,
 )
-from warrenapp.workflows.static_energy.pbe import StaticEnergy__Warren__Pbe
+from warrenapp.workflows.static_energy import StaticEnergy__Warren__SeededHse
+from warrenapp.workflows.static_energy.hse import StaticEnergy__Warren__Hse
 
 
-class StaticEnergy__Warren__PrebadelfPbe(StaticEnergy__Warren__Pbe):
+class StaticEnergy__Warren__PrebadelfHse(StaticEnergy__Warren__Hse):
     """
-    Runs a static energy calculation with a high-density FFT grid under settings
-    from the Warren Lab. Results can be used for Bader analysis where
+    Runs a static energy calculation with a high-density FFT grid under HSE
+    settings from the Warren Lab. Results can be used for Bader analysis where
     the ELF is used as the reference instead of the CHGCAR.
 
     We do NOT recommend running this calculation on its own. Instead, you should
     use the full workflow, which runs this calculation AND the following bader
     analysis for you. This S3Task is only the first step of that workflow.
     """
 
     # The key thing for bader analysis is that we need a very fine FFT mesh. Other
     # than that, it's the same as a static energy calculation.
-    incar = StaticEnergy__Warren__Pbe.incar.copy()
+    incar = StaticEnergy__Warren__Hse.incar.copy()
     incar.update(prebadelf_incar_settings)
 
 
-class PopulationAnalysis__Warren__BadelfPbe(VaspBadElfBase):
+# We prefer to use a workflow that seeds the HSE calculation with a PBE calculation
+class StaticEnergy__Warren__PrebadelfSeededHse(StaticEnergy__Warren__SeededHse):
+
+    second_calculation = StaticEnergy__Warren__PrebadelfHse
+
+
+class PopulationAnalysis__Warren__BadelfHse(VaspBadElfBase):
     """
     Runs a static energy calculation using an extra-fine FFT grid and then
     carries out Bader analysis on the resulting charge density using the ELFCAR
-    as a reference when partitioning. Uses the PBE functional and settings from
+    as a reference when partitioning. Uses the HSE functional and settings from
     the Warren Lab.
     """
 
-    static_energy_prebadelf = StaticEnergy__Warren__PrebadelfPbe
+    static_energy_prebadelf = StaticEnergy__Warren__PrebadelfSeededHse
```

### Comparing `warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/bader_badelf_hse.py` & `warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/bader_badelf_pbe.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # -*- coding: utf-8 -*-
 
+
 from simmate.engine.workflow import Workflow
 
 from warrenapp.workflows.population_analysis.base import (
     VaspBaderBadElfBase,
     prebadelf_incar_settings,
 )
-from warrenapp.workflows.static_energy import StaticEnergy__Warren__Hse
+from warrenapp.workflows.static_energy.pbe import StaticEnergy__Warren__Pbe
 
 
-class StaticEnergy__Warren__PrebaderbadelfHse(StaticEnergy__Warren__Hse):
+class StaticEnergy__Warren__PrebaderbadelfPbe(StaticEnergy__Warren__Pbe):
     """
-    Runs a static energy calculation with a high-density FFT grid under HSE
-    settings from the Warren Lab. Results can be used for BadLEF analysis.
+    Runs a static energy calculation with a high-density FFT grid setting and
+    PBE functional. Results can be used for BadELF analysis.
 
     We do NOT recommend running this calculation on its own. Instead, you should
     use the full workflow, which runs this calculation AND the following bader
     analysis for you. This S3Task is only the first step of that workflow.
     """
 
     # The key thing for bader analysis is that we need a very fine FFT mesh. Other
     # than that, it's the same as a static energy calculation.
-    incar = StaticEnergy__Warren__Hse.incar.copy()
+    incar = StaticEnergy__Warren__Pbe.incar.copy()
     incar.update(prebadelf_incar_settings)
 
 
-class PopulationAnalysis__Warren__BaderBadelfHse(VaspBaderBadElfBase):
+class PopulationAnalysis__Warren__BaderBadelfPbe(VaspBaderBadElfBase):
     """
     Runs a static energy calculation using an extra-fine FFT grid using vasp
     and then carries out Badelf and Bader analysis on the resulting charge density.
-    Uses the Warren lab settings HSE settings.
+    Uses the Warren lab settings PBE settings.
     """
 
-    static_energy_prebadelf: Workflow = StaticEnergy__Warren__PrebaderbadelfHse
+    static_energy_prebadelf: Workflow = StaticEnergy__Warren__PrebaderbadelfPbe
```

### Comparing `warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/bader_badelf_pbe.py` & `warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/bader_pbe.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 # -*- coding: utf-8 -*-
 
-
-from simmate.engine.workflow import Workflow
-
+from warrenapp.workflows.population_analysis.badelf_pbe import (
+    StaticEnergy__Warren__PrebadelfPbe,
+)
 from warrenapp.workflows.population_analysis.base import (
-    VaspBaderBadElfBase,
-    prebadelf_incar_settings,
+    VaspBaderBase,
+    prebader_incar_settings,
 )
 from warrenapp.workflows.static_energy.pbe import StaticEnergy__Warren__Pbe
 
 
-class StaticEnergy__Warren__PrebaderbadelfPbe(StaticEnergy__Warren__Pbe):
+class StaticEnergy__Warren__PrebaderPbe(StaticEnergy__Warren__Pbe):
     """
-    Runs a static energy calculation with a high-density FFT grid setting and
-    PBE functional. Results can be used for BadELF analysis.
+    Runs a static energy calculation with a high-density FFT grid setting.
+    Results can be used for Bader analysis.
 
     We do NOT recommend running this calculation on its own. Instead, you should
     use the full workflow, which runs this calculation AND the following bader
     analysis for you. This S3Task is only the first step of that workflow.
     """
 
     # The key thing for bader analysis is that we need a very fine FFT mesh. Other
     # than that, it's the same as a static energy calculation.
     incar = StaticEnergy__Warren__Pbe.incar.copy()
-    incar.update(prebadelf_incar_settings)
+    incar.update(prebader_incar_settings)
 
 
-# !!!I would like to move most of this to the base file because that's where
-# similar code is currently.!!!
-class PopulationAnalysis__Warren__BaderBadelfPbe(VaspBaderBadElfBase):
+class PopulationAnalysis__Warren__BaderPbe(VaspBaderBase):
     """
     Runs a static energy calculation using an extra-fine FFT grid using vasp
-    and then carries out Badelf and Bader analysis on the resulting charge density.
+    and then carries out Bader analysis on the resulting charge density.
     Uses the Warren lab settings PBE settings.
     """
 
-    static_energy_prebadelf: Workflow = StaticEnergy__Warren__PrebaderbadelfPbe
+    static_energy_prebader = StaticEnergy__Warren__PrebaderPbe
+    static_energy_prebadelf = StaticEnergy__Warren__PrebadelfPbe
```

### Comparing `warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/bader_hse.py` & `warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/bader_badelf_hse.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 # -*- coding: utf-8 -*-
 
-from warrenapp.workflows.population_analysis.badelf_hse import (
-    StaticEnergy__Warren__PrebadelfHse,
-)
+from simmate.engine.workflow import Workflow
+
 from warrenapp.workflows.population_analysis.base import (
-    VaspBaderBase,
-    prebader_incar_settings,
+    VaspBaderBadElfBase,
+    prebadelf_incar_settings,
+)
+from warrenapp.workflows.static_energy import (
+    StaticEnergy__Warren__Hse,
+    StaticEnergy__Warren__SeededHse,
 )
-from warrenapp.workflows.static_energy.hse import StaticEnergy__Warren__Hse
 
 
-class StaticEnergy__Warren__PrebaderHse(StaticEnergy__Warren__Hse):
+class StaticEnergy__Warren__PrebaderbadelfHse(StaticEnergy__Warren__Hse):
     """
-    Runs a static energy calculation with a high-density FFT grid setting.
-    Results can be used for Bader analysis.
+    Runs a static energy calculation with a high-density FFT grid under HSE
+    settings from the Warren Lab. Results can be used for BadELF analysis.
 
     We do NOT recommend running this calculation on its own. Instead, you should
     use the full workflow, which runs this calculation AND the following bader
     analysis for you. This S3Task is only the first step of that workflow.
     """
 
     # The key thing for bader analysis is that we need a very fine FFT mesh. Other
     # than that, it's the same as a static energy calculation.
     incar = StaticEnergy__Warren__Hse.incar.copy()
-    incar.update(prebader_incar_settings)
+    incar.update(prebadelf_incar_settings)
+
+
+# We prefer to use a workflow that seeds the HSE calculation with a PBE calculation.
+# This is inherited from our static energy seeded_hse workflow.
+class StaticEnergy__Warren__PrebaderbadelfSeededHse(StaticEnergy__Warren__SeededHse):
+
+    second_calculation = StaticEnergy__Warren__PrebaderbadelfHse
 
 
-class PopulationAnalysis__Warren__BaderHse(VaspBaderBase):
+class PopulationAnalysis__Warren__BaderBadelfHse(VaspBaderBadElfBase):
     """
     Runs a static energy calculation using an extra-fine FFT grid using vasp
-    and then carries out Bader analysis on the resulting charge density.
-    Uses the Warren lab HSE settings.
+    and then carries out Badelf and Bader analysis on the resulting charge density.
+    Uses the Warren lab settings HSE settings.
     """
 
-    static_energy_prebader = StaticEnergy__Warren__PrebaderHse
+    static_energy_prebadelf: Workflow = StaticEnergy__Warren__PrebaderbadelfSeededHse
```

### Comparing `warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/base.py` & `warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
     @classmethod
     def run_config(
         cls,
         structure: Structure,
         command: str = None,
         source: dict = None,
-        find_empties: bool = False,
+        find_empties: bool = True,
         directory: Path = None,
         **kwargs,
     ):
         if find_empties:
             # Run static energy calculation
             prebader_result = cls.static_energy_prebadelf.run(
                 structure=structure,
```

### Comparing `warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/elf_hse.py` & `warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/elf_hse.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/elf_pbe.py` & `warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/elf_pbe.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.0/src/warrenapp/workflows/population_analysis/warren_badelf_v3_7.py` & `warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/warren_badelf_v3_7.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.0/src/warrenapp/workflows/relaxation/hse.py` & `warrenapp-0.1.1/src/warrenapp/workflows/relaxation/hse.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.0/src/warrenapp/workflows/relaxation/hsesol.py` & `warrenapp-0.1.1/src/warrenapp/workflows/relaxation/hsesol.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.0/src/warrenapp/workflows/relaxation/pbe.py` & `warrenapp-0.1.1/src/warrenapp/workflows/relaxation/pbe.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.0/src/warrenapp/workflows/relaxation/scan.py` & `warrenapp-0.1.1/src/warrenapp/workflows/relaxation/scan.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.0/src/warrenapp/workflows/static_energy/pbe.py` & `warrenapp-0.1.1/src/warrenapp/workflows/static_energy/pbe.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 static_settings = dict(
     IBRION=-1,  # (optional) locks everything between ionic steps
     NSW=0,  # this is the main static energy setting
     #            LAECHG=True, # currently only set in population analysis
     LCHARG=True,
     LORBIT=11,
     LVHAR=True,
-    LWAVE=False,
+    LWAVE=True,
     ALGO="Normal",  # was "Fast" before
 )
 # These settings are saved here to make it easier to add them to other static
 # energy workflows
 
 
 class StaticEnergy__Warren__Pbe(Relaxation__Warren__Pbe):
```

### Comparing `warrenapp-0.1.0/src/warrenapp.egg-info/PKG-INFO` & `warrenapp-0.1.1/src/warrenapp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warrenapp
-Version: 0.1.0
+Version: 0.1.1
 Summary: The Warrenapp is an extension of the Simulated Materials Ecosystem (Simmate), a package designed to ease computational materials research. The WarrenApp adds several custom workflows and settings.
 Author-email: Sam Weaver <sweav@unc.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Sam M. Weaver
         All rights reserved.
```

### Comparing `warrenapp-0.1.0/src/warrenapp.egg-info/SOURCES.txt` & `warrenapp-0.1.1/src/warrenapp.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,35 +6,40 @@
 src/warrenapp/apps.py
 src/warrenapp/models.py
 src/warrenapp.egg-info/PKG-INFO
 src/warrenapp.egg-info/SOURCES.txt
 src/warrenapp.egg-info/dependency_links.txt
 src/warrenapp.egg-info/requires.txt
 src/warrenapp.egg-info/top_level.txt
+src/warrenapp/badelf_tools/acf.py
 src/warrenapp/badelf_tools/badelf_algorithm_functions.py
 src/warrenapp/badelf_tools/utilities.py
 src/warrenapp/workflows/__init__.py
 src/warrenapp/workflows/population_analysis/__init__.py
 src/warrenapp/workflows/population_analysis/badelf_hse.py
 src/warrenapp/workflows/population_analysis/badelf_pbe.py
 src/warrenapp/workflows/population_analysis/bader_badelf_hse.py
 src/warrenapp/workflows/population_analysis/bader_badelf_pbe.py
+src/warrenapp/workflows/population_analysis/bader_badelf_relaxation_hse.py
+src/warrenapp/workflows/population_analysis/bader_badelf_relaxation_pbe.py
 src/warrenapp/workflows/population_analysis/bader_hse.py
 src/warrenapp/workflows/population_analysis/bader_pbe.py
 src/warrenapp/workflows/population_analysis/base.py
 src/warrenapp/workflows/population_analysis/elf_hse.py
 src/warrenapp/workflows/population_analysis/elf_pbe.py
+src/warrenapp/workflows/population_analysis/relaxation_base.py
 src/warrenapp/workflows/population_analysis/warren_badelf_v3_7.py
 src/warrenapp/workflows/relaxation/__init__.py
 src/warrenapp/workflows/relaxation/hse.py
 src/warrenapp/workflows/relaxation/hsesol.py
 src/warrenapp/workflows/relaxation/pbe.py
 src/warrenapp/workflows/relaxation/pbe_metal.py
 src/warrenapp/workflows/relaxation/pbesol.py
 src/warrenapp/workflows/relaxation/scan.py
 src/warrenapp/workflows/static_energy/__init__.py
 src/warrenapp/workflows/static_energy/hse.py
 src/warrenapp/workflows/static_energy/hsesol.py
 src/warrenapp/workflows/static_energy/pbe.py
 src/warrenapp/workflows/static_energy/pbe_metal.py
 src/warrenapp/workflows/static_energy/pbesol.py
-src/warrenapp/workflows/static_energy/scan.py
+src/warrenapp/workflows/static_energy/scan.py
+src/warrenapp/workflows/static_energy/seeded_hse.py
```

