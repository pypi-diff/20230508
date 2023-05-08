# Comparing `tmp/exalusAPI-0.5.2.tar.gz` & `tmp/exalusAPI-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exalusAPI-0.5.2.tar", last modified: Mon Apr 24 11:01:07 2023, max compression
+gzip compressed data, was "exalusAPI-0.6.1.tar", last modified: Mon May  8 06:54:18 2023, max compression
```

## Comparing `exalusAPI-0.5.2.tar` & `exalusAPI-0.6.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 11:01:07.476934 exalusAPI-0.5.2/
--rw-rw-rw-   0        0        0    11558 2022-10-21 05:28:52.000000 exalusAPI-0.5.2/LICENSE
--rw-rw-rw-   0        0        0    13973 2023-04-24 11:01:07.475807 exalusAPI-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      161 2023-03-16 07:02:58.000000 exalusAPI-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 11:01:07.464804 exalusAPI-0.5.2/exalusAPI.egg-info/
--rw-rw-rw-   0        0        0    13973 2023-04-24 11:01:07.000000 exalusAPI-0.5.2/exalusAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-24 11:01:07.000000 exalusAPI-0.5.2/exalusAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 11:01:07.000000 exalusAPI-0.5.2/exalusAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-24 11:01:07.000000 exalusAPI-0.5.2/exalusAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-24 11:01:07.000000 exalusAPI-0.5.2/exalusAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2023-04-24 11:00:58.000000 exalusAPI-0.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 11:01:07.477925 exalusAPI-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0      639 2023-04-24 11:00:45.000000 exalusAPI-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 11:01:07.470810 exalusAPI-0.5.2/src/
--rw-rw-rw-   0        0        0     6588 2023-04-24 06:27:01.000000 exalusAPI-0.5.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 06:54:18.892181 exalusAPI-0.6.1/
+-rw-rw-rw-   0        0        0    11558 2022-10-21 05:28:52.000000 exalusAPI-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0    13894 2023-05-08 06:54:18.891216 exalusAPI-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2023-03-16 07:02:58.000000 exalusAPI-0.6.1/README.md
+-rw-rw-rw-   0        0        0     1089 2023-05-08 06:53:17.000000 exalusAPI-0.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 06:54:18.893187 exalusAPI-0.6.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 06:54:18.870182 exalusAPI-0.6.1/src/
+-rw-rw-rw-   0        0        0     6588 2023-04-24 06:27:01.000000 exalusAPI-0.6.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 06:54:18.886214 exalusAPI-0.6.1/src/exalusAPI.egg-info/
+-rw-rw-rw-   0        0        0    13894 2023-05-08 06:54:18.000000 exalusAPI-0.6.1/src/exalusAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-05-08 06:54:18.000000 exalusAPI-0.6.1/src/exalusAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 06:54:18.000000 exalusAPI-0.6.1/src/exalusAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-08 06:54:18.000000 exalusAPI-0.6.1/src/exalusAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-08 06:54:18.000000 exalusAPI-0.6.1/src/exalusAPI.egg-info/top_level.txt
```

### Comparing `exalusAPI-0.5.2/LICENSE` & `exalusAPI-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exalusAPI-0.5.2/PKG-INFO` & `exalusAPI-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: exalusAPI
-Version: 0.5.2
+Version: 0.6.1
 Summary: Simple Exalus integration wrapper, created specifically for HomeAssistant integration.
-Home-page: https://github.com/marceljanicki/ExalusAPI
-Author: Marcel Janicki
 Author-email: Marcel Janicki <majanicki00@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `exalusAPI-0.5.2/exalusAPI.egg-info/PKG-INFO` & `exalusAPI-0.6.1/src/exalusAPI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: exalusAPI
-Version: 0.5.2
+Version: 0.6.1
 Summary: Simple Exalus integration wrapper, created specifically for HomeAssistant integration.
-Home-page: https://github.com/marceljanicki/ExalusAPI
-Author: Marcel Janicki
 Author-email: Marcel Janicki <majanicki00@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `exalusAPI-0.5.2/pyproject.toml` & `exalusAPI-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "exalusAPI"
-version = "0.5.2"
+version = "0.6.1"
 description = "Simple Exalus integration wrapper, created specifically for HomeAssistant integration."
 readme = "README.md"
 authors = [{ name = "Marcel Janicki", email = "majanicki00@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

### Comparing `exalusAPI-0.5.2/src/__init__.py` & `exalusAPI-0.6.1/src/__init__.py`

 * *Files identical despite different names*

