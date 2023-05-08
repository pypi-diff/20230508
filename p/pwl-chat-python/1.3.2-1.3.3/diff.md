# Comparing `tmp/pwl-chat-python-1.3.2.tar.gz` & `tmp/pwl-chat-python-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwl-chat-python-1.3.2.tar", last modified: Mon May  8 09:02:37 2023, max compression
+gzip compressed data, was "pwl-chat-python-1.3.3.tar", last modified: Mon May  8 09:06:03 2023, max compression
```

## Comparing `pwl-chat-python-1.3.2.tar` & `pwl-chat-python-1.3.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:02:37.925065 pwl-chat-python-1.3.2/
--rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-08 06:12:10.000000 pwl-chat-python-1.3.2/LICENSE
--rw-r--r--   0 fangcong   (501) staff       (20)     1999 2023-05-08 09:02:37.924618 pwl-chat-python-1.3.2/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)     1400 2023-05-08 02:08:19.000000 pwl-chat-python-1.3.2/README.md
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:02:37.911471 pwl-chat-python-1.3.2/api/
--rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.2/api/__api__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1992 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.2/api/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1735 2023-05-08 06:43:12.000000 pwl-chat-python-1.3.2/api/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1120 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.2/api/user.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:02:37.918612 pwl-chat-python-1.3.2/core/
--rw-r--r--   0 fangcong   (501) staff       (20)     2239 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.2/core/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1623 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.2/core/blacklist.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1822 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.2/core/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1966 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.2/core/cli.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1633 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.2/core/config.py
--rw-r--r--   0 fangcong   (501) staff       (20)     4435 2023-05-08 03:41:01.000000 pwl-chat-python-1.3.2/core/redpacket.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1356 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.2/core/user.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1230 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.2/core/websocket.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:02:37.922813 pwl-chat-python-1.3.2/pwl_chat_python.egg-info/
--rw-r--r--   0 fangcong   (501) staff       (20)     1999 2023-05-08 09:02:37.000000 pwl-chat-python-1.3.2/pwl_chat_python.egg-info/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)      481 2023-05-08 09:02:37.000000 pwl-chat-python-1.3.2/pwl_chat_python.egg-info/SOURCES.txt
--rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-05-08 09:02:37.000000 pwl-chat-python-1.3.2/pwl_chat_python.egg-info/dependency_links.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-08 09:02:37.000000 pwl-chat-python-1.3.2/pwl_chat_python.egg-info/entry_points.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-08 09:02:37.000000 pwl-chat-python-1.3.2/pwl_chat_python.egg-info/requires.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       15 2023-05-08 09:02:37.000000 pwl-chat-python-1.3.2/pwl_chat_python.egg-info/top_level.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-05-08 09:02:37.925291 pwl-chat-python-1.3.2/setup.cfg
--rw-r--r--   0 fangcong   (501) staff       (20)     3741 2023-05-08 09:02:14.000000 pwl-chat-python-1.3.2/setup.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:02:37.923994 pwl-chat-python-1.3.2/utils/
--rw-r--r--   0 fangcong   (501) staff       (20)      739 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.2/utils/utils.py
--rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-05-08 09:02:19.000000 pwl-chat-python-1.3.2/utils/version.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:06:03.698743 pwl-chat-python-1.3.3/
+-rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-08 06:12:10.000000 pwl-chat-python-1.3.3/LICENSE
+-rw-r--r--   0 fangcong   (501) staff       (20)     1999 2023-05-08 09:06:03.698242 pwl-chat-python-1.3.3/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)     1400 2023-05-08 02:08:19.000000 pwl-chat-python-1.3.3/README.md
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:06:03.689174 pwl-chat-python-1.3.3/api/
+-rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.3/api/__api__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1992 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.3/api/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1735 2023-05-08 06:43:12.000000 pwl-chat-python-1.3.3/api/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1120 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.3/api/user.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:06:03.693088 pwl-chat-python-1.3.3/core/
+-rw-r--r--   0 fangcong   (501) staff       (20)     2239 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.3/core/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1623 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.3/core/blacklist.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1822 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.3/core/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1966 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.3/core/cli.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1633 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.3/core/config.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     4435 2023-05-08 03:41:01.000000 pwl-chat-python-1.3.3/core/redpacket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1356 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.3/core/user.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1230 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.3/core/websocket.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:06:03.696363 pwl-chat-python-1.3.3/pwl_chat_python.egg-info/
+-rw-r--r--   0 fangcong   (501) staff       (20)     1999 2023-05-08 09:06:03.000000 pwl-chat-python-1.3.3/pwl_chat_python.egg-info/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)      481 2023-05-08 09:06:03.000000 pwl-chat-python-1.3.3/pwl_chat_python.egg-info/SOURCES.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-05-08 09:06:03.000000 pwl-chat-python-1.3.3/pwl_chat_python.egg-info/dependency_links.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       40 2023-05-08 09:06:03.000000 pwl-chat-python-1.3.3/pwl_chat_python.egg-info/entry_points.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-08 09:06:03.000000 pwl-chat-python-1.3.3/pwl_chat_python.egg-info/requires.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       15 2023-05-08 09:06:03.000000 pwl-chat-python-1.3.3/pwl_chat_python.egg-info/top_level.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-05-08 09:06:03.698926 pwl-chat-python-1.3.3/setup.cfg
+-rw-r--r--   0 fangcong   (501) staff       (20)     3512 2023-05-08 09:06:00.000000 pwl-chat-python-1.3.3/setup.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:06:03.697389 pwl-chat-python-1.3.3/utils/
+-rw-r--r--   0 fangcong   (501) staff       (20)      739 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.3/utils/utils.py
+-rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-05-08 09:04:11.000000 pwl-chat-python-1.3.3/utils/version.py
```

### Comparing `pwl-chat-python-1.3.2/LICENSE` & `pwl-chat-python-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.2/PKG-INFO` & `pwl-chat-python-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.3.2
+Version: 1.3.3
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pwl-chat-python-1.3.2/README.md` & `pwl-chat-python-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.2/api/__init__.py` & `pwl-chat-python-1.3.3/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.2/api/chatroom.py` & `pwl-chat-python-1.3.3/api/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.2/api/user.py` & `pwl-chat-python-1.3.3/api/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.2/core/__init__.py` & `pwl-chat-python-1.3.3/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.2/core/blacklist.py` & `pwl-chat-python-1.3.3/core/blacklist.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.2/core/chatroom.py` & `pwl-chat-python-1.3.3/core/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.2/core/cli.py` & `pwl-chat-python-1.3.3/core/cli.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.2/core/config.py` & `pwl-chat-python-1.3.3/core/config.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.2/core/redpacket.py` & `pwl-chat-python-1.3.3/core/redpacket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.2/core/user.py` & `pwl-chat-python-1.3.3/core/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.2/core/websocket.py` & `pwl-chat-python-1.3.3/core/websocket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.2/pwl_chat_python.egg-info/PKG-INFO` & `pwl-chat-python-1.3.3/pwl_chat_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.3.2
+Version: 1.3.3
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pwl-chat-python-1.3.2/setup.py` & `pwl-chat-python-1.3.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 # Note: To use the 'upload' functionality of this file, you must:
 #   $ pipenv install twine --dev
 
 import io
 import os
 import sys
 from shutil import rmtree
