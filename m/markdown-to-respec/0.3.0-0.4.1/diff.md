# Comparing `tmp/markdown-to-respec-0.3.0.tar.gz` & `tmp/markdown-to-respec-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown-to-respec-0.3.0.tar", last modified: Sat May  6 14:49:54 2023, max compression
+gzip compressed data, was "markdown-to-respec-0.4.1.tar", last modified: Mon May  8 13:13:11 2023, max compression
```

## Comparing `markdown-to-respec-0.3.0.tar` & `markdown-to-respec-0.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-06 14:49:54.074030 markdown-to-respec-0.3.0/
--rw-r--r--   0 edsummers   (505) staff       (20)     4032 2023-05-06 14:49:54.074166 markdown-to-respec-0.3.0/PKG-INFO
--rw-r--r--   0 edsummers   (505) staff       (20)     3727 2023-05-06 14:45:54.000000 markdown-to-respec-0.3.0/README.md
-drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-06 14:49:54.073713 markdown-to-respec-0.3.0/markdown_to_respec.egg-info/
--rw-r--r--   0 edsummers   (505) staff       (20)     4032 2023-05-06 14:49:54.000000 markdown-to-respec-0.3.0/markdown_to_respec.egg-info/PKG-INFO
--rw-r--r--   0 edsummers   (505) staff       (20)      304 2023-05-06 14:49:54.000000 markdown-to-respec-0.3.0/markdown_to_respec.egg-info/SOURCES.txt
--rw-r--r--   0 edsummers   (505) staff       (20)        1 2023-05-06 14:49:54.000000 markdown-to-respec-0.3.0/markdown_to_respec.egg-info/dependency_links.txt
--rw-r--r--   0 edsummers   (505) staff       (20)       63 2023-05-06 14:49:54.000000 markdown-to-respec-0.3.0/markdown_to_respec.egg-info/entry_points.txt
--rw-r--r--   0 edsummers   (505) staff       (20)       29 2023-05-06 14:49:54.000000 markdown-to-respec-0.3.0/markdown_to_respec.egg-info/requires.txt
--rw-r--r--   0 edsummers   (505) staff       (20)       19 2023-05-06 14:49:54.000000 markdown-to-respec-0.3.0/markdown_to_respec.egg-info/top_level.txt
--rwxr-xr-x   0 edsummers   (505) staff       (20)     6756 2023-05-06 14:26:46.000000 markdown-to-respec-0.3.0/markdown_to_respec.py
--rw-r--r--   0 edsummers   (505) staff       (20)       63 2023-05-06 14:49:54.074650 markdown-to-respec-0.3.0/setup.cfg
--rw-r--r--   0 edsummers   (505) staff       (20)      907 2023-05-06 14:18:05.000000 markdown-to-respec-0.3.0/setup.py
+drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-08 13:13:11.576685 markdown-to-respec-0.4.1/
+-rw-r--r--   0 edsummers   (505) staff       (20)     4031 2023-05-08 13:13:11.576820 markdown-to-respec-0.4.1/PKG-INFO
+-rw-r--r--   0 edsummers   (505) staff       (20)     3726 2023-05-08 13:11:07.000000 markdown-to-respec-0.4.1/README.md
+drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-08 13:13:11.576360 markdown-to-respec-0.4.1/markdown_to_respec.egg-info/
+-rw-r--r--   0 edsummers   (505) staff       (20)     4031 2023-05-08 13:13:11.000000 markdown-to-respec-0.4.1/markdown_to_respec.egg-info/PKG-INFO
+-rw-r--r--   0 edsummers   (505) staff       (20)      304 2023-05-08 13:13:11.000000 markdown-to-respec-0.4.1/markdown_to_respec.egg-info/SOURCES.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)        1 2023-05-08 13:13:11.000000 markdown-to-respec-0.4.1/markdown_to_respec.egg-info/dependency_links.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)       63 2023-05-08 13:13:11.000000 markdown-to-respec-0.4.1/markdown_to_respec.egg-info/entry_points.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)       29 2023-05-08 13:13:11.000000 markdown-to-respec-0.4.1/markdown_to_respec.egg-info/requires.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)       19 2023-05-08 13:13:11.000000 markdown-to-respec-0.4.1/markdown_to_respec.egg-info/top_level.txt
+-rwxr-xr-x   0 edsummers   (505) staff       (20)     6756 2023-05-06 14:55:15.000000 markdown-to-respec-0.4.1/markdown_to_respec.py
+-rw-r--r--   0 edsummers   (505) staff       (20)       63 2023-05-08 13:13:11.577617 markdown-to-respec-0.4.1/setup.cfg
+-rw-r--r--   0 edsummers   (505) staff       (20)      907 2023-05-08 13:11:44.000000 markdown-to-respec-0.4.1/setup.py
```

### Comparing `markdown-to-respec-0.3.0/PKG-INFO` & `markdown-to-respec-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-to-respec
-Version: 0.3.0
+Version: 0.4.1
 Summary: Convert specifications written in Markdown to ReSpec HTML
 Home-page: https://github.com/webrecorder/markdown-to-respec
 Author: Ed Summers
 Author-email: info@webrecorder.net
 License: Apache 2.0
 Description-Content-Type: text/markdown
 
