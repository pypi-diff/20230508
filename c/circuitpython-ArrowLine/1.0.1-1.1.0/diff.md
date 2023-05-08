# Comparing `tmp/circuitpython-ArrowLine-1.0.1.tar.gz` & `tmp/circuitpython-ArrowLine-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-ArrowLine-1.0.1.tar", last modified: Mon May  8 01:51:14 2023, max compression
+gzip compressed data, was "circuitpython-ArrowLine-1.1.0.tar", last modified: Mon May  8 14:07:17 2023, max compression
```

## Comparing `circuitpython-ArrowLine-1.0.1.tar` & `circuitpython-ArrowLine-1.1.0.tar`

### file list

```diff
@@ -1,44 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.028372 circuitpython-ArrowLine-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.020372 circuitpython-ArrowLine-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.024371 circuitpython-ArrowLine-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.024371 circuitpython-ArrowLine-1.0.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-08 01:51:14.028372 circuitpython-ArrowLine-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/README.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (123)    10952 2023-05-08 01:51:03.000000 circuitpython-ArrowLine-1.0.1/arrowline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.024371 circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-08 01:51:13.000000 circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-08 01:51:14.000000 circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 01:51:13.000000 circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 01:51:13.000000 circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 01:51:13.000000 circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.028372 circuitpython-ArrowLine-1.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.028372 circuitpython-ArrowLine-1.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.028372 circuitpython-ArrowLine-1.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-08 01:51:03.000000 circuitpython-ArrowLine-1.0.1/examples/arrowline_dotted.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-08 01:51:03.000000 circuitpython-ArrowLine-1.0.1/examples/arrowline_multiple_arrows.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-08 01:51:03.000000 circuitpython-ArrowLine-1.0.1/examples/arrowline_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-08 01:51:03.000000 circuitpython-ArrowLine-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 01:51:14.028372 circuitpython-ArrowLine-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:07:17.929785 circuitpython-ArrowLine-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:07:17.925785 circuitpython-ArrowLine-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:07:17.925785 circuitpython-ArrowLine-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:07:17.925785 circuitpython-ArrowLine-1.1.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-08 14:07:17.929785 circuitpython-ArrowLine-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/README.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10608 2023-05-08 14:07:10.000000 circuitpython-ArrowLine-1.1.0/arrowline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:07:17.929785 circuitpython-ArrowLine-1.1.0/circuitpython_ArrowLine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-08 14:07:17.000000 circuitpython-ArrowLine-1.1.0/circuitpython_ArrowLine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-08 14:07:17.000000 circuitpython-ArrowLine-1.1.0/circuitpython_ArrowLine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 14:07:17.000000 circuitpython-ArrowLine-1.1.0/circuitpython_ArrowLine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 14:07:17.000000 circuitpython-ArrowLine-1.1.0/circuitpython_ArrowLine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 14:07:17.000000 circuitpython-ArrowLine-1.1.0/circuitpython_ArrowLine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:07:17.929785 circuitpython-ArrowLine-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:07:17.929785 circuitpython-ArrowLine-1.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:07:17.929785 circuitpython-ArrowLine-1.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-08 14:07:10.000000 circuitpython-ArrowLine-1.1.0/examples/arrowline_dotted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-08 14:07:10.000000 circuitpython-ArrowLine-1.1.0/examples/arrowline_multiple_arrows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-08 14:07:10.000000 circuitpython-ArrowLine-1.1.0/examples/arrowline_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-08 14:07:10.000000 circuitpython-ArrowLine-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-08 14:07:00.000000 circuitpython-ArrowLine-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 14:07:17.929785 circuitpython-ArrowLine-1.1.0/setup.cfg
```

### Comparing `circuitpython-ArrowLine-1.0.1/.pre-commit-config.yaml` & `circuitpython-ArrowLine-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.1/.pylintrc` & `circuitpython-ArrowLine-1.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.1/CODE_OF_CONDUCT.md` & `circuitpython-ArrowLine-1.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.1/LICENSE` & `circuitpython-ArrowLine-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.1/LICENSES/CC-BY-4.0.txt` & `circuitpython-ArrowLine-1.1.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.1/LICENSES/MIT.txt` & `circuitpython-ArrowLine-1.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.1/LICENSES/Unlicense.txt` & `circuitpython-ArrowLine-1.1.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.1/PKG-INFO` & `circuitpython-ArrowLine-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-ArrowLine
-Version: 1.0.1
+Version: 1.1.0
 Summary: CircuitPython library to draw Arrowlines.
 Author-email: "Jose D. Montoya" <arrowline@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_ArrowLine.git
 Keywords: hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-ArrowLine-1.0.1/README.rst` & `circuitpython-ArrowLine-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.1/arrowline.py` & `circuitpython-ArrowLine-1.1.0/arrowline.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from vectorio import Polygon, Circle
 
 try:
     from typing import Optional
 except ImportError:
     pass
 
