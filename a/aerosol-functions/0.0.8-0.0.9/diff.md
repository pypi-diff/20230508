# Comparing `tmp/aerosol-functions-0.0.8.tar.gz` & `tmp/aerosol-functions-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aerosol-functions-0.0.8.tar", last modified: Sat Apr  1 07:05:35 2023, max compression
+gzip compressed data, was "aerosol-functions-0.0.9.tar", last modified: Tue Apr 11 23:11:28 2023, max compression
```

## Comparing `aerosol-functions-0.0.8.tar` & `aerosol-functions-0.0.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2023-04-01 07:05:35.578432 aerosol-functions-0.0.8/
--rw-rw-r--   0 jlam      (1000) jlam      (1000)     1073 2023-03-24 08:39:39.000000 aerosol-functions-0.0.8/LICENSE.txt
--rw-rw-r--   0 jlam      (1000) jlam      (1000)       50 2023-04-01 07:01:34.000000 aerosol-functions-0.0.8/MANIFEST.in
--rw-rw-r--   0 jlam      (1000) jlam      (1000)      556 2023-04-01 07:05:35.578432 aerosol-functions-0.0.8/PKG-INFO
--rw-rw-r--   0 jlam      (1000) jlam      (1000)      229 2023-04-01 06:36:09.000000 aerosol-functions-0.0.8/README.md
-drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2023-04-01 07:05:35.571432 aerosol-functions-0.0.8/docs/
--rw-rw-r--   0 jlam      (1000) jlam      (1000)      230 2023-04-01 06:25:21.000000 aerosol-functions-0.0.8/docs/.buildinfo
--rw-rw-r--   0 jlam      (1000) jlam      (1000)        0 2023-03-24 23:20:21.000000 aerosol-functions-0.0.8/docs/.nojekyll
-drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2023-04-01 07:05:35.572433 aerosol-functions-0.0.8/docs/_images/
--rw-rw-r--   0 jlam      (1000) jlam      (1000)   140955 2023-04-01 06:25:21.000000 aerosol-functions-0.0.8/docs/_images/plotting_tutorial_1_0.png
--rw-rw-r--   0 jlam      (1000) jlam      (1000)   106264 2023-04-01 06:25:21.000000 aerosol-functions-0.0.8/docs/_images/plotting_tutorial_3_0.png
-drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2023-04-01 07:05:35.573433 aerosol-functions-0.0.8/docs/_sources/
--rw-rw-r--   0 jlam      (1000) jlam      (1000)      228 2023-03-31 13:51:02.000000 aerosol-functions-0.0.8/docs/_sources/aerosol.rst.txt
--rw-rw-r--   0 jlam      (1000) jlam      (1000)      551 2023-03-31 22:29:35.000000 aerosol-functions-0.0.8/docs/_sources/index.rst.txt
--rw-rw-r--   0 jlam      (1000) jlam      (1000)       45 2023-03-24 21:57:24.000000 aerosol-functions-0.0.8/docs/_sources/modules.rst.txt
--rw-rw-r--   0 jlam      (1000) jlam      (1000)   334191 2023-04-01 06:25:05.000000 aerosol-functions-0.0.8/docs/_sources/plotting_tutorial.ipynb.txt
-drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2023-04-01 07:05:35.576433 aerosol-functions-0.0.8/docs/_static/
--rw-rw-r--   0 jlam      (1000) jlam      (1000)    11230 2023-04-01 06:25:21.000000 aerosol-functions-0.0.8/docs/_static/alabaster.css
--rw-rw-r--   0 jlam      (1000) jlam      (1000)    14813 2023-04-01 06:25:21.000000 aerosol-functions-0.0.8/docs/_static/basic.css
--rw-rw-r--   0 jlam      (1000) jlam      (1000)       42 2023-03-24 13:54:05.000000 aerosol-functions-0.0.8/docs/_static/custom.css
--rw-rw-r--   0 jlam      (1000) jlam      (1000)     4472 2023-03-24 13:54:05.000000 aerosol-functions-0.0.8/docs/_static/doctools.js
--rw-rw-r--   0 jlam      (1000) jlam      (1000)      420 2023-04-01 06:25:21.000000 aerosol-functions-0.0.8/docs/_static/documentation_options.js
--rw-rw-r--   0 jlam      (1000) jlam      (1000)      286 2023-03-24 13:54:05.000000 aerosol-functions-0.0.8/docs/_static/file.png
--rw-rw-r--   0 jlam      (1000) jlam      (1000)     4758 2023-04-01 06:25:21.000000 aerosol-functions-0.0.8/docs/_static/language_data.js
--rw-rw-r--   0 jlam      (1000) jlam      (1000)    25050 2023-03-24 13:39:01.000000 aerosol-functions-0.0.8/docs/_static/logo.png
--rw-rw-r--   0 jlam      (1000) jlam      (1000)       90 2023-03-24 13:54:05.000000 aerosol-functions-0.0.8/docs/_static/minus.png
--rw-rw-r--   0 jlam      (1000) jlam      (1000)     4467 2023-03-29 18:24:47.000000 aerosol-functions-0.0.8/docs/_static/nbsphinx-broken-thumbnail.svg
--rw-rw-r--   0 jlam      (1000) jlam      (1000)     6625 2023-04-01 06:25:21.000000 aerosol-functions-0.0.8/docs/_static/nbsphinx-code-cells.css
--rw-rw-r--   0 jlam      (1000) jlam      (1000)      584 2023-03-29 18:24:47.000000 aerosol-functions-0.0.8/docs/_static/nbsphinx-gallery.css
--rw-rw-r--   0 jlam      (1000) jlam      (1000)     2871 2023-03-29 18:24:47.000000 aerosol-functions-0.0.8/docs/_static/nbsphinx-no-thumbnail.svg
--rw-rw-r--   0 jlam      (1000) jlam      (1000)       90 2023-03-24 13:54:05.000000 aerosol-functions-0.0.8/docs/_static/plus.png
--rw-rw-r--   0 jlam      (1000) jlam      (1000)     5327 2023-04-01 06:25:21.000000 aerosol-functions-0.0.8/docs/_static/pygments.css
--rw-rw-r--   0 jlam      (1000) jlam      (1000)    18215 2023-03-24 13:54:05.000000 aerosol-functions-0.0.8/docs/_static/searchtools.js
--rw-rw-r--   0 jlam      (1000) jlam      (1000)     4712 2023-03-24 13:54:05.000000 aerosol-functions-0.0.8/docs/_static/sphinx_highlight.js
--rw-rw-r--   0 jlam      (1000) jlam      (1000)    58970 2023-04-01 06:25:21.000000 aerosol-functions-0.0.8/docs/aerosol.html
--rw-rw-r--   0 jlam      (1000) jlam      (1000)     9224 2023-04-01 06:25:21.000000 aerosol-functions-0.0.8/docs/genindex.html
--rw-rw-r--   0 jlam      (1000) jlam      (1000)     9859 2023-04-01 06:25:21.000000 aerosol-functions-0.0.8/docs/index.html
--rw-rw-r--   0 jlam      (1000) jlam      (1000)     9368 2023-04-01 06:25:21.000000 aerosol-functions-0.0.8/docs/modules.html
--rw-rw-r--   0 jlam      (1000) jlam      (1000)     1016 2023-04-01 06:25:21.000000 aerosol-functions-0.0.8/docs/objects.inv
--rw-rw-r--   0 jlam      (1000) jlam      (1000)    18049 2023-04-01 06:25:21.000000 aerosol-functions-0.0.8/docs/plotting_tutorial.html
--rw-rw-r--   0 jlam      (1000) jlam      (1000)   334191 2023-04-01 06:25:20.000000 aerosol-functions-0.0.8/docs/plotting_tutorial.ipynb
--rw-rw-r--   0 jlam      (1000) jlam      (1000)     3911 2023-04-01 06:25:21.000000 aerosol-functions-0.0.8/docs/py-modindex.html
--rw-rw-r--   0 jlam      (1000) jlam      (1000)     3260 2023-04-01 06:25:21.000000 aerosol-functions-0.0.8/docs/search.html
--rw-rw-r--   0 jlam      (1000) jlam      (1000)    11055 2023-04-01 06:25:21.000000 aerosol-functions-0.0.8/docs/searchindex.js
--rw-rw-r--   0 jlam      (1000) jlam      (1000)       38 2023-04-01 07:05:35.578432 aerosol-functions-0.0.8/setup.cfg
--rw-rw-r--   0 jlam      (1000) jlam      (1000)      673 2023-04-01 07:01:26.000000 aerosol-functions-0.0.8/setup.py
-drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2023-04-01 07:05:35.566433 aerosol-functions-0.0.8/src/
-drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2023-04-01 07:05:35.577432 aerosol-functions-0.0.8/src/aerosol/
--rw-rw-r--   0 jlam      (1000) jlam      (1000)       35 2023-03-31 14:12:16.000000 aerosol-functions-0.0.8/src/aerosol/__init__.py
--rw-rw-r--   0 jlam      (1000) jlam      (1000)    20679 2023-03-31 14:21:35.000000 aerosol-functions-0.0.8/src/aerosol/functions.py
--rw-rw-r--   0 jlam      (1000) jlam      (1000)    13771 2023-03-31 22:02:56.000000 aerosol-functions-0.0.8/src/aerosol/plotting.py
-drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2023-04-01 07:05:35.578432 aerosol-functions-0.0.8/src/aerosol_functions.egg-info/
--rw-rw-r--   0 jlam      (1000) jlam      (1000)      556 2023-04-01 07:05:35.000000 aerosol-functions-0.0.8/src/aerosol_functions.egg-info/PKG-INFO
--rw-rw-r--   0 jlam      (1000) jlam      (1000)     1278 2023-04-01 07:05:35.000000 aerosol-functions-0.0.8/src/aerosol_functions.egg-info/SOURCES.txt
--rw-rw-r--   0 jlam      (1000) jlam      (1000)        1 2023-04-01 07:05:35.000000 aerosol-functions-0.0.8/src/aerosol_functions.egg-info/dependency_links.txt
--rw-rw-r--   0 jlam      (1000) jlam      (1000)       59 2023-04-01 07:05:35.000000 aerosol-functions-0.0.8/src/aerosol_functions.egg-info/requires.txt
--rw-rw-r--   0 jlam      (1000) jlam      (1000)        8 2023-04-01 07:05:35.000000 aerosol-functions-0.0.8/src/aerosol_functions.egg-info/top_level.txt
+drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2023-04-11 23:11:28.671105 aerosol-functions-0.0.9/
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)     1073 2023-03-24 08:39:39.000000 aerosol-functions-0.0.9/LICENSE.txt
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)       50 2023-04-01 07:14:17.000000 aerosol-functions-0.0.9/MANIFEST.in
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)      556 2023-04-11 23:11:28.671105 aerosol-functions-0.0.9/PKG-INFO
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)      229 2023-04-01 07:06:51.000000 aerosol-functions-0.0.9/README.md
+drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2023-04-11 23:11:28.665105 aerosol-functions-0.0.9/docs/
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)      230 2023-04-11 23:06:39.000000 aerosol-functions-0.0.9/docs/.buildinfo
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)        0 2023-03-24 23:20:21.000000 aerosol-functions-0.0.9/docs/.nojekyll
+drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2023-04-11 23:11:28.665105 aerosol-functions-0.0.9/docs/_images/
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)   140955 2023-04-11 23:06:39.000000 aerosol-functions-0.0.9/docs/_images/plotting_tutorial_1_0.png
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)   106264 2023-04-11 23:06:39.000000 aerosol-functions-0.0.9/docs/_images/plotting_tutorial_3_0.png
+drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2023-04-11 23:11:28.666105 aerosol-functions-0.0.9/docs/_sources/
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)      228 2023-03-31 13:51:02.000000 aerosol-functions-0.0.9/docs/_sources/aerosol.rst.txt
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)      551 2023-03-31 22:29:35.000000 aerosol-functions-0.0.9/docs/_sources/index.rst.txt
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)       45 2023-03-24 21:57:24.000000 aerosol-functions-0.0.9/docs/_sources/modules.rst.txt
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)   334123 2023-04-03 14:41:34.000000 aerosol-functions-0.0.9/docs/_sources/plotting_tutorial.ipynb.txt
+drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2023-04-11 23:11:28.669105 aerosol-functions-0.0.9/docs/_static/
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)    11230 2023-04-11 23:06:39.000000 aerosol-functions-0.0.9/docs/_static/alabaster.css
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)    14813 2023-04-11 23:06:39.000000 aerosol-functions-0.0.9/docs/_static/basic.css
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)       42 2023-03-24 13:54:05.000000 aerosol-functions-0.0.9/docs/_static/custom.css
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)     4472 2023-03-24 13:54:05.000000 aerosol-functions-0.0.9/docs/_static/doctools.js
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)      420 2023-04-11 23:06:39.000000 aerosol-functions-0.0.9/docs/_static/documentation_options.js
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)      286 2023-03-24 13:54:05.000000 aerosol-functions-0.0.9/docs/_static/file.png
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)     4758 2023-04-11 23:06:39.000000 aerosol-functions-0.0.9/docs/_static/language_data.js
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)    25050 2023-03-24 13:39:01.000000 aerosol-functions-0.0.9/docs/_static/logo.png
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)       90 2023-03-24 13:54:05.000000 aerosol-functions-0.0.9/docs/_static/minus.png
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)     4467 2023-03-29 18:24:47.000000 aerosol-functions-0.0.9/docs/_static/nbsphinx-broken-thumbnail.svg
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)     6625 2023-04-11 23:06:39.000000 aerosol-functions-0.0.9/docs/_static/nbsphinx-code-cells.css
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)      584 2023-03-29 18:24:47.000000 aerosol-functions-0.0.9/docs/_static/nbsphinx-gallery.css
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)     2871 2023-03-29 18:24:47.000000 aerosol-functions-0.0.9/docs/_static/nbsphinx-no-thumbnail.svg
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)       90 2023-03-24 13:54:05.000000 aerosol-functions-0.0.9/docs/_static/plus.png
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)     5327 2023-04-11 23:06:39.000000 aerosol-functions-0.0.9/docs/_static/pygments.css
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)    18215 2023-03-24 13:54:05.000000 aerosol-functions-0.0.9/docs/_static/searchtools.js
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)     4712 2023-03-24 13:54:05.000000 aerosol-functions-0.0.9/docs/_static/sphinx_highlight.js
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)    59180 2023-04-11 23:06:39.000000 aerosol-functions-0.0.9/docs/aerosol.html
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)     9224 2023-04-11 23:06:39.000000 aerosol-functions-0.0.9/docs/genindex.html
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)     9859 2023-04-11 23:06:39.000000 aerosol-functions-0.0.9/docs/index.html
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)     9368 2023-04-11 23:06:39.000000 aerosol-functions-0.0.9/docs/modules.html
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)     1016 2023-04-11 23:06:39.000000 aerosol-functions-0.0.9/docs/objects.inv
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)    17742 2023-04-11 23:06:39.000000 aerosol-functions-0.0.9/docs/plotting_tutorial.html
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)   334123 2023-04-11 23:06:38.000000 aerosol-functions-0.0.9/docs/plotting_tutorial.ipynb
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)     3911 2023-04-11 23:06:39.000000 aerosol-functions-0.0.9/docs/py-modindex.html
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)     3260 2023-04-11 23:06:39.000000 aerosol-functions-0.0.9/docs/search.html
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)    11004 2023-04-11 23:06:39.000000 aerosol-functions-0.0.9/docs/searchindex.js
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)       38 2023-04-11 23:11:28.671105 aerosol-functions-0.0.9/setup.cfg
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)      673 2023-04-11 23:09:20.000000 aerosol-functions-0.0.9/setup.py
+drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2023-04-11 23:11:28.662105 aerosol-functions-0.0.9/src/
+drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2023-04-11 23:11:28.670105 aerosol-functions-0.0.9/src/aerosol/
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)       35 2023-03-31 14:12:16.000000 aerosol-functions-0.0.9/src/aerosol/__init__.py
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)    20690 2023-04-11 23:05:06.000000 aerosol-functions-0.0.9/src/aerosol/functions.py
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)    13907 2023-04-11 23:05:59.000000 aerosol-functions-0.0.9/src/aerosol/plotting.py
+drwxrwxr-x   0 jlam      (1000) jlam      (1000)        0 2023-04-11 23:11:28.671105 aerosol-functions-0.0.9/src/aerosol_functions.egg-info/
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)      556 2023-04-11 23:11:28.000000 aerosol-functions-0.0.9/src/aerosol_functions.egg-info/PKG-INFO
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)     1278 2023-04-11 23:11:28.000000 aerosol-functions-0.0.9/src/aerosol_functions.egg-info/SOURCES.txt
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)        1 2023-04-11 23:11:28.000000 aerosol-functions-0.0.9/src/aerosol_functions.egg-info/dependency_links.txt
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)       59 2023-04-11 23:11:28.000000 aerosol-functions-0.0.9/src/aerosol_functions.egg-info/requires.txt
+-rw-rw-r--   0 jlam      (1000) jlam      (1000)        8 2023-04-11 23:11:28.000000 aerosol-functions-0.0.9/src/aerosol_functions.egg-info/top_level.txt
```

### Comparing `aerosol-functions-0.0.8/LICENSE.txt` & `aerosol-functions-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aerosol-functions-0.0.8/PKG-INFO` & `aerosol-functions-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aerosol-functions
-Version: 0.0.8
+Version: 0.0.9
 Summary: Functions to analyze atmospheric aerosol data
 Home-page: https://github.com/jlpl/aerosol-functions
 Author: Janne Lampilahti
 Author-email: janne.lampilahti@helsinki.fi
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `aerosol-functions-0.0.8/docs/_images/plotting_tutorial_1_0.png` & `aerosol-functions-0.0.9/docs/_images/plotting_tutorial_1_0.png`

 * *Files identical despite different names*

