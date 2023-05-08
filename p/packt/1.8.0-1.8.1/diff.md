# Comparing `tmp/packt-1.8.0.tar.gz` & `tmp/packt-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packt-1.8.0.tar", last modified: Wed Jan  4 16:30:31 2023, max compression
+gzip compressed data, was "packt-1.8.1.tar", last modified: Mon May  8 15:41:46 2023, max compression
```

## Comparing `packt-1.8.0.tar` & `packt-1.8.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 16:30:31.551296 packt-1.8.0/
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-01-04 16:30:20.000000 packt-1.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6773 2023-01-04 16:30:31.551296 packt-1.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6283 2023-01-04 16:30:20.000000 packt-1.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 16:30:31.547295 packt-1.8.0/packt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 16:30:20.000000 packt-1.8.0/packt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2567 2023-01-04 16:30:20.000000 packt-1.8.0/packt/api.py
--rw-rw-rw-   0 root         (0) root         (0)     2473 2023-01-04 16:30:20.000000 packt-1.8.0/packt/claimer.py
--rw-rw-rw-   0 root         (0) root         (0)     1373 2023-01-04 16:30:20.000000 packt-1.8.0/packt/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-01-04 16:30:20.000000 packt-1.8.0/packt/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     6755 2023-01-04 16:30:20.000000 packt-1.8.0/packt/downloader.py
--rw-rw-rw-   0 root         (0) root         (0)     6246 2023-01-04 16:30:20.000000 packt-1.8.0/packt/packtPublishingFreeEbook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 16:30:31.551296 packt-1.8.0/packt/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 16:30:20.000000 packt-1.8.0/packt/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2626 2023-01-04 16:30:20.000000 packt-1.8.0/packt/utils/anticaptcha.py
--rw-rw-rw-   0 root         (0) root         (0)     8211 2023-01-04 16:30:20.000000 packt-1.8.0/packt/utils/google_drive.py
--rw-rw-rw-   0 root         (0) root         (0)     3518 2023-01-04 16:30:20.000000 packt-1.8.0/packt/utils/mail.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 16:30:31.550296 packt-1.8.0/packt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6773 2023-01-04 16:30:31.000000 packt-1.8.0/packt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      455 2023-01-04 16:30:31.000000 packt-1.8.0/packt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-04 16:30:31.000000 packt-1.8.0/packt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-01-04 16:30:31.000000 packt-1.8.0/packt.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      194 2023-01-04 16:30:31.000000 packt-1.8.0/packt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-01-04 16:30:31.000000 packt-1.8.0/packt.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-01-04 16:30:31.552296 packt-1.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1483 2023-01-04 16:30:20.000000 packt-1.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 15:41:46.915501 packt-1.8.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-05-08 15:41:35.000000 packt-1.8.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6723 2023-05-08 15:41:46.916503 packt-1.8.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6283 2023-05-08 15:41:35.000000 packt-1.8.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 15:41:46.911495 packt-1.8.1/packt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 15:41:35.000000 packt-1.8.1/packt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2567 2023-05-08 15:41:35.000000 packt-1.8.1/packt/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2473 2023-05-08 15:41:35.000000 packt-1.8.1/packt/claimer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1373 2023-05-08 15:41:35.000000 packt-1.8.1/packt/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-05-08 15:41:35.000000 packt-1.8.1/packt/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     6755 2023-05-08 15:41:35.000000 packt-1.8.1/packt/downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     6246 2023-05-08 15:41:35.000000 packt-1.8.1/packt/packtPublishingFreeEbook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 15:41:46.915501 packt-1.8.1/packt/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 15:41:35.000000 packt-1.8.1/packt/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2626 2023-05-08 15:41:35.000000 packt-1.8.1/packt/utils/anticaptcha.py
+-rw-rw-rw-   0 root         (0) root         (0)     8211 2023-05-08 15:41:35.000000 packt-1.8.1/packt/utils/google_drive.py
+-rw-rw-rw-   0 root         (0) root         (0)     3518 2023-05-08 15:41:35.000000 packt-1.8.1/packt/utils/mail.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 15:41:46.914500 packt-1.8.1/packt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6723 2023-05-08 15:41:46.000000 packt-1.8.1/packt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-08 15:41:46.000000 packt-1.8.1/packt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 15:41:46.000000 packt-1.8.1/packt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-08 15:41:46.000000 packt-1.8.1/packt.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      194 2023-05-08 15:41:46.000000 packt-1.8.1/packt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-08 15:41:46.000000 packt-1.8.1/packt.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-05-08 15:41:46.916503 packt-1.8.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1434 2023-05-08 15:41:35.000000 packt-1.8.1/setup.py
```

### Comparing `packt-1.8.0/LICENSE` & `packt-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `packt-1.8.0/PKG-INFO` & `packt-1.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: packt
-Version: 1.8.0
+Version: 1.8.1
 Summary: Script for grabbing daily Packt Free Learning ebooks
 Home-page: https://gitlab.com/packt-cli/packt-cli
-Download-URL: https://gitlab.com/packt-cli/packt-cli/-/archive/v1.8.0/packt-cli-v1.8.0.tar.gz
+Download-URL: https://gitlab.com/packt-cli/packt-cli/-/archive/v1.8.1/packt-cli-v1.8.1.tar.gz
 Author: Łukasz Uszko
 Author-email: lukasz.uszko@gmail.com
 License: MIT
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `packt-1.8.0/README.md` & `packt-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `packt-1.8.0/packt/api.py` & `packt-1.8.1/packt/api.py`

 * *Files identical despite different names*

