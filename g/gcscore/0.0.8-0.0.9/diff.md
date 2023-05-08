# Comparing `tmp/gcscore-0.0.8.tar.gz` & `tmp/gcscore-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcscore-0.0.8.tar", last modified: Mon May  8 06:54:25 2023, max compression
+gzip compressed data, was "gcscore-0.0.9.tar", last modified: Mon May  8 06:55:34 2023, max compression
```

## Comparing `gcscore-0.0.8.tar` & `gcscore-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 06:54:25.585071 gcscore-0.0.8/
--rw-rw-rw-   0        0        0     1091 2023-05-07 13:08:51.000000 gcscore-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      665 2023-05-08 06:54:25.585071 gcscore-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-05-07 13:11:19.000000 gcscore-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 06:54:25.563888 gcscore-0.0.8/gcscore/
--rw-rw-rw-   0        0        0      111 2023-05-07 13:08:51.000000 gcscore-0.0.8/gcscore/__init__.py
--rw-rw-rw-   0        0        0     6671 2023-05-07 13:08:51.000000 gcscore-0.0.8/gcscore/_command_renderer.py
--rw-rw-rw-   0        0        0       97 2023-05-07 13:08:50.000000 gcscore-0.0.8/gcscore/_commons.py
--rw-rw-rw-   0        0        0     1453 2023-05-07 13:08:51.000000 gcscore-0.0.8/gcscore/_error_history.py
--rw-rw-rw-   0        0        0     2780 2023-05-07 13:08:51.000000 gcscore-0.0.8/gcscore/_j2ext.py
-drwxrwxrwx   0        0        0        0 2023-05-08 06:54:25.584072 gcscore-0.0.8/gcscore/mod/
--rw-rw-rw-   0        0        0       97 2023-05-07 13:08:51.000000 gcscore-0.0.8/gcscore/mod/__init__.py
--rw-rw-rw-   0        0        0     2490 2023-05-08 06:52:06.000000 gcscore-0.0.8/gcscore/mod/_base.py
--rw-rw-rw-   0        0        0     2092 2023-05-07 13:08:51.000000 gcscore-0.0.8/gcscore/mod/_context.py
--rw-rw-rw-   0        0        0     2941 2023-05-07 13:08:51.000000 gcscore-0.0.8/gcscore/mod/_helpers.py
--rw-rw-rw-   0        0        0     2316 2023-05-07 13:08:51.000000 gcscore-0.0.8/gcscore/mod/_visitor.py
-drwxrwxrwx   0        0        0        0 2023-05-08 06:54:25.575979 gcscore-0.0.8/gcscore.egg-info/
--rw-rw-rw-   0        0        0      665 2023-05-08 06:54:25.000000 gcscore-0.0.8/gcscore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-05-08 06:54:25.000000 gcscore-0.0.8/gcscore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 06:54:25.000000 gcscore-0.0.8/gcscore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-08 06:54:25.000000 gcscore-0.0.8/gcscore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-08 06:54:25.000000 gcscore-0.0.8/gcscore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      736 2023-05-08 06:52:24.000000 gcscore-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 06:54:25.585071 gcscore-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 06:55:34.863994 gcscore-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-05-07 13:08:51.000000 gcscore-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      665 2023-05-08 06:55:34.863994 gcscore-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-07 13:11:19.000000 gcscore-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 06:55:34.842789 gcscore-0.0.9/gcscore/
+-rw-rw-rw-   0        0        0      111 2023-05-07 13:08:51.000000 gcscore-0.0.9/gcscore/__init__.py
+-rw-rw-rw-   0        0        0     6671 2023-05-07 13:08:51.000000 gcscore-0.0.9/gcscore/_command_renderer.py
+-rw-rw-rw-   0        0        0       97 2023-05-07 13:08:50.000000 gcscore-0.0.9/gcscore/_commons.py
+-rw-rw-rw-   0        0        0     1453 2023-05-07 13:08:51.000000 gcscore-0.0.9/gcscore/_error_history.py
+-rw-rw-rw-   0        0        0     2780 2023-05-07 13:08:51.000000 gcscore-0.0.9/gcscore/_j2ext.py
+drwxrwxrwx   0        0        0        0 2023-05-08 06:55:34.862996 gcscore-0.0.9/gcscore/mod/
+-rw-rw-rw-   0        0        0       97 2023-05-07 13:08:51.000000 gcscore-0.0.9/gcscore/mod/__init__.py
+-rw-rw-rw-   0        0        0     2495 2023-05-08 06:55:16.000000 gcscore-0.0.9/gcscore/mod/_base.py
+-rw-rw-rw-   0        0        0     2092 2023-05-07 13:08:51.000000 gcscore-0.0.9/gcscore/mod/_context.py
+-rw-rw-rw-   0        0        0     2941 2023-05-07 13:08:51.000000 gcscore-0.0.9/gcscore/mod/_helpers.py
+-rw-rw-rw-   0        0        0     2316 2023-05-07 13:08:51.000000 gcscore-0.0.9/gcscore/mod/_visitor.py
+drwxrwxrwx   0        0        0        0 2023-05-08 06:55:34.854909 gcscore-0.0.9/gcscore.egg-info/
+-rw-rw-rw-   0        0        0      665 2023-05-08 06:55:34.000000 gcscore-0.0.9/gcscore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-05-08 06:55:34.000000 gcscore-0.0.9/gcscore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 06:55:34.000000 gcscore-0.0.9/gcscore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-08 06:55:34.000000 gcscore-0.0.9/gcscore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-08 06:55:34.000000 gcscore-0.0.9/gcscore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      736 2023-05-08 06:55:25.000000 gcscore-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 06:55:34.863994 gcscore-0.0.9/setup.cfg
```

### Comparing `gcscore-0.0.8/LICENSE` & `gcscore-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gcscore-0.0.8/PKG-INFO` & `gcscore-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcscore
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generic Command System, a tool to help the creation of custom procedures.
 Author-email: Leikt <leikt.solreihin@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `gcscore-0.0.8/gcscore/_command_renderer.py` & `gcscore-0.0.9/gcscore/_command_renderer.py`

 * *Files identical despite different names*

