# Comparing `tmp/birentechci-0.0.8.tar.gz` & `tmp/birentechci-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "birentechci-0.0.8.tar", last modified: Tue Apr 18 10:29:15 2023, max compression
+gzip compressed data, was "birentechci-0.0.9.tar", last modified: Tue Apr 18 10:56:38 2023, max compression
```

## Comparing `birentechci-0.0.8.tar` & `birentechci-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:29:15.649099 birentechci-0.0.8/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     2045 2023-04-18 10:29:15.649099 birentechci-0.0.8/PKG-INFO
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1609 2023-04-18 03:36:01.000000 birentechci-0.0.8/README.md
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:29:15.649099 birentechci-0.0.8/birentechci.egg-info/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     2045 2023-04-18 10:29:15.000000 birentechci-0.0.8/birentechci.egg-info/PKG-INFO
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      826 2023-04-18 10:29:15.000000 birentechci-0.0.8/birentechci.egg-info/SOURCES.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        1 2023-04-18 10:29:15.000000 birentechci-0.0.8/birentechci.egg-info/dependency_links.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       68 2023-04-18 10:29:15.000000 birentechci-0.0.8/birentechci.egg-info/requires.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        5 2023-04-18 10:29:15.000000 birentechci-0.0.8/birentechci.egg-info/top_level.txt
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:29:15.649099 birentechci-0.0.8/brci/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:17:20.000000 birentechci-0.0.8/brci/__init__.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:29:15.649099 birentechci-0.0.8/brci/apis/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/apis/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1530 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/apis/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/apis/client.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     4188 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/apis/pdu.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1932 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/apis/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1291 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/apis/pr.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:29:15.649099 birentechci-0.0.8/brci/config/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      378 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/config/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      175 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/config/develop.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/config/prod.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:29:15.649099 birentechci-0.0.8/brci/handles/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:28:58.000000 birentechci-0.0.8/brci/handles/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3694 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/handles/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3429 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/handles/pdu.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     7944 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/handles/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1502 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/handles/pr.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3309 2023-04-18 10:22:03.000000 birentechci-0.0.8/brci/main.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3697 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/run.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:29:15.649099 birentechci-0.0.8/brci/schemas/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/schemas/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      499 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/schemas/jenkins.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      619 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/schemas/pull_request.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      144 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/schemas/pull_request_job.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       94 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/schemas/test_case.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      540 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/test_hander_perf.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:29:15.649099 birentechci-0.0.8/brci/utils/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/utils/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1292 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/utils/csv_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      369 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/utils/file_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      269 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/utils/json_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       83 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/utils/pd_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      533 2023-04-18 03:37:21.000000 birentechci-0.0.8/brci/utils/xml_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-04-18 10:29:15.649099 birentechci-0.0.8/setup.cfg
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1148 2023-04-18 10:29:13.000000 birentechci-0.0.8/setup.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:56:38.486957 birentechci-0.0.9/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2008 2023-04-18 10:56:38.486957 birentechci-0.0.9/PKG-INFO
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1609 2023-04-18 10:45:04.000000 birentechci-0.0.9/README.md
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:56:38.486957 birentechci-0.0.9/birentechci.egg-info/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2008 2023-04-18 10:56:38.000000 birentechci-0.0.9/birentechci.egg-info/PKG-INFO
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      826 2023-04-18 10:56:38.000000 birentechci-0.0.9/birentechci.egg-info/SOURCES.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        1 2023-04-18 10:56:38.000000 birentechci-0.0.9/birentechci.egg-info/dependency_links.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       68 2023-04-18 10:56:38.000000 birentechci-0.0.9/birentechci.egg-info/requires.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        5 2023-04-18 10:56:38.000000 birentechci-0.0.9/birentechci.egg-info/top_level.txt
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:56:38.486957 birentechci-0.0.9/brci/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/__init__.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:56:38.486957 birentechci-0.0.9/brci/apis/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/apis/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1530 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/apis/build.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/apis/client.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     4188 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/apis/pdu.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1932 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/apis/perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1291 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/apis/pr.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:56:38.486957 birentechci-0.0.9/brci/config/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      378 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/config/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      175 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/config/develop.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/config/prod.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:56:38.486957 birentechci-0.0.9/brci/handles/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       11 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/handles/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3694 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/handles/build.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3429 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/handles/pdu.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     7944 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/handles/perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1502 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/handles/pr.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3308 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/main.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3697 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/run.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:56:38.486957 birentechci-0.0.9/brci/schemas/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/schemas/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      499 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/schemas/jenkins.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      619 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/schemas/pull_request.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      144 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/schemas/pull_request_job.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       94 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/schemas/test_case.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      540 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/test_hander_perf.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:56:38.486957 birentechci-0.0.9/brci/utils/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/utils/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1292 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/utils/csv_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      369 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/utils/file_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      269 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/utils/json_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       83 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/utils/pd_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      533 2023-04-18 10:45:04.000000 birentechci-0.0.9/brci/utils/xml_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-04-18 10:56:38.486957 birentechci-0.0.9/setup.cfg
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1148 2023-04-18 10:56:06.000000 birentechci-0.0.9/setup.py
```

### Comparing `birentechci-0.0.8/PKG-INFO` & `birentechci-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: birentechci
-Version: 0.0.8
+Version: 0.0.9
 Summary: biren ci sdk
 Home-page: https://gitlab.birentech.com/software/br_ci_db
 Author: br_infra
 Author-email: br_infra@birentech.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # 介绍
