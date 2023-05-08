# Comparing `tmp/eeecalc-0.0.3.tar.gz` & `tmp/eeecalc-0.0.4.tar.gz`

## Comparing `eeecalc-0.0.3.tar` & `eeecalc-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.0.3/.DS_Store
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.0.3/.idea/.gitignore
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.0.3/.idea/base-eeeCalc.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 eeecalc-0.0.3/.idea/misc.xml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 eeecalc-0.0.3/.idea/modules.xml
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 eeecalc-0.0.3/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.0.3/src/.DS_Store
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 eeecalc-0.0.3/src/eeeCalc/__init__.py
--rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 eeecalc-0.0.3/src/eeeCalc/dBtoRatio.py
--rwxr-xr-x   0        0        0     4921 2020-02-02 00:00:00.000000 eeecalc-0.0.3/src/eeeCalc/filter.py
--rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 eeecalc-0.0.3/src/eeeCalc/general.py
--rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 eeecalc-0.0.3/src/eeeCalc/phasors.py
--rwxr-xr-x   0        0        0     1842 2020-02-02 00:00:00.000000 eeecalc-0.0.3/src/eeeCalc/secondDegreeDiffEq.py
--rwxr-xr-x   0        0        0      480 2020-02-02 00:00:00.000000 eeecalc-0.0.3/src/eeeCalc/signalFunctions.py
--rwxr-xr-x   0        0        0     2244 2020-02-02 00:00:00.000000 eeecalc-0.0.3/src/eeeCalc/transferFunctionPlot.py
--rwxr-xr-x   0        0        0      338 2020-02-02 00:00:00.000000 eeecalc-0.0.3/src/eeeCalc/trigFunc.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.0.3/src/eeeCalc/.idea/.gitignore
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.0.3/src/eeeCalc/.idea/eeeCalc.iml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 eeecalc-0.0.3/src/eeeCalc/.idea/misc.xml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 eeecalc-0.0.3/src/eeeCalc/.idea/modules.xml
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 eeecalc-0.0.3/src/eeeCalc/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.0.3/src/eeeCalc/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 eeecalc-0.0.3/LICENSE
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 eeecalc-0.0.3/README.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 eeecalc-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 eeecalc-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.0.4/.DS_Store
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.0.4/.idea/.gitignore
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.0.4/.idea/base-eeeCalc.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 eeecalc-0.0.4/.idea/misc.xml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 eeecalc-0.0.4/.idea/modules.xml
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 eeecalc-0.0.4/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.0.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.0.4/src/.DS_Store
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 eeecalc-0.0.4/src/eeeCalc/__init__.py
+-rwxr-xr-x   0        0        0      615 2020-02-02 00:00:00.000000 eeecalc-0.0.4/src/eeeCalc/dBtoRatio.py
+-rwxr-xr-x   0        0        0     5118 2020-02-02 00:00:00.000000 eeecalc-0.0.4/src/eeeCalc/filter.py
+-rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 eeecalc-0.0.4/src/eeeCalc/general.py
+-rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 eeecalc-0.0.4/src/eeeCalc/phasors.py
+-rwxr-xr-x   0        0        0     1842 2020-02-02 00:00:00.000000 eeecalc-0.0.4/src/eeeCalc/secondDegreeDiffEq.py
+-rwxr-xr-x   0        0        0      480 2020-02-02 00:00:00.000000 eeecalc-0.0.4/src/eeeCalc/signalFunctions.py
+-rwxr-xr-x   0        0        0     2244 2020-02-02 00:00:00.000000 eeecalc-0.0.4/src/eeeCalc/transferFunctionPlot.py
+-rwxr-xr-x   0        0        0      338 2020-02-02 00:00:00.000000 eeecalc-0.0.4/src/eeeCalc/trigFunc.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.0.4/src/eeeCalc/.idea/.gitignore
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.0.4/src/eeeCalc/.idea/eeeCalc.iml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 eeecalc-0.0.4/src/eeeCalc/.idea/misc.xml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 eeecalc-0.0.4/src/eeeCalc/.idea/modules.xml
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 eeecalc-0.0.4/src/eeeCalc/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.0.4/src/eeeCalc/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 eeecalc-0.0.4/LICENSE
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 eeecalc-0.0.4/README.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 eeecalc-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 eeecalc-0.0.4/PKG-INFO
```

### Comparing `eeecalc-0.0.3/.DS_Store` & `eeecalc-0.0.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.3/.idea/workspace.xml` & `eeecalc-0.0.4/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.3/src/.DS_Store` & `eeecalc-0.0.4/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.3/src/eeeCalc/filter.py` & `eeecalc-0.0.4/src/eeeCalc/filter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import numpy as np
 from cmath import polar as pol
 from math import sin,cos,pi,e,ceil,log10 as log,log as ln,sqrt,acosh,asinh,cosh,sinh,fabs
 from dBtoRatio import *
 from transferFunctionPlot import transferFunctionPlot as tplt
 
 def ChebyshevPolynomial(n,x):
+    """
+    :param n: degree of chebyshev polynomial
+    :param x: value where chebyshev polynomial is evaluated
+    :return: uses recursion to calculate value of chebyshev polynomial at x
+    """
     if(n==0):
         return 1
     if(n==1):
         return x
     return 2*x*ChebyshevPolynomial(n-1,x) - ChebyshevPolynomial(n-2,x)
 
 def polarComplex(m,th):
```

### Comparing `eeecalc-0.0.3/src/eeeCalc/general.py` & `eeecalc-0.0.4/src/eeeCalc/general.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.3/src/eeeCalc/phasors.py` & `eeecalc-0.0.4/src/eeeCalc/phasors.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.3/src/eeeCalc/secondDegreeDiffEq.py` & `eeecalc-0.0.4/src/eeeCalc/secondDegreeDiffEq.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.3/src/eeeCalc/transferFunctionPlot.py` & `eeecalc-0.0.4/src/eeeCalc/transferFunctionPlot.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.3/src/eeeCalc/.idea/workspace.xml` & `eeecalc-0.0.4/src/eeeCalc/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.3/LICENSE` & `eeecalc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.3/pyproject.toml` & `eeecalc-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "eeeCalc"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Kevin Johnson", email="john2003.kjj@gmail.com" },
 ]
 description = "Package to aid electrical engineering calculations"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

