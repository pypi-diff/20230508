# Comparing `tmp/chromedriver_autoupdate-1.1.1.tar.gz` & `tmp/chromedriver_autoupdate-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromedriver_autoupdate-1.1.1.tar", last modified: Thu Mar  9 14:13:04 2023, max compression
+gzip compressed data, was "chromedriver_autoupdate-1.1.2.tar", last modified: Mon May  8 11:50:50 2023, max compression
```

## Comparing `chromedriver_autoupdate-1.1.1.tar` & `chromedriver_autoupdate-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:13:04.156116 chromedriver_autoupdate-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-03-09 14:12:54.000000 chromedriver_autoupdate-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-09 14:13:04.156116 chromedriver_autoupdate-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-09 14:12:54.000000 chromedriver_autoupdate-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:13:04.152115 chromedriver_autoupdate-1.1.1/chromedriver_autoupdate/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-09 14:12:54.000000 chromedriver_autoupdate-1.1.1/chromedriver_autoupdate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-03-09 14:12:54.000000 chromedriver_autoupdate-1.1.1/chromedriver_autoupdate/driver_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:13:04.156116 chromedriver_autoupdate-1.1.1/chromedriver_autoupdate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-09 14:13:04.000000 chromedriver_autoupdate-1.1.1/chromedriver_autoupdate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-09 14:13:04.000000 chromedriver_autoupdate-1.1.1/chromedriver_autoupdate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 14:13:04.000000 chromedriver_autoupdate-1.1.1/chromedriver_autoupdate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-09 14:13:04.000000 chromedriver_autoupdate-1.1.1/chromedriver_autoupdate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-09 14:13:04.000000 chromedriver_autoupdate-1.1.1/chromedriver_autoupdate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 14:13:04.156116 chromedriver_autoupdate-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-09 14:12:54.000000 chromedriver_autoupdate-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:50:50.461684 chromedriver_autoupdate-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-05-08 11:50:36.000000 chromedriver_autoupdate-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-08 11:50:50.461684 chromedriver_autoupdate-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-08 11:50:36.000000 chromedriver_autoupdate-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:50:50.461684 chromedriver_autoupdate-1.1.2/chromedriver_autoupdate/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 11:50:36.000000 chromedriver_autoupdate-1.1.2/chromedriver_autoupdate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-08 11:50:36.000000 chromedriver_autoupdate-1.1.2/chromedriver_autoupdate/driver_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:50:50.461684 chromedriver_autoupdate-1.1.2/chromedriver_autoupdate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-08 11:50:50.000000 chromedriver_autoupdate-1.1.2/chromedriver_autoupdate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-08 11:50:50.000000 chromedriver_autoupdate-1.1.2/chromedriver_autoupdate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:50:50.000000 chromedriver_autoupdate-1.1.2/chromedriver_autoupdate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 11:50:50.000000 chromedriver_autoupdate-1.1.2/chromedriver_autoupdate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-08 11:50:50.000000 chromedriver_autoupdate-1.1.2/chromedriver_autoupdate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 11:50:50.461684 chromedriver_autoupdate-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-08 11:50:37.000000 chromedriver_autoupdate-1.1.2/setup.py
```

### Comparing `chromedriver_autoupdate-1.1.1/LICENSE` & `chromedriver_autoupdate-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chromedriver_autoupdate-1.1.1/PKG-INFO` & `chromedriver_autoupdate-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromedriver_autoupdate
-Version: 1.1.1
+Version: 1.1.2
 Summary: chromedriver的自动更新
 Home-page: https://github.com/roiding/chromedriver-autoupdate
 Author: roiding
 Author-email: dingran@ran-ding.ga
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `chromedriver_autoupdate-1.1.1/chromedriver_autoupdate/driver_check.py` & `chromedriver_autoupdate-1.1.2/chromedriver_autoupdate/driver_check.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 import subprocess
 import sys
 import zipfile  # 操作.zip文件
 
 import requests
 from tqdm import tqdm
 from urllib3.exceptions import InsecureRequestWarning
-
+'''
+ODO 还有一种方式获取版本
+https://sites.google.com/a/chromium.org/chromedriver/downloads/version-selection
+'''
 # 匹配三位版本号的正则
 version_re =re.compile(r'[1-9]\d*\.\d*\.\d*')
 '''
 driver_path: chrome_driver的路径
 '''
 def checkAndUpdate(driver_path:str):
     chrome_version=_getChromeVersion()
@@ -48,15 +51,15 @@
     platform_name=platform.system()
     if platform_name == "Linux":
         chrome_path=('/opt/google/chrome',)
         path=_checkPathExit(chrome_path)
         return _matchChromeVersion(path+" --version")
     elif platform_name == "Darwin":
         chrome_path=('/Applications/Google Chrome.app/Contents/MacOS/Google Chrome',)
-        path=_checkPathExit(chrome_path)
+        path=_checkPathExit(chrome_path).replace(' ','\ ')
         return _matchChromeVersion(path+" --version")
     elif platform_name == "Windows":
         chrome_path=('C:\\\\Program Files\\\\Google\\\\Chrome\\\\Application\\\\chrome.exe','C:\\\\Program Files (x86)\\\\Google\\\\Chrome\\\\Application\\\\chrome.exe');
         path=_checkPathExit(chrome_path)
         return _matchChromeVersion("wmic datafile where name=\"%s\" get Version /value"%(path))
     else:
         raise RuntimeError("该操作系统暂不支持")
```

### Comparing `chromedriver_autoupdate-1.1.1/chromedriver_autoupdate.egg-info/PKG-INFO` & `chromedriver_autoupdate-1.1.2/chromedriver_autoupdate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromedriver-autoupdate
-Version: 1.1.1
+Version: 1.1.2
 Summary: chromedriver的自动更新
 Home-page: https://github.com/roiding/chromedriver-autoupdate
 Author: roiding
 Author-email: dingran@ran-ding.ga
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `chromedriver_autoupdate-1.1.1/setup.py` & `chromedriver_autoupdate-1.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md",'r',encoding='utf-8') as fh:
     long_description = fh.read()
 
 
 
 setuptools.setup(
     name="chromedriver_autoupdate", #模块名称
-    version='v1.1.1', #当前版本
+    version='v1.1.2', #当前版本
     author="roiding", # 作者
     author_email="dingran@ran-ding.ga", #作者邮箱
     description="chromedriver的自动更新", #模块介绍
     long_description=long_description, #模块详细介绍
     long_description_content_type="text/markdown", #模块详细介绍格式
     url="https://github.com/roiding/chromedriver-autoupdate", #项目地址
     packages=setuptools.find_packages(), #自动找到项目中倒入的模块
```

