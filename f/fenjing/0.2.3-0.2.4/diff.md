# Comparing `tmp/fenjing-0.2.3.tar.gz` & `tmp/fenjing-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.2.3.tar", last modified: Sun May  7 11:01:08 2023, max compression
+gzip compressed data, was "fenjing-0.2.4.tar", last modified: Mon May  8 08:33:45 2023, max compression
```

## Comparing `fenjing-0.2.3.tar` & `fenjing-0.2.4.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-07 11:01:08.578000 fenjing-0.2.3/
--rw-r--r--   0 user      (1000) user      (1000)    16725 2023-03-31 12:04:28.000000 fenjing-0.2.3/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     4608 2023-05-07 11:01:08.578000 fenjing-0.2.3/PKG-INFO
--rwxr-xr-x   0 user      (1000) user      (1000)     4170 2023-05-07 05:47:36.000000 fenjing-0.2.3/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-07 11:01:08.573000 fenjing-0.2.3/fenjing/
--rwxr-xr-x   0 user      (1000) user      (1000)      146 2023-05-07 11:00:43.000000 fenjing-0.2.3/fenjing/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)       60 2023-03-31 08:38:41.000000 fenjing-0.2.3/fenjing/__main__.py
--rw-r--r--   0 user      (1000) user      (1000)     3473 2023-05-07 11:00:45.000000 fenjing-0.2.3/fenjing/cli.py
--rw-r--r--   0 user      (1000) user      (1000)      515 2023-05-07 05:22:05.000000 fenjing-0.2.3/fenjing/colorize.py
--rwxr-xr-x   0 user      (1000) user      (1000)      605 2023-05-07 05:47:36.000000 fenjing-0.2.3/fenjing/example.py
--rwxr-x---   0 user      (1000) user      (1000)       36 2023-03-31 08:02:21.000000 fenjing-0.2.3/fenjing/exceptions.py
--rw-r--r--   0 user      (1000) user      (1000)     2030 2023-05-07 05:22:05.000000 fenjing-0.2.3/fenjing/form.py
--rw-r--r--   0 user      (1000) user      (1000)     4709 2023-05-07 11:00:45.000000 fenjing-0.2.3/fenjing/form_cracker.py
--rwxr-xr-x   0 user      (1000) user      (1000)     2832 2023-04-26 05:00:35.000000 fenjing-0.2.3/fenjing/int_vars.py
--rwxr-xr-x   0 user      (1000) user      (1000)    39085 2023-04-26 05:00:35.000000 fenjing-0.2.3/fenjing/pattern.py
--rw-r--r--   0 user      (1000) user      (1000)    27484 2023-05-07 11:00:45.000000 fenjing-0.2.3/fenjing/payload_gen.py
--rw-r--r--   0 user      (1000) user      (1000)     1543 2023-05-07 05:22:05.000000 fenjing-0.2.3/fenjing/requester.py
--rw-r--r--   0 user      (1000) user      (1000)     1066 2023-05-07 11:00:43.000000 fenjing-0.2.3/fenjing/scan_url.py
--rwxr-xr-x   0 user      (1000) user      (1000)     2326 2023-05-07 11:00:45.000000 fenjing-0.2.3/fenjing/shell_payload.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-07 11:01:08.577000 fenjing-0.2.3/fenjing.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     4608 2023-05-07 11:01:08.000000 fenjing-0.2.3/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      464 2023-05-07 11:01:08.000000 fenjing-0.2.3/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-07 11:01:08.000000 fenjing-0.2.3/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       30 2023-05-07 11:01:08.000000 fenjing-0.2.3/fenjing.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2023-05-07 11:01:08.000000 fenjing-0.2.3/fenjing.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-07 11:01:08.579000 fenjing-0.2.3/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      860 2023-03-31 12:05:47.000000 fenjing-0.2.3/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-08 08:33:45.884000 fenjing-0.2.4/
+-rw-r--r--   0 user      (1000) user      (1000)    16725 2023-05-08 08:15:46.000000 fenjing-0.2.4/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     4600 2023-05-08 08:33:45.884000 fenjing-0.2.4/PKG-INFO
+-rwxr-xr-x   0 user      (1000) user      (1000)     4162 2023-05-08 08:32:55.000000 fenjing-0.2.4/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-08 08:33:45.884000 fenjing-0.2.4/fenjing/
+-rwxr-xr-x   0 user      (1000) user      (1000)      146 2023-05-08 08:32:55.000000 fenjing-0.2.4/fenjing/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)       60 2023-03-31 08:38:41.000000 fenjing-0.2.4/fenjing/__main__.py
+-rw-r--r--   0 user      (1000) user      (1000)     3789 2023-05-08 08:32:55.000000 fenjing-0.2.4/fenjing/cli.py
+-rw-r--r--   0 user      (1000) user      (1000)      515 2023-05-08 08:32:55.000000 fenjing-0.2.4/fenjing/colorize.py
+-rwxr-x---   0 user      (1000) user      (1000)       36 2023-03-31 08:02:21.000000 fenjing-0.2.4/fenjing/exceptions.py
+-rw-r--r--   0 user      (1000) user      (1000)     2030 2023-05-08 08:32:55.000000 fenjing-0.2.4/fenjing/form.py
+-rw-r--r--   0 user      (1000) user      (1000)     4709 2023-05-08 08:32:55.000000 fenjing-0.2.4/fenjing/form_cracker.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     2832 2023-04-26 05:00:35.000000 fenjing-0.2.4/fenjing/int_vars.py
+-rwxr-xr-x   0 user      (1000) user      (1000)    39085 2023-04-26 05:00:35.000000 fenjing-0.2.4/fenjing/pattern.py
+-rw-r--r--   0 user      (1000) user      (1000)    27484 2023-05-08 08:32:55.000000 fenjing-0.2.4/fenjing/payload_gen.py
+-rw-r--r--   0 user      (1000) user      (1000)     1543 2023-05-08 08:32:55.000000 fenjing-0.2.4/fenjing/requester.py
+-rw-r--r--   0 user      (1000) user      (1000)     1066 2023-05-08 08:32:55.000000 fenjing-0.2.4/fenjing/scan_url.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     2326 2023-05-08 08:32:55.000000 fenjing-0.2.4/fenjing/shell_payload.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-08 08:33:45.884000 fenjing-0.2.4/fenjing.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     4600 2023-05-08 08:33:45.000000 fenjing-0.2.4/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      445 2023-05-08 08:33:45.000000 fenjing-0.2.4/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-08 08:33:45.000000 fenjing-0.2.4/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       30 2023-05-08 08:33:45.000000 fenjing-0.2.4/fenjing.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2023-05-08 08:33:45.000000 fenjing-0.2.4/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-08 08:33:45.884000 fenjing-0.2.4/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      860 2023-05-08 04:12:10.000000 fenjing-0.2.4/setup.py
```

### Comparing `fenjing-0.2.3/LICENSE` & `fenjing-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.3/PKG-INFO` & `fenjing-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -153,15 +153,15 @@
   --interval FLOAT     每次请求的间隔
   --user-agent TEXT    请求时使用的User Agent
   --help               Show this message and exit.
 ```
 
 ### 作为python库使用
 
-参考[example.py](fenjing/example.py)
+参考[example.py](example.py)
 
 ```python
 from fenjing import exec_cmd_payload
 
 import logging
 
 logging.basicConfig(level = logging.INFO)
