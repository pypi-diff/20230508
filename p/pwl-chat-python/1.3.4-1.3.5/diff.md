# Comparing `tmp/pwl-chat-python-1.3.4.tar.gz` & `tmp/pwl-chat-python-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwl-chat-python-1.3.4.tar", last modified: Mon May  8 09:09:08 2023, max compression
+gzip compressed data, was "pwl-chat-python-1.3.5.tar", last modified: Mon May  8 09:10:54 2023, max compression
```

## Comparing `pwl-chat-python-1.3.4.tar` & `pwl-chat-python-1.3.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:09:08.126711 pwl-chat-python-1.3.4/
--rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-08 06:12:10.000000 pwl-chat-python-1.3.4/LICENSE
--rw-r--r--   0 fangcong   (501) staff       (20)     1999 2023-05-08 09:09:08.126259 pwl-chat-python-1.3.4/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)     1400 2023-05-08 02:08:19.000000 pwl-chat-python-1.3.4/README.md
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:09:08.114553 pwl-chat-python-1.3.4/api/
--rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.4/api/__api__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1992 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.4/api/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1735 2023-05-08 06:43:12.000000 pwl-chat-python-1.3.4/api/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1120 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.4/api/user.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:09:08.119711 pwl-chat-python-1.3.4/core/
--rw-r--r--   0 fangcong   (501) staff       (20)     2239 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.4/core/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1623 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.4/core/blacklist.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1822 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.4/core/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1966 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.4/core/cli.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1633 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.4/core/config.py
--rw-r--r--   0 fangcong   (501) staff       (20)     4435 2023-05-08 03:41:01.000000 pwl-chat-python-1.3.4/core/redpacket.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1356 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.4/core/user.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1230 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.4/core/websocket.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:09:08.120298 pwl-chat-python-1.3.4/main/
--rw-r--r--   0 fangcong   (501) staff       (20)      967 2023-05-08 09:06:58.000000 pwl-chat-python-1.3.4/main/main.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:09:08.124046 pwl-chat-python-1.3.4/pwl_chat_python.egg-info/
--rw-r--r--   0 fangcong   (501) staff       (20)     1999 2023-05-08 09:09:07.000000 pwl-chat-python-1.3.4/pwl_chat_python.egg-info/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)      494 2023-05-08 09:09:08.000000 pwl-chat-python-1.3.4/pwl_chat_python.egg-info/SOURCES.txt
--rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-05-08 09:09:07.000000 pwl-chat-python-1.3.4/pwl_chat_python.egg-info/dependency_links.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-08 09:09:07.000000 pwl-chat-python-1.3.4/pwl_chat_python.egg-info/entry_points.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-08 09:09:07.000000 pwl-chat-python-1.3.4/pwl_chat_python.egg-info/requires.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       20 2023-05-08 09:09:07.000000 pwl-chat-python-1.3.4/pwl_chat_python.egg-info/top_level.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-05-08 09:09:08.126935 pwl-chat-python-1.3.4/setup.cfg
--rw-r--r--   0 fangcong   (501) staff       (20)     3527 2023-05-08 09:07:43.000000 pwl-chat-python-1.3.4/setup.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:09:08.125609 pwl-chat-python-1.3.4/utils/
--rw-r--r--   0 fangcong   (501) staff       (20)      739 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.4/utils/utils.py
--rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-05-08 09:08:35.000000 pwl-chat-python-1.3.4/utils/version.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:10:54.147136 pwl-chat-python-1.3.5/
+-rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-08 06:12:10.000000 pwl-chat-python-1.3.5/LICENSE
+-rw-r--r--   0 fangcong   (501) staff       (20)     1999 2023-05-08 09:10:54.146561 pwl-chat-python-1.3.5/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)     1400 2023-05-08 02:08:19.000000 pwl-chat-python-1.3.5/README.md
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:10:54.136424 pwl-chat-python-1.3.5/api/
+-rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/api/__api__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1992 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/api/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1735 2023-05-08 06:43:12.000000 pwl-chat-python-1.3.5/api/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1120 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/api/user.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:10:54.140741 pwl-chat-python-1.3.5/core/
+-rw-r--r--   0 fangcong   (501) staff       (20)     2239 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/core/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1623 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/core/blacklist.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1822 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/core/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1966 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/core/cli.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1633 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/core/config.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     4435 2023-05-08 03:41:01.000000 pwl-chat-python-1.3.5/core/redpacket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1356 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/core/user.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1230 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/core/websocket.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:10:54.141224 pwl-chat-python-1.3.5/main/
+-rw-r--r--   0 fangcong   (501) staff       (20)      967 2023-05-08 09:06:58.000000 pwl-chat-python-1.3.5/main/main.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:10:54.144505 pwl-chat-python-1.3.5/pwl_chat_python.egg-info/
+-rw-r--r--   0 fangcong   (501) staff       (20)     1999 2023-05-08 09:10:54.000000 pwl-chat-python-1.3.5/pwl_chat_python.egg-info/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)      494 2023-05-08 09:10:54.000000 pwl-chat-python-1.3.5/pwl_chat_python.egg-info/SOURCES.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-05-08 09:10:54.000000 pwl-chat-python-1.3.5/pwl_chat_python.egg-info/dependency_links.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       50 2023-05-08 09:10:54.000000 pwl-chat-python-1.3.5/pwl_chat_python.egg-info/entry_points.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-08 09:10:54.000000 pwl-chat-python-1.3.5/pwl_chat_python.egg-info/requires.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       20 2023-05-08 09:10:54.000000 pwl-chat-python-1.3.5/pwl_chat_python.egg-info/top_level.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-05-08 09:10:54.147329 pwl-chat-python-1.3.5/setup.cfg
+-rw-r--r--   0 fangcong   (501) staff       (20)     3532 2023-05-08 09:10:37.000000 pwl-chat-python-1.3.5/setup.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:10:54.145745 pwl-chat-python-1.3.5/utils/
+-rw-r--r--   0 fangcong   (501) staff       (20)      739 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/utils/utils.py
+-rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-05-08 09:10:50.000000 pwl-chat-python-1.3.5/utils/version.py
```

### Comparing `pwl-chat-python-1.3.4/LICENSE` & `pwl-chat-python-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.4/PKG-INFO` & `pwl-chat-python-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.3.4
+Version: 1.3.5
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pwl-chat-python-1.3.4/README.md` & `pwl-chat-python-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.4/api/__init__.py` & `pwl-chat-python-1.3.5/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.4/api/chatroom.py` & `pwl-chat-python-1.3.5/api/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.4/api/user.py` & `pwl-chat-python-1.3.5/api/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.4/core/__init__.py` & `pwl-chat-python-1.3.5/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.4/core/blacklist.py` & `pwl-chat-python-1.3.5/core/blacklist.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.4/core/chatroom.py` & `pwl-chat-python-1.3.5/core/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.4/core/cli.py` & `pwl-chat-python-1.3.5/core/cli.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.4/core/config.py` & `pwl-chat-python-1.3.5/core/config.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.4/core/redpacket.py` & `pwl-chat-python-1.3.5/core/redpacket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.4/core/user.py` & `pwl-chat-python-1.3.5/core/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.4/core/websocket.py` & `pwl-chat-python-1.3.5/core/websocket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.4/main/main.py` & `pwl-chat-python-1.3.5/main/main.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.4/pwl_chat_python.egg-info/PKG-INFO` & `pwl-chat-python-1.3.5/pwl_chat_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.3.4
+Version: 1.3.5
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pwl-chat-python-1.3.4/setup.py` & `pwl-chat-python-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,12 +118,12 @@
     ],
     # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
     },
     entry_points={
         'console_scripts': [
-            'pwl-chat-python = main:cli',
+            'pwl-chat-python = main.main:cli',
         ],
     }
 
 )
```

### Comparing `pwl-chat-python-1.3.4/utils/utils.py` & `pwl-chat-python-1.3.5/utils/utils.py`

 * *Files identical despite different names*