@@ -75,9 +73,7 @@
 install chromedriver
 wget http://chromedriver.storage.googleapis.com/105.0.5195.19/chromedriver_linux64.zip
 unzip chromedriver_linux64.zip
 chmod +x chromedriver
 sudo mv chromedriver /usr/local/share/chromedriver
 ```
 
-
-
```

### Comparing `birentechci-0.0.8/README.md` & `birentechci-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.8/birentechci.egg-info/PKG-INFO` & `birentechci-0.0.9/birentechci.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: birentechci
-Version: 0.0.8
+Version: 0.0.9
 Summary: biren ci sdk
 Home-page: https://gitlab.birentech.com/software/br_ci_db
 Author: br_infra
 Author-email: br_infra@birentech.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # 介绍
@@ -75,9 +73,7 @@
 install chromedriver
 wget http://chromedriver.storage.googleapis.com/105.0.5195.19/chromedriver_linux64.zip
 unzip chromedriver_linux64.zip
 chmod +x chromedriver
 sudo mv chromedriver /usr/local/share/chromedriver
 ```
 
-
-
```

### Comparing `birentechci-0.0.8/birentechci.egg-info/SOURCES.txt` & `birentechci-0.0.9/birentechci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.8/brci/apis/build.py` & `birentechci-0.0.9/brci/apis/build.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.8/brci/apis/client.py` & `birentechci-0.0.9/brci/apis/client.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.8/brci/apis/pdu.py` & `birentechci-0.0.9/brci/apis/pdu.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.8/brci/apis/perf.py` & `birentechci-0.0.9/brci/apis/perf.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.8/brci/apis/pr.py` & `birentechci-0.0.9/brci/apis/pr.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.8/brci/handles/build.py` & `birentechci-0.0.9/brci/handles/build.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.8/brci/handles/pdu.py` & `birentechci-0.0.9/brci/handles/pdu.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.8/brci/handles/perf.py` & `birentechci-0.0.9/brci/handles/perf.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.8/brci/handles/pr.py` & `birentechci-0.0.9/brci/handles/pr.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.8/brci/main.py` & `birentechci-0.0.9/brci/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import io
 import sys
 
-from .handles import build, pdu, perf, pr
+from handles import build, pdu, perf, pr
 
 sys.stdout = sys.__stdout__ = io.TextIOWrapper(
     sys.stdout.detach(), encoding="utf-8", line_buffering=True
 )
 sys.stderr = sys.__stderr__ = io.TextIOWrapper(
     sys.stderr.detach(), encoding="utf-8", line_buffering=True
 )
```

### Comparing `birentechci-0.0.8/brci/run.py` & `birentechci-0.0.9/brci/run.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.8/brci/schemas/pull_request.py` & `birentechci-0.0.9/brci/schemas/pull_request.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.8/brci/test_hander_perf.py` & `birentechci-0.0.9/brci/test_hander_perf.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.8/brci/utils/csv_utils.py` & `birentechci-0.0.9/brci/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.8/brci/utils/xml_utils.py` & `birentechci-0.0.9/brci/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.8/setup.py` & `birentechci-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         else:
             requires.append(pkg)
     return requires
 
 
 setuptools.setup(
     name="birentechci", 
-    version="0.0.8",    
+    version="0.0.9",    
     author="br_infra",    
     author_email="br_infra@birentech.com",    
     description="biren ci sdk",
     long_description=long_description,    
     long_description_content_type="text/markdown",
     url="https://gitlab.birentech.com/software/br_ci_db",    
     packages=setuptools.find_packages(),
```

