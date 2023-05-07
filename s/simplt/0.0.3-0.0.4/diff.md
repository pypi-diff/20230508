# Comparing `tmp/simplt-0.0.3.tar.gz` & `tmp/simplt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplt-0.0.3.tar", last modified: Sun May  7 22:30:19 2023, max compression
+gzip compressed data, was "simplt-0.0.4.tar", last modified: Sun May  7 23:33:25 2023, max compression
```

## Comparing `simplt-0.0.3.tar` & `simplt-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 22:30:19.774613 simplt-0.0.3/
--rw-rw-r--   0 name      (1000) name      (1000)     4792 2023-05-07 22:30:19.774613 simplt-0.0.3/PKG-INFO
--rw-rw-r--   0 name      (1000) name      (1000)     3979 2023-05-07 22:28:05.000000 simplt-0.0.3/README.md
--rw-rw-r--   0 name      (1000) name      (1000)    34523 2023-05-07 21:29:00.000000 simplt-0.0.3/licence
--rw-rw-r--   0 name      (1000) name      (1000)     1395 2023-05-07 21:29:00.000000 simplt-0.0.3/pyproject.toml
--rw-rw-r--   0 name      (1000) name      (1000)     1341 2023-05-07 22:30:19.774613 simplt-0.0.3/setup.cfg
--rw-rw-r--   0 name      (1000) name      (1000)      198 2023-05-07 21:29:00.000000 simplt-0.0.3/setup.py
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 22:30:19.770613 simplt-0.0.3/src/
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 22:30:19.774613 simplt-0.0.3/src/simplt/
--rw-rw-r--   0 name      (1000) name      (1000)      141 2023-05-07 22:29:51.000000 simplt-0.0.3/src/simplt/__init__.py
--rw-rw-r--   0 name      (1000) name      (1000)      448 2023-05-07 21:29:00.000000 simplt-0.0.3/src/simplt/__main__.py
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 22:30:19.774613 simplt-0.0.3/src/simplt/arg_parser/
--rw-rw-r--   0 name      (1000) name      (1000)        0 2023-05-07 21:29:00.000000 simplt-0.0.3/src/simplt/arg_parser/__init__.py
--rw-rw-r--   0 name      (1000) name      (1000)     1661 2023-05-07 21:58:16.000000 simplt-0.0.3/src/simplt/arg_parser/arg_parser.py
--rw-rw-r--   0 name      (1000) name      (1000)     1706 2023-05-07 21:58:33.000000 simplt-0.0.3/src/simplt/arg_parser/process_args.py
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 22:30:19.774613 simplt-0.0.3/src/simplt/box_plot/
--rw-rw-r--   0 name      (1000) name      (1000)        0 2023-05-07 21:29:00.000000 simplt-0.0.3/src/simplt/box_plot/__init__.py
--rw-rw-r--   0 name      (1000) name      (1000)     3464 2023-05-07 21:34:44.000000 simplt-0.0.3/src/simplt/box_plot/box_plot.py
--rw-rw-r--   0 name      (1000) name      (1000)      393 2023-05-07 21:29:00.000000 simplt-0.0.3/src/simplt/export_plot.py
--rw-rw-r--   0 name      (1000) name      (1000)       74 2023-05-07 21:29:00.000000 simplt-0.0.3/src/simplt/helper.py
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 22:30:19.774613 simplt-0.0.3/src/simplt/latex_table/
--rw-rw-r--   0 name      (1000) name      (1000)        0 2023-05-07 21:29:00.000000 simplt-0.0.3/src/simplt/latex_table/__init__.py
--rw-rw-r--   0 name      (1000) name      (1000)     2428 2023-05-07 21:29:00.000000 simplt-0.0.3/src/simplt/latex_table/latex_table.py
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 22:30:19.774613 simplt-0.0.3/src/simplt/line_plot/
--rw-rw-r--   0 name      (1000) name      (1000)        0 2023-05-07 21:29:00.000000 simplt-0.0.3/src/simplt/line_plot/__init__.py
--rw-rw-r--   0 name      (1000) name      (1000)     3706 2023-05-07 21:45:02.000000 simplt-0.0.3/src/simplt/line_plot/line_plot.py
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 22:30:19.774613 simplt-0.0.3/src/simplt.egg-info/
--rw-rw-r--   0 name      (1000) name      (1000)     4792 2023-05-07 22:30:19.000000 simplt-0.0.3/src/simplt.egg-info/PKG-INFO
--rw-rw-r--   0 name      (1000) name      (1000)      662 2023-05-07 22:30:19.000000 simplt-0.0.3/src/simplt.egg-info/SOURCES.txt
--rw-rw-r--   0 name      (1000) name      (1000)        1 2023-05-07 22:30:19.000000 simplt-0.0.3/src/simplt.egg-info/dependency_links.txt
--rw-rw-r--   0 name      (1000) name      (1000)       39 2023-05-07 22:30:19.000000 simplt-0.0.3/src/simplt.egg-info/entry_points.txt
--rw-rw-r--   0 name      (1000) name      (1000)       86 2023-05-07 22:30:19.000000 simplt-0.0.3/src/simplt.egg-info/requires.txt
--rw-rw-r--   0 name      (1000) name      (1000)        7 2023-05-07 22:30:19.000000 simplt-0.0.3/src/simplt.egg-info/top_level.txt
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 23:33:25.971112 simplt-0.0.4/
+-rw-rw-r--   0 name      (1000) name      (1000)     5100 2023-05-07 23:33:25.971112 simplt-0.0.4/PKG-INFO
+-rw-rw-r--   0 name      (1000) name      (1000)     4287 2023-05-07 23:26:43.000000 simplt-0.0.4/README.md
+-rw-rw-r--   0 name      (1000) name      (1000)    34523 2023-05-07 21:29:00.000000 simplt-0.0.4/licence
+-rw-rw-r--   0 name      (1000) name      (1000)     1395 2023-05-07 21:29:00.000000 simplt-0.0.4/pyproject.toml
+-rw-rw-r--   0 name      (1000) name      (1000)     1322 2023-05-07 23:33:25.971112 simplt-0.0.4/setup.cfg
+-rw-rw-r--   0 name      (1000) name      (1000)      198 2023-05-07 21:29:00.000000 simplt-0.0.4/setup.py
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 23:33:25.971112 simplt-0.0.4/src/
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 23:33:25.971112 simplt-0.0.4/src/simplt/
+-rw-rw-r--   0 name      (1000) name      (1000)        0 2023-05-07 23:32:21.000000 simplt-0.0.4/src/simplt/__init__.py
+-rw-rw-r--   0 name      (1000) name      (1000)      448 2023-05-07 21:29:00.000000 simplt-0.0.4/src/simplt/__main__.py
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 23:33:25.971112 simplt-0.0.4/src/simplt/arg_parser/
+-rw-rw-r--   0 name      (1000) name      (1000)        0 2023-05-07 21:29:00.000000 simplt-0.0.4/src/simplt/arg_parser/__init__.py
+-rw-rw-r--   0 name      (1000) name      (1000)     1661 2023-05-07 21:58:16.000000 simplt-0.0.4/src/simplt/arg_parser/arg_parser.py
+-rw-rw-r--   0 name      (1000) name      (1000)     1706 2023-05-07 21:58:33.000000 simplt-0.0.4/src/simplt/arg_parser/process_args.py
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 23:33:25.971112 simplt-0.0.4/src/simplt/box_plot/
+-rw-rw-r--   0 name      (1000) name      (1000)        0 2023-05-07 21:29:00.000000 simplt-0.0.4/src/simplt/box_plot/__init__.py
+-rw-rw-r--   0 name      (1000) name      (1000)     3464 2023-05-07 21:34:44.000000 simplt-0.0.4/src/simplt/box_plot/box_plot.py
+-rw-rw-r--   0 name      (1000) name      (1000)      393 2023-05-07 21:29:00.000000 simplt-0.0.4/src/simplt/export_plot.py
+-rw-rw-r--   0 name      (1000) name      (1000)       74 2023-05-07 21:29:00.000000 simplt-0.0.4/src/simplt/helper.py
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 23:33:25.971112 simplt-0.0.4/src/simplt/latex_table/
+-rw-rw-r--   0 name      (1000) name      (1000)        0 2023-05-07 21:29:00.000000 simplt-0.0.4/src/simplt/latex_table/__init__.py
+-rw-rw-r--   0 name      (1000) name      (1000)     2428 2023-05-07 21:29:00.000000 simplt-0.0.4/src/simplt/latex_table/latex_table.py
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 23:33:25.971112 simplt-0.0.4/src/simplt/line_plot/
+-rw-rw-r--   0 name      (1000) name      (1000)        0 2023-05-07 21:29:00.000000 simplt-0.0.4/src/simplt/line_plot/__init__.py
+-rw-rw-r--   0 name      (1000) name      (1000)     3706 2023-05-07 21:45:02.000000 simplt-0.0.4/src/simplt/line_plot/line_plot.py
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-05-07 23:33:25.971112 simplt-0.0.4/src/simplt.egg-info/
+-rw-rw-r--   0 name      (1000) name      (1000)     5100 2023-05-07 23:33:25.000000 simplt-0.0.4/src/simplt.egg-info/PKG-INFO
+-rw-rw-r--   0 name      (1000) name      (1000)      662 2023-05-07 23:33:25.000000 simplt-0.0.4/src/simplt.egg-info/SOURCES.txt
+-rw-rw-r--   0 name      (1000) name      (1000)        1 2023-05-07 23:33:25.000000 simplt-0.0.4/src/simplt.egg-info/dependency_links.txt
+-rw-rw-r--   0 name      (1000) name      (1000)       39 2023-05-07 23:33:25.000000 simplt-0.0.4/src/simplt.egg-info/entry_points.txt
+-rw-rw-r--   0 name      (1000) name      (1000)       86 2023-05-07 23:33:25.000000 simplt-0.0.4/src/simplt.egg-info/requires.txt
+-rw-rw-r--   0 name      (1000) name      (1000)        7 2023-05-07 23:33:25.000000 simplt-0.0.4/src/simplt.egg-info/top_level.txt
```

### Comparing `simplt-0.0.3/PKG-INFO` & `simplt-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplt
-Version: 0.0.3
+Version: 0.0.4
 Summary: Makes plotting matplotlib easy.
 Home-page: https://github.com/a-t-0/simplt
 Author: a-t-0
 Author-email: no-email@no-email.org
 Maintainer: a-t-0
 Maintainer-email: no-email@no-email.org
 License: AGPLv3
