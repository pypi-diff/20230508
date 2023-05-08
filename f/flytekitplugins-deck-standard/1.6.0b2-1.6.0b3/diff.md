# Comparing `tmp/flytekitplugins-deck-standard-1.6.0b2.tar.gz` & `tmp/flytekitplugins-deck-standard-1.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-deck-standard-1.6.0b2.tar", last modified: Fri May  5 17:49:42 2023, max compression
+gzip compressed data, was "flytekitplugins-deck-standard-1.6.0b3.tar", last modified: Mon May  8 20:18:40 2023, max compression
```

## Comparing `flytekitplugins-deck-standard-1.6.0b2.tar` & `flytekitplugins-deck-standard-1.6.0b3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:42.966118 flytekitplugins-deck-standard-1.6.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-05 17:49:42.962118 flytekitplugins-deck-standard-1.6.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-05 17:49:25.000000 flytekitplugins-deck-standard-1.6.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:42.962118 flytekitplugins-deck-standard-1.6.0b2/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:42.962118 flytekitplugins-deck-standard-1.6.0b2/flytekitplugins/deck/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-05 17:49:25.000000 flytekitplugins-deck-standard-1.6.0b2/flytekitplugins/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-05-05 17:49:25.000000 flytekitplugins-deck-standard-1.6.0b2/flytekitplugins/deck/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:42.962118 flytekitplugins-deck-standard-1.6.0b2/flytekitplugins_deck_standard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-05 17:49:42.000000 flytekitplugins-deck-standard-1.6.0b2/flytekitplugins_deck_standard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-05 17:49:42.000000 flytekitplugins-deck-standard-1.6.0b2/flytekitplugins_deck_standard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:49:42.000000 flytekitplugins-deck-standard-1.6.0b2/flytekitplugins_deck_standard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 17:49:42.000000 flytekitplugins-deck-standard-1.6.0b2/flytekitplugins_deck_standard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:42.000000 flytekitplugins-deck-standard-1.6.0b2/flytekitplugins_deck_standard.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-05 17:49:42.000000 flytekitplugins-deck-standard-1.6.0b2/flytekitplugins_deck_standard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:42.000000 flytekitplugins-deck-standard-1.6.0b2/flytekitplugins_deck_standard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:49:42.966118 flytekitplugins-deck-standard-1.6.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-05 17:49:40.000000 flytekitplugins-deck-standard-1.6.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:40.172877 flytekitplugins-deck-standard-1.6.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-08 20:18:40.168877 flytekitplugins-deck-standard-1.6.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 20:18:20.000000 flytekitplugins-deck-standard-1.6.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:40.168877 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:40.168877 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins/deck/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-08 20:18:20.000000 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-08 20:18:20.000000 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins/deck/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:40.168877 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins_deck_standard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-08 20:18:40.000000 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins_deck_standard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-08 20:18:40.000000 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins_deck_standard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:18:40.000000 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins_deck_standard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-08 20:18:40.000000 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins_deck_standard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:40.000000 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins_deck_standard.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-08 20:18:40.000000 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins_deck_standard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:40.000000 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins_deck_standard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:18:40.172877 flytekitplugins-deck-standard-1.6.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-08 20:18:37.000000 flytekitplugins-deck-standard-1.6.0b3/setup.py
```

### Comparing `flytekitplugins-deck-standard-1.6.0b2/PKG-INFO` & `flytekitplugins-deck-standard-1.6.0b3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-deck-standard
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: This Plugin provides more renderers to improve task visibility
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-data-fsspec
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-deck-standard-1.6.0b2/flytekitplugins/deck/renderer.py` & `flytekitplugins-deck-standard-1.6.0b3/flytekitplugins/deck/renderer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-import base64
-from io import BytesIO
-from typing import List, Optional, Union
-
-import markdown
-import pandas as pd
-import plotly.express as px
-from PIL import Image
-from ydata_profiling import ProfileReport
+from typing import TYPE_CHECKING, List, Optional, Union
 
+from flytekit import lazy_module
 from flytekit.types.file import FlyteFile
 
