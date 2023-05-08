# Comparing `tmp/rdfizer-4.7.dev1682603874.tar.gz` & `tmp/rdfizer-4.7.dev1682603926.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfizer-4.7.dev1682603874.tar", last modified: Thu Apr 27 13:57:54 2023, max compression
+gzip compressed data, was "rdfizer-4.7.dev1682603926.tar", last modified: Thu Apr 27 13:58:46 2023, max compression
```

## Comparing `rdfizer-4.7.dev1682603874.tar` & `rdfizer-4.7.dev1682603926.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:54.536656 rdfizer-4.7.dev1682603874/
--rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-04-27 13:57:54.536656 rdfizer-4.7.dev1682603874/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-04-27 13:57:45.000000 rdfizer-4.7.dev1682603874/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:54.532656 rdfizer-4.7.dev1682603874/rdfizer/
--rwxr-xr-x   0 runner    (1001) docker     (123)   271030 2023-04-27 13:57:45.000000 rdfizer-4.7.dev1682603874/rdfizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-27 13:57:45.000000 rdfizer-4.7.dev1682603874/rdfizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55665 2023-04-27 13:57:45.000000 rdfizer-4.7.dev1682603874/rdfizer/functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   271030 2023-04-27 13:57:45.000000 rdfizer-4.7.dev1682603874/rdfizer/semantify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:54.536656 rdfizer-4.7.dev1682603874/rdfizer/triples_map/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4995 2023-04-27 13:57:45.000000 rdfizer-4.7.dev1682603874/rdfizer/triples_map/TriplesMap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:45.000000 rdfizer-4.7.dev1682603874/rdfizer/triples_map/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:57:54.532656 rdfizer-4.7.dev1682603874/rdfizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-04-27 13:57:54.000000 rdfizer-4.7.dev1682603874/rdfizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-27 13:57:54.000000 rdfizer-4.7.dev1682603874/rdfizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:57:54.000000 rdfizer-4.7.dev1682603874/rdfizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-27 13:57:54.000000 rdfizer-4.7.dev1682603874/rdfizer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-27 13:57:54.000000 rdfizer-4.7.dev1682603874/rdfizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 13:57:54.000000 rdfizer-4.7.dev1682603874/rdfizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 13:57:54.536656 rdfizer-4.7.dev1682603874/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-27 13:57:45.000000 rdfizer-4.7.dev1682603874/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:58:46.486722 rdfizer-4.7.dev1682603926/
+-rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-04-27 13:58:46.486722 rdfizer-4.7.dev1682603926/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-04-27 13:58:32.000000 rdfizer-4.7.dev1682603926/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:58:46.482722 rdfizer-4.7.dev1682603926/rdfizer/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   271030 2023-04-27 13:58:32.000000 rdfizer-4.7.dev1682603926/rdfizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-27 13:58:32.000000 rdfizer-4.7.dev1682603926/rdfizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55665 2023-04-27 13:58:32.000000 rdfizer-4.7.dev1682603926/rdfizer/functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   271030 2023-04-27 13:58:32.000000 rdfizer-4.7.dev1682603926/rdfizer/semantify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:58:46.486722 rdfizer-4.7.dev1682603926/rdfizer/triples_map/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4995 2023-04-27 13:58:32.000000 rdfizer-4.7.dev1682603926/rdfizer/triples_map/TriplesMap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:58:32.000000 rdfizer-4.7.dev1682603926/rdfizer/triples_map/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:58:46.482722 rdfizer-4.7.dev1682603926/rdfizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-04-27 13:58:46.000000 rdfizer-4.7.dev1682603926/rdfizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-27 13:58:46.000000 rdfizer-4.7.dev1682603926/rdfizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:58:46.000000 rdfizer-4.7.dev1682603926/rdfizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-27 13:58:46.000000 rdfizer-4.7.dev1682603926/rdfizer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-27 13:58:46.000000 rdfizer-4.7.dev1682603926/rdfizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 13:58:46.000000 rdfizer-4.7.dev1682603926/rdfizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 13:58:46.486722 rdfizer-4.7.dev1682603926/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-27 13:58:32.000000 rdfizer-4.7.dev1682603926/setup.py
```

### Comparing `rdfizer-4.7.dev1682603874/PKG-INFO` & `rdfizer-4.7.dev1682603926/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfizer
-Version: 4.7.dev1682603874
+Version: 4.7.dev1682603926
 Summary: This project presents the SDM-RDFizer, an interpreter of mapping rules that allows the transformation of (un)structured data into RDF knowledge graphs. The current version of the SDM-RDFizer assumes mapping rules are defined in the RDF Mapping Language (RML) by Dimou et al.
 Home-page: https://github.com/SDM-TIB/SDM-RDFizer
 Author: Maria-Esther Vidal
 Author-email: maria.vidal@tib.eu
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `rdfizer-4.7.dev1682603874/README.md` & `rdfizer-4.7.dev1682603926/README.md`

 * *Files identical despite different names*

### Comparing `rdfizer-4.7.dev1682603874/rdfizer/__init__.py` & `rdfizer-4.7.dev1682603926/rdfizer/__init__.py`

 * *Files identical despite different names*

### Comparing `rdfizer-4.7.dev1682603874/rdfizer/__main__.py` & `rdfizer-4.7.dev1682603926/rdfizer/__main__.py`

 * *Files identical despite different names*

### Comparing `rdfizer-4.7.dev1682603874/rdfizer/functions.py` & `rdfizer-4.7.dev1682603926/rdfizer/functions.py`

 * *Files identical despite different names*

### Comparing `rdfizer-4.7.dev1682603874/rdfizer/semantify.py` & `rdfizer-4.7.dev1682603926/rdfizer/semantify.py`

 * *Files identical despite different names*

### Comparing `rdfizer-4.7.dev1682603874/rdfizer/triples_map/TriplesMap.py` & `rdfizer-4.7.dev1682603926/rdfizer/triples_map/TriplesMap.py`

 * *Files identical despite different names*

### Comparing `rdfizer-4.7.dev1682603874/rdfizer.egg-info/PKG-INFO` & `rdfizer-4.7.dev1682603926/rdfizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfizer
-Version: 4.7.dev1682603874
+Version: 4.7.dev1682603926
 Summary: This project presents the SDM-RDFizer, an interpreter of mapping rules that allows the transformation of (un)structured data into RDF knowledge graphs. The current version of the SDM-RDFizer assumes mapping rules are defined in the RDF Mapping Language (RML) by Dimou et al.
 Home-page: https://github.com/SDM-TIB/SDM-RDFizer
 Author: Maria-Esther Vidal
 Author-email: maria.vidal@tib.eu
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `rdfizer-4.7.dev1682603874/setup.py` & `rdfizer-4.7.dev1682603926/setup.py`

 * *Files identical despite different names*

