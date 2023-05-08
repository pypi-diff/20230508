# Comparing `tmp/circuitpython-ArrowLine-0.9.3.tar.gz` & `tmp/circuitpython-ArrowLine-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-ArrowLine-0.9.3.tar", last modified: Fri Jan 27 01:58:08 2023, max compression
+gzip compressed data, was "circuitpython-ArrowLine-1.0.1.tar", last modified: Mon May  8 01:51:14 2023, max compression
```

## Comparing `circuitpython-ArrowLine-0.9.3.tar` & `circuitpython-ArrowLine-1.0.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 01:58:08.224624 circuitpython-ArrowLine-0.9.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 01:58:08.220624 circuitpython-ArrowLine-0.9.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 01:58:08.220624 circuitpython-ArrowLine-0.9.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 01:58:08.220624 circuitpython-ArrowLine-0.9.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-01-27 01:58:08.224624 circuitpython-ArrowLine-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/README.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (123)     6783 2023-01-27 01:58:00.000000 circuitpython-ArrowLine-0.9.3/arrowline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 01:58:08.224624 circuitpython-ArrowLine-0.9.3/circuitpython_ArrowLine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-01-27 01:58:08.000000 circuitpython-ArrowLine-0.9.3/circuitpython_ArrowLine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-01-27 01:58:08.000000 circuitpython-ArrowLine-0.9.3/circuitpython_ArrowLine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 01:58:08.000000 circuitpython-ArrowLine-0.9.3/circuitpython_ArrowLine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-27 01:58:08.000000 circuitpython-ArrowLine-0.9.3/circuitpython_ArrowLine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-27 01:58:08.000000 circuitpython-ArrowLine-0.9.3/circuitpython_ArrowLine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 01:58:08.224624 circuitpython-ArrowLine-0.9.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 01:58:08.224624 circuitpython-ArrowLine-0.9.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 01:58:08.224624 circuitpython-ArrowLine-0.9.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-01-27 01:58:00.000000 circuitpython-ArrowLine-0.9.3/examples/arrowline_multiple_arrows.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-01-27 01:58:00.000000 circuitpython-ArrowLine-0.9.3/examples/arrowline_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-01-27 01:58:00.000000 circuitpython-ArrowLine-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-27 01:57:52.000000 circuitpython-ArrowLine-0.9.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 01:58:08.224624 circuitpython-ArrowLine-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-01-27 01:58:00.000000 circuitpython-ArrowLine-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.028372 circuitpython-ArrowLine-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.020372 circuitpython-ArrowLine-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.024371 circuitpython-ArrowLine-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.024371 circuitpython-ArrowLine-1.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-08 01:51:14.028372 circuitpython-ArrowLine-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/README.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10952 2023-05-08 01:51:03.000000 circuitpython-ArrowLine-1.0.1/arrowline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.024371 circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-08 01:51:13.000000 circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-08 01:51:14.000000 circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 01:51:13.000000 circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 01:51:13.000000 circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 01:51:13.000000 circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.028372 circuitpython-ArrowLine-1.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.028372 circuitpython-ArrowLine-1.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:51:14.028372 circuitpython-ArrowLine-1.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-08 01:51:03.000000 circuitpython-ArrowLine-1.0.1/examples/arrowline_dotted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-08 01:51:03.000000 circuitpython-ArrowLine-1.0.1/examples/arrowline_multiple_arrows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-08 01:51:03.000000 circuitpython-ArrowLine-1.0.1/examples/arrowline_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-08 01:51:03.000000 circuitpython-ArrowLine-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-08 01:50:48.000000 circuitpython-ArrowLine-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 01:51:14.028372 circuitpython-ArrowLine-1.0.1/setup.cfg
```

### Comparing `circuitpython-ArrowLine-0.9.3/.pre-commit-config.yaml` & `circuitpython-ArrowLine-1.0.1/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
     rev: 22.3.0
     hooks:
       - id: black
