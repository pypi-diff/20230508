# Comparing `tmp/mkdocs-ultralytics-plugin-0.0.8.tar.gz` & `tmp/mkdocs-ultralytics-plugin-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-ultralytics-plugin-0.0.8.tar", last modified: Mon May  8 17:43:54 2023, max compression
+gzip compressed data, was "mkdocs-ultralytics-plugin-0.0.9.tar", last modified: Mon May  8 17:45:42 2023, max compression
```

## Comparing `mkdocs-ultralytics-plugin-0.0.8.tar` & `mkdocs-ultralytics-plugin-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-05-08 17:43:54.737547 mkdocs-ultralytics-plugin-0.0.8/
--rw-r--r--   0 glennjocher   (501) staff       (20)    34523 2023-05-08 15:34:41.000000 mkdocs-ultralytics-plugin-0.0.8/LICENSE
--rw-r--r--   0 glennjocher   (501) staff       (20)      297 2023-05-08 17:43:54.737439 mkdocs-ultralytics-plugin-0.0.8/PKG-INFO
--rw-r--r--   0 glennjocher   (501) staff       (20)       76 2023-05-08 15:34:41.000000 mkdocs-ultralytics-plugin-0.0.8/README.md
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-05-08 17:43:54.737076 mkdocs-ultralytics-plugin-0.0.8/mkdocs_ultralytics_plugin.egg-info/
--rw-r--r--   0 glennjocher   (501) staff       (20)      297 2023-05-08 17:43:54.000000 mkdocs-ultralytics-plugin-0.0.8/mkdocs_ultralytics_plugin.egg-info/PKG-INFO
--rw-r--r--   0 glennjocher   (501) staff       (20)      356 2023-05-08 17:43:54.000000 mkdocs-ultralytics-plugin-0.0.8/mkdocs_ultralytics_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 glennjocher   (501) staff       (20)        1 2023-05-08 17:43:54.000000 mkdocs-ultralytics-plugin-0.0.8/mkdocs_ultralytics_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 glennjocher   (501) staff       (20)       57 2023-05-08 17:43:54.000000 mkdocs-ultralytics-plugin-0.0.8/mkdocs_ultralytics_plugin.egg-info/entry_points.txt
--rw-r--r--   0 glennjocher   (501) staff       (20)       34 2023-05-08 17:43:54.000000 mkdocs-ultralytics-plugin-0.0.8/mkdocs_ultralytics_plugin.egg-info/requires.txt
--rw-r--r--   0 glennjocher   (501) staff       (20)        7 2023-05-08 17:43:54.000000 mkdocs-ultralytics-plugin-0.0.8/mkdocs_ultralytics_plugin.egg-info/top_level.txt
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-05-08 17:43:54.737290 mkdocs-ultralytics-plugin-0.0.8/plugin/
--rw-r--r--   0 glennjocher   (501) staff       (20)       29 2023-05-08 17:43:28.000000 mkdocs-ultralytics-plugin-0.0.8/plugin/__init__.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     1535 2023-05-08 17:42:10.000000 mkdocs-ultralytics-plugin-0.0.8/plugin/main.py
--rw-r--r--   0 glennjocher   (501) staff       (20)       38 2023-05-08 17:43:54.737581 mkdocs-ultralytics-plugin-0.0.8/setup.cfg
--rw-r--r--   0 glennjocher   (501) staff       (20)      738 2023-05-08 17:43:46.000000 mkdocs-ultralytics-plugin-0.0.8/setup.py
+drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-05-08 17:45:42.708444 mkdocs-ultralytics-plugin-0.0.9/
+-rw-r--r--   0 glennjocher   (501) staff       (20)    34523 2023-05-08 15:34:41.000000 mkdocs-ultralytics-plugin-0.0.9/LICENSE
+-rw-r--r--   0 glennjocher   (501) staff       (20)      297 2023-05-08 17:45:42.708335 mkdocs-ultralytics-plugin-0.0.9/PKG-INFO
+-rw-r--r--   0 glennjocher   (501) staff       (20)       76 2023-05-08 15:34:41.000000 mkdocs-ultralytics-plugin-0.0.9/README.md
+drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-05-08 17:45:42.707906 mkdocs-ultralytics-plugin-0.0.9/mkdocs_ultralytics_plugin.egg-info/
+-rw-r--r--   0 glennjocher   (501) staff       (20)      297 2023-05-08 17:45:42.000000 mkdocs-ultralytics-plugin-0.0.9/mkdocs_ultralytics_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 glennjocher   (501) staff       (20)      356 2023-05-08 17:45:42.000000 mkdocs-ultralytics-plugin-0.0.9/mkdocs_ultralytics_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 glennjocher   (501) staff       (20)        1 2023-05-08 17:45:42.000000 mkdocs-ultralytics-plugin-0.0.9/mkdocs_ultralytics_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 glennjocher   (501) staff       (20)       49 2023-05-08 17:45:42.000000 mkdocs-ultralytics-plugin-0.0.9/mkdocs_ultralytics_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 glennjocher   (501) staff       (20)       34 2023-05-08 17:45:42.000000 mkdocs-ultralytics-plugin-0.0.9/mkdocs_ultralytics_plugin.egg-info/requires.txt
+-rw-r--r--   0 glennjocher   (501) staff       (20)        7 2023-05-08 17:45:42.000000 mkdocs-ultralytics-plugin-0.0.9/mkdocs_ultralytics_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-05-08 17:45:42.708163 mkdocs-ultralytics-plugin-0.0.9/plugin/
+-rw-r--r--   0 glennjocher   (501) staff       (20)       29 2023-05-08 17:43:28.000000 mkdocs-ultralytics-plugin-0.0.9/plugin/__init__.py
+-rw-r--r--   0 glennjocher   (501) staff       (20)     1535 2023-05-08 17:42:10.000000 mkdocs-ultralytics-plugin-0.0.9/plugin/main.py
+-rw-r--r--   0 glennjocher   (501) staff       (20)       38 2023-05-08 17:45:42.708489 mkdocs-ultralytics-plugin-0.0.9/setup.cfg
+-rw-r--r--   0 glennjocher   (501) staff       (20)      730 2023-05-08 17:45:37.000000 mkdocs-ultralytics-plugin-0.0.9/setup.py
```

### Comparing `mkdocs-ultralytics-plugin-0.0.8/LICENSE` & `mkdocs-ultralytics-plugin-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-ultralytics-plugin-0.0.8/plugin/main.py` & `mkdocs-ultralytics-plugin-0.0.9/plugin/main.py`

 * *Files identical despite different names*

### Comparing `mkdocs-ultralytics-plugin-0.0.8/setup.py` & `mkdocs-ultralytics-plugin-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 #   - search
 #   - ultralytics
 
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-ultralytics-plugin',
-    version='0.0.8',
+    version='0.0.9',
     description='An MkDocs plugin that generates meta description and image tags based on the first paragraph and the '
                 'first image in a page',
     author='Ultralytics',
     author_email='hello@ultralytics.com',
     license='AGPL-3.0',
     packages=find_packages(),
     install_requires=[
         'mkdocs>=1.0',
         'beautifulsoup4>=4.9.3',
     ],
     entry_points={
         'mkdocs.plugins': [
-            'mkdocs_ultralytics2 = plugin:MetaPlugin'
+            'ultralytics = plugin:MetaPlugin'
         ]
     }
 )
```

