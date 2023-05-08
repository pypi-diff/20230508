# Comparing `tmp/camtono-derivatives-1.0.2.tar.gz` & `tmp/camtono-derivatives-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/camtono-derivatives-1.0.2.tar", last modified: Wed Apr  5 21:05:32 2023, max compression
+gzip compressed data, was "dist/camtono-derivatives-1.0.3.tar", last modified: Mon May  8 15:31:09 2023, max compression
```

## Comparing `camtono-derivatives-1.0.2.tar` & `camtono-derivatives-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 21:05:32.000000 camtono-derivatives-1.0.2/
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-04-05 21:05:02.000000 camtono-derivatives-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      479 2023-04-05 21:05:32.000000 camtono-derivatives-1.0.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 21:05:32.000000 camtono-derivatives-1.0.2/camtono/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 21:05:32.000000 camtono-derivatives-1.0.2/camtono/derivatives/
--rw-rw-rw-   0 root         (0) root         (0)      193 2023-04-05 21:05:02.000000 camtono-derivatives-1.0.2/camtono/derivatives/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4706 2023-04-05 21:05:02.000000 camtono-derivatives-1.0.2/camtono/derivatives/combine.py
--rw-rw-rw-   0 root         (0) root         (0)     9583 2023-04-05 21:05:02.000000 camtono-derivatives-1.0.2/camtono/derivatives/features.py
--rw-rw-rw-   0 root         (0) root         (0)     4586 2023-04-05 21:05:02.000000 camtono-derivatives-1.0.2/camtono/derivatives/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     5683 2023-04-05 21:05:02.000000 camtono-derivatives-1.0.2/camtono/derivatives/generate.py
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-05 21:05:02.000000 camtono-derivatives-1.0.2/camtono/derivatives/outputs.py
--rw-rw-rw-   0 root         (0) root         (0)    10093 2023-04-05 21:05:02.000000 camtono-derivatives-1.0.2/camtono/derivatives/selects.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2023-04-05 21:05:02.000000 camtono-derivatives-1.0.2/camtono/derivatives/transforms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 21:05:32.000000 camtono-derivatives-1.0.2/camtono/derivatives_v2/
--rw-rw-rw-   0 root         (0) root         (0)      196 2023-04-05 21:05:02.000000 camtono-derivatives-1.0.2/camtono/derivatives_v2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3677 2023-04-05 21:05:02.000000 camtono-derivatives-1.0.2/camtono/derivatives_v2/combine.py
--rw-rw-rw-   0 root         (0) root         (0)     5962 2023-04-05 21:05:02.000000 camtono-derivatives-1.0.2/camtono/derivatives_v2/generate.py
--rw-rw-rw-   0 root         (0) root         (0)     5299 2023-04-05 21:05:02.000000 camtono-derivatives-1.0.2/camtono/derivatives_v2/selects.py
--rw-rw-rw-   0 root         (0) root         (0)     3490 2023-04-05 21:05:02.000000 camtono-derivatives-1.0.2/camtono/derivatives_v2/union_query_formatting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 21:05:32.000000 camtono-derivatives-1.0.2/camtono_derivatives.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      479 2023-04-05 21:05:32.000000 camtono-derivatives-1.0.2/camtono_derivatives.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-04-05 21:05:32.000000 camtono-derivatives-1.0.2/camtono_derivatives.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-05 21:05:32.000000 camtono-derivatives-1.0.2/camtono_derivatives.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-05 21:05:32.000000 camtono-derivatives-1.0.2/camtono_derivatives.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        8 2023-04-05 21:05:32.000000 camtono-derivatives-1.0.2/camtono_derivatives.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-04-05 21:05:32.000000 camtono-derivatives-1.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      912 2023-04-05 21:05:02.000000 camtono-derivatives-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 15:31:09.000000 camtono-derivatives-1.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-08 15:30:36.000000 camtono-derivatives-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      479 2023-05-08 15:31:09.000000 camtono-derivatives-1.0.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 15:31:08.000000 camtono-derivatives-1.0.3/camtono/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 15:31:08.000000 camtono-derivatives-1.0.3/camtono/derivatives/
+-rw-rw-rw-   0 root         (0) root         (0)      193 2023-05-08 15:30:36.000000 camtono-derivatives-1.0.3/camtono/derivatives/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4706 2023-05-08 15:30:36.000000 camtono-derivatives-1.0.3/camtono/derivatives/combine.py
+-rw-rw-rw-   0 root         (0) root         (0)     9583 2023-05-08 15:30:36.000000 camtono-derivatives-1.0.3/camtono/derivatives/features.py
+-rw-rw-rw-   0 root         (0) root         (0)     4586 2023-05-08 15:30:36.000000 camtono-derivatives-1.0.3/camtono/derivatives/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     5683 2023-05-08 15:30:36.000000 camtono-derivatives-1.0.3/camtono/derivatives/generate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-05-08 15:30:36.000000 camtono-derivatives-1.0.3/camtono/derivatives/outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)    10093 2023-05-08 15:30:36.000000 camtono-derivatives-1.0.3/camtono/derivatives/selects.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2023-05-08 15:30:36.000000 camtono-derivatives-1.0.3/camtono/derivatives/transforms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 15:31:09.000000 camtono-derivatives-1.0.3/camtono/derivatives_v2/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-05-08 15:30:36.000000 camtono-derivatives-1.0.3/camtono/derivatives_v2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3677 2023-05-08 15:30:36.000000 camtono-derivatives-1.0.3/camtono/derivatives_v2/combine.py
+-rw-rw-rw-   0 root         (0) root         (0)     5962 2023-05-08 15:30:36.000000 camtono-derivatives-1.0.3/camtono/derivatives_v2/generate.py
+-rw-rw-rw-   0 root         (0) root         (0)     5299 2023-05-08 15:30:36.000000 camtono-derivatives-1.0.3/camtono/derivatives_v2/selects.py
+-rw-rw-rw-   0 root         (0) root         (0)     3490 2023-05-08 15:30:36.000000 camtono-derivatives-1.0.3/camtono/derivatives_v2/union_query_formatting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 15:31:09.000000 camtono-derivatives-1.0.3/camtono_derivatives.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-05-08 15:31:08.000000 camtono-derivatives-1.0.3/camtono_derivatives.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-05-08 15:31:08.000000 camtono-derivatives-1.0.3/camtono_derivatives.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-08 15:31:08.000000 camtono-derivatives-1.0.3/camtono_derivatives.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-08 15:31:08.000000 camtono-derivatives-1.0.3/camtono_derivatives.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        8 2023-05-08 15:31:08.000000 camtono-derivatives-1.0.3/camtono_derivatives.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-05-08 15:31:09.000000 camtono-derivatives-1.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      912 2023-05-08 15:30:36.000000 camtono-derivatives-1.0.3/setup.py
```

### Comparing `camtono-derivatives-1.0.2/camtono/derivatives/combine.py` & `camtono-derivatives-1.0.3/camtono/derivatives/combine.py`

 * *Files identical despite different names*

### Comparing `camtono-derivatives-1.0.2/camtono/derivatives/features.py` & `camtono-derivatives-1.0.3/camtono/derivatives/features.py`

 * *Files identical despite different names*

### Comparing `camtono-derivatives-1.0.2/camtono/derivatives/filters.py` & `camtono-derivatives-1.0.3/camtono/derivatives/filters.py`

 * *Files identical despite different names*

### Comparing `camtono-derivatives-1.0.2/camtono/derivatives/generate.py` & `camtono-derivatives-1.0.3/camtono/derivatives/generate.py`

 * *Files identical despite different names*

### Comparing `camtono-derivatives-1.0.2/camtono/derivatives/outputs.py` & `camtono-derivatives-1.0.3/camtono/derivatives/outputs.py`

 * *Files identical despite different names*

### Comparing `camtono-derivatives-1.0.2/camtono/derivatives/selects.py` & `camtono-derivatives-1.0.3/camtono/derivatives/selects.py`

 * *Files identical despite different names*

### Comparing `camtono-derivatives-1.0.2/camtono/derivatives/transforms.py` & `camtono-derivatives-1.0.3/camtono/derivatives/transforms.py`

 * *Files identical despite different names*

### Comparing `camtono-derivatives-1.0.2/camtono/derivatives_v2/combine.py` & `camtono-derivatives-1.0.3/camtono/derivatives_v2/combine.py`

 * *Files identical despite different names*

### Comparing `camtono-derivatives-1.0.2/camtono/derivatives_v2/generate.py` & `camtono-derivatives-1.0.3/camtono/derivatives_v2/generate.py`

 * *Files identical despite different names*

### Comparing `camtono-derivatives-1.0.2/camtono/derivatives_v2/selects.py` & `camtono-derivatives-1.0.3/camtono/derivatives_v2/selects.py`

 * *Files identical despite different names*

### Comparing `camtono-derivatives-1.0.2/camtono/derivatives_v2/union_query_formatting.py` & `camtono-derivatives-1.0.3/camtono/derivatives_v2/union_query_formatting.py`

 * *Files identical despite different names*

### Comparing `camtono-derivatives-1.0.2/camtono_derivatives.egg-info/SOURCES.txt` & `camtono-derivatives-1.0.3/camtono_derivatives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `camtono-derivatives-1.0.2/setup.py` & `camtono-derivatives-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # with open("README.md", "r") as fh:
 #     long_description = fh.read()
 # with open('requirements.txt') as f:
 #     requirements = f.readlines()
 
 setuptools.setup(
     name="camtono-derivatives",  # Replace with your own username
-    version="1.0.2",
+    version="1.0.3",
     author="DOT",
     author_email="dot@adara.com",
     description="Simplified advertising integrations",
     long_description="",
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://bitbucket.org/adarainc/camtono-derivatives-pkg",
```