@@ -67,15 +67,15 @@
     y_axis_label="y-axis label [units]",
     y_series=y_series,
 )
 ```
 
 And creates:
 
-<img src="output/example_box.png" width="640" height="480" />
+<img src="https://github.com/a-t-0/simplt/blob/main/output/example_box.png" width="640" height="480" />
 
 ## Example Multi-Line Plot
 ```py
 python -m simplt --line-plot
 ```
 Which is the same as running:
 ```py
@@ -108,56 +108,60 @@
     y_axis_label="y-axis label [units]",
     y_series=multiple_y_series,
 )
 ```
 
 And creates a (colorblind-friendly) lineplot:
 
-<img src="output/example_line.png" width="640" height="480" />
+<img src="https://github.com/a-t-0/simplt/blob/main/output/example_line.png" width="640" height="480" />
 
-## Example Multi-Line Plot
+## Example Multi-Group Scatter Plot
 ```py
 python -m simplt --dot-plot
 ```
 Which is the same as running:
 ```py
 from simplt.dotted_plot.dotted_plot import plot_multiple_dotted_groups
 import numpy as np
 
-extensions=[
-    ".png",
-],
-filename="example_dots",
-output_dir="output",
+single_x_series = [3., 5.]
+multiple_y_series:Dict[int,Dict[float,List[float]]] = {}
 
