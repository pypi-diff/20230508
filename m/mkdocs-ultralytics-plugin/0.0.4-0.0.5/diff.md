# Comparing `tmp/mkdocs-ultralytics-plugin-0.0.4.tar.gz` & `tmp/mkdocs-ultralytics-plugin-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-ultralytics-plugin-0.0.4.tar", last modified: Mon May  8 15:56:53 2023, max compression
+gzip compressed data, was "mkdocs-ultralytics-plugin-0.0.5.tar", last modified: Mon May  8 16:00:13 2023, max compression
```

## Comparing `mkdocs-ultralytics-plugin-0.0.4.tar` & `mkdocs-ultralytics-plugin-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-05-08 15:56:53.648413 mkdocs-ultralytics-plugin-0.0.4/
--rw-r--r--   0 glennjocher   (501) staff       (20)    34523 2023-05-08 15:34:41.000000 mkdocs-ultralytics-plugin-0.0.4/LICENSE
--rw-r--r--   0 glennjocher   (501) staff       (20)      297 2023-05-08 15:56:53.648291 mkdocs-ultralytics-plugin-0.0.4/PKG-INFO
--rw-r--r--   0 glennjocher   (501) staff       (20)       76 2023-05-08 15:34:41.000000 mkdocs-ultralytics-plugin-0.0.4/README.md
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-05-08 15:56:53.648127 mkdocs-ultralytics-plugin-0.0.4/mkdocs_ultralytics_plugin.egg-info/
--rw-r--r--   0 glennjocher   (501) staff       (20)      297 2023-05-08 15:56:53.000000 mkdocs-ultralytics-plugin-0.0.4/mkdocs_ultralytics_plugin.egg-info/PKG-INFO
--rw-r--r--   0 glennjocher   (501) staff       (20)      322 2023-05-08 15:56:53.000000 mkdocs-ultralytics-plugin-0.0.4/mkdocs_ultralytics_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 glennjocher   (501) staff       (20)        1 2023-05-08 15:56:53.000000 mkdocs-ultralytics-plugin-0.0.4/mkdocs_ultralytics_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 glennjocher   (501) staff       (20)       61 2023-05-08 15:56:53.000000 mkdocs-ultralytics-plugin-0.0.4/mkdocs_ultralytics_plugin.egg-info/entry_points.txt
--rw-r--r--   0 glennjocher   (501) staff       (20)       34 2023-05-08 15:56:53.000000 mkdocs-ultralytics-plugin-0.0.4/mkdocs_ultralytics_plugin.egg-info/requires.txt
--rw-r--r--   0 glennjocher   (501) staff       (20)        1 2023-05-08 15:56:53.000000 mkdocs-ultralytics-plugin-0.0.4/mkdocs_ultralytics_plugin.egg-info/top_level.txt
--rw-r--r--   0 glennjocher   (501) staff       (20)       38 2023-05-08 15:56:53.648454 mkdocs-ultralytics-plugin-0.0.4/setup.cfg
--rw-r--r--   0 glennjocher   (501) staff       (20)      742 2023-05-08 15:56:31.000000 mkdocs-ultralytics-plugin-0.0.4/setup.py
+drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-05-08 16:00:13.256636 mkdocs-ultralytics-plugin-0.0.5/
+-rw-r--r--   0 glennjocher   (501) staff       (20)    34523 2023-05-08 15:34:41.000000 mkdocs-ultralytics-plugin-0.0.5/LICENSE
+-rw-r--r--   0 glennjocher   (501) staff       (20)      297 2023-05-08 16:00:13.256509 mkdocs-ultralytics-plugin-0.0.5/PKG-INFO
+-rw-r--r--   0 glennjocher   (501) staff       (20)       76 2023-05-08 15:34:41.000000 mkdocs-ultralytics-plugin-0.0.5/README.md
+drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-05-08 16:00:13.256333 mkdocs-ultralytics-plugin-0.0.5/mkdocs_ultralytics_plugin.egg-info/
+-rw-r--r--   0 glennjocher   (501) staff       (20)      297 2023-05-08 16:00:13.000000 mkdocs-ultralytics-plugin-0.0.5/mkdocs_ultralytics_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 glennjocher   (501) staff       (20)      322 2023-05-08 16:00:13.000000 mkdocs-ultralytics-plugin-0.0.5/mkdocs_ultralytics_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 glennjocher   (501) staff       (20)        1 2023-05-08 16:00:13.000000 mkdocs-ultralytics-plugin-0.0.5/mkdocs_ultralytics_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 glennjocher   (501) staff       (20)       68 2023-05-08 16:00:13.000000 mkdocs-ultralytics-plugin-0.0.5/mkdocs_ultralytics_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 glennjocher   (501) staff       (20)       34 2023-05-08 16:00:13.000000 mkdocs-ultralytics-plugin-0.0.5/mkdocs_ultralytics_plugin.egg-info/requires.txt
+-rw-r--r--   0 glennjocher   (501) staff       (20)        1 2023-05-08 16:00:13.000000 mkdocs-ultralytics-plugin-0.0.5/mkdocs_ultralytics_plugin.egg-info/top_level.txt
+-rw-r--r--   0 glennjocher   (501) staff       (20)       38 2023-05-08 16:00:13.256720 mkdocs-ultralytics-plugin-0.0.5/setup.cfg
+-rw-r--r--   0 glennjocher   (501) staff       (20)      749 2023-05-08 16:00:07.000000 mkdocs-ultralytics-plugin-0.0.5/setup.py
```

### Comparing `mkdocs-ultralytics-plugin-0.0.4/LICENSE` & `mkdocs-ultralytics-plugin-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-ultralytics-plugin-0.0.4/setup.py` & `mkdocs-ultralytics-plugin-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 #   - search
 #   - ultralytics
 
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-ultralytics-plugin',
-    version='0.0.4',
+    version='0.0.5',
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
-            'ultralytics = plugin:DescriptionImagePlugin'
+            'mkdocs-ultralytics = plugin:DescriptionImagePlugin'
         ]
     }
 )
```

