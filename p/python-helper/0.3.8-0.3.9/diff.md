# Comparing `tmp/python_helper-0.3.8.tar.gz` & `tmp/python_helper-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_helper-0.3.8.tar", last modified: Sat Sep 25 10:02:58 2021, max compression
+gzip compressed data, was "python_helper-0.3.9.tar", last modified: Wed Oct 13 01:55:53 2021, max compression
```

## Comparing `python_helper-0.3.8.tar` & `python_helper-0.3.9.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2021-09-25 10:02:58.337951 python_helper-0.3.8/
--rw-rw-rw-   0        0        0      672 2021-09-25 10:02:58.338862 python_helper-0.3.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-09-25 10:02:58.288859 python_helper-0.3.8/python_helper/
--rw-rw-rw-   0        0        0      752 2021-05-01 20:50:09.005437 python_helper-0.3.8/python_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-25 10:02:58.281859 python_helper-0.3.8/python_helper/api/
-drwxrwxrwx   0        0        0        0 2021-09-25 10:02:58.284863 python_helper-0.3.8/python_helper/api/src/
-drwxrwxrwx   0        0        0        0 2021-09-25 10:02:58.294862 python_helper-0.3.8/python_helper/api/src/annotation/
--rw-rw-rw-   0        0        0     1163 2021-01-26 14:47:34.836890 python_helper-0.3.8/python_helper/api/src/annotation/EnvironmentAnnotation.py
--rw-rw-rw-   0        0        0     1431 2021-09-24 18:15:23.191892 python_helper-0.3.8/python_helper/api/src/annotation/MethodAnnotation.py
--rw-rw-rw-   0        0        0     7663 2021-01-29 06:26:59.767867 python_helper-0.3.8/python_helper/api/src/annotation/TestAnnotation.py
-drwxrwxrwx   0        0        0        0 2021-09-25 10:02:58.295859 python_helper-0.3.8/python_helper/api/src/domain/
--rw-rw-rw-   0        0        0     5881 2021-09-24 18:18:21.347771 python_helper-0.3.8/python_helper/api/src/domain/Constant.py
-drwxrwxrwx   0        0        0        0 2021-09-25 10:02:58.318863 python_helper-0.3.8/python_helper/api/src/helper/
--rw-rw-rw-   0        0        0     8531 2021-09-25 06:54:34.597077 python_helper-0.3.8/python_helper/api/src/helper/LogHelperHelper.py
--rw-rw-rw-   0        0        0     1682 2021-02-07 03:47:35.830956 python_helper-0.3.8/python_helper/api/src/helper/ObjectHelperHelper.py
--rw-rw-rw-   0        0        0      611 2021-01-01 02:51:56.840024 python_helper-0.3.8/python_helper/api/src/helper/RandomHelperHelper.py
--rw-rw-rw-   0        0        0    30107 2021-03-18 00:46:10.493662 python_helper-0.3.8/python_helper/api/src/helper/SettingHelperHelper.py
--rw-rw-rw-   0        0        0     6228 2021-04-12 04:26:01.632108 python_helper-0.3.8/python_helper/api/src/helper/StringHelperHelper.py
-drwxrwxrwx   0        0        0        0 2021-09-25 10:02:58.336863 python_helper-0.3.8/python_helper/api/src/service/
--rw-rw-rw-   0        0        0     6686 2021-05-25 02:56:45.839953 python_helper-0.3.8/python_helper/api/src/service/DateTimeHelper.py
--rw-rw-rw-   0        0        0     3358 2021-09-24 23:07:27.346609 python_helper-0.3.8/python_helper/api/src/service/EnvironmentHelper.py
--rw-rw-rw-   0        0        0    12752 2021-09-24 18:18:44.312837 python_helper-0.3.8/python_helper/api/src/service/LogHelper.py
--rw-rw-rw-   0        0        0     6526 2021-08-29 15:33:43.894852 python_helper-0.3.8/python_helper/api/src/service/ObjectHelper.py
--rw-rw-rw-   0        0        0     2142 2021-01-01 02:52:41.847450 python_helper-0.3.8/python_helper/api/src/service/RandomHelper.py
--rw-rw-rw-   0        0        0    13514 2021-09-25 07:40:09.539438 python_helper-0.3.8/python_helper/api/src/service/ReflectionHelper.py
--rw-rw-rw-   0        0        0    12416 2021-03-16 02:49:53.469561 python_helper-0.3.8/python_helper/api/src/service/SettingHelper.py
--rw-rw-rw-   0        0        0     7303 2021-09-08 05:21:28.799772 python_helper-0.3.8/python_helper/api/src/service/StringHelper.py
--rw-rw-rw-   0        0        0    14843 2021-09-25 09:55:20.125668 python_helper-0.3.8/python_helper/api/src/service/TestHelper.py
--rw-rw-rw-   0        0        0       42 2020-07-08 02:57:32.031591 python_helper-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1318 2021-09-25 10:01:55.612850 python_helper-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-10-13 01:55:53.532439 python_helper-0.3.9/
+-rw-rw-rw-   0        0        0      672 2021-10-13 01:55:53.533435 python_helper-0.3.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2021-10-13 01:55:53.463434 python_helper-0.3.9/python_helper/
+-rw-rw-rw-   0        0        0      764 2021-09-29 01:21:50.395869 python_helper-0.3.9/python_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2021-10-13 01:55:53.442020 python_helper-0.3.9/python_helper/api/
+drwxrwxrwx   0        0        0        0 2021-10-13 01:55:53.457431 python_helper-0.3.9/python_helper/api/src/
+drwxrwxrwx   0        0        0        0 2021-10-13 01:55:53.474817 python_helper-0.3.9/python_helper/api/src/annotation/
+-rw-rw-rw-   0        0        0     1163 2021-01-26 14:47:34.836890 python_helper-0.3.9/python_helper/api/src/annotation/EnvironmentAnnotation.py
+-rw-rw-rw-   0        0        0     1431 2021-09-24 18:15:23.191892 python_helper-0.3.9/python_helper/api/src/annotation/MethodAnnotation.py
+-rw-rw-rw-   0        0        0     7663 2021-01-29 06:26:59.767867 python_helper-0.3.9/python_helper/api/src/annotation/TestAnnotation.py
+drwxrwxrwx   0        0        0        0 2021-10-13 01:55:53.480440 python_helper-0.3.9/python_helper/api/src/domain/
+-rw-rw-rw-   0        0        0     5881 2021-09-24 18:18:21.347771 python_helper-0.3.9/python_helper/api/src/domain/Constant.py
+drwxrwxrwx   0        0        0        0 2021-10-13 01:55:53.502431 python_helper-0.3.9/python_helper/api/src/helper/
+-rw-rw-rw-   0        0        0     8531 2021-09-25 06:54:34.597077 python_helper-0.3.9/python_helper/api/src/helper/LogHelperHelper.py
+-rw-rw-rw-   0        0        0     1682 2021-02-07 03:47:35.830956 python_helper-0.3.9/python_helper/api/src/helper/ObjectHelperHelper.py
+-rw-rw-rw-   0        0        0      611 2021-01-01 02:51:56.840024 python_helper-0.3.9/python_helper/api/src/helper/RandomHelperHelper.py
+-rw-rw-rw-   0        0        0    30107 2021-03-18 00:46:10.493662 python_helper-0.3.9/python_helper/api/src/helper/SettingHelperHelper.py
+-rw-rw-rw-   0        0        0     6228 2021-04-12 04:26:01.632108 python_helper-0.3.9/python_helper/api/src/helper/StringHelperHelper.py
+drwxrwxrwx   0        0        0        0 2021-10-13 01:55:53.530432 python_helper-0.3.9/python_helper/api/src/service/
+-rw-rw-rw-   0        0        0     6686 2021-05-25 02:56:45.839953 python_helper-0.3.9/python_helper/api/src/service/DateTimeHelper.py
+-rw-rw-rw-   0        0        0     3358 2021-09-24 23:07:27.346609 python_helper-0.3.9/python_helper/api/src/service/EnvironmentHelper.py
+-rw-rw-rw-   0        0        0      482 2021-10-13 01:53:59.960696 python_helper-0.3.9/python_helper/api/src/service/FileHelper.py
+-rw-rw-rw-   0        0        0    12752 2021-09-24 18:18:44.312837 python_helper-0.3.9/python_helper/api/src/service/LogHelper.py
+-rw-rw-rw-   0        0        0     6526 2021-08-29 15:33:43.894852 python_helper-0.3.9/python_helper/api/src/service/ObjectHelper.py
+-rw-rw-rw-   0        0        0     2142 2021-01-01 02:52:41.847450 python_helper-0.3.9/python_helper/api/src/service/RandomHelper.py
+-rw-rw-rw-   0        0        0    13514 2021-09-29 01:20:14.177707 python_helper-0.3.9/python_helper/api/src/service/ReflectionHelper.py
+-rw-rw-rw-   0        0        0    12384 2021-09-29 01:21:32.995113 python_helper-0.3.9/python_helper/api/src/service/SettingHelper.py
+-rw-rw-rw-   0        0        0     7303 2021-09-08 05:21:28.799772 python_helper-0.3.9/python_helper/api/src/service/StringHelper.py
+-rw-rw-rw-   0        0        0    14776 2021-09-25 10:11:09.100772 python_helper-0.3.9/python_helper/api/src/service/TestHelper.py
+-rw-rw-rw-   0        0        0       42 2020-07-08 02:57:32.031591 python_helper-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1318 2021-10-13 01:55:21.158934 python_helper-0.3.9/setup.py
```

### Comparing `python_helper-0.3.8/PKG-INFO` & `python_helper-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: python_helper
-Version: 0.3.8
+Version: 0.3.9
 Summary: python helper package
 Home-page: https://github.com/SamuelJansen/python_helper/
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
-Download-URL: https://github.com/SamuelJansen/python_helper/archive/v0.3.8.tar.gz
+Download-URL: https://github.com/SamuelJansen/python_helper/archive/v0.3.9.tar.gz
 Description: UNKNOWN
 Keywords: helper,python helper package,python helper,helper package
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `python_helper-0.3.8/python_helper/__init__.py` & `python_helper-0.3.9/python_helper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from python_helper.api.src.service import LogHelper as log
 from python_helper.api.src.domain import Constant
-from python_helper.api.src.service import ObjectHelper, SettingHelper, StringHelper, EnvironmentHelper, ReflectionHelper, RandomHelper, DateTimeHelper
+from python_helper.api.src.service import ObjectHelper, SettingHelper, StringHelper, EnvironmentHelper, ReflectionHelper, RandomHelper, DateTimeHelper, FileHelper
 from python_helper.api.src.helper import ObjectHelperHelper, SettingHelperHelper, SettingHelperHelper, LogHelperHelper, RandomHelperHelper
 from python_helper.api.src.annotation.EnvironmentAnnotation import EnvironmentVariable
 from python_helper.api.src.annotation.MethodAnnotation import Method, Function
 from python_helper.api.src.annotation import TestAnnotation
 from python_helper.api.src.annotation.TestAnnotation import Test
 from python_helper.api.src.service import TestHelper
```

