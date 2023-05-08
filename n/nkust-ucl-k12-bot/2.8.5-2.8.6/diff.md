# Comparing `tmp/nkust-ucl-k12-bot-2.8.5.tar.gz` & `tmp/nkust-ucl-k12-bot-2.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkust-ucl-k12-bot-2.8.5.tar", last modified: Mon May  8 04:04:14 2023, max compression
+gzip compressed data, was "nkust-ucl-k12-bot-2.8.6.tar", last modified: Mon May  8 04:06:37 2023, max compression
```

## Comparing `nkust-ucl-k12-bot-2.8.5.tar` & `nkust-ucl-k12-bot-2.8.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-08 04:04:14.120660 nkust-ucl-k12-bot-2.8.5/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.8.5/LICENSE
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     5377 2023-05-08 04:04:14.120438 nkust-ucl-k12-bot-2.8.5/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     4964 2023-05-07 11:45:37.000000 nkust-ucl-k12-bot-2.8.5/README.md
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-08 04:04:14.117488 nkust-ucl-k12-bot-2.8.5/nkust_ucl/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.8.5/nkust_ucl/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)    10504 2023-05-07 11:23:38.000000 nkust-ucl-k12-bot-2.8.5/nkust_ucl/k12.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-08 04:04:14.119254 nkust-ucl-k12-bot-2.8.5/nkust_ucl/utils/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.8.5/nkust_ucl/utils/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1021 2023-05-06 17:09:58.000000 nkust-ucl-k12-bot-2.8.5/nkust_ucl/utils/attachment.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.8.5/nkust_ucl/utils/config.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.8.5/nkust_ucl/utils/log.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.8.5/nkust_ucl/utils/mqtt_client.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-08 04:04:14.120228 nkust-ucl-k12-bot-2.8.5/nkust_ucl_k12_bot.egg-info/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     5377 2023-05-08 04:04:14.000000 nkust-ucl-k12-bot-2.8.5/nkust_ucl_k12_bot.egg-info/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      407 2023-05-08 04:04:14.000000 nkust-ucl-k12-bot-2.8.5/nkust_ucl_k12_bot.egg-info/SOURCES.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-08 04:04:14.000000 nkust-ucl-k12-bot-2.8.5/nkust_ucl_k12_bot.egg-info/dependency_links.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      744 2023-05-08 04:04:14.000000 nkust-ucl-k12-bot-2.8.5/nkust_ucl_k12_bot.egg-info/requires.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-08 04:04:14.000000 nkust-ucl-k12-bot-2.8.5/nkust_ucl_k12_bot.egg-info/top_level.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-08 04:04:14.120711 nkust-ucl-k12-bot-2.8.5/setup.cfg
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      742 2023-05-08 04:03:19.000000 nkust-ucl-k12-bot-2.8.5/setup.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-08 04:06:37.120787 nkust-ucl-k12-bot-2.8.6/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.8.6/LICENSE
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     5377 2023-05-08 04:06:37.120521 nkust-ucl-k12-bot-2.8.6/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     4964 2023-05-07 11:45:37.000000 nkust-ucl-k12-bot-2.8.6/README.md
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-08 04:06:37.117088 nkust-ucl-k12-bot-2.8.6/nkust_ucl/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.8.6/nkust_ucl/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)    10504 2023-05-07 11:23:38.000000 nkust-ucl-k12-bot-2.8.6/nkust_ucl/k12.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-08 04:06:37.118950 nkust-ucl-k12-bot-2.8.6/nkust_ucl/utils/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.8.6/nkust_ucl/utils/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1021 2023-05-06 17:09:58.000000 nkust-ucl-k12-bot-2.8.6/nkust_ucl/utils/attachment.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.8.6/nkust_ucl/utils/config.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.8.6/nkust_ucl/utils/log.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.8.6/nkust_ucl/utils/mqtt_client.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-08 04:06:37.120213 nkust-ucl-k12-bot-2.8.6/nkust_ucl_k12_bot.egg-info/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     5377 2023-05-08 04:06:37.000000 nkust-ucl-k12-bot-2.8.6/nkust_ucl_k12_bot.egg-info/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      407 2023-05-08 04:06:37.000000 nkust-ucl-k12-bot-2.8.6/nkust_ucl_k12_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-08 04:06:37.000000 nkust-ucl-k12-bot-2.8.6/nkust_ucl_k12_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      744 2023-05-08 04:06:37.000000 nkust-ucl-k12-bot-2.8.6/nkust_ucl_k12_bot.egg-info/requires.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-08 04:06:37.000000 nkust-ucl-k12-bot-2.8.6/nkust_ucl_k12_bot.egg-info/top_level.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-08 04:06:37.121526 nkust-ucl-k12-bot-2.8.6/setup.cfg
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1880 2023-05-08 04:06:30.000000 nkust-ucl-k12-bot-2.8.6/setup.py
```

### Comparing `nkust-ucl-k12-bot-2.8.5/LICENSE` & `nkust-ucl-k12-bot-2.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.8.5/PKG-INFO` & `nkust-ucl-k12-bot-2.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkust-ucl-k12-bot
-Version: 2.8.5
+Version: 2.8.6
 Summary: 一個用於k12的bot包
 Home-page: https://github.com/xinbow99/k12-telegram
 Author: Ethan Cheng
 Author-email: asdewq45445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nkust-ucl-k12-bot-2.8.5/README.md` & `nkust-ucl-k12-bot-2.8.6/README.md`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.8.5/nkust_ucl/k12.py` & `nkust-ucl-k12-bot-2.8.6/nkust_ucl/k12.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.8.5/nkust_ucl/utils/attachment.py` & `nkust-ucl-k12-bot-2.8.6/nkust_ucl/utils/attachment.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.8.5/nkust_ucl/utils/mqtt_client.py` & `nkust-ucl-k12-bot-2.8.6/nkust_ucl/utils/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.8.5/nkust_ucl_k12_bot.egg-info/PKG-INFO` & `nkust-ucl-k12-bot-2.8.6/nkust_ucl_k12_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkust-ucl-k12-bot
-Version: 2.8.5
+Version: 2.8.6
 Summary: 一個用於k12的bot包
 Home-page: https://github.com/xinbow99/k12-telegram
 Author: Ethan Cheng
 Author-email: asdewq45445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nkust-ucl-k12-bot-2.8.5/nkust_ucl_k12_bot.egg-info/requires.txt` & `nkust-ucl-k12-bot-2.8.6/nkust_ucl_k12_bot.egg-info/requires.txt`

 * *Files identical despite different names*

