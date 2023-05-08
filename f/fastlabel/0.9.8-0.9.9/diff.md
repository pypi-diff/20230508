# Comparing `tmp/fastlabel-0.9.8.tar.gz` & `tmp/fastlabel-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fastlabel-0.9.8.tar", last modified: Fri Jul 30 08:29:12 2021, max compression
+gzip compressed data, was "dist/fastlabel-0.9.9.tar", last modified: Fri Jul 30 11:21:35 2021, max compression
```

## Comparing `fastlabel-0.9.8.tar` & `fastlabel-0.9.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-30 08:29:12.000000 fastlabel-0.9.8/
--rw-r--r--   0 root         (0) root         (0)     1069 2021-02-21 06:32:54.000000 fastlabel-0.9.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       42 2021-02-21 06:32:54.000000 fastlabel-0.9.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    19029 2021-07-30 08:29:12.000000 fastlabel-0.9.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18698 2021-07-30 01:49:42.000000 fastlabel-0.9.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-30 08:29:12.000000 fastlabel-0.9.8/fastlabel/
--rw-r--r--   0 root         (0) root         (0)    36411 2021-07-30 08:27:44.000000 fastlabel-0.9.8/fastlabel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4304 2021-07-30 08:28:08.000000 fastlabel-0.9.8/fastlabel/api.py
--rw-r--r--   0 root         (0) root         (0)     1067 2021-07-30 01:49:42.000000 fastlabel-0.9.8/fastlabel/const.py
--rw-r--r--   0 root         (0) root         (0)    12147 2021-07-30 08:27:44.000000 fastlabel-0.9.8/fastlabel/converters.py
--rw-r--r--   0 root         (0) root         (0)      301 2021-05-25 08:46:48.000000 fastlabel-0.9.8/fastlabel/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      548 2021-05-26 08:00:30.000000 fastlabel-0.9.8/fastlabel/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-30 08:29:12.000000 fastlabel-0.9.8/fastlabel.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19029 2021-07-30 08:29:12.000000 fastlabel-0.9.8/fastlabel.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      344 2021-07-30 08:29:12.000000 fastlabel-0.9.8/fastlabel.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-30 08:29:12.000000 fastlabel-0.9.8/fastlabel.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       78 2021-07-30 08:29:12.000000 fastlabel-0.9.8/fastlabel.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2021-07-30 08:29:12.000000 fastlabel-0.9.8/fastlabel.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       77 2021-07-30 01:49:42.000000 fastlabel-0.9.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-07-30 08:29:12.000000 fastlabel-0.9.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      654 2021-07-30 08:27:44.000000 fastlabel-0.9.8/setup.py
+drwxr-xr-x   0 eisuke     (501) staff       (20)        0 2021-07-30 11:21:35.000000 fastlabel-0.9.9/
+-rw-r--r--   0 eisuke     (501) staff       (20)     1069 2020-12-29 13:24:43.000000 fastlabel-0.9.9/LICENSE
+-rw-r--r--   0 eisuke     (501) staff       (20)       42 2020-12-29 13:24:43.000000 fastlabel-0.9.9/MANIFEST.in
+-rw-r--r--   0 eisuke     (501) staff       (20)    26242 2021-07-30 11:21:35.000000 fastlabel-0.9.9/PKG-INFO
+-rw-r--r--   0 eisuke     (501) staff       (20)    18698 2021-07-27 00:24:51.000000 fastlabel-0.9.9/README.md
+drwxr-xr-x   0 eisuke     (501) staff       (20)        0 2021-07-30 11:21:35.000000 fastlabel-0.9.9/fastlabel/
+-rw-r--r--   0 eisuke     (501) staff       (20)    36738 2021-07-30 11:19:49.000000 fastlabel-0.9.9/fastlabel/__init__.py
+-rw-r--r--   0 eisuke     (501) staff       (20)     4101 2021-07-30 10:49:41.000000 fastlabel-0.9.9/fastlabel/api.py
+-rw-r--r--   0 eisuke     (501) staff       (20)     1067 2021-07-27 00:24:51.000000 fastlabel-0.9.9/fastlabel/const.py
+-rw-r--r--   0 eisuke     (501) staff       (20)    14117 2021-07-30 11:19:58.000000 fastlabel-0.9.9/fastlabel/converters.py
+-rw-r--r--   0 eisuke     (501) staff       (20)      301 2021-05-28 11:11:36.000000 fastlabel-0.9.9/fastlabel/exceptions.py
+-rw-r--r--   0 eisuke     (501) staff       (20)      548 2021-07-23 03:22:17.000000 fastlabel-0.9.9/fastlabel/utils.py
+drwxr-xr-x   0 eisuke     (501) staff       (20)        0 2021-07-30 11:21:35.000000 fastlabel-0.9.9/fastlabel.egg-info/
+-rw-r--r--   0 eisuke     (501) staff       (20)    26242 2021-07-30 11:21:35.000000 fastlabel-0.9.9/fastlabel.egg-info/PKG-INFO
+-rw-r--r--   0 eisuke     (501) staff       (20)      344 2021-07-30 11:21:35.000000 fastlabel-0.9.9/fastlabel.egg-info/SOURCES.txt
+-rw-r--r--   0 eisuke     (501) staff       (20)        1 2021-07-30 11:21:35.000000 fastlabel-0.9.9/fastlabel.egg-info/dependency_links.txt
+-rw-r--r--   0 eisuke     (501) staff       (20)      102 2021-07-30 11:21:35.000000 fastlabel-0.9.9/fastlabel.egg-info/requires.txt
+-rw-r--r--   0 eisuke     (501) staff       (20)       10 2021-07-30 11:21:35.000000 fastlabel-0.9.9/fastlabel.egg-info/top_level.txt
+-rw-r--r--   0 eisuke     (501) staff       (20)      101 2021-07-30 11:04:41.000000 fastlabel-0.9.9/requirements.txt
+-rw-r--r--   0 eisuke     (501) staff       (20)       38 2021-07-30 11:21:35.000000 fastlabel-0.9.9/setup.cfg
+-rw-r--r--   0 eisuke     (501) staff       (20)      654 2021-07-30 11:10:09.000000 fastlabel-0.9.9/setup.py
```

### Comparing `fastlabel-0.9.8/LICENSE` & `fastlabel-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastlabel-0.9.8/PKG-INFO` & `fastlabel-0.9.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: fastlabel
-Version: 0.9.8
-Summary: The official Python SDK for FastLabel API, the Data Platform for AI
-Home-page: UNKNOWN
-Author: eisuke-ueta
-Author-email: eisuke.ueta@fastlabel.ai
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # FastLabel Python SDK
 
 _If you are using FastLabel prototype, please install version 0.2.2._
 
 ## Table of Contents
 
 - [Installation](#installation)
@@ -910,9 +897,7 @@
 ```
 
 > Please check const.COLOR_PALLETE for index colors.
 
 ## API Docs
 
 Check [this](https://api.fastlabel.ai/docs/) for further information.
-
-
```

### Comparing `fastlabel-0.9.8/fastlabel/__init__.py` & `fastlabel-0.9.9/fastlabel/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import glob
 import json
 from typing import List
 from logging import getLogger
-from PIL import Image, ImageDraw
+from PIL import Image
+import cv2
+import numpy as np
 
 import xmltodict
 
 from .exceptions import FastLabelInvalidException
 from .api import Api
 from fastlabel import converters, utils, const
 from fastlabel.const import AnnotationType
@@ -649,43 +651,45 @@
 
         tasks = converters.to_pixel_coordinates(tasks)
         for task in tasks:
             self.__export_index_color_image(task=task, output_dir=output_dir, pallete=pallete, is_instance_segmentation=False, classes=classes)
 
     def __export_index_color_image(self, task: list, output_dir: str, pallete: List[int], is_instance_segmentation: bool = True, classes: list = []) -> None:
         image = Image.new("RGB", (task["width"], task["height"]), 0)
-        image = image.convert('P')
-        image.putpalette(pallete)
-        draw = ImageDraw.Draw(image)
+        image = np.array(image)
+        image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
 
         index = 1
         for annotation in task["annotations"]:
             color = index if is_instance_segmentation else classes.index(annotation["value"]) + 1
             if annotation["type"] == AnnotationType.segmentation.value:
                 for region in annotation["points"]:
                     for points in region:
-                        pillow_draw_points = self.__get_pillow_draw_points(points)
-                        draw.polygon(pillow_draw_points, fill=color)
+                        cv_draw_points = self.__get_cv_draw_points(points)
+                        cv2.fillPoly(image, [cv_draw_points], color, lineType=cv2.LINE_8, shift=0)
                         # hollowd points are not supported
                         break
             elif annotation["type"] == AnnotationType.polygon.value:
-                pillow_draw_points = self.__get_pillow_draw_points(annotation["points"])
-                draw.polygon(pillow_draw_points, fill=color)
+                cv_draw_points = self.__get_cv_draw_points(annotation["points"])
+                cv2.fillPoly(image, [cv_draw_points], color, lineType=cv2.LINE_8, shift=0)
             elif annotation["type"] == AnnotationType.bbox.value:
-                pillow_draw_points = self.__get_pillow_draw_points(annotation["points"])
-                draw.polygon(pillow_draw_points, fill=color)
+                cv_draw_points = self.__get_cv_draw_points(annotation["points"])
+                cv2.fillPoly(image, [cv_draw_points], color, lineType=cv2.LINE_8, shift=0)
             else:
                 continue
             index += 1
 
         image_path = os.path.join(output_dir, utils.get_basename(task["name"]) + ".png")
         os.makedirs(os.path.dirname(image_path), exist_ok=True)
+        image = Image.fromarray(image)
+        image = image.convert('P')
+        image.putpalette(pallete)
         image.save(image_path)
 
-    def __get_pillow_draw_points(self, points: List[int]) -> List[int]:
+    def __get_cv_draw_points(self, points: List[int]) -> List[int]:
         """
         Convert points to pillow draw points. Diagonal points are not supported.
         """
         x_points = []
         x_points.append(points[0])
         x_points.append(points[1])
         for i in range(int(len(points) / 2)):
@@ -713,15 +717,19 @@
             y_points.append(x)
             y_points.append(y)
 
         new_points = []
         for i in range(int(len(points) / 2)):
             new_points.append(x_points[i * 2])
             new_points.append(y_points[i * 2 + 1])
-        return new_points
+
+        cv_points = []
+        for i in range(int(len(new_points) / 2)):
+            cv_points.append((new_points[i * 2], new_points[i * 2 + 1]))
+        return np.array(cv_points)
 
 
     # Annotation
 
     def find_annotation(self, annotation_id: str) -> dict:
         """
         Find an annotation.
```

### Comparing `fastlabel-0.9.8/fastlabel/api.py` & `fastlabel-0.9.9/fastlabel/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import os
 import requests
 
 from .exceptions import FastLabelException, FastLabelInvalidException
 
-# FASTLABEL_ENDPOINT = "https://api.fastlabel.ai/v1/"
-
-FASTLABEL_ENDPOINT = "http://api:4000/v1/" # remote container
-FASTLABEL_ENDPOINT = "http://localhost:4000/v1/" # local
-# export FASTLABEL_ACCESS_TOKEN=NTI3MmI4NTUtNWE1NC00ZWFiLWE4MDUtZDE5ZmQ0MjMzMjRi
+FASTLABEL_ENDPOINT = "https://api.fastlabel.ai/v1/"
 
 
 class Api:
 
     access_token = None
 
     def __init__(self):
```

### Comparing `fastlabel-0.9.8/fastlabel/const.py` & `fastlabel-0.9.9/fastlabel/const.py`

 * *Files identical despite different names*

### Comparing `fastlabel-0.9.8/fastlabel/converters.py` & `fastlabel-0.9.9/fastlabel/converters.py`

 * *Files 8% similar despite different names*

```diff
@@ -297,22 +297,73 @@
                     xmin, ymin,
                     xmax, ymin,
                     xmax, ymax,
                     xmin, ymax,
                 ]
             else:
                 continue
+
+    # Remove duplicate points
+    for task in tasks:
+        for anno in task["annotations"]:
+            if annotation["type"] == AnnotationType.segmentation.value:
+                new_regions = []
+                for region in anno["points"]:
+                    new_region = []
+                    for points in region:
+                        new_points = __remove_duplicated_coordinates(points)
+                        new_region.append(new_points)
+                    new_regions.append(new_region)
+                anno["points"] = new_regions
+            elif annotation["type"] == AnnotationType.polygon.value:
+                new_points = __remove_duplicated_coordinates(annotation["points"])
+                annotation["points"] = new_points
     return tasks
 
+def __remove_duplicated_coordinates(points: List[int]) -> List[int]:
+    """
+    Remove duplicated coordinates.
+    """
+    if len(points) == 0:
+        return []
+
+    new_points = []
+    for i in range(int(len(points) / 2)):
+        if i == 0:
+            new_points.append(points[i*2])
+            new_points.append(points[i*2 + 1])
+
+        if new_points[-2] == points[i*2] and new_points[-1] == points[i*2 + 1]:
+            continue
+
+        if len(new_points) <= 2:
+            new_points.append(points[i*2])
+            new_points.append(points[i*2 + 1])
+        else:
+            if new_points[-4] == new_points[-2] and new_points[-2] == points[i*2]:
+                new_points.pop()
+                new_points.pop()
+                new_points.append(points[i*2])
+                new_points.append(points[i*2 + 1])
+            elif new_points[-3] == new_points[-1] and new_points[-1] == points[i*2 + 1]:
+                new_points.pop()
+                new_points.pop()
+                new_points.append(points[i*2])
+                new_points.append(points[i*2 + 1])
+            else:
+                new_points.append(points[i*2])
+                new_points.append(points[i*2 + 1])
+    return new_points
+
 def __get_pixel_coordinates(points: List[int or float]) -> List[int]:
     """
     Remove diagonal coordinates and return pixel outline coordinates.
     """
     if len(points) == 0:
-        return
+        return []
 
     new_points = []
     new_points.append(int(points[0]))
     new_points.append(int(points[1]))
     for i in range(int(len(points) / 2)):
         if i == 0:
             continue
```

### Comparing `fastlabel-0.9.8/fastlabel/utils.py` & `fastlabel-0.9.9/fastlabel/utils.py`

 * *Files identical despite different names*

### Comparing `fastlabel-0.9.8/setup.py` & `fastlabel-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = file.read()
 
 with open("requirements.txt", encoding="utf-8") as file:
     install_requires = file.read()
 
 setuptools.setup(
     name="fastlabel",
-    version="0.9.8",
+    version="0.9.9",
     author="eisuke-ueta",
     author_email="eisuke.ueta@fastlabel.ai",
     description="The official Python SDK for FastLabel API, the Data Platform for AI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=install_requires,
```