### Comparing `aerosol-functions-0.0.8/docs/_images/plotting_tutorial_3_0.png` & `aerosol-functions-0.0.9/docs/_images/plotting_tutorial_3_0.png`

 * *Files identical despite different names*

### Comparing `aerosol-functions-0.0.8/docs/_sources/index.rst.txt` & `aerosol-functions-0.0.9/docs/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `aerosol-functions-0.0.8/docs/_sources/plotting_tutorial.ipynb.txt` & `aerosol-functions-0.0.9/docs/_sources/plotting_tutorial.ipynb.txt`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999445921985816%*

 * *Differences: {"'cells'": "{1: {'source': {delete: [45]}}}"}*

```diff
@@ -71,15 +71,14 @@
                 "axy.set_ylabel(\"$f(x)$\")\n",
                 "fig.set_figheight(6)\n",
                 "fig.set_figwidth(4)\n",
                 "fig.suptitle(\"Log-normal distributions\\n $f(x;s) = \\\n",
                 "    \\\\frac{1}{sx\\\\sqrt{2\\\\pi}}e^{-\\\\frac{\\\\log^2 x}{2s^2}}$\",\n",
                 "    y=1.05,fontsize=12)\n",
                 "\n",
-                "plt.savefig(\"lognormal_dists.png\",bbox_inches=\"tight\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "22c156fa-d246-4ae8-93da-8c0ba536490d",
             "metadata": {},
```

