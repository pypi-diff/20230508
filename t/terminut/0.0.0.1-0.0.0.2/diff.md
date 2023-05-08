# Comparing `tmp/terminut-0.0.0.1.tar.gz` & `tmp/terminut-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminut-0.0.0.1.tar", last modified: Mon May  8 01:36:48 2023, max compression
+gzip compressed data, was "terminut-0.0.0.2.tar", last modified: Mon May  8 01:45:28 2023, max compression
```

## Comparing `terminut-0.0.0.1.tar` & `terminut-0.0.0.2.tar`

### file list

```diff
@@ -1,10 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 01:36:48.504335 terminut-0.0.0.1/
--rw-rw-rw-   0        0        0      990 2023-05-08 01:36:48.503335 terminut-0.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-08 01:36:48.504335 terminut-0.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1301 2023-05-08 01:36:29.000000 terminut-0.0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:36:48.503335 terminut-0.0.0.1/terminut.egg-info/
--rw-rw-rw-   0        0        0      990 2023-05-08 01:36:48.000000 terminut-0.0.0.1/terminut.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-05-08 01:36:48.000000 terminut-0.0.0.1/terminut.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 01:36:48.000000 terminut-0.0.0.1/terminut.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-08 01:36:48.000000 terminut-0.0.0.1/terminut.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 01:36:48.000000 terminut-0.0.0.1/terminut.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 01:45:28.886674 terminut-0.0.0.2/
+-rw-rw-rw-   0        0        0      984 2023-05-08 01:45:28.886674 terminut-0.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-08 01:45:28.886674 terminut-0.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1298 2023-05-08 01:45:05.000000 terminut-0.0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:45:28.879946 terminut-0.0.0.2/terminut/
+-rw-rw-rw-   0        0        0      240 2023-05-08 01:43:34.000000 terminut-0.0.0.2/terminut/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-08 01:40:13.000000 terminut-0.0.0.2/terminut/console.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:45:28.886211 terminut-0.0.0.2/terminut.egg-info/
+-rw-rw-rw-   0        0        0      984 2023-05-08 01:45:28.000000 terminut-0.0.0.2/terminut.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-05-08 01:45:28.000000 terminut-0.0.0.2/terminut.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 01:45:28.000000 terminut-0.0.0.2/terminut.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-08 01:45:28.000000 terminut-0.0.0.2/terminut.egg-info/top_level.txt
```

### Comparing `terminut-0.0.0.1/PKG-INFO` & `terminut-0.0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: terminut
-Version: 0.0.0.1
-Summary: package sniper // vast#1337
+Version: 0.0.0.2
+Summary: Terminut // vast#1337
 Home-page: http://pypi.python.org/pypi/(terminut)
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `terminut-0.0.0.1/setup.py` & `terminut-0.0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
 projname = "terminut"
 
 setup(name=f"{projname}",
-      version="0.0.0.1",
-      description="package sniper // vast#1337",
+      version="0.0.0.2",
+      description="Terminut // vast#1337",
       packages=find_packages(exclude=['tests']),
       author="vast#1337",
       url=f"http://pypi.python.org/pypi/({projname})",
       author_email="vastcord@proton.me",
       license="MIT",
       classifiers=[
           "Development Status :: 3 - Alpha",
@@ -28,11 +28,11 @@
           "Topic :: Scientific/Engineering :: Visualization",
           "Topic :: Software Development :: Libraries",
           "Topic :: Utilities",
       ],
 
       python_requires="~=3.7",
 
-      install_requires=[
-          "config4py>=0.1.0"
-      ]
+      #install_requires=[
+      #    "config4py>=0.1.0"
+      #]
 )
```

### Comparing `terminut-0.0.0.1/terminut.egg-info/PKG-INFO` & `terminut-0.0.0.2/terminut.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: terminut
-Version: 0.0.0.1
-Summary: package sniper // vast#1337
+Version: 0.0.0.2
+Summary: Terminut // vast#1337
 Home-page: http://pypi.python.org/pypi/(terminut)
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

