# Comparing `tmp/simplt-0.0.2.tar.gz` & `tmp/simplt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplt-0.0.2.tar", last modified: Tue Jan 31 21:17:03 2023, max compression
+gzip compressed data, was "simplt-0.0.3.tar", last modified: Sun May  7 22:30:19 2023, max compression
```

## Comparing `simplt-0.0.2.tar` & `simplt-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-01-31 21:17:03.255438 simplt-0.0.2/
--rw-rw-r--   0 name      (1000) name      (1000)     9513 2023-01-31 21:17:03.255438 simplt-0.0.2/PKG-INFO
--rw-------   0 name      (1000) name      (1000)     8700 2023-01-31 21:16:07.000000 simplt-0.0.2/README.md
--rw-rw-r--   0 name      (1000) name      (1000)    34523 2023-01-19 10:51:45.000000 simplt-0.0.2/licence
--rw-rw-r--   0 name      (1000) name      (1000)     1395 2022-11-30 09:54:42.000000 simplt-0.0.2/pyproject.toml
--rw-rw-r--   0 name      (1000) name      (1000)     1341 2023-01-31 21:17:03.255438 simplt-0.0.2/setup.cfg
--rw-rw-r--   0 name      (1000) name      (1000)      198 2023-01-31 21:16:07.000000 simplt-0.0.2/setup.py
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-01-31 21:17:03.255438 simplt-0.0.2/src/
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-01-31 21:17:03.255438 simplt-0.0.2/src/simplt/
--rw-rw-r--   0 name      (1000) name      (1000)      141 2023-01-31 21:10:30.000000 simplt-0.0.2/src/simplt/__init__.py
--rw-rw-r--   0 name      (1000) name      (1000)      448 2023-01-21 15:29:34.000000 simplt-0.0.2/src/simplt/__main__.py
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-01-31 21:17:03.255438 simplt-0.0.2/src/simplt/arg_parser/
--rw-rw-r--   0 name      (1000) name      (1000)        0 2022-11-30 09:54:42.000000 simplt-0.0.2/src/simplt/arg_parser/__init__.py
--rw-rw-r--   0 name      (1000) name      (1000)     1476 2023-01-21 15:30:50.000000 simplt-0.0.2/src/simplt/arg_parser/arg_parser.py
--rw-rw-r--   0 name      (1000) name      (1000)     1390 2023-01-31 21:16:07.000000 simplt-0.0.2/src/simplt/arg_parser/process_args.py
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-01-31 21:17:03.255438 simplt-0.0.2/src/simplt/box_plot/
--rw-rw-r--   0 name      (1000) name      (1000)        0 2022-11-30 09:54:42.000000 simplt-0.0.2/src/simplt/box_plot/__init__.py
--rw-rw-r--   0 name      (1000) name      (1000)     3462 2023-01-24 14:55:42.000000 simplt-0.0.2/src/simplt/box_plot/box_plot.py
--rw-rw-r--   0 name      (1000) name      (1000)      393 2023-01-21 16:26:18.000000 simplt-0.0.2/src/simplt/export_plot.py
--rw-rw-r--   0 name      (1000) name      (1000)       74 2023-01-21 15:00:05.000000 simplt-0.0.2/src/simplt/helper.py
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-01-31 21:17:03.255438 simplt-0.0.2/src/simplt/latex_table/
--rw-rw-r--   0 name      (1000) name      (1000)        0 2022-11-30 09:54:42.000000 simplt-0.0.2/src/simplt/latex_table/__init__.py
--rw-rw-r--   0 name      (1000) name      (1000)     2428 2023-01-21 16:25:18.000000 simplt-0.0.2/src/simplt/latex_table/latex_table.py
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-01-31 21:17:03.255438 simplt-0.0.2/src/simplt/line_plot/
--rw-rw-r--   0 name      (1000) name      (1000)        0 2022-11-30 09:54:42.000000 simplt-0.0.2/src/simplt/line_plot/__init__.py
--rw-rw-r--   0 name      (1000) name      (1000)     3638 2023-01-21 18:51:28.000000 simplt-0.0.2/src/simplt/line_plot/line_plot.py
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-01-31 21:17:03.255438 simplt-0.0.2/src/simplt.egg-info/
--rw-rw-r--   0 name      (1000) name      (1000)     9513 2023-01-31 21:17:03.000000 simplt-0.0.2/src/simplt.egg-info/PKG-INFO
--rw-rw-r--   0 name      (1000) name      (1000)      662 2023-01-31 21:17:03.000000 simplt-0.0.2/src/simplt.egg-info/SOURCES.txt
--rw-rw-r--   0 name      (1000) name      (1000)        1 2023-01-31 21:17:03.000000 simplt-0.0.2/src/simplt.egg-info/dependency_links.txt
--rw-rw-r--   0 name      (1000) name      (1000)       39 2023-01-31 21:17:03.000000 simplt-0.0.2/src/simplt.egg-info/entry_points.txt
--rw-rw-r--   0 name      (1000) name      (1000)       86 2023-01-31 21:17:03.000000 simplt-0.0.2/src/simplt.egg-info/requires.txt
--rw-rw-r--   0 name      (1000) name      (1000)        7 2023-01-31 21:17:03.000000 simplt-0.0.2/src/simplt.egg-info/top_level.txt
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 22:30:19.774613 simplt-0.0.3/
+-rw-rw-r--   0 name      (1000) name      (1000)     4792 2023-05-07 22:30:19.774613 simplt-0.0.3/PKG-INFO
+-rw-rw-r--   0 name      (1000) name      (1000)     3979 2023-05-07 22:28:05.000000 simplt-0.0.3/README.md
+-rw-rw-r--   0 name      (1000) name      (1000)    34523 2023-05-07 21:29:00.000000 simplt-0.0.3/licence
+-rw-rw-r--   0 name      (1000) name      (1000)     1395 2023-05-07 21:29:00.000000 simplt-0.0.3/pyproject.toml
+-rw-rw-r--   0 name      (1000) name      (1000)     1341 2023-05-07 22:30:19.774613 simplt-0.0.3/setup.cfg
+-rw-rw-r--   0 name      (1000) name      (1000)      198 2023-05-07 21:29:00.000000 simplt-0.0.3/setup.py
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 22:30:19.770613 simplt-0.0.3/src/
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 22:30:19.774613 simplt-0.0.3/src/simplt/
+-rw-rw-r--   0 name      (1000) name      (1000)      141 2023-05-07 22:29:51.000000 simplt-0.0.3/src/simplt/__init__.py
+-rw-rw-r--   0 name      (1000) name      (1000)      448 2023-05-07 21:29:00.000000 simplt-0.0.3/src/simplt/__main__.py
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 22:30:19.774613 simplt-0.0.3/src/simplt/arg_parser/
+-rw-rw-r--   0 name      (1000) name      (1000)        0 2023-05-07 21:29:00.000000 simplt-0.0.3/src/simplt/arg_parser/__init__.py
+-rw-rw-r--   0 name      (1000) name      (1000)     1661 2023-05-07 21:58:16.000000 simplt-0.0.3/src/simplt/arg_parser/arg_parser.py
+-rw-rw-r--   0 name      (1000) name      (1000)     1706 2023-05-07 21:58:33.000000 simplt-0.0.3/src/simplt/arg_parser/process_args.py
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 22:30:19.774613 simplt-0.0.3/src/simplt/box_plot/
+-rw-rw-r--   0 name      (1000) name      (1000)        0 2023-05-07 21:29:00.000000 simplt-0.0.3/src/simplt/box_plot/__init__.py
+-rw-rw-r--   0 name      (1000) name      (1000)     3464 2023-05-07 21:34:44.000000 simplt-0.0.3/src/simplt/box_plot/box_plot.py
+-rw-rw-r--   0 name      (1000) name      (1000)      393 2023-05-07 21:29:00.000000 simplt-0.0.3/src/simplt/export_plot.py
+-rw-rw-r--   0 name      (1000) name      (1000)       74 2023-05-07 21:29:00.000000 simplt-0.0.3/src/simplt/helper.py
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 22:30:19.774613 simplt-0.0.3/src/simplt/latex_table/
+-rw-rw-r--   0 name      (1000) name      (1000)        0 2023-05-07 21:29:00.000000 simplt-0.0.3/src/simplt/latex_table/__init__.py
+-rw-rw-r--   0 name      (1000) name      (1000)     2428 2023-05-07 21:29:00.000000 simplt-0.0.3/src/simplt/latex_table/latex_table.py
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 22:30:19.774613 simplt-0.0.3/src/simplt/line_plot/
+-rw-rw-r--   0 name      (1000) name      (1000)        0 2023-05-07 21:29:00.000000 simplt-0.0.3/src/simplt/line_plot/__init__.py
+-rw-rw-r--   0 name      (1000) name      (1000)     3706 2023-05-07 21:45:02.000000 simplt-0.0.3/src/simplt/line_plot/line_plot.py
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 22:30:19.774613 simplt-0.0.3/src/simplt.egg-info/
+-rw-rw-r--   0 name      (1000) name      (1000)     4792 2023-05-07 22:30:19.000000 simplt-0.0.3/src/simplt.egg-info/PKG-INFO
+-rw-rw-r--   0 name      (1000) name      (1000)      662 2023-05-07 22:30:19.000000 simplt-0.0.3/src/simplt.egg-info/SOURCES.txt
+-rw-rw-r--   0 name      (1000) name      (1000)        1 2023-05-07 22:30:19.000000 simplt-0.0.3/src/simplt.egg-info/dependency_links.txt
+-rw-rw-r--   0 name      (1000) name      (1000)       39 2023-05-07 22:30:19.000000 simplt-0.0.3/src/simplt.egg-info/entry_points.txt
+-rw-rw-r--   0 name      (1000) name      (1000)       86 2023-05-07 22:30:19.000000 simplt-0.0.3/src/simplt.egg-info/requires.txt
+-rw-rw-r--   0 name      (1000) name      (1000)        7 2023-05-07 22:30:19.000000 simplt-0.0.3/src/simplt.egg-info/top_level.txt
```

### Comparing `simplt-0.0.2/licence` & `simplt-0.0.3/licence`

 * *Files identical despite different names*

### Comparing `simplt-0.0.2/pyproject.toml` & `simplt-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simplt-0.0.2/setup.cfg` & `simplt-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `simplt-0.0.2/src/simplt/arg_parser/arg_parser.py` & `simplt-0.0.3/src/simplt/arg_parser/arg_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 
     # Instantiate the parser
     parser = argparse.ArgumentParser(
         description="Optional description for arg parser"
     )
 
     parser.add_argument(
-        "-d",
-        "--delete-images",
+        "-r",
+        "--remove-images",
         action="store_true",
         default=False,
         help=(
-            "Delete the images in the (specified) output directory at start."
+            "Remove the images in the (specified) output directory at start."
         ),
     )
 
     parser.add_argument(
         "-b",
         "--box-plot",
         action="store_true",
@@ -33,15 +33,23 @@
     )
 
     parser.add_argument(
         "-l",
         "--line-plot",
         action="store_true",
         default=False,
-        help=("Create a box-plot based on your input data."),
+        help=("Create a colour-blind friendly multi-line plot."),
+    )
+
+    parser.add_argument(
+        "-d",
+        "--dot-plot",
+        action="store_true",
+        default=False,
+        help=("Create a dotted with multiple groups plot."),
     )
 
     parser.add_argument(
         "-o",
         "--output-path",
         action="store",
         type=str,
```

