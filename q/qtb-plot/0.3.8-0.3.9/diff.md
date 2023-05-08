# Comparing `tmp/qtb_plot-0.3.8.tar.gz` & `tmp/qtb_plot-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtb_plot-0.3.8.tar", max compression
+gzip compressed data, was "qtb_plot-0.3.9.tar", max compression
```

## Comparing `qtb_plot-0.3.8.tar` & `qtb_plot-0.3.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1207 2023-03-31 09:47:12.631177 qtb_plot-0.3.8/README.md
--rw-r--r--   0        0        0     1093 2023-03-31 09:47:12.666179 qtb_plot-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1116 2023-03-31 09:47:12.666179 qtb_plot-0.3.8/src/qtbplot/__init__.py
--rw-r--r--   0        0        0    12370 2023-03-31 09:47:12.666179 qtb_plot-0.3.8/src/qtbplot/colors.py
--rw-r--r--   0        0        0     3652 2023-03-31 09:47:12.666179 qtb_plot-0.3.8/src/qtbplot/plot.py
--rw-r--r--   0        0        0     1970 1970-01-01 00:00:00.000000 qtb_plot-0.3.8/setup.py
--rw-r--r--   0        0        0     1945 1970-01-01 00:00:00.000000 qtb_plot-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1207 2023-05-05 10:13:12.728451 qtb_plot-0.3.9/README.md
+-rw-r--r--   0        0        0     1093 2023-05-05 10:13:12.762454 qtb_plot-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1116 2023-05-05 10:13:12.763454 qtb_plot-0.3.9/src/qtbplot/__init__.py
+-rw-r--r--   0        0        0    12370 2023-05-05 10:13:12.763454 qtb_plot-0.3.9/src/qtbplot/colors.py
+-rw-r--r--   0        0        0     3652 2023-05-05 10:13:12.763454 qtb_plot-0.3.9/src/qtbplot/plot.py
+-rw-r--r--   0        0        0     1970 1970-01-01 00:00:00.000000 qtb_plot-0.3.9/setup.py
+-rw-r--r--   0        0        0     1945 1970-01-01 00:00:00.000000 qtb_plot-0.3.9/PKG-INFO
```

### Comparing `qtb_plot-0.3.8/README.md` & `qtb_plot-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `qtb_plot-0.3.8/pyproject.toml` & `qtb_plot-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtb-plot"
-version = "0.3.8"
+version = "0.3.9"
 description = "Standard plotting styles of our institute"
 authors = ["Marvin van Aalst <marvin.vanaalst@gmail.com>"]
 license = "GPL-4"
 readme = "README.md"
 repository = "https://gitlab.com/marvin.vanaalst/qtb-plot"
 packages = [{include = "qtbplot", from = "src"}]
 keywords = ["plotting"]
```

### Comparing `qtb_plot-0.3.8/src/qtbplot/__init__.py` & `qtb_plot-0.3.9/src/qtbplot/__init__.py`

 * *Files identical despite different names*

### Comparing `qtb_plot-0.3.8/src/qtbplot/colors.py` & `qtb_plot-0.3.9/src/qtbplot/colors.py`

 * *Files identical despite different names*

### Comparing `qtb_plot-0.3.8/src/qtbplot/plot.py` & `qtb_plot-0.3.9/src/qtbplot/plot.py`

 * *Files identical despite different names*

### Comparing `qtb_plot-0.3.8/setup.py` & `qtb_plot-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'qtb-plot',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'Standard plotting styles of our institute',
     'long_description': '# QTB Plot\n\n[![pipeline status](https://gitlab.com/marvin.vanaalst/qtb-plot/badges/main/pipeline.svg)](https://gitlab.com/marvin.vanaalst/qtb-plot/-/commits/main)\n[![coverage report](https://gitlab.com/marvin.vanaalst/qtb-plot/badges/main/coverage.svg)](https://gitlab.com/marvin.vanaalst/qtb-plot/-/commits/main)\n[![PyPi](https://img.shields.io/pypi/v/qtb-plot)](https://pypi.org/project/qtb-plot/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n[![Downloads](https://pepy.tech/badge/qtb-plot)](https://pepy.tech/project/qtb-plot)\n\nThis package is basically just a convenience matplotlib option setter.\nYou have two ways of using it.\nWith `set_style` you set the style for the entire notebook or whatever session\nyou are working in and with `plotting_context` you create a context manager\nthat will only set the style locally for the current plot.\n\nTake a look at the supplied tutorial notebok to see how this is done.\n\n\nThe easiest way of installing the package is to cd into the package folder and to install it locally with\n`pip install -e .`\n',
     'author': 'Marvin van Aalst',
     'author_email': 'marvin.vanaalst@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/marvin.vanaalst/qtb-plot',
```

### Comparing `qtb_plot-0.3.8/PKG-INFO` & `qtb_plot-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtb-plot
-Version: 0.3.8
+Version: 0.3.9
 Summary: Standard plotting styles of our institute
 Home-page: https://gitlab.com/marvin.vanaalst/qtb-plot
 License: GPL-4
 Keywords: plotting
 Author: Marvin van Aalst
 Author-email: marvin.vanaalst@gmail.com
 Requires-Python: >=3.8,<4.0
```

