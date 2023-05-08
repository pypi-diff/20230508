# Comparing `tmp/subtitle-filter-1.4.5.tar.gz` & `tmp/subtitle-filter-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subtitle-filter-1.4.5.tar", last modified: Fri Mar 10 10:52:27 2023, max compression
+gzip compressed data, was "subtitle-filter-1.4.6.tar", last modified: Mon May  8 21:12:12 2023, max compression
```

## Comparing `subtitle-filter-1.4.5.tar` & `subtitle-filter-1.4.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:52:27.337424 subtitle-filter-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-10 10:52:17.000000 subtitle-filter-1.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-03-10 10:52:27.337424 subtitle-filter-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-03-10 10:52:17.000000 subtitle-filter-1.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 10:52:27.337424 subtitle-filter-1.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-10 10:52:17.000000 subtitle-filter-1.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:52:27.333424 subtitle-filter-1.4.5/subtitle_filter/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-10 10:52:17.000000 subtitle-filter-1.4.5/subtitle_filter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:52:27.333424 subtitle-filter-1.4.5/subtitle_filter/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-03-10 10:52:17.000000 subtitle-filter-1.4.5/subtitle_filter/bin/filter-subtitles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:52:27.337424 subtitle-filter-1.4.5/subtitle_filter/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 10:52:17.000000 subtitle-filter-1.4.5/subtitle_filter/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-03-10 10:52:17.000000 subtitle-filter-1.4.5/subtitle_filter/libs/subtitle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:52:27.333424 subtitle-filter-1.4.5/subtitle_filter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-03-10 10:52:27.000000 subtitle-filter-1.4.5/subtitle_filter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-10 10:52:27.000000 subtitle-filter-1.4.5/subtitle_filter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 10:52:27.000000 subtitle-filter-1.4.5/subtitle_filter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-10 10:52:27.000000 subtitle-filter-1.4.5/subtitle_filter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:12:12.847033 subtitle-filter-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-08 21:12:00.000000 subtitle-filter-1.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-08 21:12:12.847033 subtitle-filter-1.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-08 21:12:00.000000 subtitle-filter-1.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 21:12:12.847033 subtitle-filter-1.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-08 21:12:00.000000 subtitle-filter-1.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:12:12.847033 subtitle-filter-1.4.6/subtitle_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 21:12:00.000000 subtitle-filter-1.4.6/subtitle_filter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:12:12.847033 subtitle-filter-1.4.6/subtitle_filter/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-08 21:12:00.000000 subtitle-filter-1.4.6/subtitle_filter/bin/filter-subtitles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:12:12.847033 subtitle-filter-1.4.6/subtitle_filter/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:12:00.000000 subtitle-filter-1.4.6/subtitle_filter/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-05-08 21:12:00.000000 subtitle-filter-1.4.6/subtitle_filter/libs/subtitle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:12:12.847033 subtitle-filter-1.4.6/subtitle_filter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-08 21:12:12.000000 subtitle-filter-1.4.6/subtitle_filter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-08 21:12:12.000000 subtitle-filter-1.4.6/subtitle_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:12:12.000000 subtitle-filter-1.4.6/subtitle_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-08 21:12:12.000000 subtitle-filter-1.4.6/subtitle_filter.egg-info/top_level.txt
```

### Comparing `subtitle-filter-1.4.5/LICENSE` & `subtitle-filter-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `subtitle-filter-1.4.5/PKG-INFO` & `subtitle-filter-1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: subtitle-filter
-Version: 1.4.5
+Version: 1.4.6
 Summary: Filter SDH entries and more from .srt files
 Home-page: https://github.com/mattlyon93/filter-subs
-Download-URL: https://github.com/mattlyon93/filter-subs/archive/v1.4.5.tar.gz
+Download-URL: https://github.com/mattlyon93/filter-subs/archive/v1.4.6.tar.gz
 Author: Matt Lyon
 Author-email: matthewlyon18@gmail.com
 License: MIT License
 Keywords: subtitle,SDH,hard-of-hearing,filter,movie,tv
 Classifier: Programming Language :: Python
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
```

### Comparing `subtitle-filter-1.4.5/README.md` & `subtitle-filter-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `subtitle-filter-1.4.5/setup.py` & `subtitle-filter-1.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 '''setup.py, use this to install module'''
 from os import path
 from setuptools import setup
 
-version = '1.4.5'
+version = '1.4.6'
 this_dir = path.abspath(path.dirname(__file__))
 with open(path.join(this_dir, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='subtitle-filter',
     version=version,
```

### Comparing `subtitle-filter-1.4.5/subtitle_filter/bin/filter-subtitles.py` & `subtitle-filter-1.4.6/subtitle_filter/bin/filter-subtitles.py`

 * *Files identical despite different names*

### Comparing `subtitle-filter-1.4.5/subtitle_filter/libs/subtitle.py` & `subtitle-filter-1.4.6/subtitle_filter/libs/subtitle.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 '''Module containing Subtitle and Subtitles classes'''
 import os
 import re
-import codecs
 
 AUTHOR_STRINGS = (
     'synced and corrected by',
     'sync and corrections by',
     'subtitles by',
     'encoded and released by',
     'opensubtitles.org',
     'please rate this subtitle',
     'captioning sponsored by',
     'captioned by',
 )
 
 
+def has_bom(filename):
+    '''Tests whether file byte order marking'''
+    with open(filename, 'rb') as file:
+        bom_bytes = file.read(4)
+        return bom_bytes.startswith(
+            (b'\xef\xbb\xbf', b'\xff\xfe', b'\xfe\xff', b'\xff\xfe\x00\x00', b'\x00\x00\xfe\xff')
+        )
+
+
 class Subtitle:
     '''Subtitle contents object
     (invidual subtitle entry)
     '''
 
     def __init__(self):
         self._index = None
@@ -220,16 +228,20 @@
     @property
     def ext(self):
         '''Extension of mediafile'''
         _, ext = os.path.splitext(self._fullpath)
         return ext
 
     def _get_line_list(self):
-        with codecs.open(self.filepath, 'r', encoding='utf-8-sig', errors='ignore') as fdata:
-            line_list = fdata.readlines()
+        if has_bom(self.filepath):
+            with open(self.filepath, 'r', encoding='utf-8-sig') as fdata:
+                line_list = fdata.readlines()
+        else:
+            with open(self.filepath, 'r', encoding='utf-8') as fdata:
+                line_list = fdata.readlines()
         line_list_filtered = [x.rstrip() for x in line_list]
         return line_list_filtered
 
     def _parse_subs(self):
         sub_list = [Subtitle()]
         for line in self._line_list:
             # If the index has not yet been created in latest sublist item
```

### Comparing `subtitle-filter-1.4.5/subtitle_filter.egg-info/PKG-INFO` & `subtitle-filter-1.4.6/subtitle_filter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: subtitle-filter
-Version: 1.4.5
+Version: 1.4.6
 Summary: Filter SDH entries and more from .srt files
 Home-page: https://github.com/mattlyon93/filter-subs
-Download-URL: https://github.com/mattlyon93/filter-subs/archive/v1.4.5.tar.gz
+Download-URL: https://github.com/mattlyon93/filter-subs/archive/v1.4.6.tar.gz
 Author: Matt Lyon
 Author-email: matthewlyon18@gmail.com
 License: MIT License
 Keywords: subtitle,SDH,hard-of-hearing,filter,movie,tv
 Classifier: Programming Language :: Python
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
```

