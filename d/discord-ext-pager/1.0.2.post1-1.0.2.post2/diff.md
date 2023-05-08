# Comparing `tmp/discord-ext-pager-1.0.2.post1.tar.gz` & `tmp/discord-ext-pager-1.0.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-ext-pager-1.0.2.post1.tar", last modified: Mon May  8 14:57:04 2023, max compression
+gzip compressed data, was "discord-ext-pager-1.0.2.post2.tar", last modified: Mon May  8 15:01:06 2023, max compression
```

## Comparing `discord-ext-pager-1.0.2.post1.tar` & `discord-ext-pager-1.0.2.post2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:57:04.022245 discord-ext-pager-1.0.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-08 14:56:51.000000 discord-ext-pager-1.0.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-08 14:57:04.022245 discord-ext-pager-1.0.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-08 14:56:51.000000 discord-ext-pager-1.0.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-08 14:56:51.000000 discord-ext-pager-1.0.2.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 14:57:04.022245 discord-ext-pager-1.0.2.post1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:57:04.022245 discord-ext-pager-1.0.2.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:57:04.022245 discord-ext-pager-1.0.2.post1/src/discord/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:57:04.022245 discord-ext-pager-1.0.2.post1/src/discord/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:57:04.022245 discord-ext-pager-1.0.2.post1/src/discord/ext/pager/
--rw-r--r--   0 runner    (1001) docker     (123)    15645 2023-05-08 14:56:51.000000 discord-ext-pager-1.0.2.post1/src/discord/ext/pager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:57:04.022245 discord-ext-pager-1.0.2.post1/src/discord_ext_pager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-08 14:57:04.000000 discord-ext-pager-1.0.2.post1/src/discord_ext_pager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-08 14:57:04.000000 discord-ext-pager-1.0.2.post1/src/discord_ext_pager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 14:57:04.000000 discord-ext-pager-1.0.2.post1/src/discord_ext_pager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 14:57:04.000000 discord-ext-pager-1.0.2.post1/src/discord_ext_pager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 14:57:04.000000 discord-ext-pager-1.0.2.post1/src/discord_ext_pager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:01:06.245339 discord-ext-pager-1.0.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-08 15:00:51.000000 discord-ext-pager-1.0.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-08 15:01:06.245339 discord-ext-pager-1.0.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-08 15:00:51.000000 discord-ext-pager-1.0.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-08 15:00:51.000000 discord-ext-pager-1.0.2.post2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:01:06.245339 discord-ext-pager-1.0.2.post2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:01:06.241339 discord-ext-pager-1.0.2.post2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:01:06.241339 discord-ext-pager-1.0.2.post2/src/discord/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:01:06.241339 discord-ext-pager-1.0.2.post2/src/discord/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:01:06.245339 discord-ext-pager-1.0.2.post2/src/discord/ext/pager/
+-rw-r--r--   0 runner    (1001) docker     (123)    15645 2023-05-08 15:00:51.000000 discord-ext-pager-1.0.2.post2/src/discord/ext/pager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:01:06.245339 discord-ext-pager-1.0.2.post2/src/discord_ext_pager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-08 15:01:06.000000 discord-ext-pager-1.0.2.post2/src/discord_ext_pager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-08 15:01:06.000000 discord-ext-pager-1.0.2.post2/src/discord_ext_pager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:01:06.000000 discord-ext-pager-1.0.2.post2/src/discord_ext_pager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 15:01:06.000000 discord-ext-pager-1.0.2.post2/src/discord_ext_pager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 15:01:06.000000 discord-ext-pager-1.0.2.post2/src/discord_ext_pager.egg-info/top_level.txt
```

### Comparing `discord-ext-pager-1.0.2.post1/LICENSE` & `discord-ext-pager-1.0.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-ext-pager-1.0.2.post1/PKG-INFO` & `discord-ext-pager-1.0.2.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: discord-ext-pager
-Version: 1.0.2.post1
+Version: 1.0.2.post2
 Summary: A view-based paginator library for discord.py 2.0
 Author: thegamecracks
-Project-URL: homepage, https://github.com/thegamecracks/discord-ext-pager
+Project-URL: Homepage, https://github.com/thegamecracks/discord-ext-pager
 Keywords: discord,discord.py,paginator,view
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python
```

### Comparing `discord-ext-pager-1.0.2.post1/README.md` & `discord-ext-pager-1.0.2.post2/README.md`

 * *Files identical despite different names*

### Comparing `discord-ext-pager-1.0.2.post1/pyproject.toml` & `discord-ext-pager-1.0.2.post2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -34,11 +34,11 @@
 dependencies = [
     "discord.py>=2.0.0",
     "typing-extensions>=4.5.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
-homepage = "https://github.com/thegamecracks/discord-ext-pager"
+Homepage = "https://github.com/thegamecracks/discord-ext-pager"
 
 [tool.setuptools.dynamic]
 version = { attr = "discord.ext.pager.__version__" }
```

### Comparing `discord-ext-pager-1.0.2.post1/src/discord/ext/pager/__init__.py` & `discord-ext-pager-1.0.2.post2/src/discord/ext/pager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     Union,
     cast,
 )
 
 import discord
 from typing_extensions import TypeAlias
 
-__version__ = "1.0.2.post1"
+__version__ = "1.0.2.post2"
 
 __all__ = (
     "PageOption",
     "PageSource",
     "ListPageSource",
     "AsyncIteratorPageSource",
     "TimeoutAction",
```

### Comparing `discord-ext-pager-1.0.2.post1/src/discord_ext_pager.egg-info/PKG-INFO` & `discord-ext-pager-1.0.2.post2/src/discord_ext_pager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: discord-ext-pager
-Version: 1.0.2.post1
+Version: 1.0.2.post2
 Summary: A view-based paginator library for discord.py 2.0
 Author: thegamecracks
-Project-URL: homepage, https://github.com/thegamecracks/discord-ext-pager
+Project-URL: Homepage, https://github.com/thegamecracks/discord-ext-pager
 Keywords: discord,discord.py,paginator,view
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python
```