-multiple_y_series = np.zeros((2, 2), dtype=int)
 # actually fill with data
-multiple_y_series[0] = [1, 2]
+multiple_y_series[0]={}
+multiple_y_series[0][single_x_series[0]] = [1., 2., 5.]
+multiple_y_series[0][single_x_series[1]] = [0., 6.]
+
+multiple_y_series[1]={}
+multiple_y_series[1][single_x_series[0]] = [3., 4.]
+multiple_y_series[1][single_x_series[1]] = [1., 5.]
+
+
+
 groupLabels = [
     "first_group",
     "second_group",
 ]  # add a label for each dataseries
-single_x_series = [3, 5]
 
+print(multiple_y_series)
 plot_multiple_dotted_groups(
     extensions=extensions,
     filename=filename,
     label=groupLabels,
     legendPosition=0,
     output_dir=output_dir,
-    x=single_x_series,
     x_axis_label="x-axis label [units]",
     y_axis_label="y-axis label [units]",
     y_series=multiple_y_series,
 )
 ```
 
 And creates a (colorblind-friendly) dotplot:
 
-<img src="output/example_dots.png" width="640" height="480" />
+<img src="https://github.com/a-t-0/simplt/blob/main/output/example_dots.png" width="640" height="480" />
 
 
 ## For Developers
 Below are pip-package publication instructions.
 ### Releasing pip package update
 
 To udate the Python pip package, one can first satisfy the following requirements:
```

