# Comparing `tmp/openai_api_call-0.3.8.tar.gz` & `tmp/openai_api_call-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_api_call-0.3.8.tar", last modified: Mon Apr 17 13:36:36 2023, max compression
+gzip compressed data, was "openai_api_call-0.3.9.tar", last modified: Mon May  8 01:47:42 2023, max compression
```

## Comparing `openai_api_call-0.3.8.tar` & `openai_api_call-0.3.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:36:36.493137 openai_api_call-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-17 13:36:24.000000 openai_api_call-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-17 13:36:36.493137 openai_api_call-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-17 13:36:24.000000 openai_api_call-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:36:36.489138 openai_api_call-0.3.8/openai_api_call/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-17 13:36:24.000000 openai_api_call-0.3.8/openai_api_call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-04-17 13:36:24.000000 openai_api_call-0.3.8/openai_api_call/chattool.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-17 13:36:24.000000 openai_api_call-0.3.8/openai_api_call/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-17 13:36:24.000000 openai_api_call-0.3.8/openai_api_call/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-17 13:36:24.000000 openai_api_call-0.3.8/openai_api_call/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-17 13:36:24.000000 openai_api_call-0.3.8/openai_api_call/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:36:36.489138 openai_api_call-0.3.8/openai_api_call.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-17 13:36:36.000000 openai_api_call-0.3.8/openai_api_call.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-17 13:36:36.000000 openai_api_call-0.3.8/openai_api_call.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:36:36.000000 openai_api_call-0.3.8/openai_api_call.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 13:36:36.000000 openai_api_call-0.3.8/openai_api_call.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:36:36.000000 openai_api_call-0.3.8/openai_api_call.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 13:36:36.000000 openai_api_call-0.3.8/openai_api_call.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 13:36:36.000000 openai_api_call-0.3.8/openai_api_call.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 13:36:36.493137 openai_api_call-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-17 13:36:24.000000 openai_api_call-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:47:42.665205 openai_api_call-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-08 01:47:31.000000 openai_api_call-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-08 01:47:42.665205 openai_api_call-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-08 01:47:31.000000 openai_api_call-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:47:42.665205 openai_api_call-0.3.9/openai_api_call/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-08 01:47:31.000000 openai_api_call-0.3.9/openai_api_call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-05-08 01:47:31.000000 openai_api_call-0.3.9/openai_api_call/chattool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-08 01:47:31.000000 openai_api_call-0.3.9/openai_api_call/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-08 01:47:31.000000 openai_api_call-0.3.9/openai_api_call/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-08 01:47:31.000000 openai_api_call-0.3.9/openai_api_call/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-08 01:47:31.000000 openai_api_call-0.3.9/openai_api_call/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:47:42.665205 openai_api_call-0.3.9/openai_api_call.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-08 01:47:42.000000 openai_api_call-0.3.9/openai_api_call.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-08 01:47:42.000000 openai_api_call-0.3.9/openai_api_call.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 01:47:42.000000 openai_api_call-0.3.9/openai_api_call.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 01:47:42.000000 openai_api_call-0.3.9/openai_api_call.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 01:47:42.000000 openai_api_call-0.3.9/openai_api_call.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-08 01:47:42.000000 openai_api_call-0.3.9/openai_api_call.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 01:47:42.000000 openai_api_call-0.3.9/openai_api_call.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 01:47:42.665205 openai_api_call-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-08 01:47:31.000000 openai_api_call-0.3.9/setup.py
```

### Comparing `openai_api_call-0.3.8/LICENSE` & `openai_api_call-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.8/PKG-INFO` & `openai_api_call-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: openai_api_call
-Version: 0.3.8
+Version: 0.3.9
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/RexWzh/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
         
         # Openai API call
         [![PyPI version](https://img.shields.io/pypi/v/openai_api_call.svg)](https://pypi.python.org/pypi/openai_api_call)
         [![Tests](https://github.com/RexWzh/openai_api_call/actions/workflows/test.yml/badge.svg)](https://github.com/RexWzh/openai_api_call/actions/workflows/test.yml/)
         [![Documentation Status](https://img.shields.io/badge/docs-github_pages-blue.svg)](https://apicall.wzhecnu.cn)
+        [![Coverage](https://codecov.io/gh/RexWzh/openai_api_call/branch/master/graph/badge.svg)](https://codecov.io/gh/RexWzh/openai_api_call.jl)
         
         <!-- 
         [![Updates](https://pyup.io/repos/github/RexWzh/openai_api_call/shield.svg)](https://pyup.io/repos/github/RexWzh/openai_api_call/) 
         -->
         
         A simple wrapper for OpenAI API, which can be used to send requests and get responses.
```

### Comparing `openai_api_call-0.3.8/README.md` & `openai_api_call-0.3.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 > **中文文档移步[这里](README_zh_CN.md)。**
 
 # Openai API call
 [![PyPI version](https://img.shields.io/pypi/v/openai_api_call.svg)](https://pypi.python.org/pypi/openai_api_call)
 [![Tests](https://github.com/RexWzh/openai_api_call/actions/workflows/test.yml/badge.svg)](https://github.com/RexWzh/openai_api_call/actions/workflows/test.yml/)
 [![Documentation Status](https://img.shields.io/badge/docs-github_pages-blue.svg)](https://apicall.wzhecnu.cn)
+[![Coverage](https://codecov.io/gh/RexWzh/openai_api_call/branch/master/graph/badge.svg)](https://codecov.io/gh/RexWzh/openai_api_call.jl)
 
 <!-- 
 [![Updates](https://pyup.io/repos/github/RexWzh/openai_api_call/shield.svg)](https://pyup.io/repos/github/RexWzh/openai_api_call/) 
 -->
 
 A simple wrapper for OpenAI API, which can be used to send requests and get responses.
```

### Comparing `openai_api_call-0.3.8/openai_api_call/__init__.py` & `openai_api_call-0.3.9/openai_api_call/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Openai API call."""
 
 __author__ = """Rex Wang"""
 __email__ = '1073853456@qq.com'
-__version__ = '0.3.8'
+__version__ = '0.3.9'
 
 import os
 from .chattool import Chat, Resp, chat_completion, usage_status
 from .proxy import proxy_on, proxy_off, proxy_status
 
 # read API key from the environment variable
 if os.environ.get('OPENAI_API_KEY') is not None:
```

### Comparing `openai_api_call-0.3.8/openai_api_call/chattool.py` & `openai_api_call-0.3.9/openai_api_call/chattool.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,25 +129,29 @@
         for day in dailyusage:
             date = datetime.datetime.fromtimestamp(day.get("timestamp")).strftime("%Y-%m-%d")
             line_items = day.get("line_items")
             cost = sum([item.get("cost") for item in line_items]) / 100
             status[-1].update({date: cost})
         return status
     
-    def show_usage_status(self, recent:int=10, duration:int=99):
+    def show_usage_status(self, thismonth:bool=True, recent:int=10, duration:int=99):
         """Show the usage status
         
         Args:
+            thismonth (bool): 
             recent (int, optional): number of the usage of recent days. Defaults to 10.
             duration (int, optional): duration of the usage. Defaults to 99.
         """
+        if thismonth:
+            duration = datetime.datetime.now().day - 1
         storage, usage, rem, recent_usage = self.get_usage_status(recent=recent, duration=duration)
         print(f"Total account: {storage:.4f}$")
-        print(f"Total usage: {usage:.4f}$")
-        print(f"Total remaining: {rem:.4f}$")
+        print(f"Total usage(the last {len(recent_usage)} days): {usage:.4f}$")
+        if thismonth:
+            print(f"Total remaining(this month): {rem:.4f}$")
         for date, cost in recent_usage.items():
             print(f"{date}: {cost:.4f}$")
 
     def add(self, role:str, msg:str):
         """Add a message to the chat log"""
         assert role in ['user', 'assistant', 'system'], "role should be 'user', 'assistant' or 'system'"
         self._chat_log.append({"role": role, "content": msg})
```

### Comparing `openai_api_call-0.3.8/openai_api_call/proxy.py` & `openai_api_call-0.3.9/openai_api_call/proxy.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.8/openai_api_call/request.py` & `openai_api_call-0.3.9/openai_api_call/request.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.8/openai_api_call/response.py` & `openai_api_call-0.3.9/openai_api_call/response.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.8/openai_api_call.egg-info/PKG-INFO` & `openai_api_call-0.3.9/openai_api_call.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: openai-api-call
-Version: 0.3.8
+Version: 0.3.9
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/RexWzh/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
         
         # Openai API call
         [![PyPI version](https://img.shields.io/pypi/v/openai_api_call.svg)](https://pypi.python.org/pypi/openai_api_call)
         [![Tests](https://github.com/RexWzh/openai_api_call/actions/workflows/test.yml/badge.svg)](https://github.com/RexWzh/openai_api_call/actions/workflows/test.yml/)
         [![Documentation Status](https://img.shields.io/badge/docs-github_pages-blue.svg)](https://apicall.wzhecnu.cn)
+        [![Coverage](https://codecov.io/gh/RexWzh/openai_api_call/branch/master/graph/badge.svg)](https://codecov.io/gh/RexWzh/openai_api_call.jl)
         
         <!-- 
         [![Updates](https://pyup.io/repos/github/RexWzh/openai_api_call/shield.svg)](https://pyup.io/repos/github/RexWzh/openai_api_call/) 
         -->
         
         A simple wrapper for OpenAI API, which can be used to send requests and get responses.
```

### Comparing `openai_api_call-0.3.8/setup.py` & `openai_api_call-0.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
-VERSION = '0.3.8'
+VERSION = '0.3.9'
 
 requirements = ['Click>=7.0', 'requests>=2.20']
 
 test_requirements = ['pytest>=3', 'unittest']
 
 setup(
     author="Rex Wang",
```

