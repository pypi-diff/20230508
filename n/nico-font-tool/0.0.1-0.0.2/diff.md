# Comparing `tmp/nico-font-tool-0.0.1.tar.gz` & `tmp/nico-font-tool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nico-font-tool-0.0.1.tar", last modified: Mon May  8 09:50:10 2023, max compression
+gzip compressed data, was "nico-font-tool-0.0.2.tar", last modified: Mon May  8 11:34:25 2023, max compression
```

## Comparing `nico-font-tool-0.0.1.tar` & `nico-font-tool-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:50:10.936936 nico-font-tool-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 09:49:59.000000 nico-font-tool-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-05-08 09:50:10.936936 nico-font-tool-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-08 09:49:59.000000 nico-font-tool-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-08 09:49:59.000000 nico-font-tool-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 09:50:10.936936 nico-font-tool-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:50:10.932936 nico-font-tool-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:50:10.936936 nico-font-tool-0.0.1/src/nico_font_tool/
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-08 09:49:59.000000 nico-font-tool-0.0.1/src/nico_font_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-08 09:49:59.000000 nico-font-tool-0.0.1/src/nico_font_tool/bdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-08 09:49:59.000000 nico-font-tool-0.0.1/src/nico_font_tool/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-08 09:49:59.000000 nico-font-tool-0.0.1/src/nico_font_tool/opentype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:50:10.936936 nico-font-tool-0.0.1/src/nico_font_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-05-08 09:50:10.000000 nico-font-tool-0.0.1/src/nico_font_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-08 09:50:10.000000 nico-font-tool-0.0.1/src/nico_font_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:50:10.000000 nico-font-tool-0.0.1/src/nico_font_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-08 09:50:10.000000 nico-font-tool-0.0.1/src/nico_font_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 09:50:10.000000 nico-font-tool-0.0.1/src/nico_font_tool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:50:10.936936 nico-font-tool-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-08 09:49:59.000000 nico-font-tool-0.0.1/tests/test_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:34:25.692727 nico-font-tool-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 11:34:09.000000 nico-font-tool-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-08 11:34:25.692727 nico-font-tool-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-08 11:34:09.000000 nico-font-tool-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-08 11:34:09.000000 nico-font-tool-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 11:34:25.692727 nico-font-tool-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:34:25.688727 nico-font-tool-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:34:25.692727 nico-font-tool-0.0.2/src/nico_font_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-08 11:34:09.000000 nico-font-tool-0.0.2/src/nico_font_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-08 11:34:09.000000 nico-font-tool-0.0.2/src/nico_font_tool/bdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-08 11:34:09.000000 nico-font-tool-0.0.2/src/nico_font_tool/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-08 11:34:09.000000 nico-font-tool-0.0.2/src/nico_font_tool/nicofont.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-08 11:34:09.000000 nico-font-tool-0.0.2/src/nico_font_tool/opentype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:34:25.692727 nico-font-tool-0.0.2/src/nico_font_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-08 11:34:25.000000 nico-font-tool-0.0.2/src/nico_font_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-08 11:34:25.000000 nico-font-tool-0.0.2/src/nico_font_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:34:25.000000 nico-font-tool-0.0.2/src/nico_font_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-08 11:34:25.000000 nico-font-tool-0.0.2/src/nico_font_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-08 11:34:25.000000 nico-font-tool-0.0.2/src/nico_font_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 11:34:25.000000 nico-font-tool-0.0.2/src/nico_font_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:34:25.692727 nico-font-tool-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-08 11:34:09.000000 nico-font-tool-0.0.2/tests/test_.py
```

### Comparing `nico-font-tool-0.0.1/LICENSE` & `nico-font-tool-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.1/pyproject.toml` & `nico-font-tool-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nico-font-tool"
-version = "0.0.1"
+version = "0.0.2"
 description = "A tool for converting fonts to NICO Game Framework format fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
@@ -27,11 +27,14 @@
 ]
 
 [project.urls]
 homepage = "https://github.com/TakWolf/nico-font-tool.python"
 source = "https://github.com/TakWolf/nico-font-tool.python"
 issues = "https://github.com/TakWolf/nico-font-tool.python/issues"
 
+[project.scripts]
+nicofont = "nico_font_tool.nicofont:main"
+
 [tool.pytest.ini_options]
 pythonpath = [
     "src",
 ]
```

### Comparing `nico-font-tool-0.0.1/src/nico_font_tool/__init__.py` & `nico-font-tool-0.0.2/src/nico_font_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.1/src/nico_font_tool/bdf.py` & `nico-font-tool-0.0.2/src/nico_font_tool/bdf.py`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.1/src/nico_font_tool/font.py` & `nico-font-tool-0.0.2/src/nico_font_tool/font.py`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.1/src/nico_font_tool/opentype.py` & `nico-font-tool-0.0.2/src/nico_font_tool/opentype.py`

 * *Files identical despite different names*