### Comparing `simplt-0.0.3/README.md` & `simplt-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     y_axis_label="y-axis label [units]",
     y_series=y_series,
 )
 ```
 
 And creates:
 
-<img src="output/example_box.png" width="640" height="480" />
+<img src="https://github.com/a-t-0/simplt/blob/main/output/example_box.png" width="640" height="480" />
 
 ## Example Multi-Line Plot
 ```py
 python -m simplt --line-plot
 ```
 Which is the same as running:
 ```py
@@ -85,56 +85,60 @@
     y_axis_label="y-axis label [units]",
     y_series=multiple_y_series,
 )
 ```
 
 And creates a (colorblind-friendly) lineplot:
 
-<img src="output/example_line.png" width="640" height="480" />
+<img src="https://github.com/a-t-0/simplt/blob/main/output/example_line.png" width="640" height="480" />
 
-## Example Multi-Line Plot
+## Example Multi-Group Scatter Plot
 ```py
 python -m simplt --dot-plot
 ```
 Which is the same as running:
 ```py
 from simplt.dotted_plot.dotted_plot import plot_multiple_dotted_groups
 import numpy as np
 
-extensions=[
-    ".png",
-],
-filename="example_dots",
-output_dir="output",
+single_x_series = [3., 5.]
+multiple_y_series:Dict[int,Dict[float,List[float]]] = {}
 
-multiple_y_series = np.zeros((2, 2), dtype=int)
 # actually fill with data
-multiple_y_series[0] = [1, 2]
+multiple_y_series[0]={}
+multiple_y_series[0][single_x_series[0]] = [1., 2., 5.]
+multiple_y_series[0][single_x_series[1]] = [0., 6.]
+
+multiple_y_series[1]={}
+multiple_y_series[1][single_x_series[0]] = [3., 4.]
+multiple_y_series[1][single_x_series[1]] = [1., 5.]
+
+
+
 groupLabels = [
     "first_group",
     "second_group",
 ]  # add a label for each dataseries
-single_x_series = [3, 5]
 
+print(multiple_y_series)
 plot_multiple_dotted_groups(
     extensions=extensions,
     filename=filename,
     label=groupLabels,
     legendPosition=0,
     output_dir=output_dir,
-    x=single_x_series,
     x_axis_label="x-axis label [units]",
     y_axis_label="y-axis label [units]",
     y_series=multiple_y_series,
 )
 ```
 
 And creates a (colorblind-friendly) dotplot:
 
-<img src="output/example_dots.png" width="640" height="480" />
+<img src="https://github.com/a-t-0/simplt/blob/main/output/example_dots.png" width="640" height="480" />
 
 
 ## For Developers
 Below are pip-package publication instructions.
 ### Releasing pip package update
 
 To udate the Python pip package, one can first satisfy the following requirements:
```

### Comparing `simplt-0.0.3/licence` & `simplt-0.0.4/licence`

 * *Files identical despite different names*

### Comparing `simplt-0.0.3/pyproject.toml` & `simplt-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simplt-0.0.3/setup.cfg` & `simplt-0.0.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = simplt
-version = attr: simplt.__version__
+version = 0.0.4
 description = Makes plotting matplotlib easy.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/a-t-0/simplt
 author = a-t-0
 author_email = no-email@no-email.org
 maintainer = a-t-0