### Comparing `aerosol-functions-0.0.8/docs/_static/alabaster.css` & `aerosol-functions-0.0.9/docs/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `aerosol-functions-0.0.8/docs/_static/basic.css` & `aerosol-functions-0.0.9/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `aerosol-functions-0.0.8/docs/_static/doctools.js` & `aerosol-functions-0.0.9/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `aerosol-functions-0.0.8/docs/_static/language_data.js` & `aerosol-functions-0.0.9/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `aerosol-functions-0.0.8/docs/_static/logo.png` & `aerosol-functions-0.0.9/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `aerosol-functions-0.0.8/docs/_static/nbsphinx-broken-thumbnail.svg` & `aerosol-functions-0.0.9/docs/_static/nbsphinx-broken-thumbnail.svg`

 * *Files identical despite different names*

### Comparing `aerosol-functions-0.0.8/docs/_static/nbsphinx-code-cells.css` & `aerosol-functions-0.0.9/docs/_static/nbsphinx-code-cells.css`

 * *Files identical despite different names*

### Comparing `aerosol-functions-0.0.8/docs/_static/nbsphinx-gallery.css` & `aerosol-functions-0.0.9/docs/_static/nbsphinx-gallery.css`

 * *Files identical despite different names*

### Comparing `aerosol-functions-0.0.8/docs/_static/nbsphinx-no-thumbnail.svg` & `aerosol-functions-0.0.9/docs/_static/nbsphinx-no-thumbnail.svg`

 * *Files identical despite different names*