+if TYPE_CHECKING:
+    import markdown
+    import pandas as pd
+    import PIL
+    import plotly.express as px
+else:
+    pd = lazy_module("pandas")
+    markdown = lazy_module("markdown")
+    px = lazy_module("plotly.express")
+    PIL = lazy_module("PIL")
+
 
 class FrameProfilingRenderer:
     """
     Generate a ProfileReport based on a pandas DataFrame
     """
 
     def __init__(self, title: str = "Pandas Profiling Report"):
         self._title = title
 
-    def to_html(self, df: pd.DataFrame) -> str:
+    def to_html(self, df: "pd.DataFrame") -> str:
         assert isinstance(df, pd.DataFrame)
-        profile = ProfileReport(df, title=self._title)
+        import ydata_profiling
+
+        profile = ydata_profiling.ProfileReport(df, title=self._title)
         return profile.to_html()
 
 
 class MarkdownRenderer:
     """Convert a markdown string to HTML and return HTML as a unicode string.
 
     This is a shortcut function for `Markdown` class to cover the most
@@ -40,48 +46,51 @@
 class BoxRenderer:
     """
     In a box plot, rows of `data_frame` are grouped together into a
     box-and-whisker mark to visualize their distribution.
 
     Each box spans from quartile 1 (Q1) to quartile 3 (Q3). The second
     quartile (Q2) is marked by a line inside the box. By default, the
-    whiskers correspond to the box' edges +/- 1.5 times the interquartile
+    whiskers correspond to the box edges +/- 1.5 times the interquartile
     range (IQR: Q3-Q1), see "points" for other options.
     """
 
     # More detail, see https://plotly.com/python/box-plots/
     def __init__(self, column_name):
         self._column_name = column_name
 
-    def to_html(self, df: pd.DataFrame) -> str:
+    def to_html(self, df: "pd.DataFrame") -> str:
         fig = px.box(df, y=self._column_name)
         return fig.to_html()
 
 
 class ImageRenderer:
     """Converts a FlyteFile or PIL.Image.Image object to an HTML string with the image data
     represented as a base64-encoded string.
     """
 
-    def to_html(cls, image_src: Union[FlyteFile, Image.Image]) -> str:
-        img = cls._get_image_object(image_src)
-        return cls._image_to_html_string(img)
+    def to_html(self, image_src: Union[FlyteFile, "PIL.Image.Image"]) -> str:
+        img = self._get_image_object(image_src)
+        return self._image_to_html_string(img)
 
     @staticmethod
-    def _get_image_object(image_src: Union[FlyteFile, Image.Image]) -> Image.Image:
+    def _get_image_object(image_src: Union[FlyteFile, "PIL.Image.Image"]) -> "PIL.Image.Image":
         if isinstance(image_src, FlyteFile):
             local_path = image_src.download()
-            return Image.open(local_path)
-        elif isinstance(image_src, Image.Image):
+            return PIL.Image.open(local_path)
+        elif isinstance(image_src, PIL.Image.Image):
             return image_src
         else:
             raise ValueError("Unsupported image source type")
 
     @staticmethod
-    def _image_to_html_string(img: Image.Image) -> str:
+    def _image_to_html_string(img: "PIL.Image.Image") -> str:
+        import base64
+        from io import BytesIO
+
         buffered = BytesIO()
         img.save(buffered, format="PNG")
         img_base64 = base64.b64encode(buffered.getvalue()).decode()
         return f'<img src="data:image/png;base64,{img_base64}" alt="Rendered Image" />'
 
 
 class TableRenderer:
```

### Comparing `flytekitplugins-deck-standard-1.6.0b2/flytekitplugins_deck_standard.egg-info/PKG-INFO` & `flytekitplugins-deck-standard-1.6.0b3/flytekitplugins_deck_standard.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-deck-standard
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: This Plugin provides more renderers to improve task visibility
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-data-fsspec
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-deck-standard-1.6.0b2/setup.py` & `flytekitplugins-deck-standard-1.6.0b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "deck"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}-standard"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "markdown", "plotly", "ydata-profiling", "ipywidgets"]
 
-__version__ = "1.6.0b2"
+__version__ = "1.6.0b3"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This Plugin provides more renderers to improve task visibility",
```