### Comparing `simplt-0.0.2/src/simplt/arg_parser/process_args.py` & `simplt-0.0.3/src/simplt/arg_parser/process_args.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Completes the tasks specified in the arg_parser."""
 import argparse
+from src.simplt.dotted_plot.dotted_plot import example_create_multi_group_dotted_plot
 
 from typeguard import typechecked
 
 from src.simplt.box_plot.box_plot import example_box_plot
 from src.simplt.export_plot import create_target_dir_if_not_exists
 from src.simplt.latex_table.latex_table import example_create_a_table
 from src.simplt.line_plot.line_plot import example_create_multi_line_plot
@@ -14,15 +15,15 @@
     """Processes the arguments and ensures the accompanying tasks are
     executed."""
     # Create output path.
     create_target_dir_if_not_exists(default_output_path)
     print(f"TODO: create: {default_output_path}")
 
     # Delete output images if desired.
-    if args.delete_images:
+    if args.remove_images:
         print("TODO: delete images.")
 
     if args.box_plot:
         example_box_plot(
             extensions=[
                 ".png",
             ],
@@ -34,13 +35,22 @@
         example_create_multi_line_plot(
             extensions=[
                 ".png",
             ],
             filename="example_line",
             output_dir=default_output_path,
         )
+    
+    if args.dot_plot:
+        example_create_multi_group_dotted_plot(
+            extensions=[
+                ".png",
+            ],
+            filename="example_dots",
+            output_dir=default_output_path,
+        )
 
     if args.latex_table:
         print("TODO: Create LaTex table.")
         example_create_a_table(
             filename="example", output_dir=default_output_path
         )
```

### Comparing `simplt-0.0.2/src/simplt/box_plot/box_plot.py` & `simplt-0.0.3/src/simplt/box_plot/box_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     Copy paste it in your own code and modify the values accordingly.
     """
 
     # Fixing random state for reproducibility
     np.random.seed(7)
 
-    # fake up some data
+    # Generate dummy data.
     first = [39, 44, 50, 50, 58, 63]
     second = [80, 100, 100, 120]
 
     # Add a name for each boxplot for in the legend, and y values.
     y_series = {"data_1": first, "data_2": second}
 
     create_box_plot(
@@ -118,10 +118,10 @@
     )
 
     # configure plot layout
     plt.legend(loc=legendPosition)
     plt.xlabel(x_axis_label)
     plt.ylabel(y_axis_label)
     for extension in extensions:
-        plt.savefig(f"{output_dir}/{filename}.{extension}")
+        plt.savefig(f"{output_dir}/{filename}{extension}")
     plt.clf()
     plt.close()
```

### Comparing `simplt-0.0.2/src/simplt/latex_table/latex_table.py` & `simplt-0.0.3/src/simplt/latex_table/latex_table.py`

 * *Files identical despite different names*

### Comparing `simplt-0.0.2/src/simplt/line_plot/line_plot.py` & `simplt-0.0.3/src/simplt/line_plot/line_plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """File used to create and export plots and tables directly into latex. Can be
 used to automatically update your results each time you run latex.
 
 For copy-pastable examples, see:     example_create_a_table()
 example_create_multi_line_plot()     example_create_single_line_plot()
 at the bottom of this file.
 """
-from typing import List
+from typing import Any, List, Optional
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib import lines
 from typeguard import typechecked
 
@@ -72,15 +72,15 @@
     """
     # pylint: disable=R0913
     # TODO: reduce 9/5 arguments to at most 5/5 arguments.
     fig = plt.figure()
     ax = fig.add_subplot(111)
 
     # Set line colours in plot object.
-    set_cmap(plt, len(y_series[:, 0]))
+    set_cmap(some_plt=plt, nr_of_colours=len(y_series[:, 0]), name="hsv")
 
     # Generate line types.
     lineTypes = generateLineTypes(y_series)
 
     # Geneterate lines.
     for i in range(0, len(y_series)):
         ax.plot(
@@ -102,17 +102,19 @@
 
 
 # Generate random line colours
 # Source: https://stackoverflow.com/questions/14720331/
 # how-to-generate-random-colors-in-matplotlib
 @typechecked
 def set_cmap(
-    some_plt: matplotlib.pyplot,
+    *,
+    #some_plt: matplotlib.pyplot,
+    some_plt: Any,
     nr_of_colours: int,
-    name: str = "hsv",
+    name:str,
 ) -> None:
     """Returns a function that maps each index in 0, 1, ..., n-1 to a distinct
     RGB color; the keyword argument name must be a standard mpl colormap name.
 
     :param n: param name:  (Default value = "hsv")
     :param name: Default value = "hsv")
     """
```

### Comparing `simplt-0.0.2/src/simplt.egg-info/SOURCES.txt` & `simplt-0.0.3/src/simplt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

