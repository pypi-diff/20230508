# Comparing `tmp/llamabot-0.0.8.tar.gz` & `tmp/llamabot-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamabot-0.0.8.tar", last modified: Sun Apr 16 18:23:47 2023, max compression
+gzip compressed data, was "llamabot-0.0.9.tar", last modified: Thu Apr 20 01:53:11 2023, max compression
```

## Comparing `llamabot-0.0.8.tar` & `llamabot-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-16 18:23:47.719910 llamabot-0.0.8/
--rw-r--r--   0 ericmjl    (501) staff       (20)      124 2023-04-03 18:38:54.000000 llamabot-0.0.8/MANIFEST.in
--rw-r--r--   0 ericmjl    (501) staff       (20)       95 2023-04-16 18:23:47.719761 llamabot-0.0.8/PKG-INFO
--rw-r--r--   0 ericmjl    (501) staff       (20)     6237 2023-04-11 12:50:37.000000 llamabot-0.0.8/README.md
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-16 18:23:47.718025 llamabot-0.0.8/llamabot/
--rw-r--r--   0 ericmjl    (501) staff       (20)      284 2023-04-11 12:47:57.000000 llamabot-0.0.8/llamabot/__init__.py
--rw-r--r--   0 ericmjl    (501) staff       (20)     7436 2023-04-16 18:23:26.000000 llamabot-0.0.8/llamabot/bot.py
--rw-r--r--   0 ericmjl    (501) staff       (20)      652 2023-04-03 18:38:54.000000 llamabot-0.0.8/llamabot/cli.py
--rw-r--r--   0 ericmjl    (501) staff       (20)       35 2023-04-03 18:38:54.000000 llamabot-0.0.8/llamabot/preprocessing.py
--rw-r--r--   0 ericmjl    (501) staff       (20)      182 2023-04-03 18:38:54.000000 llamabot-0.0.8/llamabot/schemas.py
--rw-r--r--   0 ericmjl    (501) staff       (20)       30 2023-04-03 18:38:54.000000 llamabot-0.0.8/llamabot/utils.py
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-16 18:23:47.719138 llamabot-0.0.8/llamabot.egg-info/
--rw-r--r--   0 ericmjl    (501) staff       (20)       95 2023-04-16 18:23:47.000000 llamabot-0.0.8/llamabot.egg-info/PKG-INFO
--rw-r--r--   0 ericmjl    (501) staff       (20)      409 2023-04-16 18:23:47.000000 llamabot-0.0.8/llamabot.egg-info/SOURCES.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)        1 2023-04-16 18:23:47.000000 llamabot-0.0.8/llamabot.egg-info/dependency_links.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)       46 2023-04-16 18:23:47.000000 llamabot-0.0.8/llamabot.egg-info/entry_points.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)      102 2023-04-16 18:23:47.000000 llamabot-0.0.8/llamabot.egg-info/requires.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)        9 2023-04-16 18:23:47.000000 llamabot-0.0.8/llamabot.egg-info/top_level.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)     1549 2023-04-16 18:23:44.000000 llamabot-0.0.8/pyproject.toml
--rw-r--r--   0 ericmjl    (501) staff       (20)       38 2023-04-16 18:23:47.719958 llamabot-0.0.8/setup.cfg
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-16 18:23:47.719562 llamabot-0.0.8/tests/
--rw-r--r--   0 ericmjl    (501) staff       (20)       26 2023-04-03 18:38:54.000000 llamabot-0.0.8/tests/test___init__.py
--rw-r--r--   0 ericmjl    (501) staff       (20)       30 2023-04-03 18:38:54.000000 llamabot-0.0.8/tests/test_cli.py
--rw-r--r--   0 ericmjl    (501) staff       (20)       52 2023-04-03 18:38:54.000000 llamabot-0.0.8/tests/test_models.py
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-20 01:53:11.062571 llamabot-0.0.9/
+-rw-r--r--   0 ericmjl    (501) staff       (20)      124 2023-04-03 18:38:54.000000 llamabot-0.0.9/MANIFEST.in
+-rw-r--r--   0 ericmjl    (501) staff       (20)       95 2023-04-20 01:53:11.062428 llamabot-0.0.9/PKG-INFO
+-rw-r--r--   0 ericmjl    (501) staff       (20)     6237 2023-04-11 12:50:37.000000 llamabot-0.0.9/README.md
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-20 01:53:11.059405 llamabot-0.0.9/llamabot/
+-rw-r--r--   0 ericmjl    (501) staff       (20)      284 2023-04-11 12:47:57.000000 llamabot-0.0.9/llamabot/__init__.py
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-20 01:53:11.061601 llamabot-0.0.9/llamabot/bot/
+-rw-r--r--   0 ericmjl    (501) staff       (20)      371 2023-04-17 23:12:57.000000 llamabot-0.0.9/llamabot/bot/__init__.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)     4811 2023-04-20 01:51:42.000000 llamabot-0.0.9/llamabot/bot/chatbot.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)     4268 2023-04-17 23:09:57.000000 llamabot-0.0.9/llamabot/bot/querybot.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)     3792 2023-04-19 12:22:32.000000 llamabot-0.0.9/llamabot/bot/simplebot.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)      652 2023-04-03 18:38:54.000000 llamabot-0.0.9/llamabot/cli.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)     2717 2023-04-19 12:17:38.000000 llamabot-0.0.9/llamabot/panel_utils.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)       35 2023-04-03 18:38:54.000000 llamabot-0.0.9/llamabot/preprocessing.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)      182 2023-04-03 18:38:54.000000 llamabot-0.0.9/llamabot/schemas.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)       30 2023-04-03 18:38:54.000000 llamabot-0.0.9/llamabot/utils.py
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-20 01:53:11.060614 llamabot-0.0.9/llamabot.egg-info/
+-rw-r--r--   0 ericmjl    (501) staff       (20)       95 2023-04-20 01:53:11.000000 llamabot-0.0.9/llamabot.egg-info/PKG-INFO
+-rw-r--r--   0 ericmjl    (501) staff       (20)      517 2023-04-20 01:53:11.000000 llamabot-0.0.9/llamabot.egg-info/SOURCES.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)        1 2023-04-20 01:53:11.000000 llamabot-0.0.9/llamabot.egg-info/dependency_links.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)       46 2023-04-20 01:53:11.000000 llamabot-0.0.9/llamabot.egg-info/entry_points.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)       96 2023-04-20 01:53:11.000000 llamabot-0.0.9/llamabot.egg-info/requires.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)        9 2023-04-20 01:53:11.000000 llamabot-0.0.9/llamabot.egg-info/top_level.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1537 2023-04-20 01:52:51.000000 llamabot-0.0.9/pyproject.toml
+-rw-r--r--   0 ericmjl    (501) staff       (20)       38 2023-04-20 01:53:11.062612 llamabot-0.0.9/setup.cfg
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-20 01:53:11.062205 llamabot-0.0.9/tests/
+-rw-r--r--   0 ericmjl    (501) staff       (20)       26 2023-04-03 18:38:54.000000 llamabot-0.0.9/tests/test___init__.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)       30 2023-04-03 18:38:54.000000 llamabot-0.0.9/tests/test_cli.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)       52 2023-04-03 18:38:54.000000 llamabot-0.0.9/tests/test_models.py
```

### Comparing `llamabot-0.0.8/README.md` & `llamabot-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `llamabot-0.0.8/llamabot/cli.py` & `llamabot-0.0.9/llamabot/cli.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.0.8/pyproject.toml` & `llamabot-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -57,25 +57,24 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 namespaces = false
 
 [project]
 name = "llamabot"
-version = "0.0.8"
+version = "0.0.9"
 dependencies = [
     "openai",
     "langchain",
-    "typer",
     "llama_index",
 ]
 
 [project.optional-dependencies]
 tests = [
-    "pytest"
+    "pytest",
 ]
 docs = [
     "mkdocs-material",
     "mkdocs",
     "panel",
     "jupyter_bokeh"
 ]
```