### Comparing `packt-1.8.0/packt/claimer.py` & `packt-1.8.1/packt/claimer.py`

 * *Files identical despite different names*

### Comparing `packt-1.8.0/packt/configuration.py` & `packt-1.8.1/packt/configuration.py`

 * *Files identical despite different names*

### Comparing `packt-1.8.0/packt/constants.py` & `packt-1.8.1/packt/constants.py`

 * *Files identical despite different names*

### Comparing `packt-1.8.0/packt/downloader.py` & `packt-1.8.1/packt/downloader.py`

 * *Files identical despite different names*

### Comparing `packt-1.8.0/packt/packtPublishingFreeEbook.py` & `packt-1.8.1/packt/packtPublishingFreeEbook.py`

 * *Files identical despite different names*

### Comparing `packt-1.8.0/packt/utils/anticaptcha.py` & `packt-1.8.1/packt/utils/anticaptcha.py`

 * *Files identical despite different names*

### Comparing `packt-1.8.0/packt/utils/google_drive.py` & `packt-1.8.1/packt/utils/google_drive.py`

 * *Files identical despite different names*

### Comparing `packt-1.8.0/packt/utils/mail.py` & `packt-1.8.1/packt/utils/mail.py`

 * *Files identical despite different names*

### Comparing `packt-1.8.0/packt.egg-info/PKG-INFO` & `packt-1.8.1/packt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: packt
-Version: 1.8.0
+Version: 1.8.1
 Summary: Script for grabbing daily Packt Free Learning ebooks
 Home-page: https://gitlab.com/packt-cli/packt-cli
-Download-URL: https://gitlab.com/packt-cli/packt-cli/-/archive/v1.8.0/packt-cli-v1.8.0.tar.gz
+Download-URL: https://gitlab.com/packt-cli/packt-cli/-/archive/v1.8.1/packt-cli-v1.8.1.tar.gz
 Author: Łukasz Uszko
 Author-email: lukasz.uszko@gmail.com
 License: MIT
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `packt-1.8.0/setup.py` & `packt-1.8.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from setuptools import find_packages, setup
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as f:
     long_description = f.read()
 
-package_version = '1.8.0'
+package_version = '1.8.1'
 
 requirements = [
     'click==8.1.3',
     'google-api-python-client==2.57.0',
     'oauth2client==4.1.3',
     'requests==2.28.1',
     'python-slugify==6.1.2'
@@ -37,16 +37,15 @@
     install_requires=requirements,
     extras_require={'dev': dev_requirements},
     entry_points={
         'console_scripts': [
             'packt-cli = packt.packtPublishingFreeEbook:packt_cli',
         ],
     },
-    download_url='https://gitlab.com/packt-cli/packt-cli/-/archive/v1.8.0/packt-cli-v1.8.0.tar.gz',
+    download_url='https://gitlab.com/packt-cli/packt-cli/-/archive/v1.8.1/packt-cli-v1.8.1.tar.gz',
     classifiers=[
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11'
     ]
 )
```

