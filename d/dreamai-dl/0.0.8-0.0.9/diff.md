# Comparing `tmp/dreamai_dl-0.0.8.tar.gz` & `tmp/dreamai_dl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai_dl-0.0.8.tar", last modified: Thu May  4 03:16:01 2023, max compression
+gzip compressed data, was "dreamai_dl-0.0.9.tar", last modified: Sat May  6 23:30:23 2023, max compression
```

## Comparing `dreamai_dl-0.0.8.tar` & `dreamai_dl-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 03:16:01.903475 dreamai_dl-0.0.8/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_dl-0.0.8/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_dl-0.0.8/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      919 2023-05-04 03:16:01.903475 dreamai_dl-0.0.8/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      136 2023-05-02 16:23:03.000000 dreamai_dl-0.0.8/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 03:16:01.903475 dreamai_dl-0.0.8/dreamai_dl/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-04 03:15:50.000000 dreamai_dl-0.0.8/dreamai_dl/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      708 2023-05-04 03:15:50.000000 dreamai_dl-0.0.8/dreamai_dl/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      165 2023-05-04 03:15:50.000000 dreamai_dl-0.0.8/dreamai_dl/core.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      690 2023-05-02 21:02:32.000000 dreamai_dl-0.0.8/dreamai_dl/imports.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      724 2023-05-04 03:15:50.000000 dreamai_dl-0.0.8/dreamai_dl/utils.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 03:16:01.903475 dreamai_dl-0.0.8/dreamai_dl.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      919 2023-05-04 03:16:01.000000 dreamai_dl-0.0.8/dreamai_dl.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      396 2023-05-04 03:16:01.000000 dreamai_dl-0.0.8/dreamai_dl.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-04 03:16:01.000000 dreamai_dl-0.0.8/dreamai_dl.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       42 2023-05-04 03:16:01.000000 dreamai_dl-0.0.8/dreamai_dl.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-01 22:18:59.000000 dreamai_dl-0.0.8/dreamai_dl.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       79 2023-05-04 03:16:01.000000 dreamai_dl-0.0.8/dreamai_dl.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       11 2023-05-04 03:16:01.000000 dreamai_dl-0.0.8/dreamai_dl.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      758 2023-05-04 03:04:21.000000 dreamai_dl-0.0.8/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-04 03:16:01.903475 dreamai_dl-0.0.8/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_dl-0.0.8/setup.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-06 23:30:23.081008 dreamai_dl-0.0.9/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_dl-0.0.9/LICENSE
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_dl-0.0.9/MANIFEST.in
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      919 2023-05-06 23:30:23.081008 dreamai_dl-0.0.9/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      136 2023-05-02 16:23:03.000000 dreamai_dl-0.0.9/README.md
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-06 23:30:23.081008 dreamai_dl-0.0.9/dreamai_dl/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-06 23:30:06.000000 dreamai_dl-0.0.9/dreamai_dl/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     7019 2023-05-06 23:30:06.000000 dreamai_dl-0.0.9/dreamai_dl/_modidx.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2433 2023-05-06 23:30:06.000000 dreamai_dl-0.0.9/dreamai_dl/core.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     9913 2023-05-06 23:30:06.000000 dreamai_dl-0.0.9/dreamai_dl/data.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     1099 2023-05-06 19:20:39.000000 dreamai_dl-0.0.9/dreamai_dl/imports.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     3774 2023-05-06 23:30:06.000000 dreamai_dl-0.0.9/dreamai_dl/utils.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-06 23:30:23.081008 dreamai_dl-0.0.9/dreamai_dl.egg-info/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      919 2023-05-06 23:30:23.000000 dreamai_dl-0.0.9/dreamai_dl.egg-info/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      415 2023-05-06 23:30:23.000000 dreamai_dl-0.0.9/dreamai_dl.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-06 23:30:23.000000 dreamai_dl-0.0.9/dreamai_dl.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       42 2023-05-06 23:30:23.000000 dreamai_dl-0.0.9/dreamai_dl.egg-info/entry_points.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-01 22:18:59.000000 dreamai_dl-0.0.9/dreamai_dl.egg-info/not-zip-safe
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       92 2023-05-06 23:30:23.000000 dreamai_dl-0.0.9/dreamai_dl.egg-info/requires.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       11 2023-05-06 23:30:23.000000 dreamai_dl-0.0.9/dreamai_dl.egg-info/top_level.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      771 2023-05-06 23:24:03.000000 dreamai_dl-0.0.9/settings.ini
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-06 23:30:23.081008 dreamai_dl-0.0.9/setup.cfg
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_dl-0.0.9/setup.py
```

### Comparing `dreamai_dl-0.0.8/LICENSE` & `dreamai_dl-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamai_dl-0.0.8/PKG-INFO` & `dreamai_dl-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai_dl
-Version: 0.0.8
+Version: 0.0.9
 Summary: Deep Learning tools based on dreamai.
 Home-page: https://github.com/HamzaFarhan/dreamai_dl
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_dl-0.0.8/dreamai_dl.egg-info/PKG-INFO` & `dreamai_dl-0.0.9/dreamai_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai-dl
-Version: 0.0.8
+Version: 0.0.9
 Summary: Deep Learning tools based on dreamai.
 Home-page: https://github.com/HamzaFarhan/dreamai_dl
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_dl-0.0.8/settings.ini` & `dreamai_dl-0.0.9/settings.ini`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dreamai_dl
 lib_name = %(repo)s
-version = 0.0.8
+version = 0.0.9
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = dreamai_dl
 nbs_path = nbs
 recursive = True
@@ -22,9 +22,9 @@
 author_email = thehamza96@gmail.com
 copyright = 2023 onwards, %(author)s
 description = Deep Learning tools based on dreamai.
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = HamzaFarhan
-pip_requirements = dreamai fastai lightning setuptools timm torch torchmetrics torchvision
+pip_requirements = dreamai fastai lightning scikit_learn setuptools timm torch torchmetrics torchvision
```

### Comparing `dreamai_dl-0.0.8/setup.py` & `dreamai_dl-0.0.9/setup.py`

 * *Files identical despite different names*