-  - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
-    hooks:
-      - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.2.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
```

### Comparing `circuitpython-ArrowLine-0.9.3/.pylintrc` & `circuitpython-ArrowLine-1.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-0.9.3/CODE_OF_CONDUCT.md` & `circuitpython-ArrowLine-1.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-0.9.3/LICENSE` & `circuitpython-ArrowLine-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-0.9.3/LICENSES/CC-BY-4.0.txt` & `circuitpython-ArrowLine-1.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-0.9.3/LICENSES/MIT.txt` & `circuitpython-ArrowLine-1.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-0.9.3/LICENSES/Unlicense.txt` & `circuitpython-ArrowLine-1.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-0.9.3/PKG-INFO` & `circuitpython-ArrowLine-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: circuitpython-ArrowLine
-Version: 0.9.3
+Version: 1.0.1
 Summary: CircuitPython library to draw Arrowlines.
-Home-page: https://github.com/jposada202020/CircuitPython_ArrowLine.git
-Author: Jose David M.
 Author-email: "Jose D. Montoya" <arrowline@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_ArrowLine.git
 Keywords: hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
@@ -23,24 +21,27 @@
 
 
 .. image:: https://readthedocs.org/projects/circuitpython-arrowline/badge/?version=latest
     :target: https://circuitpython-arrowline.readthedocs.io/
     :alt: Documentation Status
 
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
-    :target: https://adafru.it/discord
-    :alt: Discord
-
-
 .. image:: https://github.com/jposada202020/CircuitPython_ArrowLine/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_ArrowLine/actions
     :alt: Build Status
 
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-arrowline.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-arrowline
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-arrowline?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-arrowline
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 Utility function to draw arrow lines using vectorio
 
 .. image:: https://user-images.githubusercontent.com/34255413/113015260-5f288d80-914b-11eb-9a68-5283612b9bae.png
```

### Comparing `circuitpython-ArrowLine-0.9.3/README.rst` & `circuitpython-ArrowLine-1.0.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -3,24 +3,27 @@
 
 
 .. image:: https://readthedocs.org/projects/circuitpython-arrowline/badge/?version=latest
     :target: https://circuitpython-arrowline.readthedocs.io/
     :alt: Documentation Status
 
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
-    :target: https://adafru.it/discord
-    :alt: Discord
-
-
 .. image:: https://github.com/jposada202020/CircuitPython_ArrowLine/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_ArrowLine/actions
     :alt: Build Status
 
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-arrowline.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-arrowline
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-arrowline?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-arrowline
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 Utility function to draw arrow lines using vectorio
 
 .. image:: https://user-images.githubusercontent.com/34255413/113015260-5f288d80-914b-11eb-9a68-5283612b9bae.png
```

### Comparing `circuitpython-ArrowLine-0.9.3/circuitpython_ArrowLine.egg-info/PKG-INFO` & `circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: circuitpython-ArrowLine
-Version: 0.9.3
+Version: 1.0.1
 Summary: CircuitPython library to draw Arrowlines.
-Home-page: https://github.com/jposada202020/CircuitPython_ArrowLine.git
-Author: Jose David M.
 Author-email: "Jose D. Montoya" <arrowline@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_ArrowLine.git
 Keywords: hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
@@ -23,24 +21,27 @@
 
 
 .. image:: https://readthedocs.org/projects/circuitpython-arrowline/badge/?version=latest
     :target: https://circuitpython-arrowline.readthedocs.io/
     :alt: Documentation Status
 
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
-    :target: https://adafru.it/discord
-    :alt: Discord
-
-
 .. image:: https://github.com/jposada202020/CircuitPython_ArrowLine/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_ArrowLine/actions
     :alt: Build Status
 
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-arrowline.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-arrowline
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-arrowline?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-arrowline
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 Utility function to draw arrow lines using vectorio
 
 .. image:: https://user-images.githubusercontent.com/34255413/113015260-5f288d80-914b-11eb-9a68-5283612b9bae.png
```

### Comparing `circuitpython-ArrowLine-0.9.3/circuitpython_ArrowLine.egg-info/SOURCES.txt` & `circuitpython-ArrowLine-1.0.1/circuitpython_ArrowLine.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 arrowline.py
 pyproject.toml
 requirements.txt
-setup.py
 .github/workflows/build.yml
 .github/workflows/release_gh.yml
 .github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 circuitpython_ArrowLine.egg-info/PKG-INFO
@@ -26,9 +25,10 @@
 docs/conf.py
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
+examples/arrowline_dotted.py
 examples/arrowline_multiple_arrows.py
 examples/arrowline_simpletest.py
