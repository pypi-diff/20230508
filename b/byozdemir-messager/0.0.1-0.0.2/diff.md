# Comparing `tmp/byozdemir-messager-0.0.1.tar.gz` & `tmp/byozdemir-messager-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byozdemir-messager-0.0.1.tar", last modified: Mon May  8 10:55:37 2023, max compression
+gzip compressed data, was "byozdemir-messager-0.0.2.tar", last modified: Mon May  8 10:58:05 2023, max compression
```

## Comparing `byozdemir-messager-0.0.1.tar` & `byozdemir-messager-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 modernistasyon  (1000) modernistasyon  (1000)        0 2023-05-08 10:55:37.860094 byozdemir-messager-0.0.1/
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      359 2023-05-08 10:55:37.860094 byozdemir-messager-0.0.1/PKG-INFO
-drwxr-xr-x   0 modernistasyon  (1000) modernistasyon  (1000)        0 2023-05-08 10:55:37.860094 byozdemir-messager-0.0.1/byozdemir_messager/
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      215 2023-05-08 10:33:48.000000 byozdemir-messager-0.0.1/byozdemir_messager/__init__.py
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      482 2023-05-08 10:26:10.000000 byozdemir-messager-0.0.1/byozdemir_messager/discord.py
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      721 2023-05-03 13:47:23.000000 byozdemir-messager-0.0.1/byozdemir_messager/mail.py
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      178 2023-05-03 13:41:55.000000 byozdemir-messager-0.0.1/byozdemir_messager/netgsm.py
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      300 2023-05-03 13:34:25.000000 byozdemir-messager-0.0.1/byozdemir_messager/telegram.py
-drwxr-xr-x   0 modernistasyon  (1000) modernistasyon  (1000)        0 2023-05-08 10:55:37.860094 byozdemir-messager-0.0.1/byozdemir_messager.egg-info/
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      359 2023-05-08 10:55:37.000000 byozdemir-messager-0.0.1/byozdemir_messager.egg-info/PKG-INFO
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      365 2023-05-08 10:55:37.000000 byozdemir-messager-0.0.1/byozdemir_messager.egg-info/SOURCES.txt
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)        1 2023-05-08 10:55:37.000000 byozdemir-messager-0.0.1/byozdemir_messager.egg-info/dependency_links.txt
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)       17 2023-05-08 10:55:37.000000 byozdemir-messager-0.0.1/byozdemir_messager.egg-info/requires.txt
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)       19 2023-05-08 10:55:37.000000 byozdemir-messager-0.0.1/byozdemir_messager.egg-info/top_level.txt
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)       38 2023-05-08 10:55:37.860094 byozdemir-messager-0.0.1/setup.cfg
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      553 2023-05-08 10:55:34.000000 byozdemir-messager-0.0.1/setup.py
+drwxr-xr-x   0 modernistasyon  (1000) modernistasyon  (1000)        0 2023-05-08 10:58:05.035791 byozdemir-messager-0.0.2/
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      359 2023-05-08 10:58:05.035791 byozdemir-messager-0.0.2/PKG-INFO
+drwxr-xr-x   0 modernistasyon  (1000) modernistasyon  (1000)        0 2023-05-08 10:58:05.035791 byozdemir-messager-0.0.2/byozdemir_messager/
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      259 2023-05-08 10:57:52.000000 byozdemir-messager-0.0.2/byozdemir_messager/__init__.py
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      482 2023-05-08 10:26:10.000000 byozdemir-messager-0.0.2/byozdemir_messager/discord.py
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      721 2023-05-03 13:47:23.000000 byozdemir-messager-0.0.2/byozdemir_messager/mail.py
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      178 2023-05-03 13:41:55.000000 byozdemir-messager-0.0.2/byozdemir_messager/netgsm.py
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      300 2023-05-03 13:34:25.000000 byozdemir-messager-0.0.2/byozdemir_messager/telegram.py
+drwxr-xr-x   0 modernistasyon  (1000) modernistasyon  (1000)        0 2023-05-08 10:58:05.035791 byozdemir-messager-0.0.2/byozdemir_messager.egg-info/
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      359 2023-05-08 10:58:05.000000 byozdemir-messager-0.0.2/byozdemir_messager.egg-info/PKG-INFO
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      365 2023-05-08 10:58:05.000000 byozdemir-messager-0.0.2/byozdemir_messager.egg-info/SOURCES.txt
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)        1 2023-05-08 10:58:05.000000 byozdemir-messager-0.0.2/byozdemir_messager.egg-info/dependency_links.txt
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)       17 2023-05-08 10:58:05.000000 byozdemir-messager-0.0.2/byozdemir_messager.egg-info/requires.txt
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)       19 2023-05-08 10:58:05.000000 byozdemir-messager-0.0.2/byozdemir_messager.egg-info/top_level.txt
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)       38 2023-05-08 10:58:05.036791 byozdemir-messager-0.0.2/setup.cfg
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      553 2023-05-08 10:57:22.000000 byozdemir-messager-0.0.2/setup.py
```

### Comparing `byozdemir-messager-0.0.1/byozdemir_messager/mail.py` & `byozdemir-messager-0.0.2/byozdemir_messager/mail.py`

 * *Files identical despite different names*

### Comparing `byozdemir-messager-0.0.1/setup.py` & `byozdemir-messager-0.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup,find_packages
 
 
 
 setup(
     name = "byozdemir-messager",
-    version = "0.0.1",
+    version = "0.0.2",
     author = "Byozdemir",
     author_email = "emrenetwork@yandex.com",
     description = ("It's helps you tou send message via populer apps"),
     license = "MIT",
     keywords = "telegram messager,discord messager",
     packages=find_packages(),
     install_requires = ['requests','telepot'],
```

