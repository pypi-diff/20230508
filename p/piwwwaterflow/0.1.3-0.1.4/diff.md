# Comparing `tmp/piwwwaterflow-0.1.3.tar.gz` & `tmp/piwwwaterflow-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwwwaterflow-0.1.3.tar", last modified: Sun May  7 11:29:32 2023, max compression
+gzip compressed data, was "piwwwaterflow-0.1.4.tar", last modified: Mon May  8 07:10:28 2023, max compression
```

## Comparing `piwwwaterflow-0.1.3.tar` & `piwwwaterflow-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:29:32.963359 piwwwaterflow-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-07 11:29:32.963359 piwwwaterflow-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-07 11:29:19.000000 piwwwaterflow-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:29:32.959359 piwwwaterflow-0.1.3/piwwwaterflow/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-07 11:29:19.000000 piwwwaterflow-0.1.3/piwwwaterflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:29:32.959359 piwwwaterflow-0.1.3/piwwwaterflow/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 11:29:19.000000 piwwwaterflow-0.1.3/piwwwaterflow/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:29:32.963359 piwwwaterflow-0.1.3/piwwwaterflow/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 11:29:19.000000 piwwwaterflow-0.1.3/piwwwaterflow/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-07 11:29:19.000000 piwwwaterflow-0.1.3/piwwwaterflow/webservice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-07 11:29:19.000000 piwwwaterflow-0.1.3/piwwwaterflow/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:29:32.959359 piwwwaterflow-0.1.3/piwwwaterflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-07 11:29:32.000000 piwwwaterflow-0.1.3/piwwwaterflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-07 11:29:32.000000 piwwwaterflow-0.1.3/piwwwaterflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 11:29:32.000000 piwwwaterflow-0.1.3/piwwwaterflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-07 11:29:32.000000 piwwwaterflow-0.1.3/piwwwaterflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 11:29:32.000000 piwwwaterflow-0.1.3/piwwwaterflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 11:29:32.963359 piwwwaterflow-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-07 11:29:19.000000 piwwwaterflow-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:29:32.963359 piwwwaterflow-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 11:29:19.000000 piwwwaterflow-0.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:28.389373 piwwwaterflow-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-08 07:10:28.389373 piwwwaterflow-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:28.385373 piwwwaterflow-0.1.4/piwwwaterflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:28.385373 piwwwaterflow-0.1.4/piwwwaterflow/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:28.385373 piwwwaterflow-0.1.4/piwwwaterflow/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/css/iepngfix.htc
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/css/view.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:28.385373 piwwwaterflow-0.1.4/piwwwaterflow/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/img/blank.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/img/bottom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33683 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/img/icon-256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/img/icon-32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/img/piwaterflow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/img/play.png
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/img/shadow.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/img/top.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:28.385373 piwwwaterflow-0.1.4/piwwwaterflow/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/static/js/code.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:28.389373 piwwwaterflow-0.1.4/piwwwaterflow/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/webservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/piwwwaterflow/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:28.385373 piwwwaterflow-0.1.4/piwwwaterflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-08 07:10:28.000000 piwwwaterflow-0.1.4/piwwwaterflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-08 07:10:28.000000 piwwwaterflow-0.1.4/piwwwaterflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 07:10:28.000000 piwwwaterflow-0.1.4/piwwwaterflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-08 07:10:28.000000 piwwwaterflow-0.1.4/piwwwaterflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-08 07:10:28.000000 piwwwaterflow-0.1.4/piwwwaterflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 07:10:28.389373 piwwwaterflow-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:28.389373 piwwwaterflow-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:16.000000 piwwwaterflow-0.1.4/tests/__init__.py
```

### Comparing `piwwwaterflow-0.1.3/PKG-INFO` & `piwwwaterflow-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwwwaterflow
-Version: 0.1.3
+Version: 0.1.4
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwwwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # piwwwaterflow
         Flask/Gunicorn Webservice for piwaterflow system
```

### Comparing `piwwwaterflow-0.1.3/piwwwaterflow/webservice.py` & `piwwwaterflow-0.1.4/piwwwaterflow/webservice.py`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.3/piwwwaterflow/wsgi.py` & `piwwwaterflow-0.1.4/piwwwaterflow/wsgi.py`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.3/piwwwaterflow.egg-info/PKG-INFO` & `piwwwaterflow-0.1.4/piwwwaterflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwwwaterflow
-Version: 0.1.3
+Version: 0.1.4
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwwwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # piwwwaterflow
         Flask/Gunicorn Webservice for piwaterflow system
```

### Comparing `piwwwaterflow-0.1.3/setup.py` & `piwwwaterflow-0.1.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,28 +2,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="piwwwaterflow",
-    version="0.1.3",
+    version="0.1.4",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Waterflow resilient system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/piwwwaterflow",
     packages=setuptools.find_packages(),
-    package_data={
-        'static.css': ['*.css'],
-        'static.img': ['*.*'],
-        'static.js': ['*.js'],
-        'templates': ['*.html'],
-    },
+    include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Home Automation",
     ],
     install_requires=[
```

