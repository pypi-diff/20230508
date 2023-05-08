# Comparing `tmp/eeecalc-0.0.6.tar.gz` & `tmp/eeecalc-0.0.7.tar.gz`

## Comparing `eeecalc-0.0.6.tar` & `eeecalc-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.0.6/.DS_Store
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.0.6/.idea/.gitignore
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.0.6/.idea/base-eeeCalc.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 eeecalc-0.0.6/.idea/misc.xml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 eeecalc-0.0.6/.idea/modules.xml
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 eeecalc-0.0.6/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.0.6/src/.DS_Store
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 eeecalc-0.0.6/src/eeeCalc/__init__.py
--rwxr-xr-x   0        0        0      615 2020-02-02 00:00:00.000000 eeecalc-0.0.6/src/eeeCalc/dBtoRatio.py
--rwxr-xr-x   0        0        0     4801 2020-02-02 00:00:00.000000 eeecalc-0.0.6/src/eeeCalc/filter.py
--rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 eeecalc-0.0.6/src/eeeCalc/general.py
--rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 eeecalc-0.0.6/src/eeeCalc/phasors.py
--rwxr-xr-x   0        0        0     1842 2020-02-02 00:00:00.000000 eeecalc-0.0.6/src/eeeCalc/secondDegreeDiffEq.py
--rwxr-xr-x   0        0        0      480 2020-02-02 00:00:00.000000 eeecalc-0.0.6/src/eeeCalc/signalFunctions.py
--rwxr-xr-x   0        0        0     2244 2020-02-02 00:00:00.000000 eeecalc-0.0.6/src/eeeCalc/transferFunctionPlot.py
--rwxr-xr-x   0        0        0      338 2020-02-02 00:00:00.000000 eeecalc-0.0.6/src/eeeCalc/trigFunc.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.0.6/src/eeeCalc/.idea/.gitignore
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.0.6/src/eeeCalc/.idea/eeeCalc.iml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 eeecalc-0.0.6/src/eeeCalc/.idea/misc.xml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 eeecalc-0.0.6/src/eeeCalc/.idea/modules.xml
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 eeecalc-0.0.6/src/eeeCalc/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.0.6/src/eeeCalc/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 eeecalc-0.0.6/LICENSE
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 eeecalc-0.0.6/README.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 eeecalc-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 eeecalc-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.0.7/.DS_Store
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.0.7/.idea/.gitignore
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.0.7/.idea/base-eeeCalc.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 eeecalc-0.0.7/.idea/misc.xml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 eeecalc-0.0.7/.idea/modules.xml
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 eeecalc-0.0.7/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.0.7/src/.DS_Store
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 eeecalc-0.0.7/src/eeeCalc/__init__.py
+-rwxr-xr-x   0        0        0      615 2020-02-02 00:00:00.000000 eeecalc-0.0.7/src/eeeCalc/dBtoRatio.py
+-rwxr-xr-x   0        0        0     4801 2020-02-02 00:00:00.000000 eeecalc-0.0.7/src/eeeCalc/filter.py
+-rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 eeecalc-0.0.7/src/eeeCalc/general.py
+-rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 eeecalc-0.0.7/src/eeeCalc/phasors.py
+-rwxr-xr-x   0        0        0     1842 2020-02-02 00:00:00.000000 eeecalc-0.0.7/src/eeeCalc/secondDegreeDiffEq.py
+-rwxr-xr-x   0        0        0      480 2020-02-02 00:00:00.000000 eeecalc-0.0.7/src/eeeCalc/signalFunctions.py
+-rwxr-xr-x   0        0        0     2244 2020-02-02 00:00:00.000000 eeecalc-0.0.7/src/eeeCalc/transferFunctionPlot.py
+-rwxr-xr-x   0        0        0      338 2020-02-02 00:00:00.000000 eeecalc-0.0.7/src/eeeCalc/trigFunc.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.0.7/src/eeeCalc/.idea/.gitignore
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.0.7/src/eeeCalc/.idea/eeeCalc.iml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 eeecalc-0.0.7/src/eeeCalc/.idea/misc.xml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 eeecalc-0.0.7/src/eeeCalc/.idea/modules.xml
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 eeecalc-0.0.7/src/eeeCalc/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.0.7/src/eeeCalc/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 eeecalc-0.0.7/LICENSE
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 eeecalc-0.0.7/README.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 eeecalc-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 eeecalc-0.0.7/PKG-INFO
```

### Comparing `eeecalc-0.0.6/.DS_Store` & `eeecalc-0.0.7/.DS_Store`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.6/.idea/workspace.xml` & `eeecalc-0.0.7/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.6/src/.DS_Store` & `eeecalc-0.0.7/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.6/src/eeeCalc/dBtoRatio.py` & `eeecalc-0.0.7/src/eeeCalc/dBtoRatio.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.6/src/eeeCalc/filter.py` & `eeecalc-0.0.7/src/eeeCalc/filter.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.6/src/eeeCalc/general.py` & `eeecalc-0.0.7/src/eeeCalc/general.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.6/src/eeeCalc/phasors.py` & `eeecalc-0.0.7/src/eeeCalc/phasors.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.6/src/eeeCalc/secondDegreeDiffEq.py` & `eeecalc-0.0.7/src/eeeCalc/secondDegreeDiffEq.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.6/src/eeeCalc/transferFunctionPlot.py` & `eeecalc-0.0.7/src/eeeCalc/transferFunctionPlot.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.6/src/eeeCalc/.idea/workspace.xml` & `eeecalc-0.0.7/src/eeeCalc/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.6/LICENSE` & `eeecalc-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.6/pyproject.toml` & `eeecalc-0.0.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "eeeCalc"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Kevin Johnson", email="john2003.kjj@gmail.com" },
 ]
 description = "Package to aid electrical engineering calculations"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