```

### Comparing `fenjing-0.2.3/README.md` & `fenjing-0.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
   --interval FLOAT     每次请求的间隔
   --user-agent TEXT    请求时使用的User Agent
   --help               Show this message and exit.
 ```
 
 ### 作为python库使用
 
-参考[example.py](fenjing/example.py)
+参考[example.py](example.py)
 
 ```python
 from fenjing import exec_cmd_payload
 
 import logging
 
 logging.basicConfig(level = logging.INFO)
```

### Comparing `fenjing-0.2.3/fenjing/cli.py` & `fenjing-0.2.4/fenjing/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 from .form import Form
 from .form_cracker import FormCracker
 from .scan_url import yield_form
 from .requester import Requester, DEFAULT_USER_AGENT
 from .colorize import colored
 import click
 
+TITLE = colored("yellow", r"""
+    ____             _ _            
+   / __/__  ____    (_|_)___  ____ _
+  / /_/ _ \/ __ \  / / / __ \/ __ `/
+ / __/  __/ / / / / / / / / / /_/ / 
+/_/  \___/_/ /_/_/ /_/_/ /_/\__, /  
+              /___/        /____/   
+""".strip("\n"), bold=True)
+
 logging.basicConfig(
     level=logging.INFO,
     format="%(levelname)s:[%(name)s] | %(message)s"
 )
 logger = logging.getLogger("cli")
 
 
