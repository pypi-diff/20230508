# Comparing `tmp/pluralize-0.1.9.tar.gz` & `tmp/pluralize-20230507.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pluralize-0.1.9.tar", last modified: Sat Feb 12 18:41:11 2022, max compression
+gzip compressed data, was "pluralize-20230507.1.tar", last modified: Mon May  8 00:26:08 2023, max compression
```

## Comparing `pluralize-0.1.9.tar` & `pluralize-20230507.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2022-02-12 18:41:11.000000 pluralize-0.1.9/
--rw-rw-r--   0 mdp       (1000) mdp       (1000)     1473 2022-02-12 18:41:11.000000 pluralize-0.1.9/PKG-INFO
--rw-rw-r--   0 mdp       (1000) mdp       (1000)       38 2022-02-12 18:41:11.000000 pluralize-0.1.9/setup.cfg
--rw-r--r--   0 mdp       (1000) mdp       (1000)     1749 2019-07-23 06:13:38.000000 pluralize-0.1.9/setup.py
-drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2022-02-12 18:41:11.000000 pluralize-0.1.9/pluralize/
--rw-rw-r--   0 mdp       (1000) mdp       (1000)     5448 2022-02-12 18:34:33.000000 pluralize-0.1.9/pluralize/__init__.py
-drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2022-02-12 18:41:11.000000 pluralize-0.1.9/pluralize.egg-info/
--rw-r--r--   0 mdp       (1000) mdp       (1000)     1473 2022-02-12 18:41:11.000000 pluralize-0.1.9/pluralize.egg-info/PKG-INFO
--rw-r--r--   0 mdp       (1000) mdp       (1000)       10 2022-02-12 18:41:11.000000 pluralize-0.1.9/pluralize.egg-info/top_level.txt
--rw-r--r--   0 mdp       (1000) mdp       (1000)        1 2022-02-12 18:41:11.000000 pluralize-0.1.9/pluralize.egg-info/dependency_links.txt
--rw-r--r--   0 mdp       (1000) mdp       (1000)      204 2022-02-12 18:41:11.000000 pluralize-0.1.9/pluralize.egg-info/SOURCES.txt
--rw-r--r--   0 mdp       (1000) mdp       (1000)        1 2019-07-23 06:13:38.000000 pluralize-0.1.9/pluralize.egg-info/not-zip-safe
--rw-rw-r--   0 mdp       (1000) mdp       (1000)     2195 2021-07-16 07:51:13.000000 pluralize-0.1.9/README.md
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 00:26:08.765375 pluralize-20230507.1/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2748 2023-05-08 00:26:08.765375 pluralize-20230507.1/PKG-INFO
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     2195 2021-07-16 07:51:13.000000 pluralize-20230507.1/README.md
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 00:26:08.749375 pluralize-20230507.1/pluralize/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     5487 2023-05-08 00:23:34.000000 pluralize-20230507.1/pluralize/__init__.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 00:26:08.761375 pluralize-20230507.1/pluralize.egg-info/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     2748 2023-05-08 00:26:08.000000 pluralize-20230507.1/pluralize.egg-info/PKG-INFO
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      199 2023-05-08 00:26:08.000000 pluralize-20230507.1/pluralize.egg-info/SOURCES.txt
+-rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2023-05-08 00:26:08.000000 pluralize-20230507.1/pluralize.egg-info/dependency_links.txt
+-rw-r--r--   0 massimo   (1000) massimo   (1000)       10 2023-05-08 00:26:08.000000 pluralize-20230507.1/pluralize.egg-info/top_level.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      563 2023-05-08 00:23:34.000000 pluralize-20230507.1/pyproject.toml
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)       38 2023-05-08 00:26:08.765375 pluralize-20230507.1/setup.cfg
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 00:26:08.765375 pluralize-20230507.1/tests/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     1355 2021-07-16 07:50:13.000000 pluralize-20230507.1/tests/test_simple.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pluralize-0.1.9/pluralize/__init__.py` & `pluralize-20230507.1/pluralize/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
 import json
 import threading
 import ast
 
-__version__ = "0.1.9"
+__version__ = "20230507.1"
 
 re_language = re.compile("^\w\w(-\w+)*.json$")
 
 
 class lazyT(object):
 
     """accesssory object used to represent a T("string")"""
@@ -79,15 +79,16 @@
             with open(os.path.join(folder, filename), "w") as fp:
                 json.dump(self.languages[key], fp, sort_keys=True, indent=4)
 
     def select(self, accepted_languages="fr-CH, fr;q=0.9, en;q=0.8, de;q=0.7, *;q=0.5"):
         """given appected_langauges string from HTTP header, picks the best match"""
         if isinstance(accepted_languages, str):
             accepted_languages = [
-                tag.split(";")[0].strip() for tag in accepted_languages.split(",")
+                tag.split(";")[0].replace("_", "-").strip()
+                for tag in accepted_languages.split(",")
             ]
             for tag in accepted_languages:
                 for k in range(tag.count("-"), 0, -1):
                     subtag = "-".join(tag.split("-")[:k])
                     if not subtag in accepted_languages:
                         accepted_languages.append(subtag)
         self.local.tag = None
```

### Comparing `pluralize-0.1.9/README.md` & `pluralize-20230507.1/README.md`

 * *Files identical despite different names*

