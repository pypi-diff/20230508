# Comparing `tmp/easy-pil-0.2.2.tar.gz` & `tmp/easy-pil-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/easy-pil/easy-pil/dist/.tmp-vsxheam9/easy-pil-0.2.2.tar", last modified: Sat May  6 20:59:58 2023, max compression
+gzip compressed data, was "/home/runner/work/easy-pil/easy-pil/dist/.tmp-ih6r3587/easy-pil-0.2.3.tar", last modified: Mon May  8 08:53:19 2023, max compression
```

## Comparing `easy-pil-0.2.2.tar` & `easy-pil-0.2.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:59:58.000000 easy-pil-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-06 20:59:47.000000 easy-pil-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-06 20:59:47.000000 easy-pil-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-06 20:59:58.000000 easy-pil-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-06 20:59:47.000000 easy-pil-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:59:58.000000 easy-pil-0.2.2/easy_pil/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-06 20:59:47.000000 easy-pil-0.2.2/easy_pil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-06 20:59:47.000000 easy-pil-0.2.2/easy_pil/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-06 20:59:47.000000 easy-pil-0.2.2/easy_pil/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-05-06 20:59:47.000000 easy-pil-0.2.2/easy_pil/editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-06 20:59:47.000000 easy-pil-0.2.2/easy_pil/font.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:59:58.000000 easy-pil-0.2.2/easy_pil/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:59:58.000000 easy-pil-0.2.2/easy_pil/fonts/caveat/
--rw-r--r--   0 runner    (1001) docker     (123)   256900 2023-05-06 20:59:47.000000 easy-pil-0.2.2/easy_pil/fonts/caveat/caveat.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:59:58.000000 easy-pil-0.2.2/easy_pil/fonts/montserrat/
--rw-r--r--   0 runner    (1001) docker     (123)   244468 2023-05-06 20:59:47.000000 easy-pil-0.2.2/easy_pil/fonts/montserrat/montserrat_bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   249088 2023-05-06 20:59:47.000000 easy-pil-0.2.2/easy_pil/fonts/montserrat/montserrat_italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   242068 2023-05-06 20:59:47.000000 easy-pil-0.2.2/easy_pil/fonts/montserrat/montserrat_light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   245708 2023-05-06 20:59:47.000000 easy-pil-0.2.2/easy_pil/fonts/montserrat/montserrat_regular.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:59:58.000000 easy-pil-0.2.2/easy_pil/fonts/poppins/
--rw-r--r--   0 runner    (1001) docker     (123)   153900 2023-05-06 20:59:47.000000 easy-pil-0.2.2/easy_pil/fonts/poppins/poppins_bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   181972 2023-05-06 20:59:47.000000 easy-pil-0.2.2/easy_pil/fonts/poppins/poppins_italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   159848 2023-05-06 20:59:47.000000 easy-pil-0.2.2/easy_pil/fonts/poppins/poppins_light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   158192 2023-05-06 20:59:47.000000 easy-pil-0.2.2/easy_pil/fonts/poppins/poppins_regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-06 20:59:47.000000 easy-pil-0.2.2/easy_pil/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:59:58.000000 easy-pil-0.2.2/easy_pil/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 20:59:47.000000 easy-pil-0.2.2/easy_pil/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-06 20:59:47.000000 easy-pil-0.2.2/easy_pil/types/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-06 20:59:47.000000 easy-pil-0.2.2/easy_pil/types/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-06 20:59:47.000000 easy-pil-0.2.2/easy_pil/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-06 20:59:47.000000 easy-pil-0.2.2/easy_pil/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:59:58.000000 easy-pil-0.2.2/easy_pil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-06 20:59:58.000000 easy-pil-0.2.2/easy_pil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-06 20:59:58.000000 easy-pil-0.2.2/easy_pil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 20:59:58.000000 easy-pil-0.2.2/easy_pil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-06 20:59:58.000000 easy-pil-0.2.2/easy_pil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 20:59:58.000000 easy-pil-0.2.2/easy_pil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-06 20:59:47.000000 easy-pil-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-06 20:59:47.000000 easy-pil-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 20:59:58.000000 easy-pil-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-06 20:59:47.000000 easy-pil-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:59:58.000000 easy-pil-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-06 20:59:47.000000 easy-pil-0.2.2/tests/test_canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-06 20:59:47.000000 easy-pil-0.2.2/tests/test_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-06 20:59:47.000000 easy-pil-0.2.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:53:19.000000 easy-pil-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-08 08:53:08.000000 easy-pil-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-08 08:53:08.000000 easy-pil-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-08 08:53:19.000000 easy-pil-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-08 08:53:08.000000 easy-pil-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18545 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/font.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil/fonts/caveat/
+-rw-r--r--   0 runner    (1001) docker     (123)   256900 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/fonts/caveat/caveat.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil/fonts/montserrat/
+-rw-r--r--   0 runner    (1001) docker     (123)   244468 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/fonts/montserrat/montserrat_bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   249088 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/fonts/montserrat/montserrat_italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   242068 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/fonts/montserrat/montserrat_light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   245708 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/fonts/montserrat/montserrat_regular.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil/fonts/poppins/
+-rw-r--r--   0 runner    (1001) docker     (123)   153900 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/fonts/poppins/poppins_bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   181972 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/fonts/poppins/poppins_italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   159848 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/fonts/poppins/poppins_light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   158192 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/fonts/poppins/poppins_regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/types/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/types/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-08 08:53:08.000000 easy-pil-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-08 08:53:08.000000 easy-pil-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:53:19.000000 easy-pil-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-08 08:53:08.000000 easy-pil-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:53:19.000000 easy-pil-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-08 08:53:08.000000 easy-pil-0.2.3/tests/test_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-08 08:53:08.000000 easy-pil-0.2.3/tests/test_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-08 08:53:08.000000 easy-pil-0.2.3/tests/test_utils.py
```

### Comparing `easy-pil-0.2.2/LICENSE` & `easy-pil-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.2/PKG-INFO` & `easy-pil-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-pil
-Version: 0.2.2
+Version: 0.2.3
 Summary: A library to make common tasks of Pillow easy.
 Home-page: https://github.com/shahriyardx/easy-pil
 Author: Md Shahriyar Alam
 Author-email: contact@shahriyar.dev
 Project-URL: Documentation, https://easy-pil.readthedocs.io/en/latest/
 Project-URL: Bug Reports, https://github.com/shahriyardx/easy-pil/issues
 Project-URL: Source, https://github.com/shahriyardx/easy-pil/
