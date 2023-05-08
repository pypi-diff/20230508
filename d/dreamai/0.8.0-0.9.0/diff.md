# Comparing `tmp/dreamai-0.8.0.tar.gz` & `tmp/dreamai-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai-0.8.0.tar", last modified: Tue May  2 14:01:54 2023, max compression
+gzip compressed data, was "dreamai-0.9.0.tar", last modified: Thu May  4 00:50:09 2023, max compression
```

## Comparing `dreamai-0.8.0.tar` & `dreamai-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 14:01:54.141986 dreamai-0.8.0/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2022-09-05 16:31:43.000000 dreamai-0.8.0/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2022-09-05 16:31:43.000000 dreamai-0.8.0/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-05-02 14:01:54.141986 dreamai-0.8.0/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      130 2023-05-02 14:01:47.000000 dreamai-0.8.0/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 14:01:54.141986 dreamai-0.8.0/dreamai/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-02 14:01:42.000000 dreamai-0.8.0/dreamai/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     7897 2023-05-02 14:01:42.000000 dreamai-0.8.0/dreamai/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     8737 2023-05-02 14:01:42.000000 dreamai-0.8.0/dreamai/core.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      849 2023-05-02 14:01:07.000000 dreamai-0.8.0/dreamai/imports.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     8258 2023-05-02 14:01:42.000000 dreamai-0.8.0/dreamai/vision.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 14:01:54.141986 dreamai-0.8.0/dreamai.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-05-02 14:01:54.000000 dreamai-0.8.0/dreamai.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      361 2023-05-02 14:01:54.000000 dreamai-0.8.0/dreamai.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-02 14:01:54.000000 dreamai-0.8.0/dreamai.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       36 2023-05-02 14:01:54.000000 dreamai-0.8.0/dreamai.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-01-18 11:49:09.000000 dreamai-0.8.0/dreamai.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      483 2023-05-02 14:01:54.000000 dreamai-0.8.0/dreamai.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        8 2023-05-02 14:01:54.000000 dreamai-0.8.0/dreamai.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     1143 2023-05-02 14:01:33.000000 dreamai-0.8.0/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-02 14:01:54.141986 dreamai-0.8.0/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2641 2023-05-02 13:55:29.000000 dreamai-0.8.0/setup.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 00:50:09.494943 dreamai-0.9.0/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2022-09-05 16:31:43.000000 dreamai-0.9.0/LICENSE
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2022-09-05 16:31:43.000000 dreamai-0.9.0/MANIFEST.in
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-05-04 00:50:09.494943 dreamai-0.9.0/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      130 2023-05-02 14:01:47.000000 dreamai-0.9.0/README.md
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 00:50:09.494943 dreamai-0.9.0/dreamai/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-04 00:50:04.000000 dreamai-0.9.0/dreamai/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     7897 2023-05-04 00:50:04.000000 dreamai-0.9.0/dreamai/_modidx.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     8873 2023-05-04 00:50:04.000000 dreamai-0.9.0/dreamai/core.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      858 2023-05-02 20:23:11.000000 dreamai-0.9.0/dreamai/imports.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     8258 2023-05-04 00:50:04.000000 dreamai-0.9.0/dreamai/vision.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 00:50:09.494943 dreamai-0.9.0/dreamai.egg-info/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-05-04 00:50:09.000000 dreamai-0.9.0/dreamai.egg-info/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      361 2023-05-04 00:50:09.000000 dreamai-0.9.0/dreamai.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-04 00:50:09.000000 dreamai-0.9.0/dreamai.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       36 2023-05-04 00:50:09.000000 dreamai-0.9.0/dreamai.egg-info/entry_points.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-01-18 11:49:09.000000 dreamai-0.9.0/dreamai.egg-info/not-zip-safe
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2564 2023-05-04 00:50:09.000000 dreamai-0.9.0/dreamai.egg-info/requires.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        8 2023-05-04 00:50:09.000000 dreamai-0.9.0/dreamai.egg-info/top_level.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     3224 2023-05-04 00:50:01.000000 dreamai-0.9.0/settings.ini
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-04 00:50:09.494943 dreamai-0.9.0/setup.cfg
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2641 2023-05-02 13:55:29.000000 dreamai-0.9.0/setup.py
```

### Comparing `dreamai-0.8.0/LICENSE` & `dreamai-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamai-0.8.0/PKG-INFO` & `dreamai-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai
-Version: 0.8.0
+Version: 0.9.0
 Summary: A bunch of cool and convenient utility functions.
 Home-page: https://github.com/HamzaFarhan/dreamai
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai-0.8.0/dreamai/_modidx.py` & `dreamai-0.9.0/dreamai/_modidx.py`

 * *Files identical despite different names*

### Comparing `dreamai-0.8.0/dreamai/core.py` & `dreamai-0.9.0/dreamai/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,31 +156,33 @@
                 raise Exception(f'Path {dp} does not exist.')
             if dp.is_dir():
                 paths.append(dp.iterdir())
             else:
                 paths.append([dp])
     return chain(*paths)
     
