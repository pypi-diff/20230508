# Comparing `tmp/ZephyrusChatbot-1.0.1.tar.gz` & `tmp/ZephyrusChatbot-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ZephyrusChatbot-1.0.1.tar", last modified: Mon May  8 19:12:50 2023, max compression
+gzip compressed data, was "ZephyrusChatbot-1.0.2.tar", last modified: Mon May  8 19:26:26 2023, max compression
```

## Comparing `ZephyrusChatbot-1.0.1.tar` & `ZephyrusChatbot-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 19:12:50.019264 ZephyrusChatbot-1.0.1/
--rw-rw-rw-   0        0        0      503 2023-05-08 19:12:50.018171 ZephyrusChatbot-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      151 2023-05-08 19:02:33.000000 ZephyrusChatbot-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 19:12:50.009164 ZephyrusChatbot-1.0.1/ZephyrusChatbot/
--rw-rw-rw-   0        0        0       27 2023-05-08 19:02:33.000000 ZephyrusChatbot-1.0.1/ZephyrusChatbot/__init__.py
--rw-rw-rw-   0        0        0      225 2023-05-08 19:02:33.000000 ZephyrusChatbot-1.0.1/ZephyrusChatbot/main.py
-drwxrwxrwx   0        0        0        0 2023-05-08 19:12:50.016169 ZephyrusChatbot-1.0.1/ZephyrusChatbot.egg-info/
--rw-rw-rw-   0        0        0      503 2023-05-08 19:12:49.000000 ZephyrusChatbot-1.0.1/ZephyrusChatbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-08 19:12:49.000000 ZephyrusChatbot-1.0.1/ZephyrusChatbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 19:12:49.000000 ZephyrusChatbot-1.0.1/ZephyrusChatbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-08 19:12:49.000000 ZephyrusChatbot-1.0.1/ZephyrusChatbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-08 19:12:49.000000 ZephyrusChatbot-1.0.1/ZephyrusChatbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 19:12:50.019264 ZephyrusChatbot-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      817 2023-05-08 19:07:11.000000 ZephyrusChatbot-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 19:26:26.450526 ZephyrusChatbot-1.0.2/
+-rw-rw-rw-   0        0        0      503 2023-05-08 19:26:26.449529 ZephyrusChatbot-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      151 2023-05-08 19:25:33.000000 ZephyrusChatbot-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 19:26:26.438387 ZephyrusChatbot-1.0.2/ZephyrusChatbot/
+-rw-rw-rw-   0        0        0       35 2023-05-08 19:25:33.000000 ZephyrusChatbot-1.0.2/ZephyrusChatbot/__init__.py
+-rw-rw-rw-   0        0        0      225 2023-05-08 19:25:33.000000 ZephyrusChatbot-1.0.2/ZephyrusChatbot/main.py
+drwxrwxrwx   0        0        0        0 2023-05-08 19:26:26.448411 ZephyrusChatbot-1.0.2/ZephyrusChatbot.egg-info/
+-rw-rw-rw-   0        0        0      503 2023-05-08 19:26:26.000000 ZephyrusChatbot-1.0.2/ZephyrusChatbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-08 19:26:26.000000 ZephyrusChatbot-1.0.2/ZephyrusChatbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 19:26:26.000000 ZephyrusChatbot-1.0.2/ZephyrusChatbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-08 19:26:26.000000 ZephyrusChatbot-1.0.2/ZephyrusChatbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-08 19:26:26.000000 ZephyrusChatbot-1.0.2/ZephyrusChatbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 19:26:26.450526 ZephyrusChatbot-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-05-08 19:25:33.000000 ZephyrusChatbot-1.0.2/setup.py
```

### Comparing `ZephyrusChatbot-1.0.1/setup.py` & `ZephyrusChatbot-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'chatbot'
 LONG_DESCRIPTION = 'Just a chatbot'
 
 # Setting up
 setup(
     name="ZephyrusChatbot",
     version=VERSION,
```

