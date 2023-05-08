# Comparing `tmp/bgdiscovery-0.9.8.tar.gz` & `tmp/bgdiscovery-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgdiscovery-0.9.8.tar", last modified: Tue May  2 05:16:36 2023, max compression
+gzip compressed data, was "bgdiscovery-0.9.9.tar", last modified: Tue May  2 11:13:20 2023, max compression
```

## Comparing `bgdiscovery-0.9.8.tar` & `bgdiscovery-0.9.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 05:16:36.007733 bgdiscovery-0.9.8/
--rw-rw-rw-   0        0        0     2325 2023-05-02 05:16:36.006735 bgdiscovery-0.9.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 05:16:36.003744 bgdiscovery-0.9.8/bgdiscovery.egg-info/
--rw-rw-rw-   0        0        0     2325 2023-05-02 05:16:35.000000 bgdiscovery-0.9.8/bgdiscovery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-05-02 05:16:35.000000 bgdiscovery-0.9.8/bgdiscovery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 05:16:35.000000 bgdiscovery-0.9.8/bgdiscovery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-02 05:16:35.000000 bgdiscovery-0.9.8/bgdiscovery.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       66 2023-05-02 05:16:35.000000 bgdiscovery-0.9.8/bgdiscovery.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-02 05:16:35.000000 bgdiscovery-0.9.8/bgdiscovery.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 05:16:36.008736 bgdiscovery-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0     3340 2023-04-17 06:44:31.000000 bgdiscovery-0.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:13:20.150956 bgdiscovery-0.9.9/
+-rw-rw-rw-   0        0        0     2325 2023-05-02 11:13:20.148949 bgdiscovery-0.9.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 11:13:20.147439 bgdiscovery-0.9.9/bgdiscovery.egg-info/
+-rw-rw-rw-   0        0        0     2325 2023-05-02 11:13:19.000000 bgdiscovery-0.9.9/bgdiscovery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-05-02 11:13:20.000000 bgdiscovery-0.9.9/bgdiscovery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 11:13:19.000000 bgdiscovery-0.9.9/bgdiscovery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-02 11:13:19.000000 bgdiscovery-0.9.9/bgdiscovery.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       66 2023-05-02 11:13:19.000000 bgdiscovery-0.9.9/bgdiscovery.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-02 11:13:19.000000 bgdiscovery-0.9.9/bgdiscovery.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 11:13:20.150956 bgdiscovery-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     3340 2023-04-17 06:44:31.000000 bgdiscovery-0.9.9/setup.py
```

### Comparing `bgdiscovery-0.9.8/PKG-INFO` & `bgdiscovery-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgdiscovery
-Version: 0.9.8
+Version: 0.9.9
 Summary: biGENIUS Discovery App.
 Home-page: https://www.bigenius.info/
 Author: biGENIUS AG
 Author-email: gergely.szecsenyi@bigenius.info
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `bgdiscovery-0.9.8/bgdiscovery.egg-info/PKG-INFO` & `bgdiscovery-0.9.9/bgdiscovery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgdiscovery
-Version: 0.9.8
+Version: 0.9.9
 Summary: biGENIUS Discovery App.
 Home-page: https://www.bigenius.info/
 Author: biGENIUS AG
 Author-email: gergely.szecsenyi@bigenius.info
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `bgdiscovery-0.9.8/setup.py` & `bgdiscovery-0.9.9/setup.py`

 * *Files identical despite different names*

