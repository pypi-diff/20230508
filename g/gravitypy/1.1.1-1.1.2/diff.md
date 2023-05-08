# Comparing `tmp/gravitypy-1.1.1.tar.gz` & `tmp/gravitypy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitypy-1.1.1.tar", last modified: Mon May  8 18:40:08 2023, max compression
+gzip compressed data, was "gravitypy-1.1.2.tar", last modified: Mon May  8 18:51:02 2023, max compression
```

## Comparing `gravitypy-1.1.1.tar` & `gravitypy-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 18:40:08.920201 gravitypy-1.1.1/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 20:40:23.000000 gravitypy-1.1.1/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 20:40:23.000000 gravitypy-1.1.1/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-08 18:40:08.920201 gravitypy-1.1.1/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1340 2023-05-07 20:40:23.000000 gravitypy-1.1.1/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 18:40:08.920201 gravitypy-1.1.1/gravitypy/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 20:40:23.000000 gravitypy-1.1.1/gravitypy/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       60 2023-05-08 18:32:28.000000 gravitypy-1.1.1/gravitypy/__main__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15495 2023-05-08 18:34:31.000000 gravitypy-1.1.1/gravitypy/main.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 18:40:08.920201 gravitypy-1.1.1/gravitypy/resources/
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 18:40:08.920201 gravitypy-1.1.1/gravitypy/resources/fonts/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 20:40:23.000000 gravitypy-1.1.1/gravitypy/resources/fonts/minecraft_font.ttf
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 18:40:08.920201 gravitypy-1.1.1/gravitypy.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-08 18:40:08.000000 gravitypy-1.1.1/gravitypy.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      362 2023-05-08 18:40:08.000000 gravitypy-1.1.1/gravitypy.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-08 18:40:08.000000 gravitypy-1.1.1/gravitypy.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-05-08 18:40:08.000000 gravitypy-1.1.1/gravitypy.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-08 18:40:08.000000 gravitypy-1.1.1/gravitypy.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-05-08 18:40:08.000000 gravitypy-1.1.1/gravitypy.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 20:40:23.000000 gravitypy-1.1.1/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-08 18:40:08.920201 gravitypy-1.1.1/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      973 2023-05-08 18:39:48.000000 gravitypy-1.1.1/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 18:51:02.120184 gravitypy-1.1.2/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 20:40:23.000000 gravitypy-1.1.2/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 20:40:23.000000 gravitypy-1.1.2/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-08 18:51:02.120184 gravitypy-1.1.2/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1340 2023-05-07 20:40:23.000000 gravitypy-1.1.2/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 18:51:02.120184 gravitypy-1.1.2/gravitypy/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 20:40:23.000000 gravitypy-1.1.2/gravitypy/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-08 18:43:26.000000 gravitypy-1.1.2/gravitypy/__main__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15495 2023-05-08 18:34:31.000000 gravitypy-1.1.2/gravitypy/main.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 18:51:02.120184 gravitypy-1.1.2/gravitypy/resources/
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 18:51:02.120184 gravitypy-1.1.2/gravitypy/resources/fonts/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 20:40:23.000000 gravitypy-1.1.2/gravitypy/resources/fonts/minecraft_font.ttf
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 18:51:02.120184 gravitypy-1.1.2/gravitypy.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-08 18:51:02.000000 gravitypy-1.1.2/gravitypy.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      362 2023-05-08 18:51:02.000000 gravitypy-1.1.2/gravitypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-08 18:51:02.000000 gravitypy-1.1.2/gravitypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-05-08 18:51:02.000000 gravitypy-1.1.2/gravitypy.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-08 18:51:02.000000 gravitypy-1.1.2/gravitypy.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-05-08 18:51:02.000000 gravitypy-1.1.2/gravitypy.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 20:40:23.000000 gravitypy-1.1.2/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-08 18:51:02.120184 gravitypy-1.1.2/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      973 2023-05-08 18:50:29.000000 gravitypy-1.1.2/setup.py
```

### Comparing `gravitypy-1.1.1/LICENSE` & `gravitypy-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.1/README.md` & `gravitypy-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.1/gravitypy/main.py` & `gravitypy-1.1.2/gravitypy/main.py`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.1/gravitypy/resources/fonts/minecraft_font.ttf` & `gravitypy-1.1.2/gravitypy/resources/fonts/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.1/setup.py` & `gravitypy-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 req_file = os.path.join(here, 'requirements.txt')
 with open(req_file, 'r') as f:
     REQUIREMENTS = [line.strip() for line in f.readlines()]
 LONG_DESCRIPTION = 'Pygame N-Body gravity simulation app'
 
 setup(
    name='gravitypy',
-   version='1.1.1',
+   version='1.1.2',
    description='Particles Gravity',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/Particles_Gravity",
    long_description_content_type="text/markdown",
    package_data={'gravitypy': ['*']},
```

