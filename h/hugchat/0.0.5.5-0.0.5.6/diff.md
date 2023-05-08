# Comparing `tmp/hugchat-0.0.5.5.tar.gz` & `tmp/hugchat-0.0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugchat-0.0.5.5.tar", last modified: Fri May  5 14:27:26 2023, max compression
+gzip compressed data, was "hugchat-0.0.5.6.tar", last modified: Mon May  8 09:40:36 2023, max compression
```

## Comparing `hugchat-0.0.5.5.tar` & `hugchat-0.0.5.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 14:27:26.165608 hugchat-0.0.5.5/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34523 2023-05-01 00:33:11.000000 hugchat-0.0.5.5/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2874 2023-05-05 14:27:26.161608 hugchat-0.0.5.5/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1854 2023-05-05 02:29:43.000000 hugchat-0.0.5.5/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-05 14:27:26.165608 hugchat-0.0.5.5/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1436 2023-05-05 14:26:47.000000 hugchat-0.0.5.5/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 14:27:26.161608 hugchat-0.0.5.5/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 14:27:26.161608 hugchat-0.0.5.5/src/hugchat/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:54:22.000000 hugchat-0.0.5.5/src/hugchat/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      179 2023-05-03 15:54:22.000000 hugchat-0.0.5.5/src/hugchat/cli.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8764 2023-05-05 14:25:32.000000 hugchat-0.0.5.5/src/hugchat/hugchat.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 14:27:26.161608 hugchat-0.0.5.5/src/hugchat.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2874 2023-05-05 14:27:26.000000 hugchat-0.0.5.5/src/hugchat.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      266 2023-05-05 14:27:26.000000 hugchat-0.0.5.5/src/hugchat.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-05 14:27:26.000000 hugchat-0.0.5.5/src/hugchat.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       27 2023-05-05 14:27:26.000000 hugchat-0.0.5.5/src/hugchat.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-05-05 14:27:26.000000 hugchat-0.0.5.5/src/hugchat.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-08 09:40:36.088144 hugchat-0.0.5.6/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34523 2023-05-01 00:33:11.000000 hugchat-0.0.5.6/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3217 2023-05-08 09:40:36.088144 hugchat-0.0.5.6/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2197 2023-05-08 09:39:22.000000 hugchat-0.0.5.6/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-08 09:40:36.088144 hugchat-0.0.5.6/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1436 2023-05-08 09:40:13.000000 hugchat-0.0.5.6/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-08 09:40:36.080144 hugchat-0.0.5.6/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-08 09:40:36.084144 hugchat-0.0.5.6/src/hugchat/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:54:22.000000 hugchat-0.0.5.6/src/hugchat/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      179 2023-05-03 15:54:22.000000 hugchat-0.0.5.6/src/hugchat/cli.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9752 2023-05-08 09:39:29.000000 hugchat-0.0.5.6/src/hugchat/hugchat.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-08 09:40:36.088144 hugchat-0.0.5.6/src/hugchat.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3217 2023-05-08 09:40:35.000000 hugchat-0.0.5.6/src/hugchat.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      266 2023-05-08 09:40:35.000000 hugchat-0.0.5.6/src/hugchat.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-08 09:40:35.000000 hugchat-0.0.5.6/src/hugchat.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       27 2023-05-08 09:40:35.000000 hugchat-0.0.5.6/src/hugchat.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-05-08 09:40:35.000000 hugchat-0.0.5.6/src/hugchat.egg-info/top_level.txt
```

### Comparing `hugchat-0.0.5.5/LICENSE` & `hugchat-0.0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hugchat-0.0.5.5/PKG-INFO` & `hugchat-0.0.5.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.0.5.5
+Version: 0.0.5.6
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -30,14 +30,18 @@
 
 [![PyPi](https://img.shields.io/pypi/v/hugchat.svg)](https://pypi.python.org/pypi/hugchat)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/hugchat)](https://pypi.python.org/pypi/hugchat)
 [![Downloads](https://static.pepy.tech/badge/hugchat)](https://pypi.python.org/pypi/hugchat)
 
 Leave a star :)
 
+> When you use this project, it means that you have agreed to the following two requirements of the HuggingChat: 
+> 1. AI is an area of active research with known problems such as biased generation and misinformation. Do not use this application for high-stakes decisions or advice.
+> 2. Your conversations will be shared with model authors.
+
 ## How to Use
 
 ### Basic mode
 
 ```bash
 pip install hugchat
 ```
```

### Comparing `hugchat-0.0.5.5/README.md` & `hugchat-0.0.5.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 
 [![PyPi](https://img.shields.io/pypi/v/hugchat.svg)](https://pypi.python.org/pypi/hugchat)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/hugchat)](https://pypi.python.org/pypi/hugchat)
 [![Downloads](https://static.pepy.tech/badge/hugchat)](https://pypi.python.org/pypi/hugchat)
 
 Leave a star :)
 
+> When you use this project, it means that you have agreed to the following two requirements of the HuggingChat: 
+> 1. AI is an area of active research with known problems such as biased generation and misinformation. Do not use this application for high-stakes decisions or advice.
+> 2. Your conversations will be shared with model authors.
+
 ## How to Use
 
 ### Basic mode
 
 ```bash
 pip install hugchat
 ```
```

### Comparing `hugchat-0.0.5.5/setup.py` & `hugchat-0.0.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_namespace_packages
 from setuptools import setup
 
 setup(
     name="hugchat",
-    version="0.0.5.5",
+    version="0.0.5.6",
     description="A huggingchat python api.",
     long_description=open("README.md", "rt", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Soulter/hugging-chat-api",
     project_urls={
         "Bug Report": "https://github.com/Soulter/hugging-chat-api/issues"
     },
```

### Comparing `hugchat-0.0.5.5/src/hugchat.egg-info/PKG-INFO` & `hugchat-0.0.5.6/src/hugchat.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.0.5.5
+Version: 0.0.5.6
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -30,14 +30,18 @@
 
 [![PyPi](https://img.shields.io/pypi/v/hugchat.svg)](https://pypi.python.org/pypi/hugchat)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/hugchat)](https://pypi.python.org/pypi/hugchat)
 [![Downloads](https://static.pepy.tech/badge/hugchat)](https://pypi.python.org/pypi/hugchat)
 
 Leave a star :)
 
+> When you use this project, it means that you have agreed to the following two requirements of the HuggingChat: 
+> 1. AI is an area of active research with known problems such as biased generation and misinformation. Do not use this application for high-stakes decisions or advice.
+> 2. Your conversations will be shared with model authors.
+
 ## How to Use
 
 ### Basic mode
 
 ```bash
 pip install hugchat
 ```
```