-def yml_to_pip(yml, remove_eq=True):
+def yml_to_pip(yml, less_eq=True, remove_eq=False):
     "Get pip packages from a conda environment `yml` file."
     env = load_yaml(yml)
     env_pip = env['dependencies'][-1]['pip']
     pip_list = []
     for x in env_pip:
         if 'nvidia' not in x:
             if remove_eq:
                 x = x.split('==')[0].split('>=')[0]
+            elif less_eq and 'torch' not in x:
+                x = x.replace('==', '<=')
             pip_list.append(x)
     # if remove_eq:
         # env_pip = [x.split('==')[0].split('>=')[0] for x in env_pip]
     return " ".join(pip_list)
 
-def set_pip_req(yml, settings, remove_eq=True):
+def set_pip_req(yml, settings, less_eq=True, remove_eq=False):
     "Update the pip_requirements in settings.ini from a conda environment `yml` file."
-    env_pip = yml_to_pip(yml, remove_eq=remove_eq)
+    env_pip = yml_to_pip(yml, less_eq=less_eq, remove_eq=remove_eq)
     config = ConfigParser(delimiters=['='], allow_no_value=True)
     config.read(settings)
     cfg = config['DEFAULT']
     config.set('DEFAULT', 'pip_requirements', env_pip)
     with open(settings, 'w') as configfile:
         config.write(configfile)
```

### Comparing `dreamai-0.8.0/dreamai/imports.py` & `dreamai-0.9.0/dreamai/imports.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,12 +20,12 @@
 import matplotlib.pyplot as plt
 from collections import OrderedDict
 from itertools import chain, groupby
 from functools import reduce, partial
 from configparser import ConfigParser
 from imutils import resize as resize_img
 from PIL import Image, ImageDraw, ImageFont
-from typing import Iterable,Generator,Sequence,Iterator,List,Set,Dict,Union,Optional,Tuple
+from typing import Iterable, Generator, Sequence, Iterator, List, Set, Dict, Union, Optional, Tuple
 
 from fastcore.foundation import is_bool, L
 from fastcore.basics import merge as merge_dicts
 from fastcore.basics import chunked, store_attr, camel2snake, snake2camel, flatten
```

### Comparing `dreamai-0.8.0/dreamai/vision.py` & `dreamai-0.9.0/dreamai/vision.py`

 * *Files identical despite different names*

### Comparing `dreamai-0.8.0/dreamai.egg-info/PKG-INFO` & `dreamai-0.9.0/dreamai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai
-Version: 0.8.0
+Version: 0.9.0
 Summary: A bunch of cool and convenient utility functions.
 Home-page: https://github.com/HamzaFarhan/dreamai
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai-0.8.0/setup.py` & `dreamai-0.9.0/setup.py`

 * *Files identical despite different names*