```

### Comparing `simplt-0.0.3/src/simplt/arg_parser/arg_parser.py` & `simplt-0.0.4/src/simplt/arg_parser/arg_parser.py`

 * *Files identical despite different names*

### Comparing `simplt-0.0.3/src/simplt/arg_parser/process_args.py` & `simplt-0.0.4/src/simplt/arg_parser/process_args.py`

 * *Files identical despite different names*

### Comparing `simplt-0.0.3/src/simplt/box_plot/box_plot.py` & `simplt-0.0.4/src/simplt/box_plot/box_plot.py`

 * *Files identical despite different names*

### Comparing `simplt-0.0.3/src/simplt/latex_table/latex_table.py` & `simplt-0.0.4/src/simplt/latex_table/latex_table.py`

 * *Files identical despite different names*

### Comparing `simplt-0.0.3/src/simplt/line_plot/line_plot.py` & `simplt-0.0.4/src/simplt/line_plot/line_plot.py`

 * *Files identical despite different names*

### Comparing `simplt-0.0.3/src/simplt.egg-info/PKG-INFO` & `simplt-0.0.4/src/simplt.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplt
-Version: 0.0.3
+Version: 0.0.4
 Summary: Makes plotting matplotlib easy.
 Home-page: https://github.com/a-t-0/simplt
 Author: a-t-0
 Author-email: no-email@no-email.org
 Maintainer: a-t-0
 Maintainer-email: no-email@no-email.org
 License: AGPLv3
@@ -67,15 +67,15 @@
     y_axis_label="y-axis label [units]",
     y_series=y_series,
 )
 ```
 
 And creates:
 
-<img src="output/example_box.png" width="640" height="480" />
+<img src="https://github.com/a-t-0/simplt/blob/main/output/example_box.png" width="640" height="480" />
 
 ## Example Multi-Line Plot
 ```py
 python -m simplt --line-plot
 ```
 Which is the same as running:
 ```py
@@ -108,56 +108,60 @@
     y_axis_label="y-axis label [units]",
     y_series=multiple_y_series,
 )
 ```
 
 And creates a (colorblind-friendly) lineplot:
 
-<img src="output/example_line.png" width="640" height="480" />
+<img src="https://github.com/a-t-0/simplt/blob/main/output/example_line.png" width="640" height="480" />
 
-## Example Multi-Line Plot
+## Example Multi-Group Scatter Plot
 ```py
 python -m simplt --dot-plot
 ```
 Which is the same as running:
 ```py
 from simplt.dotted_plot.dotted_plot import plot_multiple_dotted_groups
 import numpy as np
 
-extensions=[
-    ".png",
-],
-filename="example_dots",
-output_dir="output",
+single_x_series = [3., 5.]
+multiple_y_series:Dict[int,Dict[float,List[float]]] = {}
 
-multiple_y_series = np.zeros((2, 2), dtype=int)
 # actually fill with data
-multiple_y_series[0] = [1, 2]
+multiple_y_series[0]={}
+multiple_y_series[0][single_x_series[0]] = [1., 2., 5.]
+multiple_y_series[0][single_x_series[1]] = [0., 6.]
+
+multiple_y_series[1]={}
+multiple_y_series[1][single_x_series[0]] = [3., 4.]
+multiple_y_series[1][single_x_series[1]] = [1., 5.]
+
+
+
 groupLabels = [
     "first_group",
     "second_group",
 ]  # add a label for each dataseries
-single_x_series = [3, 5]
 
+print(multiple_y_series)
 plot_multiple_dotted_groups(
     extensions=extensions,
     filename=filename,
     label=groupLabels,
     legendPosition=0,
     output_dir=output_dir,
-    x=single_x_series,
     x_axis_label="x-axis label [units]",
     y_axis_label="y-axis label [units]",
     y_series=multiple_y_series,
 )
 ```
 
 And creates a (colorblind-friendly) dotplot:
 
-<img src="output/example_dots.png" width="640" height="480" />
+<img src="https://github.com/a-t-0/simplt/blob/main/output/example_dots.png" width="640" height="480" />
 
 
 ## For Developers
 Below are pip-package publication instructions.
 ### Releasing pip package update
 
 To udate the Python pip package, one can first satisfy the following requirements:
```

### Comparing `simplt-0.0.3/src/simplt.egg-info/SOURCES.txt` & `simplt-0.0.4/src/simplt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

