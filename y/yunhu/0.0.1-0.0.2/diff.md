# Comparing `tmp/yunhu-0.0.1.tar.gz` & `tmp/yunhu-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunhu-0.0.1.tar", last modified: Mon May  8 08:03:32 2023, max compression
+gzip compressed data, was "yunhu-0.0.2.tar", last modified: Mon May  8 08:54:32 2023, max compression
```

## Comparing `yunhu-0.0.1.tar` & `yunhu-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 08:03:32.893365 yunhu-0.0.1/
--rw-rw-rw-   0        0        0     1094 2023-05-08 06:42:50.000000 yunhu-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      545 2023-05-08 08:03:32.893365 yunhu-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-05-08 06:42:00.000000 yunhu-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 08:03:32.883365 yunhu-0.0.1/example/
--rw-rw-rw-   0        0        0        0 2023-04-24 04:05:16.000000 yunhu-0.0.1/example/__init__.py
--rw-rw-rw-   0        0        0     2426 2023-05-08 01:21:14.000000 yunhu-0.0.1/example/flask_demo.py
--rw-rw-rw-   0        0        0      369 2023-05-08 08:00:05.000000 yunhu-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 08:03:32.893365 yunhu-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      725 2023-05-08 07:56:47.000000 yunhu-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:03:32.887364 yunhu-0.0.1/yhChat/
--rw-rw-rw-   0        0        0       26 2023-04-24 07:46:11.000000 yunhu-0.0.1/yhChat/__init__.py
--rw-rw-rw-   0        0        0       69 2023-05-08 01:21:22.000000 yunhu-0.0.1/yhChat/main.py
--rw-rw-rw-   0        0        0     2694 2023-04-25 08:55:43.000000 yunhu-0.0.1/yhChat/openapi.py
--rw-rw-rw-   0        0        0     2158 2023-04-25 07:39:22.000000 yunhu-0.0.1/yhChat/subscription.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:03:32.892366 yunhu-0.0.1/yunhu.egg-info/
--rw-rw-rw-   0        0        0      545 2023-05-08 08:03:32.000000 yunhu-0.0.1/yunhu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-05-08 08:03:32.000000 yunhu-0.0.1/yunhu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 08:03:32.000000 yunhu-0.0.1/yunhu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-08 08:03:32.000000 yunhu-0.0.1/yunhu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 08:54:32.098799 yunhu-0.0.2/
+-rw-rw-rw-   0        0        0     1094 2023-05-08 06:42:50.000000 yunhu-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      545 2023-05-08 08:54:32.098799 yunhu-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-05-08 06:42:00.000000 yunhu-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 08:54:32.085586 yunhu-0.0.2/example_yunhu/
+-rw-rw-rw-   0        0        0        0 2023-04-24 04:05:16.000000 yunhu-0.0.2/example_yunhu/__init__.py
+-rw-rw-rw-   0        0        0     2424 2023-05-08 08:53:16.000000 yunhu-0.0.2/example_yunhu/flask_demo.py
+-rw-rw-rw-   0        0        0      369 2023-05-08 08:45:47.000000 yunhu-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 08:54:32.098799 yunhu-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      725 2023-05-08 08:53:02.000000 yunhu-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 08:54:32.091592 yunhu-0.0.2/yunhu/
+-rw-rw-rw-   0        0        0       26 2023-04-24 07:46:11.000000 yunhu-0.0.2/yunhu/__init__.py
+-rw-rw-rw-   0        0        0       69 2023-05-08 01:21:22.000000 yunhu-0.0.2/yunhu/main.py
+-rw-rw-rw-   0        0        0     2694 2023-04-25 08:55:43.000000 yunhu-0.0.2/yunhu/openapi.py
+-rw-rw-rw-   0        0        0     2158 2023-04-25 07:39:22.000000 yunhu-0.0.2/yunhu/subscription.py
+drwxrwxrwx   0        0        0        0 2023-05-08 08:54:32.097799 yunhu-0.0.2/yunhu.egg-info/
+-rw-rw-rw-   0        0        0      545 2023-05-08 08:54:32.000000 yunhu-0.0.2/yunhu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-05-08 08:54:32.000000 yunhu-0.0.2/yunhu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 08:54:32.000000 yunhu-0.0.2/yunhu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-08 08:54:32.000000 yunhu-0.0.2/yunhu.egg-info/top_level.txt
```

### Comparing `yunhu-0.0.1/LICENSE.txt` & `yunhu-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yunhu-0.0.1/PKG-INFO` & `yunhu-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunhu
-Version: 0.0.1
+Version: 0.0.2
 Summary: 云湖官方Python SDK
 Author: yunhu
 Author-email: yunhu <1114110051@qq.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `yunhu-0.0.1/example/flask_demo.py` & `yunhu-0.0.2/example_yunhu/flask_demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import sys
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 
 from flask import Flask, request
 import json
 import requests
-from yhChat.subscription import Subscription
-from yhChat.openapi import Openapi
+from yunhu.subscription import Subscription
+from yunhu.openapi import Openapi
 
 
 app = Flask(__name__)
 sub = Subscription()
 openapi = Openapi("xxx")
 
 @app.route('/sub',methods = ['POST'])
```

### Comparing `yunhu-0.0.1/setup.py` & `yunhu-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="yunhu", 
-    version="0.0.1", 
+    version="0.0.2", 
     author="yunhu",  
     description="云湖官方Python SDK", #包的简述
     author_email="1114110051@qq.com",    
     long_description=long_description,    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yunhu-0.0.1/yhChat/openapi.py` & `yunhu-0.0.2/yunhu/openapi.py`

 * *Files identical despite different names*

### Comparing `yunhu-0.0.1/yhChat/subscription.py` & `yunhu-0.0.2/yunhu/subscription.py`

 * *Files identical despite different names*

### Comparing `yunhu-0.0.1/yunhu.egg-info/PKG-INFO` & `yunhu-0.0.2/yunhu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunhu
-Version: 0.0.1
+Version: 0.0.2
 Summary: 云湖官方Python SDK
 Author: yunhu
 Author-email: yunhu <1114110051@qq.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