### Comparing `aerosol-functions-0.0.8/docs/_static/pygments.css` & `aerosol-functions-0.0.9/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `aerosol-functions-0.0.8/docs/_static/searchtools.js` & `aerosol-functions-0.0.9/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `aerosol-functions-0.0.8/docs/_static/sphinx_highlight.js` & `aerosol-functions-0.0.9/docs/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `aerosol-functions-0.0.8/docs/aerosol.html` & `aerosol-functions-0.0.9/docs/aerosol.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
-    <title>aerosol package &#8212; aerosol-functions 0.0.8 documentation</title>
+    <title>aerosol package &#8212; aerosol-functions 0.0.9 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
     <script crossorigin="anonymous" integrity="sha256-Ae2Vz/4ePdIu6ZyI/5ZGsYnb+m0JlOmKPjt6XZ9JJkA=" src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.3.4/require.min.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
@@ -746,15 +746,15 @@
 </dl>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="aerosol.plotting.subplot_aerosol_dist">
-<span class="sig-prename descclassname"><span class="pre">aerosol.plotting.</span></span><span class="sig-name descname"><span class="pre">subplot_aerosol_dist</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">vlist</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">grid</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">cmap=&lt;matplotlib.colors.LinearSegmentedColormap</span> <span class="pre">object&gt;</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">norm=&lt;matplotlib.colors.Normalize</span> <span class="pre">object&gt;</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">xminortick_interval='1H'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">xmajortick_interval='2H'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">xticklabel_format='%H:%M'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">keep_inner_ticklabels=False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">subplot_padding=None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_subplots=False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_color='white'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">column_titles=None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#aerosol.plotting.subplot_aerosol_dist" title="Permalink to this definition">¶</a></dt>
+<span class="sig-prename descclassname"><span class="pre">aerosol.plotting.</span></span><span class="sig-name descname"><span class="pre">subplot_aerosol_dist</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">vlist</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">grid</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">cmap=&lt;matplotlib.colors.LinearSegmentedColormap</span> <span class="pre">object&gt;</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">norm=&lt;matplotlib.colors.Normalize</span> <span class="pre">object&gt;</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">xminortick_interval='1H'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">xmajortick_interval='2H'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">xticklabel_format='%H:%M'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">keep_inner_ticklabels=False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">subplot_padding=None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">subplot_labels=None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_color='black'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_size=10</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">column_titles=None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#aerosol.plotting.subplot_aerosol_dist" title="Permalink to this definition">¶</a></dt>
 <dd><p>Plot aerosol size distributions (subplots)</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><dl class="simple">
 <dt><strong>vlist</strong><span class="classifier">list of pandas.DataFrames</span></dt><dd><p>Aerosol size distributions (continuous index)</p>
 </dd>
 <dt><strong>grid</strong><span class="classifier">tuple (rows,columns)</span></dt><dd><p>define number of rows and columns</p>
