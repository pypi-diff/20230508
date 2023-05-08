# Comparing `tmp/dreamai_pdf-0.0.8.tar.gz` & `tmp/dreamai_pdf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai_pdf-0.0.8.tar", last modified: Thu May  4 00:32:55 2023, max compression
+gzip compressed data, was "dreamai_pdf-0.0.9.tar", last modified: Thu May  4 03:27:47 2023, max compression
```

## Comparing `dreamai_pdf-0.0.8.tar` & `dreamai_pdf-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 00:32:55.475934 dreamai_pdf-0.0.8/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.8/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.8/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-04 00:32:55.475934 dreamai_pdf-0.0.8/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      138 2023-05-02 22:37:14.000000 dreamai_pdf-0.0.8/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 00:32:55.475934 dreamai_pdf-0.0.8/dreamai_pdf/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-04 00:32:44.000000 dreamai_pdf-0.0.8/dreamai_pdf/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     5569 2023-05-04 00:32:44.000000 dreamai_pdf-0.0.8/dreamai_pdf/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     3434 2023-05-04 00:32:44.000000 dreamai_pdf-0.0.8/dreamai_pdf/core.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      494 2023-05-02 20:33:15.000000 dreamai_pdf-0.0.8/dreamai_pdf/imports.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     9207 2023-05-04 00:32:44.000000 dreamai_pdf-0.0.8/dreamai_pdf/parse.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2285 2023-05-04 00:32:44.000000 dreamai_pdf-0.0.8/dreamai_pdf/segment.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 00:32:55.475934 dreamai_pdf-0.0.8/dreamai_pdf.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-04 00:32:55.000000 dreamai_pdf-0.0.8/dreamai_pdf.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      431 2023-05-04 00:32:55.000000 dreamai_pdf-0.0.8/dreamai_pdf.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-04 00:32:55.000000 dreamai_pdf-0.0.8/dreamai_pdf.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       44 2023-05-04 00:32:55.000000 dreamai_pdf-0.0.8/dreamai_pdf.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-04-28 14:00:17.000000 dreamai_pdf-0.0.8/dreamai_pdf.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2951 2023-05-04 00:32:55.000000 dreamai_pdf-0.0.8/dreamai_pdf.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       12 2023-05-04 00:32:55.000000 dreamai_pdf-0.0.8/dreamai_pdf.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     3636 2023-05-04 00:30:45.000000 dreamai_pdf-0.0.8/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-04 00:32:55.475934 dreamai_pdf-0.0.8/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.8/setup.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 03:27:47.318750 dreamai_pdf-0.0.9/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.9/LICENSE
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.9/MANIFEST.in
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-04 03:27:47.318750 dreamai_pdf-0.0.9/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      138 2023-05-02 22:37:14.000000 dreamai_pdf-0.0.9/README.md
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 03:27:47.318750 dreamai_pdf-0.0.9/dreamai_pdf/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-04 03:27:36.000000 dreamai_pdf-0.0.9/dreamai_pdf/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     5569 2023-05-04 03:27:36.000000 dreamai_pdf-0.0.9/dreamai_pdf/_modidx.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     3434 2023-05-04 03:27:36.000000 dreamai_pdf-0.0.9/dreamai_pdf/core.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      494 2023-05-02 20:33:15.000000 dreamai_pdf-0.0.9/dreamai_pdf/imports.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     9207 2023-05-04 03:27:36.000000 dreamai_pdf-0.0.9/dreamai_pdf/parse.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2285 2023-05-04 03:27:36.000000 dreamai_pdf-0.0.9/dreamai_pdf/segment.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 03:27:47.318750 dreamai_pdf-0.0.9/dreamai_pdf.egg-info/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-04 03:27:47.000000 dreamai_pdf-0.0.9/dreamai_pdf.egg-info/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      431 2023-05-04 03:27:47.000000 dreamai_pdf-0.0.9/dreamai_pdf.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-04 03:27:47.000000 dreamai_pdf-0.0.9/dreamai_pdf.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       44 2023-05-04 03:27:47.000000 dreamai_pdf-0.0.9/dreamai_pdf.egg-info/entry_points.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-04-28 14:00:17.000000 dreamai_pdf-0.0.9/dreamai_pdf.egg-info/not-zip-safe
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       98 2023-05-04 03:27:47.000000 dreamai_pdf-0.0.9/dreamai_pdf.egg-info/requires.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       12 2023-05-04 03:27:47.000000 dreamai_pdf-0.0.9/dreamai_pdf.egg-info/top_level.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      783 2023-05-04 03:26:18.000000 dreamai_pdf-0.0.9/settings.ini
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-04 03:27:47.318750 dreamai_pdf-0.0.9/setup.cfg
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.9/setup.py
```

### Comparing `dreamai_pdf-0.0.8/LICENSE` & `dreamai_pdf-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.8/PKG-INFO` & `dreamai_pdf-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai_pdf
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library based on dreamai for parsing PDFs
 Home-page: https://github.com/HamzaFarhan/dreamai_pdf
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_pdf-0.0.8/dreamai_pdf/_modidx.py` & `dreamai_pdf-0.0.9/dreamai_pdf/_modidx.py`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.8/dreamai_pdf/core.py` & `dreamai_pdf-0.0.9/dreamai_pdf/core.py`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.8/dreamai_pdf/parse.py` & `dreamai_pdf-0.0.9/dreamai_pdf/parse.py`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.8/dreamai_pdf/segment.py` & `dreamai_pdf-0.0.9/dreamai_pdf/segment.py`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.8/dreamai_pdf.egg-info/PKG-INFO` & `dreamai_pdf-0.0.9/dreamai_pdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai-pdf
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library based on dreamai for parsing PDFs
 Home-page: https://github.com/HamzaFarhan/dreamai_pdf
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_pdf-0.0.8/setup.py` & `dreamai_pdf-0.0.9/setup.py`

 * *Files identical despite different names*

