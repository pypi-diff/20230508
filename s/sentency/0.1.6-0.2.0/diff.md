# Comparing `tmp/sentency-0.1.6.tar.gz` & `tmp/sentency-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sentency-0.1.6.tar", last modified: Wed Aug 17 03:42:03 2022, max compression
+gzip compressed data, was "sentency-0.2.0.tar", last modified: Mon May  8 14:30:12 2023, max compression
```

## Comparing `sentency-0.1.6.tar` & `sentency-0.2.0.tar`

### file list

```diff
@@ -1,55 +1,41 @@
-drwxr-xr-x   0 gdelong   (1000) gdelong   (1000)        0 2022-08-17 03:42:03.000000 sentency-0.1.6/
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)      160 2022-07-11 17:58:37.000000 sentency-0.1.6/AUTHORS.rst
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)     3520 2022-07-11 17:58:37.000000 sentency-0.1.6/CONTRIBUTING.rst
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)       89 2022-07-11 17:58:37.000000 sentency-0.1.6/HISTORY.rst
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)     1071 2022-07-11 17:58:37.000000 sentency-0.1.6/LICENSE
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)      262 2022-07-11 17:58:37.000000 sentency-0.1.6/MANIFEST.in
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)     3133 2022-08-17 03:42:03.000000 sentency-0.1.6/PKG-INFO
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)     2286 2022-07-13 15:09:03.000000 sentency-0.1.6/README.rst
-drwxr-xr-x   0 gdelong   (1000) gdelong   (1000)        0 2022-08-17 03:42:03.000000 sentency-0.1.6/docs/
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)      609 2022-07-11 17:58:37.000000 sentency-0.1.6/docs/Makefile
-drwxr-xr-x   0 gdelong   (1000) gdelong   (1000)        0 2022-08-17 03:42:03.000000 sentency-0.1.6/docs/_build/
-drwxr-xr-x   0 gdelong   (1000) gdelong   (1000)        0 2022-08-17 03:42:03.000000 sentency-0.1.6/docs/_build/html/
-drwxr-xr-x   0 gdelong   (1000) gdelong   (1000)        0 2022-08-17 03:42:03.000000 sentency-0.1.6/docs/_build/html/_static/
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)      673 2022-07-11 18:15:26.000000 sentency-0.1.6/docs/_build/html/_static/ajax-loader.gif
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)      756 2022-07-11 18:15:26.000000 sentency-0.1.6/docs/_build/html/_static/comment-bright.png
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)      829 2022-07-11 18:15:26.000000 sentency-0.1.6/docs/_build/html/_static/comment-close.png
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)      641 2022-07-11 18:15:26.000000 sentency-0.1.6/docs/_build/html/_static/comment.png
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)      222 2022-07-11 18:15:26.000000 sentency-0.1.6/docs/_build/html/_static/down-pressed.png
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)      202 2022-07-11 18:15:26.000000 sentency-0.1.6/docs/_build/html/_static/down.png
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)      286 2022-07-11 18:15:26.000000 sentency-0.1.6/docs/_build/html/_static/file.png
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)       90 2022-07-11 18:15:26.000000 sentency-0.1.6/docs/_build/html/_static/minus.png
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)       90 2022-07-11 18:15:26.000000 sentency-0.1.6/docs/_build/html/_static/plus.png
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)      214 2022-07-11 18:15:26.000000 sentency-0.1.6/docs/_build/html/_static/up-pressed.png
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)      203 2022-07-11 18:15:26.000000 sentency-0.1.6/docs/_build/html/_static/up.png
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)       28 2022-07-11 17:58:37.000000 sentency-0.1.6/docs/authors.rst
--rwxr-xr-x   0 gdelong   (1000) gdelong   (1000)     4952 2022-07-14 21:39:43.000000 sentency-0.1.6/docs/conf.py
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)       33 2022-07-11 17:58:37.000000 sentency-0.1.6/docs/contributing.rst
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)       28 2022-07-11 17:58:37.000000 sentency-0.1.6/docs/history.rst
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)      305 2022-07-11 17:58:37.000000 sentency-0.1.6/docs/index.rst
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)     1122 2022-07-11 17:58:37.000000 sentency-0.1.6/docs/installation.rst
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)      770 2022-07-11 17:58:37.000000 sentency-0.1.6/docs/make.bat
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)       61 2022-08-17 03:37:32.000000 sentency-0.1.6/docs/modules.rst
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)       27 2022-07-11 17:58:37.000000 sentency-0.1.6/docs/readme.rst
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)      582 2022-08-17 03:37:32.000000 sentency-0.1.6/docs/sentency.rst
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)      894 2022-07-13 15:10:34.000000 sentency-0.1.6/docs/usage.rst
-drwxr-xr-x   0 gdelong   (1000) gdelong   (1000)        0 2022-08-17 03:42:03.000000 sentency-0.1.6/sentency/
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)      143 2022-07-14 21:39:43.000000 sentency-0.1.6/sentency/__init__.py
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)       22 2022-08-16 22:59:49.000000 sentency-0.1.6/sentency/_version.py
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)     1037 2022-08-17 03:21:09.000000 sentency-0.1.6/sentency/logs.py
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)     1355 2022-08-17 03:36:31.000000 sentency-0.1.6/sentency/regex.py
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)     4605 2022-08-17 03:34:54.000000 sentency-0.1.6/sentency/sentency.py
-drwxr-xr-x   0 gdelong   (1000) gdelong   (1000)        0 2022-08-17 03:42:03.000000 sentency-0.1.6/sentency.egg-info/
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)     3133 2022-08-17 03:42:02.000000 sentency-0.1.6/sentency.egg-info/PKG-INFO
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)     1069 2022-08-17 03:42:02.000000 sentency-0.1.6/sentency.egg-info/SOURCES.txt
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)        1 2022-08-17 03:42:02.000000 sentency-0.1.6/sentency.egg-info/dependency_links.txt
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)        1 2022-08-17 03:42:02.000000 sentency-0.1.6/sentency.egg-info/not-zip-safe
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)        6 2022-08-17 03:42:02.000000 sentency-0.1.6/sentency.egg-info/requires.txt
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)        9 2022-08-17 03:42:02.000000 sentency-0.1.6/sentency.egg-info/top_level.txt
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)      177 2022-08-17 03:42:03.000000 sentency-0.1.6/setup.cfg
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)     1514 2022-07-14 21:39:43.000000 sentency-0.1.6/setup.py
-drwxr-xr-x   0 gdelong   (1000) gdelong   (1000)        0 2022-08-17 03:42:03.000000 sentency-0.1.6/tests/
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)       38 2022-07-11 17:58:37.000000 sentency-0.1.6/tests/__init__.py
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)      657 2022-07-11 17:58:37.000000 sentency-0.1.6/tests/config.py
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)     1233 2022-07-11 17:58:37.000000 sentency-0.1.6/tests/test_regex.py
--rw-r--r--   0 gdelong   (1000) gdelong   (1000)     1833 2022-08-17 03:34:40.000000 sentency-0.1.6/tests/test_sentex.py
+drwxr-xr-x   0 gdelong   (1000) gdelong   (1000)        0 2023-05-08 14:30:12.571023 sentency-0.2.0/
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)      160 2023-05-07 12:52:13.000000 sentency-0.2.0/AUTHORS.rst
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)     3520 2023-05-07 12:52:13.000000 sentency-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)       89 2023-05-07 12:52:13.000000 sentency-0.2.0/HISTORY.rst
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)     1071 2023-05-07 12:52:13.000000 sentency-0.2.0/LICENSE
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)      262 2023-05-07 12:52:13.000000 sentency-0.2.0/MANIFEST.in
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)     3133 2023-05-08 14:30:12.571023 sentency-0.2.0/PKG-INFO
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)     2286 2023-05-07 12:52:13.000000 sentency-0.2.0/README.rst
+drwxr-xr-x   0 gdelong   (1000) gdelong   (1000)        0 2023-05-08 14:30:12.561023 sentency-0.2.0/docs/
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)      609 2023-05-07 12:52:13.000000 sentency-0.2.0/docs/Makefile
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)       28 2023-05-07 12:52:13.000000 sentency-0.2.0/docs/authors.rst
+-rwxr-xr-x   0 gdelong   (1000) gdelong   (1000)     4952 2023-05-07 12:52:13.000000 sentency-0.2.0/docs/conf.py
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)       33 2023-05-07 12:52:13.000000 sentency-0.2.0/docs/contributing.rst
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)       28 2023-05-07 12:52:13.000000 sentency-0.2.0/docs/history.rst
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)      305 2023-05-07 12:52:13.000000 sentency-0.2.0/docs/index.rst
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)     1122 2023-05-07 12:52:13.000000 sentency-0.2.0/docs/installation.rst
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)      770 2023-05-07 12:52:13.000000 sentency-0.2.0/docs/make.bat
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)       61 2023-05-07 12:52:13.000000 sentency-0.2.0/docs/modules.rst
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)       27 2023-05-07 12:52:13.000000 sentency-0.2.0/docs/readme.rst
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)      582 2023-05-07 12:52:13.000000 sentency-0.2.0/docs/sentency.rst
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)      894 2023-05-07 12:52:13.000000 sentency-0.2.0/docs/usage.rst
+drwxr-xr-x   0 gdelong   (1000) gdelong   (1000)        0 2023-05-08 14:30:12.561023 sentency-0.2.0/sentency/
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)      143 2023-05-07 12:52:13.000000 sentency-0.2.0/sentency/__init__.py
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)       22 2023-05-08 14:29:17.000000 sentency-0.2.0/sentency/_version.py
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)     1037 2023-05-07 12:52:13.000000 sentency-0.2.0/sentency/logs.py
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)     1355 2023-05-07 12:52:13.000000 sentency-0.2.0/sentency/regex.py
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)     8293 2023-05-08 14:16:28.000000 sentency-0.2.0/sentency/sentency.py
+drwxr-xr-x   0 gdelong   (1000) gdelong   (1000)        0 2023-05-08 14:30:12.561023 sentency-0.2.0/sentency.egg-info/
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)     3133 2023-05-08 14:30:12.000000 sentency-0.2.0/sentency.egg-info/PKG-INFO
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)      653 2023-05-08 14:30:12.000000 sentency-0.2.0/sentency.egg-info/SOURCES.txt
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)        1 2023-05-08 14:30:12.000000 sentency-0.2.0/sentency.egg-info/dependency_links.txt
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)        1 2023-05-08 14:30:12.000000 sentency-0.2.0/sentency.egg-info/not-zip-safe
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)        6 2023-05-08 14:30:12.000000 sentency-0.2.0/sentency.egg-info/requires.txt
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)        9 2023-05-08 14:30:12.000000 sentency-0.2.0/sentency.egg-info/top_level.txt
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)      177 2023-05-08 14:30:12.571023 sentency-0.2.0/setup.cfg
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)     1514 2023-05-07 12:52:13.000000 sentency-0.2.0/setup.py
+drwxr-xr-x   0 gdelong   (1000) gdelong   (1000)        0 2023-05-08 14:30:12.571023 sentency-0.2.0/tests/
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)       38 2023-05-07 12:52:13.000000 sentency-0.2.0/tests/__init__.py
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)      657 2023-05-07 12:52:13.000000 sentency-0.2.0/tests/config.py
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)     1233 2023-05-07 12:52:13.000000 sentency-0.2.0/tests/test_regex.py
+-rw-r--r--   0 gdelong   (1000) gdelong   (1000)     3967 2023-05-08 14:28:52.000000 sentency-0.2.0/tests/test_sentex.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sentency-0.1.6/CONTRIBUTING.rst` & `sentency-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sentency-0.1.6/LICENSE` & `sentency-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sentency-0.1.6/PKG-INFO` & `sentency-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentency
-Version: 0.1.6
+Version: 0.2.0
 Summary: A small lspaCy pipeline component for matching within document sentences using regular expressi
 Home-page: https://github.com/g-delong/sentency
 Author: Grant DeLong
 Author-email: gdelong1@geisinger.edu
 License: MIT license
 Keywords: sentency
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `sentency-0.1.6/README.rst` & `sentency-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `sentency-0.1.6/docs/Makefile` & `sentency-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sentency-0.1.6/docs/conf.py` & `sentency-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sentency-0.1.6/docs/installation.rst` & `sentency-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `sentency-0.1.6/docs/make.bat` & `sentency-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sentency-0.1.6/docs/sentency.rst` & `sentency-0.2.0/docs/sentency.rst`

 * *Files identical despite different names*

### Comparing `sentency-0.1.6/docs/usage.rst` & `sentency-0.2.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `sentency-0.1.6/sentency/logs.py` & `sentency-0.2.0/sentency/logs.py`

 * *Files identical despite different names*

### Comparing `sentency-0.1.6/sentency/regex.py` & `sentency-0.2.0/sentency/regex.py`

 * *Files identical despite different names*

### Comparing `sentency-0.1.6/sentency.egg-info/PKG-INFO` & `sentency-0.2.0/sentency.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentency
-Version: 0.1.6
+Version: 0.2.0
 Summary: A small lspaCy pipeline component for matching within document sentences using regular expressi
 Home-page: https://github.com/g-delong/sentency
 Author: Grant DeLong
 Author-email: gdelong1@geisinger.edu
 License: MIT license
 Keywords: sentency
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `sentency-0.1.6/setup.py` & `sentency-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `sentency-0.1.6/tests/config.py` & `sentency-0.2.0/tests/config.py`

 * *Files identical despite different names*

### Comparing `sentency-0.1.6/tests/test_regex.py` & `sentency-0.2.0/tests/test_regex.py`

 * *Files identical despite different names*