@@ -775,17 +775,18 @@
 <a class="reference external" href="https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-code">https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-code</a></p>
 </dd>
 <dt><strong>keep_inner_ticklabels</strong><span class="classifier">bool</span></dt><dd><p>If True, use ticklabels in all subplots.
 If False, use ticklabels only on outer subplots.</p>
 </dd>
 <dt><strong>subplot_padding</strong><span class="classifier">number or None</span></dt><dd><p>Adjust space between subplots</p>
 </dd>
-<dt><strong>label_subplots</strong><span class="classifier">bool</span></dt><dd><p>Put labels on subplots</p>
+<dt><strong>subplot_labels</strong><span class="classifier">list of str or None</span></dt><dd><p>The labels to put to labels the subplots with</p>
 </dd>
 <dt><strong>label_color</strong><span class="classifier">str</span></dt><dd></dd>
+<dt><strong>label_size</strong><span class="classifier">float</span></dt><dd></dd>
 <dt><strong>column_titles</strong><span class="classifier">list of strings or None</span></dt><dd></dd>
 </dl>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><dl class="simple">
 <dt>figure object</dt><dd></dd>
 <dt>array of axes objects</dt><dd></dd>
```

#### html2text {}

```diff
@@ -405,16 +405,16 @@
                   lowest subplot x-axes
               matplotlib axes
                   lowest subplot y-axes
   aerosol.plotting.subplot_aerosol_dist(vlist, grid,
   cmap=<matplotlib.colors.LinearSegmentedColormap object>,
   norm=<matplotlib.colors.Normalize object>, xminortick_interval='1H',
   xmajortick_interval='2H', xticklabel_format='%H:%M',
-  keep_inner_ticklabels=False, subplot_padding=None, label_subplots=False,
-  label_color='white', column_titles=None)Â¶
+  keep_inner_ticklabels=False, subplot_padding=None, subplot_labels=None,
+  label_color='black', label_size=10, column_titles=None)Â¶
       Plot aerosol size distributions (subplots)
         Parameters:
               vlistlist of pandas.DataFrames
                   Aerosol size distributions (continuous index)
               gridtuple (rows,columns)
                   define number of rows and columns
               cmapmatplotlib colormap
@@ -433,17 +433,18 @@
                   docs.python.org/3/library/datetime.html#strftime-and-
                   strptime-format-code
               keep_inner_ticklabelsbool
                   If True, use ticklabels in all subplots. If False, use
                   ticklabels only on outer subplots.
               subplot_paddingnumber or None
                   Adjust space between subplots
-              label_subplotsbool
-                  Put labels on subplots
+              subplot_labelslist of str or None
+                  The labels to put to labels the subplots with
               label_colorstr
+              label_sizefloat
               column_titleslist of strings or None
         Returns:
               figure object
               array of axes objects
 
 [Logo]
 ****** aerosol-functions ******
```

### Comparing `aerosol-functions-0.0.8/docs/genindex.html` & `aerosol-functions-0.0.9/docs/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; aerosol-functions 0.0.8 documentation</title>
+    <title>Index &#8212; aerosol-functions 0.0.9 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
     <script crossorigin="anonymous" integrity="sha256-Ae2Vz/4ePdIu6ZyI/5ZGsYnb+m0JlOmKPjt6XZ9JJkA=" src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.3.4/require.min.js"></script>
     <link rel="index" title="Index" href="#" />
```

### Comparing `aerosol-functions-0.0.8/docs/index.html` & `aerosol-functions-0.0.9/docs/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
-    <title>Welcome to aerosol-functions’ documentation! &#8212; aerosol-functions 0.0.8 documentation</title>
+    <title>Welcome to aerosol-functions’ documentation! &#8212; aerosol-functions 0.0.9 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
     <script crossorigin="anonymous" integrity="sha256-Ae2Vz/4ePdIu6ZyI/5ZGsYnb+m0JlOmKPjt6XZ9JJkA=" src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.3.4/require.min.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
