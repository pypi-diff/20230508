# Comparing `tmp/textgrid-convert-0.4.4.tar.gz` & `tmp/textgrid-convert-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textgrid-convert-0.4.4.tar", last modified: Tue Jan 17 01:18:48 2023, max compression
+gzip compressed data, was "textgrid-convert-0.5.tar", last modified: Sun May  7 23:58:55 2023, max compression
```

## Comparing `textgrid-convert-0.4.4.tar` & `textgrid-convert-0.5.tar`

### file list

```diff
@@ -1,10 +1,21 @@
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-01-17 01:18:48.560858 textgrid-convert-0.4.4/
--rw-r--r--   0 patrick    (501) staff       (20)      700 2023-01-17 01:18:48.560462 textgrid-convert-0.4.4/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)       38 2023-01-17 01:18:48.560968 textgrid-convert-0.4.4/setup.cfg
--rw-r--r--   0 patrick    (501) staff       (20)     4316 2023-01-17 01:17:50.000000 textgrid-convert-0.4.4/setup.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-01-17 01:18:48.559768 textgrid-convert-0.4.4/textgrid_convert.egg-info/
--rw-r--r--   0 patrick    (501) staff       (20)      700 2023-01-17 01:18:48.000000 textgrid-convert-0.4.4/textgrid_convert.egg-info/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)      207 2023-01-17 01:18:48.000000 textgrid-convert-0.4.4/textgrid_convert.egg-info/SOURCES.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-01-17 01:18:48.000000 textgrid-convert-0.4.4/textgrid_convert.egg-info/dependency_links.txt
--rw-r--r--   0 patrick    (501) staff       (20)      423 2023-01-17 01:18:48.000000 textgrid-convert-0.4.4/textgrid_convert.egg-info/requires.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-01-17 01:18:48.000000 textgrid-convert-0.4.4/textgrid_convert.egg-info/top_level.txt
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-07 23:58:55.895986 textgrid-convert-0.5/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      679 2023-05-07 23:58:55.895986 textgrid-convert-0.5/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-05-07 23:58:55.895986 textgrid-convert-0.5/setup.cfg
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4314 2023-05-07 23:53:25.000000 textgrid-convert-0.5/setup.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-07 23:58:55.891986 textgrid-convert-0.5/tests/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2710 2023-05-07 23:47:31.000000 textgrid-convert-0.5/tests/test_argparse.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6130 2023-05-07 23:47:31.000000 textgrid-convert-0.5/tests/test_cli.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      459 2023-05-07 23:47:31.000000 textgrid-convert-0.5/tests/test_iotools.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      580 2023-05-07 23:47:31.000000 textgrid-convert-0.5/tests/test_local.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        2 2023-05-07 23:47:31.000000 textgrid-convert-0.5/tests/test_main.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      927 2023-05-07 23:47:31.000000 textgrid-convert-0.5/tests/test_preprocesstools.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1900 2023-05-07 23:47:31.000000 textgrid-convert-0.5/tests/test_revParser.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3049 2023-05-07 23:47:31.000000 textgrid-convert-0.5/tests/test_sbvparser.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2439 2023-05-07 23:47:31.000000 textgrid-convert-0.5/tests/test_srtparser.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3434 2023-05-07 23:47:31.000000 textgrid-convert-0.5/tests/test_textgridtools.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-07 23:58:55.895986 textgrid-convert-0.5/textgrid_convert.egg-info/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      679 2023-05-07 23:58:55.000000 textgrid-convert-0.5/textgrid_convert.egg-info/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      439 2023-05-07 23:58:55.000000 textgrid-convert-0.5/textgrid_convert.egg-info/SOURCES.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-05-07 23:58:55.000000 textgrid-convert-0.5/textgrid_convert.egg-info/dependency_links.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      423 2023-05-07 23:58:55.000000 textgrid-convert-0.5/textgrid_convert.egg-info/requires.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-05-07 23:58:55.000000 textgrid-convert-0.5/textgrid_convert.egg-info/top_level.txt
```

### Comparing `textgrid-convert-0.4.4/PKG-INFO` & `textgrid-convert-0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: textgrid-convert
-Version: 0.4.4
+Version: 0.5
 Summary: textgrid-convert converts audio transcripts such as sbv or srt files to Praat and DARLA compatible TextGrids.
 Home-page: https://github.com/patrickschu/textgrid-convert/
 Author: Patrick Schultz, Lars Hinrichs
 Author-email: patrickschultz@utexas.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.0.0
 
 textgrid-convert converts audio transcripts such as sbv or srt files to Praat and DARLA compatible TextGrids.
-
```

### Comparing `textgrid-convert-0.4.4/setup.py` & `textgrid-convert-0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Package meta-data.
 NAME = "textgrid-convert"
 DESCRIPTION = "textgrid-convert converts audio transcripts such as sbv or srt files to Praat and DARLA compatible TextGrids."
 URL ="https://github.com/patrickschu/textgrid-convert/"
 EMAIL ="patrickschultz@utexas.edu"
 AUTHOR = "Patrick Schultz, Lars Hinrichs"
 REQUIRES_PYTHON = '>=3.0.0'
-VERSION = '0.4.4'
+VERSION = '0.5'
 
 # What packages are required for this module to be executed?
 # FIXME is this needed
 REQUIRED = [ 
  "astroid>=2.3.3",
  "attrs>=19.3.0",
  "et-xmlfile>=1.0.1",
```

### Comparing `textgrid-convert-0.4.4/textgrid_convert.egg-info/PKG-INFO` & `textgrid-convert-0.5/textgrid_convert.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: textgrid-convert
-Version: 0.4.4
+Version: 0.5
 Summary: textgrid-convert converts audio transcripts such as sbv or srt files to Praat and DARLA compatible TextGrids.
 Home-page: https://github.com/patrickschu/textgrid-convert/
 Author: Patrick Schultz, Lars Hinrichs
 Author-email: patrickschultz@utexas.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.0.0
 
 textgrid-convert converts audio transcripts such as sbv or srt files to Praat and DARLA compatible TextGrids.
-
```

