# Comparing `tmp/mkdocs-ultralytics-plugin-0.0.1.tar.gz` & `tmp/mkdocs-ultralytics-plugin-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-ultralytics-plugin-0.0.1.tar", last modified: Mon May  8 15:44:42 2023, max compression
+gzip compressed data, was "mkdocs-ultralytics-plugin-0.0.2.tar", last modified: Mon May  8 15:48:17 2023, max compression
```

## Comparing `mkdocs-ultralytics-plugin-0.0.1.tar` & `mkdocs-ultralytics-plugin-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-05-08 15:44:42.063530 mkdocs-ultralytics-plugin-0.0.1/
--rw-r--r--   0 glennjocher   (501) staff       (20)    34523 2023-05-08 15:34:41.000000 mkdocs-ultralytics-plugin-0.0.1/LICENSE
--rw-r--r--   0 glennjocher   (501) staff       (20)      297 2023-05-08 15:44:42.063434 mkdocs-ultralytics-plugin-0.0.1/PKG-INFO
--rw-r--r--   0 glennjocher   (501) staff       (20)       76 2023-05-08 15:34:41.000000 mkdocs-ultralytics-plugin-0.0.1/README.md
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-05-08 15:44:42.063295 mkdocs-ultralytics-plugin-0.0.1/mkdocs_ultralytics_plugin.egg-info/
--rw-r--r--   0 glennjocher   (501) staff       (20)      297 2023-05-08 15:44:42.000000 mkdocs-ultralytics-plugin-0.0.1/mkdocs_ultralytics_plugin.egg-info/PKG-INFO
--rw-r--r--   0 glennjocher   (501) staff       (20)      322 2023-05-08 15:44:42.000000 mkdocs-ultralytics-plugin-0.0.1/mkdocs_ultralytics_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 glennjocher   (501) staff       (20)        1 2023-05-08 15:44:42.000000 mkdocs-ultralytics-plugin-0.0.1/mkdocs_ultralytics_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 glennjocher   (501) staff       (20)       61 2023-05-08 15:44:42.000000 mkdocs-ultralytics-plugin-0.0.1/mkdocs_ultralytics_plugin.egg-info/entry_points.txt
--rw-r--r--   0 glennjocher   (501) staff       (20)       34 2023-05-08 15:44:42.000000 mkdocs-ultralytics-plugin-0.0.1/mkdocs_ultralytics_plugin.egg-info/requires.txt
--rw-r--r--   0 glennjocher   (501) staff       (20)        1 2023-05-08 15:44:42.000000 mkdocs-ultralytics-plugin-0.0.1/mkdocs_ultralytics_plugin.egg-info/top_level.txt
--rw-r--r--   0 glennjocher   (501) staff       (20)       38 2023-05-08 15:44:42.063563 mkdocs-ultralytics-plugin-0.0.1/setup.cfg
--rw-r--r--   0 glennjocher   (501) staff       (20)      742 2023-05-08 15:43:06.000000 mkdocs-ultralytics-plugin-0.0.1/setup.py
+drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-05-08 15:48:17.155375 mkdocs-ultralytics-plugin-0.0.2/
+-rw-r--r--   0 glennjocher   (501) staff       (20)    34523 2023-05-08 15:34:41.000000 mkdocs-ultralytics-plugin-0.0.2/LICENSE
+-rw-r--r--   0 glennjocher   (501) staff       (20)      297 2023-05-08 15:48:17.155264 mkdocs-ultralytics-plugin-0.0.2/PKG-INFO
+-rw-r--r--   0 glennjocher   (501) staff       (20)       76 2023-05-08 15:34:41.000000 mkdocs-ultralytics-plugin-0.0.2/README.md
+drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-05-08 15:48:17.154788 mkdocs-ultralytics-plugin-0.0.2/mkdocs_ultralytics_plugin.egg-info/
+-rw-r--r--   0 glennjocher   (501) staff       (20)      297 2023-05-08 15:48:17.000000 mkdocs-ultralytics-plugin-0.0.2/mkdocs_ultralytics_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 glennjocher   (501) staff       (20)      375 2023-05-08 15:48:17.000000 mkdocs-ultralytics-plugin-0.0.2/mkdocs_ultralytics_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 glennjocher   (501) staff       (20)        1 2023-05-08 15:48:17.000000 mkdocs-ultralytics-plugin-0.0.2/mkdocs_ultralytics_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 glennjocher   (501) staff       (20)       61 2023-05-08 15:48:17.000000 mkdocs-ultralytics-plugin-0.0.2/mkdocs_ultralytics_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 glennjocher   (501) staff       (20)       34 2023-05-08 15:48:17.000000 mkdocs-ultralytics-plugin-0.0.2/mkdocs_ultralytics_plugin.egg-info/requires.txt
+-rw-r--r--   0 glennjocher   (501) staff       (20)        7 2023-05-08 15:48:17.000000 mkdocs-ultralytics-plugin-0.0.2/mkdocs_ultralytics_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-05-08 15:48:17.154983 mkdocs-ultralytics-plugin-0.0.2/plugin/
+-rw-r--r--   0 glennjocher   (501) staff       (20)        0 2023-05-08 15:47:47.000000 mkdocs-ultralytics-plugin-0.0.2/plugin/__init__.py
+-rw-r--r--   0 glennjocher   (501) staff       (20)     1794 2023-05-08 15:42:03.000000 mkdocs-ultralytics-plugin-0.0.2/plugin/images_and_descriptions.py
+-rw-r--r--   0 glennjocher   (501) staff       (20)       38 2023-05-08 15:48:17.155410 mkdocs-ultralytics-plugin-0.0.2/setup.cfg
+-rw-r--r--   0 glennjocher   (501) staff       (20)      742 2023-05-08 15:48:09.000000 mkdocs-ultralytics-plugin-0.0.2/setup.py
```

### Comparing `mkdocs-ultralytics-plugin-0.0.1/LICENSE` & `mkdocs-ultralytics-plugin-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-ultralytics-plugin-0.0.1/setup.py` & `mkdocs-ultralytics-plugin-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #   - search
 #   - ultralytics
 
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-ultralytics-plugin',
-    version='0.0.1',
+    version='0.0.2',
     description='An MkDocs plugin that generates meta description and image tags based on the first paragraph and the '
                 'first image in a page',
     author='Ultralytics',
     author_email='hello@ultralytics.com',
     license='AGPL-3.0',
     packages=find_packages(),
     install_requires=[
```