@@ -30,15 +30,15 @@
         <div class="bodywrapper">
           
 
           <div class="body" role="main">
             
   <section id="welcome-to-aerosol-functions-documentation">
 <h1>Welcome to aerosol-functions’ documentation!<a class="headerlink" href="#welcome-to-aerosol-functions-documentation" title="Permalink to this heading">¶</a></h1>
-<p>Version: 0.0.8</p>
+<p>Version: 0.0.9</p>
 <div class="toctree-wrapper compound">
 <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="aerosol.html">aerosol package</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="aerosol.html#module-aerosol.functions">aerosol.functions module</a><ul>
 <li class="toctree-l3"><a class="reference internal" href="aerosol.html#aerosol.functions.air_viscosity"><code class="docutils literal notranslate"><span class="pre">air_viscosity()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="aerosol.html#aerosol.functions.beta"><code class="docutils literal notranslate"><span class="pre">beta()</span></code></a></li>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 
 ****** Welcome to aerosol-functionsâ documentation!Â¶ ******
-Version: 0.0.8
+Version: 0.0.9
 Contents:
     * aerosol_package
           o aerosol.functions_module
                 # air_viscosity()
                 # beta()
                 # binary_diffusivity()
                 # calc_coags()
```

### Comparing `aerosol-functions-0.0.8/docs/modules.html` & `aerosol-functions-0.0.9/docs/modules.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
-    <title>&lt;no title&gt; &#8212; aerosol-functions 0.0.8 documentation</title>
+    <title>&lt;no title&gt; &#8212; aerosol-functions 0.0.9 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
     <script crossorigin="anonymous" integrity="sha256-Ae2Vz/4ePdIu6ZyI/5ZGsYnb+m0JlOmKPjt6XZ9JJkA=" src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.3.4/require.min.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
```

### Comparing `aerosol-functions-0.0.8/docs/objects.inv` & `aerosol-functions-0.0.9/docs/objects.inv`

 * *Files 1% similar despite different names*

#### Sphinx inventory

```diff
@@ -1,10 +1,10 @@
 # Sphinx inventory version 2
 # Project: aerosol-functions
-# Version: 0.0.8
+# Version: 0.0.9
 # The remainder of this file is compressed using zlib.
 
 aerosol.functions py:module 0 aerosol.html#module-$ -
 aerosol.functions.air_viscosity py:function 1 aerosol.html#$ -
 aerosol.functions.beta py:function 1 aerosol.html#$ -
 aerosol.functions.binary_diffusivity py:function 1 aerosol.html#$ -
 aerosol.functions.calc_coags py:function 1 aerosol.html#$ -
```

### Comparing `aerosol-functions-0.0.8/docs/plotting_tutorial.html` & `aerosol-functions-0.0.9/docs/plotting_tutorial.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
-    <title>Plotting examples &#8212; aerosol-functions 0.0.8 documentation</title>
+    <title>Plotting examples &#8212; aerosol-functions 0.0.9 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <link rel="stylesheet" type="text/css" href="_static/nbsphinx-code-cells.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
     <script crossorigin="anonymous" integrity="sha256-Ae2Vz/4ePdIu6ZyI/5ZGsYnb+m0JlOmKPjt6XZ9JJkA=" src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.3.4/require.min.js"></script>
@@ -84,15 +84,14 @@
 <span class="n">axy</span><span class="o">.</span><span class="n">set_ylabel</span><span class="p">(</span><span class="s2">&quot;$f(x)$&quot;</span><span class="p">)</span>
 <span class="n">fig</span><span class="o">.</span><span class="n">set_figheight</span><span class="p">(</span><span class="mi">6</span><span class="p">)</span>
 <span class="n">fig</span><span class="o">.</span><span class="n">set_figwidth</span><span class="p">(</span><span class="mi">4</span><span class="p">)</span>
 <span class="n">fig</span><span class="o">.</span><span class="n">suptitle</span><span class="p">(</span><span class="s2">&quot;Log-normal distributions</span><span class="se">\n</span><span class="s2"> $f(x;s) = </span><span class="se">\</span>
 <span class="s2">    </span><span class="se">\\</span><span class="s2">frac</span><span class="si">{1}</span><span class="s2">{sx</span><span class="se">\\</span><span class="s2">sqrt{2</span><span class="se">\\</span><span class="s2">pi}}e^{-</span><span class="se">\\</span><span class="s2">frac{</span><span class="se">\\</span><span class="s2">log^2 x}{2s^2}}$&quot;</span><span class="p">,</span>
     <span class="n">y</span><span class="o">=</span><span class="mf">1.05</span><span class="p">,</span><span class="n">fontsize</span><span class="o">=</span><span class="mi">12</span><span class="p">)</span>
 
-<span class="n">plt</span><span class="o">.</span><span class="n">savefig</span><span class="p">(</span><span class="s2">&quot;lognormal_dists.png&quot;</span><span class="p">,</span><span class="n">bbox_inches</span><span class="o">=</span><span class="s2">&quot;tight&quot;</span><span class="p">)</span>
 <span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
 </pre></div>
 </div>
 </div>
 <div class="nboutput nblast docutils container">
 <div class="prompt empty docutils container">
 </div>
