# Comparing `tmp/gcsaws-0.0.6.tar.gz` & `tmp/gcsaws-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcsaws-0.0.6.tar", last modified: Sun May  7 15:59:54 2023, max compression
+gzip compressed data, was "gcsaws-0.0.7.tar", last modified: Sun May  7 16:13:42 2023, max compression
```

## Comparing `gcsaws-0.0.6.tar` & `gcsaws-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 15:59:54.978002 gcsaws-0.0.6/
--rw-rw-rw-   0        0        0     1091 2023-05-07 12:57:03.000000 gcsaws-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      412 2023-05-07 15:59:54.978002 gcsaws-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0        8 2023-05-07 12:56:41.000000 gcsaws-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 15:59:54.962378 gcsaws-0.0.6/gcsaws/
--rw-rw-rw-   0        0        0      112 2023-05-07 12:59:09.000000 gcsaws-0.0.6/gcsaws/__init__.py
--rw-rw-rw-   0        0        0      684 2023-05-07 12:59:09.000000 gcsaws-0.0.6/gcsaws/helpers.py
--rw-rw-rw-   0        0        0     8669 2023-05-07 13:03:17.000000 gcsaws-0.0.6/gcsaws/nodes.py
--rw-rw-rw-   0        0        0     4037 2023-05-07 13:19:03.000000 gcsaws-0.0.6/gcsaws/visitor_procedure.py
-drwxrwxrwx   0        0        0        0 2023-05-07 15:59:54.978002 gcsaws-0.0.6/gcsaws.egg-info/
--rw-rw-rw-   0        0        0      412 2023-05-07 15:59:54.000000 gcsaws-0.0.6/gcsaws.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-05-07 15:59:54.000000 gcsaws-0.0.6/gcsaws.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 15:59:54.000000 gcsaws-0.0.6/gcsaws.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-07 15:59:54.000000 gcsaws-0.0.6/gcsaws.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-07 15:59:54.000000 gcsaws-0.0.6/gcsaws.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      662 2023-05-07 15:59:44.000000 gcsaws-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 15:59:54.978002 gcsaws-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-07 15:59:54.978002 gcsaws-0.0.6/tests/
--rw-rw-rw-   0        0        0      810 2023-05-07 11:28:19.000000 gcsaws-0.0.6/tests/test_create_target_list.py
--rw-rw-rw-   0        0        0     3258 2023-05-06 18:27:00.000000 gcsaws-0.0.6/tests/test_simple.py
+drwxrwxrwx   0        0        0        0 2023-05-07 16:13:42.556988 gcsaws-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-05-07 12:57:03.000000 gcsaws-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      412 2023-05-07 16:13:42.556988 gcsaws-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        8 2023-05-07 12:56:41.000000 gcsaws-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 16:13:42.541363 gcsaws-0.0.7/gcsaws/
+-rw-rw-rw-   0        0        0      112 2023-05-07 12:59:09.000000 gcsaws-0.0.7/gcsaws/__init__.py
+-rw-rw-rw-   0        0        0      684 2023-05-07 12:59:09.000000 gcsaws-0.0.7/gcsaws/helpers.py
+-rw-rw-rw-   0        0        0     8613 2023-05-07 16:13:11.000000 gcsaws-0.0.7/gcsaws/nodes.py
+-rw-rw-rw-   0        0        0     4037 2023-05-07 13:19:03.000000 gcsaws-0.0.7/gcsaws/visitor_procedure.py
+drwxrwxrwx   0        0        0        0 2023-05-07 16:13:42.541363 gcsaws-0.0.7/gcsaws.egg-info/
+-rw-rw-rw-   0        0        0      412 2023-05-07 16:13:42.000000 gcsaws-0.0.7/gcsaws.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-05-07 16:13:42.000000 gcsaws-0.0.7/gcsaws.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 16:13:42.000000 gcsaws-0.0.7/gcsaws.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-07 16:13:42.000000 gcsaws-0.0.7/gcsaws.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-07 16:13:42.000000 gcsaws-0.0.7/gcsaws.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      662 2023-05-07 16:13:26.000000 gcsaws-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 16:13:42.556988 gcsaws-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 16:13:42.556988 gcsaws-0.0.7/tests/
+-rw-rw-rw-   0        0        0      810 2023-05-07 11:28:19.000000 gcsaws-0.0.7/tests/test_create_target_list.py
+-rw-rw-rw-   0        0        0     3258 2023-05-06 18:27:00.000000 gcsaws-0.0.7/tests/test_simple.py
```

### Comparing `gcsaws-0.0.6/LICENSE` & `gcsaws-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gcsaws-0.0.6/gcsaws/helpers.py` & `gcsaws-0.0.7/gcsaws/helpers.py`

 * *Files identical despite different names*

### Comparing `gcsaws-0.0.6/gcsaws/nodes.py` & `gcsaws-0.0.7/gcsaws/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,23 +41,23 @@
         self.v_identifier = identifier_
         return self
 
 
 class HasScriptType:
     v_script_type: str = 'shell'
 
-    def shell(self: HasDocumentName) -> HasDocumentName:
+    def shell(self: T) -> T:
         """
         Makes the node run a shell script/command.
         :return: self
         """
         self.v_script_type = 'shell'
         return self
 
-    def powershell(self: HasDocumentName) -> HasDocumentName:
+    def powershell(self: T) -> T:
         """
         Make the node run a powershell script/command.
         :return: self
         """
         self.v_script_type = 'powershell'
         return self
```

### Comparing `gcsaws-0.0.6/gcsaws/visitor_procedure.py` & `gcsaws-0.0.7/gcsaws/visitor_procedure.py`

 * *Files identical despite different names*

### Comparing `gcsaws-0.0.6/pyproject.toml` & `gcsaws-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gcsaws"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name="Leikt", email="leikt.solreihin@gmail.com" },
 ]
 description = "GCS implementation for the aws-automation package."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `gcsaws-0.0.6/tests/test_create_target_list.py` & `gcsaws-0.0.7/tests/test_create_target_list.py`

 * *Files identical despite different names*

### Comparing `gcsaws-0.0.6/tests/test_simple.py` & `gcsaws-0.0.7/tests/test_simple.py`

 * *Files identical despite different names*

