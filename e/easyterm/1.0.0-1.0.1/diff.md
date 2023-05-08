# Comparing `tmp/easyterm-1.0.0.tar.gz` & `tmp/easyterm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyterm-1.0.0.tar", last modified: Sun Feb 19 21:46:20 2023, max compression
+gzip compressed data, was "easyterm-1.0.1.tar", last modified: Mon May  8 10:37:53 2023, max compression
```

## Comparing `easyterm-1.0.0.tar` & `easyterm-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-02-19 21:46:20.940561 easyterm-1.0.0/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2021-11-16 15:00:47.000000 easyterm-1.0.0/LICENSE
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      872 2023-02-19 21:46:20.940561 easyterm-1.0.0/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      409 2021-11-16 15:00:52.000000 easyterm-1.0.0/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-11-16 15:00:51.000000 easyterm-1.0.0/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      703 2023-02-19 21:46:20.940561 easyterm-1.0.0/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-11-16 15:00:47.000000 easyterm-1.0.0/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-02-19 21:46:20.940561 easyterm-1.0.0/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-02-19 21:46:20.940561 easyterm-1.0.0/src/easyterm/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       84 2021-11-16 15:00:52.000000 easyterm-1.0.0/src/easyterm/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     6515 2023-02-18 23:00:29.000000 easyterm-1.0.0/src/easyterm/colorprint.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    27258 2023-02-19 21:45:04.000000 easyterm-1.0.0/src/easyterm/commandlineopt.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     6962 2023-02-18 23:00:33.000000 easyterm-1.0.0/src/easyterm/commandutils.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-02-19 21:46:20.940561 easyterm-1.0.0/src/easyterm.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      872 2023-02-19 21:46:20.000000 easyterm-1.0.0/src/easyterm.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      307 2023-02-19 21:46:20.000000 easyterm-1.0.0/src/easyterm.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-02-19 21:46:20.000000 easyterm-1.0.0/src/easyterm.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        9 2023-02-19 21:46:20.000000 easyterm-1.0.0/src/easyterm.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-05-08 10:37:53.832414 easyterm-1.0.1/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2021-11-16 15:00:47.000000 easyterm-1.0.1/LICENSE
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      872 2023-05-08 10:37:53.832414 easyterm-1.0.1/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      409 2021-11-16 15:00:52.000000 easyterm-1.0.1/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-11-16 15:00:51.000000 easyterm-1.0.1/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      703 2023-05-08 10:37:53.832414 easyterm-1.0.1/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-11-16 15:00:47.000000 easyterm-1.0.1/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-05-08 10:37:53.828414 easyterm-1.0.1/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-05-08 10:37:53.828414 easyterm-1.0.1/src/easyterm/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       84 2021-11-16 15:00:52.000000 easyterm-1.0.1/src/easyterm/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     6515 2023-02-18 23:00:29.000000 easyterm-1.0.1/src/easyterm/colorprint.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    27284 2023-03-22 14:10:49.000000 easyterm-1.0.1/src/easyterm/commandlineopt.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     6962 2023-02-18 23:00:33.000000 easyterm-1.0.1/src/easyterm/commandutils.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-05-08 10:37:53.832414 easyterm-1.0.1/src/easyterm.egg-info/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      872 2023-05-08 10:37:53.000000 easyterm-1.0.1/src/easyterm.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      307 2023-05-08 10:37:53.000000 easyterm-1.0.1/src/easyterm.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-05-08 10:37:53.000000 easyterm-1.0.1/src/easyterm.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        9 2023-05-08 10:37:53.000000 easyterm-1.0.1/src/easyterm.egg-info/top_level.txt
```

### Comparing `easyterm-1.0.0/LICENSE` & `easyterm-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easyterm-1.0.0/PKG-INFO` & `easyterm-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyterm
-Version: 1.0.0
+Version: 1.0.1
 Summary: convenient python functions for everyday use of terminal
 Home-page: https://github.com/marco-mariotti/easyterm
 Author: Marco Mariotti
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `easyterm-1.0.0/setup.cfg` & `easyterm-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easyterm
-version = 1.0.0
+version = 1.0.1
 author = Marco Mariotti
 author_email = marco.mariotti@ub.edu
 description = convenient python functions for everyday use of terminal
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/marco-mariotti/easyterm
 project_urls =
```

### Comparing `easyterm-1.0.0/src/easyterm/colorprint.py` & `easyterm-1.0.1/src/easyterm/colorprint.py`

 * *Files identical despite different names*

### Comparing `easyterm-1.0.0/src/easyterm/commandlineopt.py` & `easyterm-1.0.1/src/easyterm/commandlineopt.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .colorprint import write
 
 __all__ = [
     "command_line_options",
     "read_config_file",
     "NoTracebackError",
     "set_up_no_traceback_error",
+    "CommandLineOptions"
 ]
 
 # "CommandLineOptions", "CommandLineError"
 
 
 def custom_formatwarning(msg, *args, **kwargs):
     return str(msg) + "\n"
@@ -32,14 +33,15 @@
      option1 = {option2}.extension
      option2 = somefile  
 
      After opt.resolve_links() you have:
      option1 = somefile.extension
      option2 = somefile
 
+
     """
 
     accepted_option_chars = set(string.ascii_uppercase + string.ascii_lowercase)
     accepted_option_types = {bool, int, float, list, str}
 
     def __repr__(self):
         max_charlen = max([len(k) for k in self]) if self else 0
```

### Comparing `easyterm-1.0.0/src/easyterm/commandutils.py` & `easyterm-1.0.1/src/easyterm/commandutils.py`

 * *Files identical despite different names*

### Comparing `easyterm-1.0.0/src/easyterm.egg-info/PKG-INFO` & `easyterm-1.0.1/src/easyterm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyterm
-Version: 1.0.0
+Version: 1.0.1
 Summary: convenient python functions for everyday use of terminal
 Home-page: https://github.com/marco-mariotti/easyterm
 Author: Marco Mariotti
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

