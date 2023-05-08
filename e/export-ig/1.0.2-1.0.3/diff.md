# Comparing `tmp/export_ig-1.0.2.tar.gz` & `tmp/export_ig-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "export_ig-1.0.2.tar", last modified: Mon May  8 05:34:56 2023, max compression
+gzip compressed data, was "export_ig-1.0.3.tar", last modified: Mon May  8 18:43:46 2023, max compression
```

## Comparing `export_ig-1.0.2.tar` & `export_ig-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 synch      (501) staff       (20)        0 2023-05-08 05:34:56.508825 export_ig-1.0.2/
--rw-r--r--   0 synch      (501) staff       (20)    11357 2023-05-08 05:17:43.000000 export_ig-1.0.2/LICENSE
--rw-r--r--   0 synch      (501) staff       (20)     1701 2023-05-08 05:34:56.508672 export_ig-1.0.2/PKG-INFO
--rw-r--r--   0 synch      (501) staff       (20)     1331 2023-05-08 05:22:50.000000 export_ig-1.0.2/README.md
-drwxr-xr-x   0 synch      (501) staff       (20)        0 2023-05-08 05:34:56.507211 export_ig-1.0.2/export_ig/
--rw-r--r--   0 synch      (501) staff       (20)        0 2023-05-08 05:08:54.000000 export_ig-1.0.2/export_ig/__init__.py
--rw-r--r--   0 synch      (501) staff       (20)      556 2023-05-08 05:27:19.000000 export_ig-1.0.2/export_ig/color_utils.py
--rw-r--r--   0 synch      (501) staff       (20)     4416 2023-05-08 05:12:10.000000 export_ig-1.0.2/export_ig/export_ig.py
-drwxr-xr-x   0 synch      (501) staff       (20)        0 2023-05-08 05:34:56.508488 export_ig-1.0.2/export_ig.egg-info/
--rw-r--r--   0 synch      (501) staff       (20)     1701 2023-05-08 05:34:56.000000 export_ig-1.0.2/export_ig.egg-info/PKG-INFO
--rw-r--r--   0 synch      (501) staff       (20)      328 2023-05-08 05:34:56.000000 export_ig-1.0.2/export_ig.egg-info/SOURCES.txt
--rw-r--r--   0 synch      (501) staff       (20)        1 2023-05-08 05:34:56.000000 export_ig-1.0.2/export_ig.egg-info/dependency_links.txt
--rw-r--r--   0 synch      (501) staff       (20)       54 2023-05-08 05:34:56.000000 export_ig-1.0.2/export_ig.egg-info/entry_points.txt
--rw-r--r--   0 synch      (501) staff       (20)        1 2023-05-08 05:13:33.000000 export_ig-1.0.2/export_ig.egg-info/not-zip-safe
--rw-r--r--   0 synch      (501) staff       (20)       19 2023-05-08 05:34:56.000000 export_ig-1.0.2/export_ig.egg-info/requires.txt
--rw-r--r--   0 synch      (501) staff       (20)       10 2023-05-08 05:34:56.000000 export_ig-1.0.2/export_ig.egg-info/top_level.txt
--rw-r--r--   0 synch      (501) staff       (20)       38 2023-05-08 05:34:56.508869 export_ig-1.0.2/setup.cfg
--rw-r--r--   0 synch      (501) staff       (20)      867 2023-05-08 05:33:34.000000 export_ig-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:43:46.444607 export_ig-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 18:43:37.000000 export_ig-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-08 18:43:46.444607 export_ig-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-08 18:43:37.000000 export_ig-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:43:46.440607 export_ig-1.0.3/export_ig/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:43:37.000000 export_ig-1.0.3/export_ig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-08 18:43:37.000000 export_ig-1.0.3/export_ig/color_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-08 18:43:37.000000 export_ig-1.0.3/export_ig/export_ig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-05-08 18:43:37.000000 export_ig-1.0.3/export_ig/shadow_pad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:43:46.444607 export_ig-1.0.3/export_ig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-08 18:43:46.000000 export_ig-1.0.3/export_ig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-08 18:43:46.000000 export_ig-1.0.3/export_ig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:43:46.000000 export_ig-1.0.3/export_ig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 18:43:46.000000 export_ig-1.0.3/export_ig.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:43:46.000000 export_ig-1.0.3/export_ig.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-08 18:43:46.000000 export_ig-1.0.3/export_ig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 18:43:46.000000 export_ig-1.0.3/export_ig.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 18:43:46.444607 export_ig-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-08 18:43:37.000000 export_ig-1.0.3/setup.py
```

### Comparing `export_ig-1.0.2/LICENSE` & `export_ig-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `export_ig-1.0.2/PKG-INFO` & `export_ig-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: export_ig
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package for processing images for Instagram upload.
 Home-page: https://github.com/syncdoth/export_ig
 Author: Sehyun Choi
 Author-email: choisehyun98@gmail.com
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `export_ig-1.0.2/README.md` & `export_ig-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `export_ig-1.0.2/export_ig/color_utils.py` & `export_ig-1.0.3/export_ig/color_utils.py`

 * *Files identical despite different names*