### Comparing `python_helper-0.3.8/python_helper/api/src/annotation/EnvironmentAnnotation.py` & `python_helper-0.3.9/python_helper/api/src/annotation/EnvironmentAnnotation.py`

 * *Files identical despite different names*

### Comparing `python_helper-0.3.8/python_helper/api/src/annotation/MethodAnnotation.py` & `python_helper-0.3.9/python_helper/api/src/annotation/MethodAnnotation.py`

 * *Files identical despite different names*

### Comparing `python_helper-0.3.8/python_helper/api/src/annotation/TestAnnotation.py` & `python_helper-0.3.9/python_helper/api/src/annotation/TestAnnotation.py`

 * *Files identical despite different names*

### Comparing `python_helper-0.3.8/python_helper/api/src/domain/Constant.py` & `python_helper-0.3.9/python_helper/api/src/domain/Constant.py`

 * *Files identical despite different names*

### Comparing `python_helper-0.3.8/python_helper/api/src/helper/LogHelperHelper.py` & `python_helper-0.3.9/python_helper/api/src/helper/LogHelperHelper.py`

 * *Files identical despite different names*

### Comparing `python_helper-0.3.8/python_helper/api/src/helper/ObjectHelperHelper.py` & `python_helper-0.3.9/python_helper/api/src/helper/ObjectHelperHelper.py`

 * *Files identical despite different names*