@@ -42,14 +51,15 @@
 @click.option("--action", "-a", default=None, help="form的action，默认为当前路径")
 @click.option("--method", "-m", default="POST", help="form的提交方式，默认为POST")
 @click.option("--inputs", "-i", help="form的参数，以逗号分隔")
 @click.option("--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则成功后进入交互模式")
 @click.option("--interval", default=0.0, help="每次请求的间隔")
 @click.option("--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent")
 def crack(url, action, method, inputs, exec_cmd, interval, user_agent):
+    print(TITLE)
     assert all(param is not None for param in [
                url, inputs]), "Please check your param"
     form = Form(
         action=action or urlparse(url)[3],
         method=method,
         inputs=inputs.split(",")
     )
@@ -75,14 +85,15 @@
 
 @main.command()
 @click.option("--url", "-u", help="需要扫描的URL")
 @click.option("--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则进入交互模式")
 @click.option("--interval", default=0.0, help="每次请求的间隔")
 @click.option("--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent")
 def scan(url, exec_cmd, interval, user_agent):
+    print(TITLE)
     requester = Requester(interval=interval, user_agent=user_agent)
     for page_url, forms in yield_form(requester, url):
         for form in forms:
             cracker = FormCracker(url=url, form=form, requester=requester)
             result = cracker.crack()
             if result is None:
                 continue
```

### Comparing `fenjing-0.2.3/fenjing/colorize.py` & `fenjing-0.2.4/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.3/fenjing/form.py` & `fenjing-0.2.4/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.3/fenjing/form_cracker.py` & `fenjing-0.2.4/fenjing/form_cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.3/fenjing/int_vars.py` & `fenjing-0.2.4/fenjing/int_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.3/fenjing/pattern.py` & `fenjing-0.2.4/fenjing/pattern.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.3/fenjing/payload_gen.py` & `fenjing-0.2.4/fenjing/payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.3/fenjing/requester.py` & `fenjing-0.2.4/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.3/fenjing/scan_url.py` & `fenjing-0.2.4/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.3/fenjing/shell_payload.py` & `fenjing-0.2.4/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.3/fenjing.egg-info/PKG-INFO` & `fenjing-0.2.4/fenjing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -153,15 +153,15 @@
   --interval FLOAT     每次请求的间隔
   --user-agent TEXT    请求时使用的User Agent
   --help               Show this message and exit.
 ```
 
 ### 作为python库使用
 
-参考[example.py](fenjing/example.py)
+参考[example.py](example.py)
 
 ```python
 from fenjing import exec_cmd_payload
 
 import logging
 
 logging.basicConfig(level = logging.INFO)
```

### Comparing `fenjing-0.2.3/setup.py` & `fenjing-0.2.4/setup.py`

 * *Files identical despite different names*