### Comparing `export_ig-1.0.2/export_ig/export_ig.py` & `export_ig-1.0.3/export_ig/shadow_pad.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,80 @@
-import glob
-import os
+from dataclasses import dataclass, field
 
-import fire
-from joblib import Parallel, delayed
 from PIL import Image, ImageFilter
 
 from .color_utils import parse_hex_color
 
 
+@dataclass
+class ShadowPadOptions:
+    aspect_ratio: str = field(
+        default="4x5", metadata={"help": "Aspect ratio of the output image. Separated by `x`"})
+    shadow_offset: int | float = field(
+        default=33,
+        metadata={
+            "help": "Offset of the shadow (in pixels))."
+                    "if float, it is a ratio of the longer side of the image instead."
+        })
+    pad: int | float = field(
+        default=100,
+        metadata={
+            "help": "Padding around the image (in pixels)."
+                    "if float, it is a ratio of the longer side of the image instead."
+        })
+    radius: int = field(default=15, metadata={"help": "Radius of the shadow blur"})
+    bg_color: str = field(default="white",
+                          metadata={"help": "Background color of the output image"})
+    shadow_color: str = field(default="gray", metadata={"help": "Shadow color"})
+
+    def __post_init__(self):
+        self.aspect_ratio = tuple(
+            int(x) for x in self.aspect_ratio.replace(" ", "").lower().split("x"))
+
+
+def shadow_pad(args: ShadowPadOptions):
+
+    def _process(image):
+        shadowed = make_shadow(image, (args.shadow_offset, args.shadow_offset),
+                               args.shadow_offset,
+                               args.bg_color,
+                               args.shadow_color,
+                               radius=args.radius)
+        padded = add_padding(image,
+                             args.pad,
+                             image_to_paste=shadowed,
+                             aspect_ratio=args.aspect_ratio,
+                             bg_color=args.bg_color)
+        return padded
+
+    return _process
+
+
 def make_shadow(image: Image,
-                offset: tuple[int],
-                border: int,
+                offset: tuple[int | float],
+                border: int | float,
                 bg_color: str,
                 shadow_color: str,
                 radius: int = 10):
     """
     image: base image to give a drop shadow
     iterations: number of times to apply the blur filter to the shadow
     offset: offset of the shadow as [x,y]
     bg_color: colour of the background
     shadow_color: colour of the drop shadow
     """
 
     #Calculate the size of the shadow's image
-    full_width = image.size[0] + abs(offset[0]) + border
-    full_height = image.size[1] + abs(offset[1]) + border
+    width, height = image.size
+    if isinstance(offset[0], float):
+        offset = (int(offset[0] * width), int(offset[1] * height))
+    if isinstance(border, float):
+        border = int(border * max(width, height))
+    full_width = width + abs(offset[0]) + border
+    full_height = height + abs(offset[1]) + border
 
     # parse colors
     bg_color = parse_hex_color(bg_color)
     shadow_color = parse_hex_color(shadow_color)
 
     #Create the shadow's image. Match the parent image's mode.
     shadow = Image.new(image.mode, (full_width, full_height), bg_color)
