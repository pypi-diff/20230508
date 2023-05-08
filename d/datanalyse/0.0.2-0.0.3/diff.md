# Comparing `tmp/datanalyse-0.0.2.tar.gz` & `tmp/datanalyse-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datanalyse-0.0.2.tar", last modified: Sat May  6 20:46:07 2023, max compression
+gzip compressed data, was "datanalyse-0.0.3.tar", last modified: Mon May  8 20:02:59 2023, max compression
```

## Comparing `datanalyse-0.0.2.tar` & `datanalyse-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,17 @@
--rw-r--r--   0        0        0     1078 2023-05-06 19:06:32.333418 datanalyse-0.0.2/LICENSE
--rw-r--r--   0        0        0      459 2023-05-06 20:17:48.271205 datanalyse-0.0.2/README.md
--rw-r--r--   0        0        0      609 2023-05-06 20:46:07.702109 datanalyse-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       51 2023-05-06 20:41:01.003922 datanalyse-0.0.2/src/datanalyse/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 12:49:40.254042 datanalyse-0.0.2/src/datanalyse/dataelement/__init__.py
--rw-r--r--   0        0        0     8724 2023-05-06 19:27:23.414206 datanalyse-0.0.2/src/datanalyse/dataelement/dataelement.py
--rw-r--r--   0        0        0      703 2023-04-28 12:58:07.459695 datanalyse-0.0.2/src/datanalyse/pfade.py
--rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 datanalyse-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-06 19:06:32.333418 datanalyse-0.0.3/LICENSE
+-rw-r--r--   0        0        0      459 2023-05-06 20:17:48.271205 datanalyse-0.0.3/README.md
+-rw-r--r--   0        0        0      685 2023-05-08 20:02:59.044623 datanalyse-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-08 18:40:19.058776 datanalyse-0.0.3/src/datanalyse/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 12:49:40.254042 datanalyse-0.0.3/src/datanalyse/dataelement/__init__.py
+-rw-r--r--   0        0        0     8724 2023-05-06 19:27:23.414206 datanalyse-0.0.3/src/datanalyse/dataelement/dataelement.py
+-rw-r--r--   0        0        0     3492 2023-05-08 19:59:39.673710 datanalyse-0.0.3/src/datanalyse/dataelement/dfmanipulation.py
+-rw-r--r--   0        0        0    32076 2023-05-08 19:59:42.082985 datanalyse-0.0.3/src/datanalyse/dataelement/formate.py
+-rw-r--r--   0        0        0      362 2023-05-08 19:59:45.459719 datanalyse-0.0.3/src/datanalyse/dataelement/stoffwerte.py
+-rw-r--r--   0        0        0        0 2023-05-08 18:40:19.069280 datanalyse-0.0.3/src/datanalyse/diagramme/__init__.py
+-rw-r--r--   0        0        0     4746 2023-05-08 19:59:07.147860 datanalyse-0.0.3/src/datanalyse/diagramme/balken.py
+-rw-r--r--   0        0        0     2863 2023-05-08 19:59:19.452792 datanalyse-0.0.3/src/datanalyse/diagramme/diagramm.py
+-rw-r--r--   0        0        0     4224 2023-05-08 19:59:23.694912 datanalyse-0.0.3/src/datanalyse/diagramme/globalbewertung.py
+-rw-r--r--   0        0        0     1102 2023-05-08 19:59:25.417764 datanalyse-0.0.3/src/datanalyse/diagramme/matplotlib_parameter.py
+-rw-r--r--   0        0        0     3110 2023-05-08 19:59:27.717897 datanalyse-0.0.3/src/datanalyse/diagramme/zeitreihe.py
+-rw-r--r--   0        0        0      703 2023-04-28 12:58:07.459695 datanalyse-0.0.3/src/datanalyse/pfade.py
+-rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 datanalyse-0.0.3/PKG-INFO
```

### Comparing `datanalyse-0.0.2/LICENSE` & `datanalyse-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.2/pyproject.toml` & `datanalyse-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-[build-system]
-requires = [
-    "pdm-backend",
-    "pandas",
-]
-build-backend = "pdm.backend"
-
 [project]
 name = "datanalyse"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "Maximilian Beyer", email = "maximilian.beyer@tu-dresden.de" },
 ]
 description = "A data analysis package."
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "pandas>=2.0.1",
+    "matplotlib>=3.7.1",
+    "black>=23.3.0",
+]
 
 [project.urls]
 Homepage = "https://github.com/MakusuB/datanalyse"
 "Bug Tracker" = "https://github.com/MakusuB/datanalyse/issues"
 
-[tool]
+[build-system]
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
+
+[tool.pdm]
```

### Comparing `datanalyse-0.0.2/src/datanalyse/dataelement/dataelement.py` & `datanalyse-0.0.3/src/datanalyse/dataelement/dataelement.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.2/src/datanalyse/pfade.py` & `datanalyse-0.0.3/src/datanalyse/pfade.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.2/PKG-INFO` & `datanalyse-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: datanalyse
-Version: 0.0.2
+Version: 0.0.3
 Summary: A data analysis package.
 Author-Email: Maximilian Beyer <maximilian.beyer@tu-dresden.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/MakusuB/datanalyse
 Project-URL: Bug tracker, https://github.com/MakusuB/datanalyse/issues
-Requires-Python: >=3.10
+Requires-Python: >=3.11
+Requires-Dist: pandas>=2.0.1
+Requires-Dist: matplotlib>=3.7.1
+Requires-Dist: black>=23.3.0
 Description-Content-Type: text/markdown
 
 # datanalyse
 
 The package name datanalyse is a suitcase word for data and analyse - mainly of experimental data from the Combined Energy Lab at TU Dresden, but perhaps useful for others as well. However, due to its absolute alpha status, I cannot recommend it to anybody in the world but me.
 
 It is more or less a tool-kit for my daily work as an experimentalist and data scientist and makes use of the fantastic packages pandas, pathlib and matplotlib.
```

