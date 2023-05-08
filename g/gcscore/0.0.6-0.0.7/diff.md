# Comparing `tmp/gcscore-0.0.6.tar.gz` & `tmp/gcscore-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcscore-0.0.6.tar", last modified: Sun May  7 15:58:24 2023, max compression
+gzip compressed data, was "gcscore-0.0.7.tar", last modified: Mon May  8 06:47:42 2023, max compression
```

## Comparing `gcscore-0.0.6.tar` & `gcscore-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 15:58:24.683235 gcscore-0.0.6/
--rw-rw-rw-   0        0        0     1091 2023-05-07 13:08:51.000000 gcscore-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      665 2023-05-07 15:58:24.683235 gcscore-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-05-07 13:11:19.000000 gcscore-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 15:58:24.667611 gcscore-0.0.6/gcscore/
--rw-rw-rw-   0        0        0      111 2023-05-07 13:08:51.000000 gcscore-0.0.6/gcscore/__init__.py
--rw-rw-rw-   0        0        0     6671 2023-05-07 13:08:51.000000 gcscore-0.0.6/gcscore/_command_renderer.py
--rw-rw-rw-   0        0        0       97 2023-05-07 13:08:50.000000 gcscore-0.0.6/gcscore/_commons.py
--rw-rw-rw-   0        0        0     1453 2023-05-07 13:08:51.000000 gcscore-0.0.6/gcscore/_error_history.py
--rw-rw-rw-   0        0        0     2780 2023-05-07 13:08:51.000000 gcscore-0.0.6/gcscore/_j2ext.py
-drwxrwxrwx   0        0        0        0 2023-05-07 15:58:24.683235 gcscore-0.0.6/gcscore/mod/
--rw-rw-rw-   0        0        0       97 2023-05-07 13:08:51.000000 gcscore-0.0.6/gcscore/mod/__init__.py
--rw-rw-rw-   0        0        0     1356 2023-05-07 13:08:51.000000 gcscore-0.0.6/gcscore/mod/_base.py
--rw-rw-rw-   0        0        0     2092 2023-05-07 13:08:51.000000 gcscore-0.0.6/gcscore/mod/_context.py
--rw-rw-rw-   0        0        0     2941 2023-05-07 13:08:51.000000 gcscore-0.0.6/gcscore/mod/_helpers.py
--rw-rw-rw-   0        0        0     2316 2023-05-07 13:08:51.000000 gcscore-0.0.6/gcscore/mod/_visitor.py
-drwxrwxrwx   0        0        0        0 2023-05-07 15:58:24.683235 gcscore-0.0.6/gcscore.egg-info/
--rw-rw-rw-   0        0        0      665 2023-05-07 15:58:24.000000 gcscore-0.0.6/gcscore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-05-07 15:58:24.000000 gcscore-0.0.6/gcscore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 15:58:24.000000 gcscore-0.0.6/gcscore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-07 15:58:24.000000 gcscore-0.0.6/gcscore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-07 15:58:24.000000 gcscore-0.0.6/gcscore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      736 2023-05-07 15:57:23.000000 gcscore-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 15:58:24.683235 gcscore-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 06:47:42.449477 gcscore-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-05-07 13:08:51.000000 gcscore-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      665 2023-05-08 06:47:42.448478 gcscore-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-07 13:11:19.000000 gcscore-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 06:47:42.400540 gcscore-0.0.7/gcscore/
+-rw-rw-rw-   0        0        0      111 2023-05-07 13:08:51.000000 gcscore-0.0.7/gcscore/__init__.py
+-rw-rw-rw-   0        0        0     6671 2023-05-07 13:08:51.000000 gcscore-0.0.7/gcscore/_command_renderer.py
+-rw-rw-rw-   0        0        0       97 2023-05-07 13:08:50.000000 gcscore-0.0.7/gcscore/_commons.py
+-rw-rw-rw-   0        0        0     1453 2023-05-07 13:08:51.000000 gcscore-0.0.7/gcscore/_error_history.py
+-rw-rw-rw-   0        0        0     2780 2023-05-07 13:08:51.000000 gcscore-0.0.7/gcscore/_j2ext.py
+drwxrwxrwx   0        0        0        0 2023-05-08 06:47:42.447476 gcscore-0.0.7/gcscore/mod/
+-rw-rw-rw-   0        0        0       97 2023-05-07 13:08:51.000000 gcscore-0.0.7/gcscore/mod/__init__.py
+-rw-rw-rw-   0        0        0     2490 2023-05-08 06:47:13.000000 gcscore-0.0.7/gcscore/mod/_base.py
+-rw-rw-rw-   0        0        0     2092 2023-05-07 13:08:51.000000 gcscore-0.0.7/gcscore/mod/_context.py
+-rw-rw-rw-   0        0        0     2941 2023-05-07 13:08:51.000000 gcscore-0.0.7/gcscore/mod/_helpers.py
+-rw-rw-rw-   0        0        0     2316 2023-05-07 13:08:51.000000 gcscore-0.0.7/gcscore/mod/_visitor.py
+drwxrwxrwx   0        0        0        0 2023-05-08 06:47:42.415192 gcscore-0.0.7/gcscore.egg-info/
+-rw-rw-rw-   0        0        0      665 2023-05-08 06:47:42.000000 gcscore-0.0.7/gcscore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-05-08 06:47:42.000000 gcscore-0.0.7/gcscore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 06:47:42.000000 gcscore-0.0.7/gcscore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-08 06:47:42.000000 gcscore-0.0.7/gcscore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-08 06:47:42.000000 gcscore-0.0.7/gcscore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      736 2023-05-08 06:47:13.000000 gcscore-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 06:47:42.449477 gcscore-0.0.7/setup.cfg
```

### Comparing `gcscore-0.0.6/LICENSE` & `gcscore-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gcscore-0.0.6/PKG-INFO` & `gcscore-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcscore
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generic Command System, a tool to help the creation of custom procedures.
 Author-email: Leikt <leikt.solreihin@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `gcscore-0.0.6/gcscore/_command_renderer.py` & `gcscore-0.0.7/gcscore/_command_renderer.py`

 * *Files identical despite different names*

### Comparing `gcscore-0.0.6/gcscore/_error_history.py` & `gcscore-0.0.7/gcscore/_error_history.py`

 * *Files identical despite different names*

### Comparing `gcscore-0.0.6/gcscore/_j2ext.py` & `gcscore-0.0.7/gcscore/_j2ext.py`

 * *Files identical despite different names*

### Comparing `gcscore-0.0.6/gcscore/mod/_context.py` & `gcscore-0.0.7/gcscore/mod/_context.py`

 * *Files identical despite different names*

### Comparing `gcscore-0.0.6/gcscore/mod/_helpers.py` & `gcscore-0.0.7/gcscore/mod/_helpers.py`

 * *Files identical despite different names*

### Comparing `gcscore-0.0.6/gcscore/mod/_visitor.py` & `gcscore-0.0.7/gcscore/mod/_visitor.py`

 * *Files identical despite different names*

### Comparing `gcscore-0.0.6/gcscore.egg-info/PKG-INFO` & `gcscore-0.0.7/gcscore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcscore
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generic Command System, a tool to help the creation of custom procedures.
 Author-email: Leikt <leikt.solreihin@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `gcscore-0.0.6/pyproject.toml` & `gcscore-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gcscore"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name="Leikt", email="leikt.solreihin@gmail.com" },
 ]
 description = "Generic Command System, a tool to help the creation of custom procedures."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

