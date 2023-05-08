# Comparing `tmp/ProcessingImg1-0.2.tar.gz` & `tmp/ProcessingImg1-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProcessingImg1-0.2.tar", last modified: Sun May  7 13:30:46 2023, max compression
+gzip compressed data, was "ProcessingImg1-0.3.tar", last modified: Mon May  8 11:54:51 2023, max compression
```

## Comparing `ProcessingImg1-0.2.tar` & `ProcessingImg1-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 13:30:46.480398 ProcessingImg1-0.2/
--rw-rw-rw-   0        0        0       46 2023-05-07 13:26:18.000000 ProcessingImg1-0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      825 2023-05-07 13:30:46.480398 ProcessingImg1-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-07 13:30:46.473416 ProcessingImg1-0.2/ProcessingImg1.egg-info/
--rw-rw-rw-   0        0        0      825 2023-05-07 13:30:46.000000 ProcessingImg1-0.2/ProcessingImg1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-05-07 13:30:46.000000 ProcessingImg1-0.2/ProcessingImg1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 13:30:46.000000 ProcessingImg1-0.2/ProcessingImg1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-07 13:30:46.000000 ProcessingImg1-0.2/ProcessingImg1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4443 2023-05-07 13:16:05.000000 ProcessingImg1-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 13:30:46.474413 ProcessingImg1-0.2/organize/
--rw-rw-rw-   0        0        0     4469 2023-05-07 13:26:48.000000 ProcessingImg1-0.2/organize/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 13:30:46.476434 ProcessingImg1-0.2/processing/
--rw-rw-rw-   0        0        0    14855 2023-05-07 13:26:37.000000 ProcessingImg1-0.2/processing/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-07 13:30:46.481394 ProcessingImg1-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1007 2023-05-07 13:25:07.000000 ProcessingImg1-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:54:51.570215 ProcessingImg1-0.3/
+-rw-rw-rw-   0        0        0       46 2023-05-07 13:26:18.000000 ProcessingImg1-0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2829 2023-05-08 11:54:51.569218 ProcessingImg1-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-08 11:54:51.562236 ProcessingImg1-0.3/ProcessingImg1.egg-info/
+-rw-rw-rw-   0        0        0     2829 2023-05-08 11:54:51.000000 ProcessingImg1-0.3/ProcessingImg1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-05-08 11:54:51.000000 ProcessingImg1-0.3/ProcessingImg1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 11:54:51.000000 ProcessingImg1-0.3/ProcessingImg1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-08 11:54:51.000000 ProcessingImg1-0.3/ProcessingImg1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1887 2023-05-08 11:38:46.000000 ProcessingImg1-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 11:54:51.565229 ProcessingImg1-0.3/organize/
+-rw-rw-rw-   0        0        0     4469 2023-05-08 11:40:52.000000 ProcessingImg1-0.3/organize/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:54:51.567223 ProcessingImg1-0.3/processing/
+-rw-rw-rw-   0        0        0    14855 2023-05-08 11:38:54.000000 ProcessingImg1-0.3/processing/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-08 11:54:51.570215 ProcessingImg1-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1101 2023-05-08 11:53:48.000000 ProcessingImg1-0.3/setup.py
```

### Comparing `ProcessingImg1-0.2/organize/__init__.py` & `ProcessingImg1-0.3/organize/__init__.py`

 * *Files identical despite different names*

### Comparing `ProcessingImg1-0.2/processing/__init__.py` & `ProcessingImg1-0.3/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `ProcessingImg1-0.2/setup.py` & `ProcessingImg1-0.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-import setuptools 
 
-with open("README.md", "r", encoding = "utf-8") as fh:
-    long_description = fh.read()
-setuptools.setup(
+from setuptools import setup, find_packages
+
+with open("README.md", "r", encoding="utf-8") as f:
+    long_description = f.read()
+
+setup(
     name="ProcessingImg1",
-    version="0.2",
-    author="Alaa Jassim Mohammed",
-    author_email = "alobede2001alobede@gmail.com",
-    url="https://github.com/Alaa-Jassim/proc-image",
+    version="0.3",
+    author="علاء جاسم محمد",
+    author_email="alobede2001alobede@gmail.com",
     description="A simple Pythonic library for image manipulation and hardware configuration that you can use alongside your project to save you time and effort",
-    packages=setuptools.find_packages(),
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/Alaa-Jassim/proc-image",
+    packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
-        "License :: OSI Approved :: MIT License"
     ]
-    )
+)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