```

#### html2text {}

```diff
@@ -51,15 +51,14 @@
 axy.set_ylabel("$f(x)$")
 fig.set_figheight(6)
 fig.set_figwidth(4)
 fig.suptitle("Log-normal distributions\n $f(x;s) = \
     \\frac{1}{sx\\sqrt{2\\pi}}e^{-\\frac{\\log^2 x}{2s^2}}$",
     y=1.05,fontsize=12)
 
-plt.savefig("lognormal_dists.png",bbox_inches="tight")
 plt.show()
 [_images/plotting_tutorial_1_0.png]
 
 ***** Aerosol size distribution subplotsÂ¶ *****
 [2]:
 import numpy as np
 import pandas as pd
```

### Comparing `aerosol-functions-0.0.8/docs/plotting_tutorial.ipynb` & `aerosol-functions-0.0.9/docs/plotting_tutorial.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999445921985816%*

 * *Differences: {"'cells'": "{1: {'source': {delete: [45]}}}"}*

```diff
@@ -71,15 +71,14 @@
                 "axy.set_ylabel(\"$f(x)$\")\n",
                 "fig.set_figheight(6)\n",
                 "fig.set_figwidth(4)\n",
                 "fig.suptitle(\"Log-normal distributions\\n $f(x;s) = \\\n",
                 "    \\\\frac{1}{sx\\\\sqrt{2\\\\pi}}e^{-\\\\frac{\\\\log^2 x}{2s^2}}$\",\n",
                 "    y=1.05,fontsize=12)\n",
                 "\n",
-                "plt.savefig(\"lognormal_dists.png\",bbox_inches=\"tight\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "22c156fa-d246-4ae8-93da-8c0ba536490d",
             "metadata": {},
```

### Comparing `aerosol-functions-0.0.8/docs/py-modindex.html` & `aerosol-functions-0.0.9/docs/py-modindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Python Module Index &#8212; aerosol-functions 0.0.8 documentation</title>
+    <title>Python Module Index &#8212; aerosol-functions 0.0.9 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
     <script crossorigin="anonymous" integrity="sha256-Ae2Vz/4ePdIu6ZyI/5ZGsYnb+m0JlOmKPjt6XZ9JJkA=" src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.3.4/require.min.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
```

### Comparing `aerosol-functions-0.0.8/docs/search.html` & `aerosol-functions-0.0.9/docs/search.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; aerosol-functions 0.0.8 documentation</title>
+    <title>Search &#8212; aerosol-functions 0.0.9 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
     <script crossorigin="anonymous" integrity="sha256-Ae2Vz/4ePdIu6ZyI/5ZGsYnb+m0JlOmKPjt6XZ9JJkA=" src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.3.4/require.min.js"></script>
```

### Comparing `aerosol-functions-0.0.8/docs/searchindex.js` & `aerosol-functions-0.0.9/docs/searchindex.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -62,15 +62,15 @@
         "org": 0,
         "10": [0, 3],
         "1016": 0,
         "0021": 0,
         "8502": 0,
         "71": 0,
         "90061": 0,
-        "9": 0,
+        "9": [0, 1],
         "m": [0, 3],
         "particl": 0,
         "n": [0, 3],
         "pressur": 0,
         "pa": 0,
         "ga": 0,
         "condens": 0,
@@ -326,28 +326,28 @@
         "y": [0, 3],
         "subplot_aerosol_dist": [0, 1, 2, 3],
         "vlist": 0,
         "grid": 0,
         "keep_inner_ticklabel": [0, 3],
         "fals": [0, 3],
         "subplot_pad": 0,
-        "label_subplot": [0, 3],
+        "subplot_label": 0,
         "label_color": [0, 3],
-        "white": 0,
+        "black": [0, 3],
+        "label_s": 0,
         "column_titl": 0,
         "tupl": 0,
         "bool": 0,
         "true": [0, 3],
         "onli": 0,
         "outer": 0,
         "adjust": 0,
         "put": 0,
         "version": 1,
         "0": [1, 3],
-        "8": [1, 3],
         "packag": [1, 2],
         "modul": [1, 2],
         "plot": [1, 2],
         "aerosol": 2,
         "function": 2,
         "import": 3,
         "np": 3,
@@ -374,17 +374,17 @@
         "ylabel": 3,
         "append": 3,
         "pdf": 3,
         "2f": 3,
         "t": 3,
         "fig": 3,
         "axx": 3,
+        "8": 3,
         "magma_r": 3,
         "edgecolor": 3,
-        "black": 3,
         "linewidth": 3,
         "30": 3,
         "set_xlabel": 3,
         "set_ylabel": 3,
         "f": 3,
         "set_figheight": 3,
         "6": 3,
@@ -395,19 +395,14 @@
         "sx": 3,
         "sqrt": 3,
         "2": 3,
         "pi": 3,
         "e": 3,
         "05": 3,
         "fontsiz": 3,
-        "savefig": 3,
-        "lognormal_dist": 3,
-        "png": 3,
-        "bbox_inch": 3,
-        "tight": 3,
         "show": 3,
         "xarrai": 3,
         "xr": 3,
         "load": 3,
         "d": 3,
         "open_dataset": 3,
         "nais_20220209": 3,
@@ -419,14 +414,15 @@
         "cax": 3,
         "turbo": 3,
         "symlognorm": 3,
         "vmin": 3,
         "vmax": 3,
         "3h": 3,
         "9h": 3,
+        "label_subplot": 3,
         "add": 3,
         "text": 3,
         "02": 3,
         "d_p": 3,
         "ha": 3,
         "center": 3,
         "set_label": 3