```

### Comparing `circuitpython-ArrowLine-0.9.3/docs/_static/favicon.ico` & `circuitpython-ArrowLine-1.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-0.9.3/docs/conf.py` & `circuitpython-ArrowLine-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-ArrowLine-0.9.3/examples/arrowline_multiple_arrows.py` & `circuitpython-ArrowLine-1.0.1/examples/arrowline_multiple_arrows.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,44 @@
-# SPDX-FileCopyrightText: 2021 Jose David M.
+# SPDX-FileCopyrightText: 2023 Jose David M.
 #
 # SPDX-License-Identifier: MIT
 #############################
 """
-This is an example of the use of the arrowline function. Using
-Multiple arrows and including a Circle Pointer
+This is a simple example of the use of the arrowline function.
 """
 
 import displayio
 import board
-from arrowline import line_arrow
+from arrowline import Line
 
 
 display = board.DISPLAY
 
 my_group = displayio.Group()
 
-bitmap = displayio.Bitmap(320, 240, 5)
+bitmap = displayio.Bitmap(300, 300, 5)
 
 screen_palette = displayio.Palette(3)
 screen_palette[1] = 0x00AA00
 screen_tilegrid = displayio.TileGrid(
     bitmap,
     pixel_shader=screen_palette,
-    x=30,
+    x=0,
     y=0,
 )
 
 my_group.append(screen_tilegrid)
 
-line = line_arrow(screen_tilegrid, 40, 32, 45, 60, 12, screen_palette, 1)
-line2 = line_arrow(screen_tilegrid, 60, 22, 33, 14, 6, screen_palette, 1)
-line3 = line_arrow(
-    screen_tilegrid, 100, 102, 150, 150, 14, screen_palette, 1, pointer="C"
-)
-line4 = line_arrow(screen_tilegrid, 0, 102, 0, 150, 12, screen_palette, 1)
-line5 = line_arrow(
-    screen_tilegrid, 239, 319, 220, 30, 12, screen_palette, 1, pointer="C"
-)
-
-
-my_group.append(line)
-my_group.append(line2)
-my_group.append(line3)
-my_group.append(line4)
-my_group.append(line5)
+a = Line(screen_tilegrid, 40, 32, 45, 60, 12, screen_palette, 1)
+my_group.append(a.draw)
+b = Line(screen_tilegrid, 60, 22, 33, 14, 6, screen_palette, 1)
+my_group.append(b.draw)
+c = Line(screen_tilegrid, 100, 102, 150, 150, 14, screen_palette, 1, pointer="C")
+my_group.append(c.draw)
+d = Line(screen_tilegrid, 0, 102, 0, 150, 12, screen_palette, 1)
+my_group.append(d.draw)
+e = Line(screen_tilegrid, 239, 319, 220, 30, 12, screen_palette, 1, pointer="C")
+my_group.append(e.draw)
 display.show(my_group)
 
 while True:
     pass
```

### Comparing `circuitpython-ArrowLine-0.9.3/examples/arrowline_simpletest.py` & `circuitpython-ArrowLine-1.0.1/examples/arrowline_simpletest.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #############################
 """
 This is a simple example of the use of the arrowline function.
 """
 
 import displayio
 import board
-from arrowline import line_arrow
+from arrowline import Line
 
 
 display = board.DISPLAY
 
 my_group = displayio.Group()
 
 bitmap = displayio.Bitmap(100, 100, 5)
@@ -24,13 +24,13 @@
     pixel_shader=screen_palette,
     x=50,
     y=50,
 )
 
 my_group.append(screen_tilegrid)
 
-line = line_arrow(screen_tilegrid, 40, 90, 90, 60, 12, screen_palette, 1)
-my_group.append(line)
+line = Line(screen_tilegrid, 40, 90, 90, 60, 12, screen_palette, 1)
+my_group.append(line.draw)
 display.show(my_group)
 
 while True:
     pass
```

### Comparing `circuitpython-ArrowLine-0.9.3/pyproject.toml` & `circuitpython-ArrowLine-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-ArrowLine"
 description = "CircuitPython library to draw Arrowlines."
-version = "0.9.3"
+version = "1.0.1"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "arrowline@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_ArrowLine.git"}
 keywords = [
     "hardware",
@@ -31,12 +31,12 @@
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["CircuitPython_Arrowline"]
+py-modules = ["arrowline"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 optional-dependencies = {optional = {file = ["optional_requirements.txt"]}}
```