+from utils.version import __version__
 
-from setuptools import find_packages, setup, Command
+from setuptools import setup, Command
 
 # Package meta-data.
 NAME = 'pwl-chat-python'
 DESCRIPTION = '摸鱼派聊天室python客户端'
 URL = 'https://github.com/gakkiyomi/pwl-chat-python'
 EMAIL = 'gakkiyomi@gmail.com'
 AUTHOR = 'gakkiyomi'
 REQUIRES_PYTHON = '>=3.10.8'
-VERSION = '1.3.2'
+VERSION = __version__
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests', 'websocket-client', 'rel', 'click', 'schedule'
 ]
 
 # What packages are optional?
@@ -44,21 +45,14 @@
 try:
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 # Load the package's __version__.py module as a dictionary.
-about = {}
-if not VERSION:
-    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
-    with open(os.path.join(here, project_slug, '__version__.py')) as f:
-        exec(f.read(), about)
-else:
-    about['__version__'] = VERSION
 
 
 class UploadCommand(Command):
     """Support setup.py upload."""
 
     description = 'Build and publish the package.'
     user_options = []
@@ -90,15 +84,15 @@
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
-    version=about['__version__'],
+    version=VERSION,
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
@@ -124,12 +118,12 @@
     ],
     # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
     },
     entry_points={
         'console_scripts': [
-            'pwl-chat-python = main:cli',
+            'pwl-chat-python = cli',
         ],
     }
 
 )
```

### Comparing `pwl-chat-python-1.3.2/utils/utils.py` & `pwl-chat-python-1.3.3/utils/utils.py`

 * *Files identical despite different names*