```

### Comparing `aerosol-functions-0.0.8/setup.py` & `aerosol-functions-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md","r") as fh: 
     long_description = fh.read()
 
 setup(
     name="aerosol-functions",
-    version="0.0.8",
+    version="0.0.9",
     description='Functions to analyze atmospheric aerosol data',
     package_dir={'':'src'},
     packages=['aerosol'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires='>=3.9',
     install_requires = [
```

### Comparing `aerosol-functions-0.0.8/src/aerosol/functions.py` & `aerosol-functions-0.0.9/src/aerosol/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -607,15 +607,15 @@
             dp_subset=dp[findex]
             conc=df.iloc[:,findex]
             logdp_mid=np.log10(dp_subset)
             logdp=(logdp_mid[:-1]+logdp_mid[1:])/2.0
             logdp=np.append(logdp,logdp_mid.max()+(logdp_mid.max()-logdp.max()))
             logdp=np.insert(logdp,0,logdp_mid.min()-(logdp.min()-logdp_mid.min()))
             dlogdp=np.diff(logdp)
-            conc=np.nansum(conc*dlogdp,axis=1)
+            conc = (conc*dlogdp).sum(axis=1, min_count=1)
 
         conc_df.insert(i,"%.2e_%.2e" % (dp1,dp2),conc)
 
     return conc_df
 
 def calc_formation_rate(
     dp1,
```

### Comparing `aerosol-functions-0.0.8/src/aerosol/plotting.py` & `aerosol-functions-0.0.9/src/aerosol/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,41 +83,43 @@
         major tick values
     list of strings
         major tick labels (powers of ten)
 
     """
 
     x=np.arange(1,10)
-    y=np.arange(min_exp,max_exp).astype(float)
+    y=np.arange(min_exp,max_exp+1).astype(float)
     log_minorticks=[]
     log_majorticks=[]
     log_majorticklabels=[]
     for j in y:
         for i in x:
             log_minorticks.append(np.log10(np.round(i*10**j,int(np.abs(j)))))
             if i==1:
                 log_majorticklabels.append("10$^{%d}$"%j)
                 log_majorticks.append(np.log10(np.round(i*10**j,int(np.abs(j)))))
 
     log_minorticks=np.array(log_minorticks)
+    log_minorticks=log_minorticks[log_minorticks<=max_exp]
     log_majorticks=np.array(log_majorticks)
     return log_minorticks,log_majorticks,log_majorticklabels
 
 def subplot_aerosol_dist(
     vlist,
     grid,
     cmap=cm.rainbow,
     norm=colors.Normalize(10,10000),
     xminortick_interval="1H",
     xmajortick_interval="2H",
     xticklabel_format="%H:%M",
     keep_inner_ticklabels=False,
     subplot_padding=None,
-    label_subplots=False,
-    label_color="white",
+    subplot_labels=None,
+    label_color="black",
+    label_size=10,
     column_titles=None):
     """ 
     Plot aerosol size distributions (subplots)
 
     Parameters
     ----------
 
@@ -141,29 +143,28 @@
         See for all options here: 
         https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-code
     keep_inner_ticklabels : bool
         If True, use ticklabels in all subplots.
         If False, use ticklabels only on outer subplots.
     subplot_padding : number or None
         Adjust space between subplots
-    label_subplots : bool
-        Put labels on subplots
+    subplot_labels : list of str or None
+        The labels to put to labels the subplots with
     label_color : str
+    label_size :  float
     column_titles : list of strings or None
     
     Returns
     -------
     
     figure object
     array of axes objects
      
     """
-    
-    labels = "abcdefghijklmnopqrstuvwxyzo"
-    
+     
     assert isinstance(vlist,list)
     
     rows = grid[0]
     columns = grid[1]
     fig,ax = plt.subplots(rows,columns)
     
     if subplot_padding is not None:
@@ -245,18 +246,18 @@
             
         if i>=len(vlist):
             axi.spines[['right','top','left','bottom']].set_visible(False)
             axi.set_yticks([],minor=True)
             axi.set_yticks([])
             axi.set_yticklabels([])
         
-        if label_subplots:
+        if subplot_labels is not None:
             if i<len(vlist):
-                axi.text(.01, .99, labels[i], ha='left', va='top', 
-                    color=label_color, transform=axi.transAxes)
+                axi.text(.01, .99, subplot_labels[i], ha='left', va='top', 
+                    color=label_color, transform=axi.transAxes, fontsize=label_size)
 
     if column_titles is not None:
         for column_title,axy in zip(column_titles,first_row_ax):
             axy.set_title(column_title)
     
     if columns>1:
         xspace = (size[0]-columns*ax_width)/(columns-1.0)
@@ -444,8 +445,8 @@
                 axi.fill_between(x,y[:,i],color=cmap(float(i)/float(n)), **kwargs)
             else:
                 axi.fill_between(x,y[:,i], **kwargs)
         
         axi.set_xlim((x.min(),x.max()))
         axi.set_ylim((y.min(),y.max()))
     
-    return fig,ax[0],axy
+    return fig,ax[0],axy
```

### Comparing `aerosol-functions-0.0.8/src/aerosol_functions.egg-info/PKG-INFO` & `aerosol-functions-0.0.9/src/aerosol_functions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aerosol-functions
-Version: 0.0.8
+Version: 0.0.9
 Summary: Functions to analyze atmospheric aerosol data
 Home-page: https://github.com/jlpl/aerosol-functions
 Author: Janne Lampilahti
 Author-email: janne.lampilahti@helsinki.fi
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `aerosol-functions-0.0.8/src/aerosol_functions.egg-info/SOURCES.txt` & `aerosol-functions-0.0.9/src/aerosol_functions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