### Comparing `python_helper-0.3.8/python_helper/api/src/helper/RandomHelperHelper.py` & `python_helper-0.3.9/python_helper/api/src/helper/RandomHelperHelper.py`

 * *Files identical despite different names*

### Comparing `python_helper-0.3.8/python_helper/api/src/helper/SettingHelperHelper.py` & `python_helper-0.3.9/python_helper/api/src/helper/SettingHelperHelper.py`

 * *Files identical despite different names*

### Comparing `python_helper-0.3.8/python_helper/api/src/helper/StringHelperHelper.py` & `python_helper-0.3.9/python_helper/api/src/helper/StringHelperHelper.py`

 * *Files identical despite different names*

### Comparing `python_helper-0.3.8/python_helper/api/src/service/DateTimeHelper.py` & `python_helper-0.3.9/python_helper/api/src/service/DateTimeHelper.py`

 * *Files identical despite different names*

### Comparing `python_helper-0.3.8/python_helper/api/src/service/EnvironmentHelper.py` & `python_helper-0.3.9/python_helper/api/src/service/EnvironmentHelper.py`

 * *Files identical despite different names*

### Comparing `python_helper-0.3.8/python_helper/api/src/service/LogHelper.py` & `python_helper-0.3.9/python_helper/api/src/service/LogHelper.py`

 * *Files identical despite different names*

