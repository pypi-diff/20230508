# Comparing `tmp/yunhu-0.0.2.tar.gz` & `tmp/yunhu-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunhu-0.0.2.tar", last modified: Mon May  8 08:54:32 2023, max compression
+gzip compressed data, was "yunhu-0.0.3.tar", last modified: Mon May  8 11:17:22 2023, max compression
```

## Comparing `yunhu-0.0.2.tar` & `yunhu-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 08:54:32.098799 yunhu-0.0.2/
--rw-rw-rw-   0        0        0     1094 2023-05-08 06:42:50.000000 yunhu-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      545 2023-05-08 08:54:32.098799 yunhu-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-05-08 06:42:00.000000 yunhu-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 08:54:32.085586 yunhu-0.0.2/example_yunhu/
--rw-rw-rw-   0        0        0        0 2023-04-24 04:05:16.000000 yunhu-0.0.2/example_yunhu/__init__.py
--rw-rw-rw-   0        0        0     2424 2023-05-08 08:53:16.000000 yunhu-0.0.2/example_yunhu/flask_demo.py
--rw-rw-rw-   0        0        0      369 2023-05-08 08:45:47.000000 yunhu-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 08:54:32.098799 yunhu-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      725 2023-05-08 08:53:02.000000 yunhu-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:54:32.091592 yunhu-0.0.2/yunhu/
--rw-rw-rw-   0        0        0       26 2023-04-24 07:46:11.000000 yunhu-0.0.2/yunhu/__init__.py
--rw-rw-rw-   0        0        0       69 2023-05-08 01:21:22.000000 yunhu-0.0.2/yunhu/main.py
--rw-rw-rw-   0        0        0     2694 2023-04-25 08:55:43.000000 yunhu-0.0.2/yunhu/openapi.py
--rw-rw-rw-   0        0        0     2158 2023-04-25 07:39:22.000000 yunhu-0.0.2/yunhu/subscription.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:54:32.097799 yunhu-0.0.2/yunhu.egg-info/
--rw-rw-rw-   0        0        0      545 2023-05-08 08:54:32.000000 yunhu-0.0.2/yunhu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-05-08 08:54:32.000000 yunhu-0.0.2/yunhu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 08:54:32.000000 yunhu-0.0.2/yunhu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-08 08:54:32.000000 yunhu-0.0.2/yunhu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 11:17:22.049909 yunhu-0.0.3/
+-rw-rw-rw-   0        0        0     1094 2023-05-08 06:42:50.000000 yunhu-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      610 2023-05-08 11:17:22.047904 yunhu-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-05-08 06:42:00.000000 yunhu-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 11:17:22.018753 yunhu-0.0.3/example_yunhu/
+-rw-rw-rw-   0        0        0        0 2023-04-24 04:05:16.000000 yunhu-0.0.3/example_yunhu/__init__.py
+-rw-rw-rw-   0        0        0     2424 2023-05-08 08:56:14.000000 yunhu-0.0.3/example_yunhu/flask_demo.py
+-rw-rw-rw-   0        0        0      426 2023-05-08 11:16:53.000000 yunhu-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 11:17:22.050907 yunhu-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      725 2023-05-08 11:16:54.000000 yunhu-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:17:22.032269 yunhu-0.0.3/yunhu/
+-rw-rw-rw-   0        0        0        0 2023-05-08 09:46:54.000000 yunhu-0.0.3/yunhu/__init__.py
+-rw-rw-rw-   0        0        0       69 2023-05-08 01:21:22.000000 yunhu-0.0.3/yunhu/main.py
+-rw-rw-rw-   0        0        0     2694 2023-04-25 08:55:43.000000 yunhu-0.0.3/yunhu/openapi.py
+-rw-rw-rw-   0        0        0     2158 2023-04-25 07:39:22.000000 yunhu-0.0.3/yunhu/subscription.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:17:22.045892 yunhu-0.0.3/yunhu.egg-info/
+-rw-rw-rw-   0        0        0      610 2023-05-08 11:17:21.000000 yunhu-0.0.3/yunhu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-05-08 11:17:21.000000 yunhu-0.0.3/yunhu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 11:17:21.000000 yunhu-0.0.3/yunhu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-08 11:17:21.000000 yunhu-0.0.3/yunhu.egg-info/top_level.txt
```

### Comparing `yunhu-0.0.2/LICENSE.txt` & `yunhu-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yunhu-0.0.2/PKG-INFO` & `yunhu-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: yunhu
-Version: 0.0.2
+Version: 0.0.3
 Summary: 云湖官方Python SDK
 Author: yunhu
 Author-email: yunhu <1114110051@qq.com>
+Project-URL: Homepage, https://github.com/yhchat/bot-python-sdk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `yunhu-0.0.2/example_yunhu/flask_demo.py` & `yunhu-0.0.3/example_yunhu/flask_demo.py`

 * *Files identical despite different names*

### Comparing `yunhu-0.0.2/setup.py` & `yunhu-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="yunhu", 
-    version="0.0.2", 
+    version="0.0.3", 
     author="yunhu",  
     description="云湖官方Python SDK", #包的简述
     author_email="1114110051@qq.com",    
     long_description=long_description,    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yunhu-0.0.2/yunhu/openapi.py` & `yunhu-0.0.3/yunhu/openapi.py`

 * *Files identical despite different names*

### Comparing `yunhu-0.0.2/yunhu/subscription.py` & `yunhu-0.0.3/yunhu/subscription.py`

 * *Files identical despite different names*

### Comparing `yunhu-0.0.2/yunhu.egg-info/PKG-INFO` & `yunhu-0.0.3/yunhu.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: yunhu
-Version: 0.0.2
+Version: 0.0.3
 Summary: 云湖官方Python SDK
 Author: yunhu
 Author-email: yunhu <1114110051@qq.com>
+Project-URL: Homepage, https://github.com/yhchat/bot-python-sdk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