### Comparing `gcscore-0.0.8/gcscore/_error_history.py` & `gcscore-0.0.9/gcscore/_error_history.py`

 * *Files identical despite different names*

### Comparing `gcscore-0.0.8/gcscore/_j2ext.py` & `gcscore-0.0.9/gcscore/_j2ext.py`

 * *Files identical despite different names*

### Comparing `gcscore-0.0.8/gcscore/mod/_base.py` & `gcscore-0.0.9/gcscore/mod/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,10 +82,10 @@
     """
     Create and add a child to the given parent node.
     :param parent: the parent node
     :param klass: the class of the child node
     :param name: name of the child node
     :return: the child node
     """
-    child = klass(name)
+    child = klass(name=name)
     parent.gcscore_children.append(child)
     return child
```

### Comparing `gcscore-0.0.8/gcscore/mod/_context.py` & `gcscore-0.0.9/gcscore/mod/_context.py`

 * *Files identical despite different names*

### Comparing `gcscore-0.0.8/gcscore/mod/_helpers.py` & `gcscore-0.0.9/gcscore/mod/_helpers.py`

 * *Files identical despite different names*

### Comparing `gcscore-0.0.8/gcscore/mod/_visitor.py` & `gcscore-0.0.9/gcscore/mod/_visitor.py`

 * *Files identical despite different names*

### Comparing `gcscore-0.0.8/gcscore.egg-info/PKG-INFO` & `gcscore-0.0.9/gcscore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcscore
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generic Command System, a tool to help the creation of custom procedures.
 Author-email: Leikt <leikt.solreihin@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `gcscore-0.0.8/pyproject.toml` & `gcscore-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gcscore"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name="Leikt", email="leikt.solreihin@gmail.com" },
 ]
 description = "Generic Command System, a tool to help the creation of custom procedures."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