### Comparing `python_helper-0.3.8/python_helper/api/src/service/ObjectHelper.py` & `python_helper-0.3.9/python_helper/api/src/service/ObjectHelper.py`

 * *Files identical despite different names*

### Comparing `python_helper-0.3.8/python_helper/api/src/service/RandomHelper.py` & `python_helper-0.3.9/python_helper/api/src/service/RandomHelper.py`

 * *Files identical despite different names*

### Comparing `python_helper-0.3.8/python_helper/api/src/service/ReflectionHelper.py` & `python_helper-0.3.9/python_helper/api/src/service/ReflectionHelper.py`

 * *Files identical despite different names*

### Comparing `python_helper-0.3.8/python_helper/api/src/service/SettingHelper.py` & `python_helper-0.3.9/python_helper/api/src/service/SettingHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from python_helper.api.src.service import StringHelper, LogHelper, ObjectHelper, EnvironmentHelper
+from python_helper.api.src.service import StringHelper, LogHelper, ObjectHelper, EnvironmentHelper, FileHelper
 from python_helper.api.src.domain import Constant as c
 from python_helper.api.src.helper import StringHelperHelper, SettingHelperHelper
 
 global ACTIVE_ENVIRONMENT_VALUE
 ACTIVE_ENVIRONMENT_VALUE = None
 
 ACTIVE_ENVIRONMENT = 'ACTIVE_ENVIRONMENT'
@@ -91,16 +91,15 @@
             lazyLoad = True,
             keepDepthInLongString = keepDepthInLongString,
             depthStep = depthStep,
             encoding = encoding
         )
     else :
         innerFallbackSettingTree = {}
-    with open(settingFilePath,c.READ,encoding=encoding) as settingsFile :
-        allSettingLines = settingsFile.readlines()
+    allSettingLines = FileHelper.getFileLines(settingFilePath, encoding=encoding)
     longStringCapturing = False
     quoteType = None
     longStringList = None
     depth = 0
     nodeRefference = 0
     nodeKey = c.NOTHING
     if settingTree is None :
```

### Comparing `python_helper-0.3.8/python_helper/api/src/service/StringHelper.py` & `python_helper-0.3.9/python_helper/api/src/service/StringHelper.py`

 * *Files identical despite different names*

### Comparing `python_helper-0.3.8/python_helper/api/src/service/TestHelper.py` & `python_helper-0.3.9/python_helper/api/src/service/TestHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,18 @@
     'argsOfCallBefore' : [GLOBALS_INSTANCE_LIST],
     'argsOfCallAfter' : [GLOBALS_INSTANCE_LIST],
     'returns' : RESULTS,
     'logResult' : False
 }
 
 def getRaisedException(callableThing, *args, **kwargs):
-    raisedException = None
     try:
         callableThing(*args, **kwargs)
     except Exception as exception:
-        raisedException = exception
-    return raisedException
+        return exception
 
 def getUnitTest(inspectGlobals, globalsInstance) :
     @Test(**getGlobalsTestKwargs(inspectGlobals, globalsInstance))
     def unitTest(testModule, testName, data, testReturns, logResult) :
         discountTimeEnd = time.time()
         unitTestException = None
         if logResult :
```

### Comparing `python_helper-0.3.8/setup.py` & `python_helper-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 import os
 
 OS_SEPARATOR = os.path.sep
 
-version = '0.3.8'
+version = '0.3.9'
 name = 'python_helper'
 url = f'https://github.com/SamuelJansen/{name}/'
 
 setup(
     name = name,
     packages = [
         name,
```

