# Comparing `tmp/pwl-chat-python-1.3.0.tar.gz` & `tmp/pwl-chat-python-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwl-chat-python-1.3.0.tar", last modified: Mon May  8 08:00:39 2023, max compression
+gzip compressed data, was "pwl-chat-python-1.3.1.tar", last modified: Mon May  8 08:49:00 2023, max compression
```

## Comparing `pwl-chat-python-1.3.0.tar` & `pwl-chat-python-1.3.1.tar`

### file list

```diff
@@ -1,14 +1,30 @@
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 08:00:39.528046 pwl-chat-python-1.3.0/
--rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-08 06:12:10.000000 pwl-chat-python-1.3.0/LICENSE
--rw-r--r--   0 fangcong   (501) staff       (20)      258 2023-05-08 08:00:39.527700 pwl-chat-python-1.3.0/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)     1400 2023-05-08 02:08:19.000000 pwl-chat-python-1.3.0/README.md
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 08:00:39.526345 pwl-chat-python-1.3.0/pwl_chat_python.egg-info/
--rw-r--r--   0 fangcong   (501) staff       (20)      258 2023-05-08 08:00:39.000000 pwl-chat-python-1.3.0/pwl_chat_python.egg-info/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)      232 2023-05-08 08:00:39.000000 pwl-chat-python-1.3.0/pwl_chat_python.egg-info/SOURCES.txt
--rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-05-08 08:00:39.000000 pwl-chat-python-1.3.0/pwl_chat_python.egg-info/dependency_links.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-08 08:00:39.000000 pwl-chat-python-1.3.0/pwl_chat_python.egg-info/requires.txt
--rw-r--r--   0 fangcong   (501) staff       (20)        4 2023-05-08 08:00:39.000000 pwl-chat-python-1.3.0/pwl_chat_python.egg-info/top_level.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-05-08 08:00:39.528125 pwl-chat-python-1.3.0/setup.cfg
--rw-r--r--   0 fangcong   (501) staff       (20)      444 2023-05-08 08:00:21.000000 pwl-chat-python-1.3.0/setup.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 08:00:39.526789 pwl-chat-python-1.3.0/src/
--rw-r--r--   0 fangcong   (501) staff       (20)      967 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.0/src/main.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 08:49:00.005028 pwl-chat-python-1.3.1/
+-rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-08 06:12:10.000000 pwl-chat-python-1.3.1/LICENSE
+-rw-r--r--   0 fangcong   (501) staff       (20)     1999 2023-05-08 08:49:00.004552 pwl-chat-python-1.3.1/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)     1400 2023-05-08 02:08:19.000000 pwl-chat-python-1.3.1/README.md
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 08:48:59.993279 pwl-chat-python-1.3.1/api/
+-rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.1/api/__api__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1992 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.1/api/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1735 2023-05-08 06:43:12.000000 pwl-chat-python-1.3.1/api/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1120 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.1/api/user.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 08:48:59.998562 pwl-chat-python-1.3.1/core/
+-rw-r--r--   0 fangcong   (501) staff       (20)     2239 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.1/core/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1623 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.1/core/blacklist.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1822 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.1/core/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1966 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.1/core/cli.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1633 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.1/core/config.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     4435 2023-05-08 03:41:01.000000 pwl-chat-python-1.3.1/core/redpacket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1356 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.1/core/user.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1230 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.1/core/websocket.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 08:49:00.002799 pwl-chat-python-1.3.1/pwl_chat_python.egg-info/
+-rw-r--r--   0 fangcong   (501) staff       (20)     1999 2023-05-08 08:48:59.000000 pwl-chat-python-1.3.1/pwl_chat_python.egg-info/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)      481 2023-05-08 08:48:59.000000 pwl-chat-python-1.3.1/pwl_chat_python.egg-info/SOURCES.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-05-08 08:48:59.000000 pwl-chat-python-1.3.1/pwl_chat_python.egg-info/dependency_links.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       55 2023-05-08 08:48:59.000000 pwl-chat-python-1.3.1/pwl_chat_python.egg-info/entry_points.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-08 08:48:59.000000 pwl-chat-python-1.3.1/pwl_chat_python.egg-info/requires.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       15 2023-05-08 08:48:59.000000 pwl-chat-python-1.3.1/pwl_chat_python.egg-info/top_level.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-05-08 08:49:00.005229 pwl-chat-python-1.3.1/setup.cfg
+-rw-r--r--   0 fangcong   (501) staff       (20)     3751 2023-05-08 08:48:55.000000 pwl-chat-python-1.3.1/setup.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 08:49:00.003893 pwl-chat-python-1.3.1/utils/
+-rw-r--r--   0 fangcong   (501) staff       (20)      739 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.1/utils/utils.py
+-rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-05-08 08:47:43.000000 pwl-chat-python-1.3.1/utils/version.py
```

### Comparing `pwl-chat-python-1.3.0/LICENSE` & `pwl-chat-python-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.0/README.md` & `pwl-chat-python-1.3.1/README.md`

 * *Files identical despite different names*