@@ -72,15 +72,15 @@
 1. Include as frontmatter in your Markdown file: see [embedded] for an example.
 2. Include as a JSON file along side your Markdown file: see [external] for an example.
 
 If you would like to use an alternate ReSpec Javascript URL you can use the `respec_js` config option either in frontmatter or the external JSON configuration.
 
 ## Command Line
 
-If you want you can install *markdown-to-respec* and run it from the command line. This can be useful in situations where you are making local changes and want to see the resulting HTML. You should be able to use your brownser to open the resulting HTML files.
+If you want you can install *markdown-to-respec* and run it from the command line. This can be useful in situations where you are making local changes and want to see the resulting HTML. You should be able to use your browser to open the resulting HTML files.
 
 ```
 usage: markdown-to-respec [-h] [--branch BRANCH] [--publish] [--ignore IGNORE] path
 
 positional arguments:
   path             Path to search for Markdown files
```

### Comparing `markdown-to-respec-0.3.0/README.md` & `markdown-to-respec-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 1. Include as frontmatter in your Markdown file: see [embedded] for an example.
 2. Include as a JSON file along side your Markdown file: see [external] for an example.
 
 If you would like to use an alternate ReSpec Javascript URL you can use the `respec_js` config option either in frontmatter or the external JSON configuration.
 
 ## Command Line
 
-If you want you can install *markdown-to-respec* and run it from the command line. This can be useful in situations where you are making local changes and want to see the resulting HTML. You should be able to use your brownser to open the resulting HTML files.
+If you want you can install *markdown-to-respec* and run it from the command line. This can be useful in situations where you are making local changes and want to see the resulting HTML. You should be able to use your browser to open the resulting HTML files.
 
 ```
 usage: markdown-to-respec [-h] [--branch BRANCH] [--publish] [--ignore IGNORE] path
 
 positional arguments:
   path             Path to search for Markdown files
```

### Comparing `markdown-to-respec-0.3.0/markdown_to_respec.egg-info/PKG-INFO` & `markdown-to-respec-0.4.1/markdown_to_respec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-to-respec
-Version: 0.3.0
+Version: 0.4.1
 Summary: Convert specifications written in Markdown to ReSpec HTML
 Home-page: https://github.com/webrecorder/markdown-to-respec
 Author: Ed Summers
 Author-email: info@webrecorder.net
 License: Apache 2.0
 Description-Content-Type: text/markdown
 
@@ -72,15 +72,15 @@
 1. Include as frontmatter in your Markdown file: see [embedded] for an example.
 2. Include as a JSON file along side your Markdown file: see [external] for an example.
 
 If you would like to use an alternate ReSpec Javascript URL you can use the `respec_js` config option either in frontmatter or the external JSON configuration.
 
 ## Command Line
 
-If you want you can install *markdown-to-respec* and run it from the command line. This can be useful in situations where you are making local changes and want to see the resulting HTML. You should be able to use your brownser to open the resulting HTML files.
+If you want you can install *markdown-to-respec* and run it from the command line. This can be useful in situations where you are making local changes and want to see the resulting HTML. You should be able to use your browser to open the resulting HTML files.
 
 ```
 usage: markdown-to-respec [-h] [--branch BRANCH] [--publish] [--ignore IGNORE] path
 
 positional arguments:
   path             Path to search for Markdown files
```

### Comparing `markdown-to-respec-0.3.0/markdown_to_respec.py` & `markdown-to-respec-0.4.1/markdown_to_respec.py`

 * *Files identical despite different names*

### Comparing `markdown-to-respec-0.3.0/setup.py` & `markdown-to-respec-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = "0.3.0"
+__version__ = "0.4.1"
 
 def load_requirements(filename):
     with open(filename, "rt") as fh:
         return fh.read().rstrip().split("\n")
 
 with open("README.md") as f:
     long_description = f.read()
```