```

### Comparing `easy-pil-0.2.2/README.md` & `easy-pil-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.2/easy_pil/canvas.py` & `easy-pil-0.2.3/easy_pil/canvas.py`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.2/easy_pil/editor.py` & `easy-pil-0.2.3/easy_pil/editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from io import BytesIO
-from typing import List, Optional, Tuple, Union
+from typing import List, Tuple, Union
 
 from PIL import Image, ImageDraw, ImageFilter, ImageFont
 from typing_extensions import Literal
 
 from .canvas import Canvas
 from .font import Font
 from .text import Text
```

### Comparing `easy-pil-0.2.2/easy_pil/font.py` & `easy-pil-0.2.3/easy_pil/font.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
+from functools import lru_cache
 
-from memoization import cached
 from PIL import ImageFont
 from typing_extensions import Literal
 
 fonts_directory = os.path.join(os.path.dirname(__file__), "fonts")
+
+
 fonts_path = {
     "caveat": {
         "regular": os.path.join(fonts_directory, "caveat", "caveat.ttf"),
         "bold": os.path.join(fonts_directory, "caveat", "caveat.ttf"),
         "italic": os.path.join(fonts_directory, "caveat", "caveat.ttf"),
         "light": os.path.join(fonts_directory, "caveat", "caveat.ttf"),
     },
@@ -53,15 +55,15 @@
     def __init__(self, path: str, size: int = 10, **kwargs) -> None:
         self.font = ImageFont.truetype(path, size=size, **kwargs)
 
     def getsize(self, text: str):
         return self.font.getsize(text)
 
     @staticmethod
-    @cached()
+    @lru_cache()
     def poppins(
         variant: Literal["regular", "bold", "italic", "light"] = "regular",
         size: int = 10,
     ):
         """Poppins font
 
         Parameters
@@ -70,15 +72,15 @@
             Font variant, by default "regular"
         size : int, optional
             Font size, by default 10
         """
         return ImageFont.truetype(fonts_path["poppins"][variant], size=size)
 
     @staticmethod
-    @cached()
+    @lru_cache()
     def caveat(
         variant: Literal["regular", "bold", "italic", "light"] = "regular",
         size: int = 10,
     ):
         """Caveat font
 
         Parameters
@@ -87,15 +89,15 @@
             Font variant, by default "regular"
         size : int, optional
             Font size, by default 10
         """
         return ImageFont.truetype(fonts_path["caveat"][variant], size=size)
 
     @staticmethod
-    @cached()
+    @lru_cache()
     def montserrat(
         variant: Literal["regular", "bold", "italic", "light"] = "regular",
         size: int = 10,
     ):
         """Montserrat font
 
         Parameters
```

### Comparing `easy-pil-0.2.2/easy_pil/fonts/caveat/caveat.ttf` & `easy-pil-0.2.3/easy_pil/fonts/caveat/caveat.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.2/easy_pil/fonts/montserrat/montserrat_bold.ttf` & `easy-pil-0.2.3/easy_pil/fonts/montserrat/montserrat_bold.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.2/easy_pil/fonts/montserrat/montserrat_italic.ttf` & `easy-pil-0.2.3/easy_pil/fonts/montserrat/montserrat_italic.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.2/easy_pil/fonts/montserrat/montserrat_light.ttf` & `easy-pil-0.2.3/easy_pil/fonts/montserrat/montserrat_light.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.2/easy_pil/fonts/montserrat/montserrat_regular.ttf` & `easy-pil-0.2.3/easy_pil/fonts/montserrat/montserrat_regular.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.2/easy_pil/fonts/poppins/poppins_bold.ttf` & `easy-pil-0.2.3/easy_pil/fonts/poppins/poppins_bold.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.2/easy_pil/fonts/poppins/poppins_italic.ttf` & `easy-pil-0.2.3/easy_pil/fonts/poppins/poppins_italic.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.2/easy_pil/fonts/poppins/poppins_light.ttf` & `easy-pil-0.2.3/easy_pil/fonts/poppins/poppins_light.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.2/easy_pil/fonts/poppins/poppins_regular.ttf` & `easy-pil-0.2.3/easy_pil/fonts/poppins/poppins_regular.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.2/easy_pil/text.py` & `easy-pil-0.2.3/easy_pil/text.py`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.2/easy_pil/types/workspace.py` & `easy-pil-0.2.3/easy_pil/types/workspace.py`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.2/easy_pil/utils.py` & `easy-pil-0.2.3/easy_pil/utils.py`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.2/easy_pil/workspace.py` & `easy-pil-0.2.3/easy_pil/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import random
 import string
-from typing import Any, Callable, Dict, Tuple, Union
+from typing import Any, Callable, Dict, Optional, Tuple, Union
 
 from .editor import Canvas, Editor
 from .types.common import Color
 from .types.workspace import ComponentKwargs
 
 
 class Workspace:
     """Workspace class for working with layers and components"""
 
     def __init__(self, size: Tuple[float, float]) -> None:
         self.size = size
-        self.layers: Dict[str, Dict[str, Dict[str, dict]]] = dict()
+        self.layers: dict = dict()
         self.working_layer = None
 
     def create_layer(self, name: str, background: Color = (0, 0, 0, 0)):
         """Creates a layer
 
         Parameters
         ----------
@@ -49,32 +49,34 @@
             self.layers.pop(name)
         except KeyError:
             raise ValueError("Invalid layer name")
 
     def update_layer(
         self,
         layer_name: str,
-        new_layer_name: str = None,
-        background: Color = None,
+        new_layer_name: Optional[str] = None,
+        background: Optional[Color] = None,
     ):
         """Creates a layer
 
         Parameters
         ----------
-        name : str
+        layer_name : str
             name of the layer
+        new_layer_name: str, Optional
+            updated name of the layer, defaults to None
         background: Color
-            background color of the layer
+            background color of the layer, defaults to None
 
         Raises
         ------
         ValueError
             if the layer is not available in the workspace
         """
-        if not layer_name in self.layers:
+        if layer_name not in self.layers:
             raise ValueError("Invalid layer name")
 
         if background:
             self.layers[layer_name]["metadata"]["background"] = background
 
         if new_layer_name:
             self.layers[new_layer_name] = self.layers.pop(layer_name)
```

### Comparing `easy-pil-0.2.2/easy_pil.egg-info/PKG-INFO` & `easy-pil-0.2.3/easy_pil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-pil
-Version: 0.2.2
+Version: 0.2.3
 Summary: A library to make common tasks of Pillow easy.
 Home-page: https://github.com/shahriyardx/easy-pil
 Author: Md Shahriyar Alam
 Author-email: contact@shahriyar.dev
 Project-URL: Documentation, https://easy-pil.readthedocs.io/en/latest/
 Project-URL: Bug Reports, https://github.com/shahriyardx/easy-pil/issues
 Project-URL: Source, https://github.com/shahriyardx/easy-pil/
```

### Comparing `easy-pil-0.2.2/easy_pil.egg-info/SOURCES.txt` & `easy-pil-0.2.3/easy_pil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.2/setup.py` & `easy-pil-0.2.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,18 @@
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
-    keywords="Pillow, PIL, Pillow wrapper, PIL wrapper, Easy Pillow, Easy PIL, discord rank card, discord card",
+    keywords=(
+        "Pillow, PIL, Pillow wrapper, PIL wrapper, Easy Pillow, "
+        "Easy PIL, discord rank card, discord card"
+    ),
     packages=find_packages(),
     package_data={
         "easy_pil": ["fonts/*/*.ttf"],
     },
     python_requires=">=3.7, <4",
     install_requires=_get_requirements(),
     extras_require={
```

### Comparing `easy-pil-0.2.2/tests/test_editor.py` & `easy-pil-0.2.3/tests/test_editor.py`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.2/tests/test_utils.py` & `easy-pil-0.2.3/tests/test_utils.py`

 * *Files identical despite different names*