@@ -54,80 +100,36 @@
                 pad: int,
                 image_to_paste: Image = None,
                 aspect_ratio: tuple[int] = (4, 5),
                 bg_color: str = "white"):
     width, height = image.size
     if width > height:
         # landscape
+        if isinstance(pad, float):
+            pad = int(pad * width)
         new_width = width + 2 * pad
         new_height = int(new_width / aspect_ratio[1] * aspect_ratio[0])
         image_pos = (pad, int((new_height - height) / 2))
     elif width < height:
         # portrait
+        if isinstance(pad, float):
+            pad = int(pad * height)
         new_height = height + 2 * pad
         new_width = int(new_height / aspect_ratio[1] * aspect_ratio[0])
         image_pos = (int((new_width - width) / 2), pad)
     else:
         #square
+        if isinstance(pad, float):
+            pad = int(pad * height)
         new_width = width + 2 * pad
         new_height = height + 2 * pad
 
     color = parse_hex_color(bg_color)
 
     canvas = Image.new(image.mode, (new_width, new_height), color)
 
     if image_to_paste is not None:
         canvas.paste(image_to_paste, image_pos)
     else:
         canvas.paste(image, image_pos)
 
     return canvas
-
-
-def main(input_path: str,
-         output_folder: str,
-         subfoloder: bool = True,
-         aspect_ratio: str = "4x5",
-         shadow_offset: int = 33,
-         pad: int = 100,
-         radius: int = 15,
-         bg_color: str = "white",
-         shadow_color: str = "gray",
-         n_jobs: int = 10):
-    if os.path.isdir(input_path):
-        input_path = os.path.join(input_path, "*")
-
-    files = [f for f in glob.glob(input_path) if not os.path.isdir(f)]
-    if len(files) == 0:
-        raise ValueError("No files found")
-
-    aspect_ratio = tuple(int(x) for x in aspect_ratio.replace(" ", "").lower().split("x"))
-    if subfoloder:
-        output_folder = os.path.join(os.path.dirname(input_path), output_folder)
-    os.makedirs(output_folder, exist_ok=True)
-
-    def _process_image(input_file_path):
-        image = Image.open(input_file_path)
-        shadowed = make_shadow(image, (shadow_offset, shadow_offset),
-                               shadow_offset,
-                               bg_color,
-                               shadow_color,
-                               radius=radius)
-        padded = add_padding(image,
-                             pad,
-                             image_to_paste=shadowed,
-                             aspect_ratio=aspect_ratio,
-                             bg_color=bg_color)
-        basename = os.path.basename(input_file_path)
-        fname, ext = os.path.splitext(basename)
-        out_fname = os.path.join(output_folder, fname + "-padded" + ext)
-        padded.save(out_fname)
-
-    Parallel(n_jobs=n_jobs)(delayed(_process_image)(fname) for fname in files)
-
-
-def run():
-    fire.Fire(main)
-
-
-if __name__ == '__main__':
-    run()
```

### Comparing `export_ig-1.0.2/export_ig.egg-info/PKG-INFO` & `export_ig-1.0.3/export_ig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: export-ig
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package for processing images for Instagram upload.
 Home-page: https://github.com/syncdoth/export_ig
 Author: Sehyun Choi
 Author-email: choisehyun98@gmail.com
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `export_ig-1.0.2/setup.py` & `export_ig-1.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="export_ig",
-    version="1.0.2",
+    version="1.0.3",
     description="Package for processing images for Instagram upload.",
     # pylint: disable-next=consider-using-with
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
@@ -16,15 +16,15 @@
     license="Apache",
     packages=find_packages(exclude=[
         ".github",
         "imgs",
     ]),
     install_requires=[
         "Pillow",
-        "joblib",
-        "fire",
+        "joblib>=1.2.0",
+        "simple-parsing",
     ],
-    entry_points={"console_scripts": ["export_ig=export_ig.export_ig:run"]},
+    entry_points={"console_scripts": ["export_ig=export_ig.export_ig:main"]},
     include_package_data=True,
     python_requires=">=3.8",
     zip_safe=False,
 )
```