-__version__ = "1.0.1"
+__version__ = "1.1.0"
 __repo__ = "https://github.com/jposada202020/CircuitPython_ArrowLine.git"
 
 
 class Line:
 
     """A Line Arrow utility.
 
@@ -51,17 +51,16 @@
     :param `displayio.Palette` palette: palette object used to display the bitmap.
      This is used to have the same color for the arrow
     :param int pal_index: pallet color index used in the bitmap to give the arrow line the color
      property
 
     :param int line_width: the width of the arrow's line, in pixels (default = 1)
     :param bool solid_line: indicates if the line is a solid line. Defaults to `True`
-    :param int line_length: Length in pixels of the line. It is recommended
-     due to floating point calculations that this value stays at 5. you could try others
-     combinations of line_lenght and line_space. Defaults to 5.
+    :param int line_length: Length in pixels of the line.
+     combinations of line_length and line_space. Defaults to 5.
     :param int line_space: Line space in pixels. Defaults to 5
 
     :param str pointer: point type. Two pointers could be selected :const:`C` Circle
      or :const:`A` Arrow. Defaults to Arrow
 
     :return: `displayio.Group`
 
@@ -125,28 +124,28 @@
         x2: int = 10,
         y2: int = 10,
         arrow_length: int = 10,
         palette: Optional[displayio.Palette] = None,
         pal_index: int = 1,
         line_width: int = 1,
         solid_line: bool = True,
-        line_lenght: int = 5,
+        line_length: int = 5,
         line_space: int = 5,
         pointer: str = "A",
     ):
         if palette is None:
             raise Exception("Must provide a valid palette")
         self.x1 = x1
         self.y1 = y1
         self.x2 = x2
         self.y2 = y2
         self._arrow_length = arrow_length
         self.line_width = line_width
 
-        self.line_length = line_lenght
+        self.line_length = line_length
         self.line_space = line_space
         self.pal_index = pal_index
         self.my_group = displayio.Group()
 
         self.arrow_palette = displayio.Palette(2)
         self.arrow_palette.make_transparent(0)
         self.arrow_palette[1] = palette[self.pal_index]
@@ -250,69 +249,66 @@
             x=0,
             y=0,
             color_index=self.pal_index,
         )
         self.my_group.append(line_base)
 
     def _dotted_line(self):
-        end_line_xx = self.x1 + int(math.ceil(self.line_length * math.cos(self._angle)))
-        end_line_yy = self.y1 + int(math.ceil(self.line_length * math.sin(self._angle)))
-        xd1 = self.x1
-        yd1 = self.y1
-
-        while True:
-            if self.x1 < self.x2:
-                if xd1 > self._arrow_base_x:
-                    break
-                if self.y1 < self.y2:
-                    if yd1 > self._arrow_base_y:
-                        break
-            if self.x1 > self.x2:
-                if xd1 < self._arrow_base_x:
-                    break
-                if self.y1 < self.y2:
-                    if yd1 > self._arrow_base_y:
-                        break
+        distance = math.sqrt((self.x2 - self.x1) ** 2 + (self.y2 - self.y1) ** 2)
 
-            _line = _angledrectangle(
-                xd1, yd1, end_line_xx, end_line_yy, stroke=self.line_width
+        suma = self.line_length
+        puntos = []
+        puntos.append((self.x2, self.y2))
+        while suma < distance:
+            puntos.append(
+                (
+                    self.x2 - int(math.ceil(suma * math.cos(self._angle))),
+                    self.y2 - int(math.ceil(suma * math.sin(self._angle))),
+                )
             )
-            # print("line draw", _line)
+            suma = suma + self.line_length + self.line_space
 
-            xd1 = int(math.ceil(self.line_space * math.cos(self._angle))) + end_line_xx
-            yd1 = int(math.ceil(self.line_space * math.sin(self._angle))) + end_line_yy
-            end_line_xx = xd1 + int(self.line_length * math.cos(self._angle))
-            end_line_yy = yd1 + int(self.line_length * math.sin(self._angle))
+        for i, ele in enumerate(puntos):
 
-            line_base = Polygon(
-                pixel_shader=self.arrow_palette,
-                points=[
-                    (
-                        self.x_reference + _line[0][0],
-                        self.y_reference + _line[0][1],
-                    ),
-                    (
-                        self.x_reference + _line[1][0],
-                        self.y_reference + _line[1][1],
-                    ),
-                    (
-                        self.x_reference + _line[2][0],
-                        self.y_reference + _line[2][1],
-                    ),
-                    (
-                        self.x_reference + _line[3][0],
-                        self.y_reference + _line[3][1],
-                    ),
-                ],
-                x=0,
-                y=0,
-                color_index=self.pal_index,
-            )
+            if i == 0:
+                continue
+            if i % 2 == 0:
+                _line = _angledrectangle(
+                    ele[0],
+                    ele[1],
+                    puntos[i - 1][0],
+                    puntos[i - 1][1],
+                    stroke=self.line_width,
+                )
+                line_base = Polygon(
+                    pixel_shader=self.arrow_palette,
+                    points=[
+                        (
+                            self.x_reference + _line[0][0],
+                            self.y_reference + _line[0][1],
+                        ),
+                        (
+                            self.x_reference + _line[1][0],
+                            self.y_reference + _line[1][1],
+                        ),
+                        (
+                            self.x_reference + _line[2][0],
+                            self.y_reference + _line[2][1],
+                        ),
+                        (
+                            self.x_reference + _line[3][0],
+                            self.y_reference + _line[3][1],
+                        ),
+                    ],
+                    x=0,
+                    y=0,
+                    color_index=self.pal_index,
+                )
 
-            self.my_group.append(line_base)
+                self.my_group.append(line_base)
 
 
 def _angledrectangle(x1, y1, x2, y2, stroke=1):
     # Code Source for this function by kmatch98 (R) 2021
     # https://github.com/adafruit/CircuitPython_Community_Bundle/pull/63
     if x2 - x1 == 0:
         xdiff1 = round(stroke / 2)
```

### Comparing `circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/PKG-INFO` & `circuitpython-ArrowLine-1.1.0/circuitpython_ArrowLine.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-ArrowLine
-Version: 1.0.1
+Version: 1.1.0
 Summary: CircuitPython library to draw Arrowlines.
 Author-email: "Jose D. Montoya" <arrowline@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_ArrowLine.git
 Keywords: hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/SOURCES.txt` & `circuitpython-ArrowLine-1.1.0/circuitpython_ArrowLine.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -23,12 +23,17 @@
 docs/api.rst
 docs/api.rst.license
 docs/conf.py
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
+docs/requirements.txt
+docs/_static/Logo.png
+docs/_static/Logo.png.license
+docs/_static/extra_css.css
+docs/_static/extra_css.css.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/arrowline_dotted.py
 examples/arrowline_multiple_arrows.py
 examples/arrowline_simpletest.py
```

### Comparing `circuitpython-ArrowLine-1.0.1/docs/_static/favicon.ico` & `circuitpython-ArrowLine-1.1.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.1/docs/examples.rst` & `circuitpython-ArrowLine-1.1.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.1/examples/arrowline_dotted.py` & `circuitpython-ArrowLine-1.1.0/examples/arrowline_dotted.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,57 +34,57 @@
     100,
     150,
     200,
     12,
     screen_palette,
     1,
     solid_line=False,
-    line_lenght=5,
+    line_length=5,
     line_space=5,
 )
 my_group.append(a.draw)
 b = Line(
     screen_tilegrid,
     100,
     100,
     200,
     200,
     12,
     screen_palette,
     1,
     solid_line=False,
-    line_lenght=5,
+    line_length=5,
     line_space=5,
 )
 my_group.append(b.draw)
 c = Line(
     screen_tilegrid,
     100,
     100,
     50,
     200,
     12,
     screen_palette,
     1,
     solid_line=False,
-    line_lenght=5,
+    line_length=5,
     line_space=5,
 )
 my_group.append(c.draw)
 d = Line(
     screen_tilegrid,
     40,
     90,
     150,
     40,
     12,
     screen_palette,
     1,
     solid_line=False,
-    line_lenght=5,
+    line_length=5,
     line_space=5,
 )
 my_group.append(d.draw)
 display.show(my_group)
 
 while True:
     pass
```

### Comparing `circuitpython-ArrowLine-1.0.1/examples/arrowline_multiple_arrows.py` & `circuitpython-ArrowLine-1.1.0/examples/arrowline_multiple_arrows.py`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.1/examples/arrowline_simpletest.py` & `circuitpython-ArrowLine-1.1.0/examples/arrowline_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-1.0.1/pyproject.toml` & `circuitpython-ArrowLine-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-ArrowLine"
 description = "CircuitPython library to draw Arrowlines."
-version = "1.0.1"
+version = "1.1.0"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "arrowline@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_ArrowLine.git"}
 keywords = [
     "hardware",
```

