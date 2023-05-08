# Comparing `tmp/pihole5-list-tool-0.6.1.tar.gz` & `tmp/pihole5-list-tool-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pihole5-list-tool-0.6.1.tar", last modified: Tue Oct 25 14:43:28 2022, max compression
+gzip compressed data, was "pihole5-list-tool-0.6.2.tar", last modified: Mon May  8 20:18:42 2023, max compression
```

## Comparing `pihole5-list-tool-0.6.1.tar` & `pihole5-list-tool-0.6.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2022-10-25 14:43:28.479364 pihole5-list-tool-0.6.1/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1064 2020-08-14 17:35:25.000000 pihole5-list-tool-0.6.1/LICENSE
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     4845 2022-10-25 14:43:28.479364 pihole5-list-tool-0.6.1/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3999 2022-10-25 14:02:24.000000 pihole5-list-tool-0.6.1/README.md
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2022-10-25 14:43:28.479364 pihole5-list-tool-0.6.1/ph5lt/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        0 2020-10-26 02:08:10.000000 pihole5-list-tool-0.6.1/ph5lt/__init__.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      228 2022-10-25 14:31:26.000000 pihole5-list-tool-0.6.1/ph5lt/__main__.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     4648 2022-10-25 14:30:17.000000 pihole5-list-tool-0.6.1/ph5lt/allowlists.py
--rwxrwxr-x   0 jesse     (1000) jesse     (1000)     4169 2022-10-25 13:57:52.000000 pihole5-list-tool-0.6.1/ph5lt/app.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      729 2022-10-25 14:42:28.000000 pihole5-list-tool-0.6.1/ph5lt/banner.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     4767 2022-10-25 14:30:24.000000 pihole5-list-tool-0.6.1/ph5lt/blocklists.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      339 2020-10-26 02:08:10.000000 pihole5-list-tool-0.6.1/ph5lt/constants.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8116 2022-10-25 13:43:20.000000 pihole5-list-tool-0.6.1/ph5lt/prompts.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     6742 2022-10-25 13:57:52.000000 pihole5-list-tool-0.6.1/ph5lt/stats.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     4196 2022-10-25 13:57:52.000000 pihole5-list-tool-0.6.1/ph5lt/utils.py
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2022-10-25 14:43:28.479364 pihole5-list-tool-0.6.1/pihole5_list_tool.egg-info/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     4845 2022-10-25 14:43:28.000000 pihole5-list-tool-0.6.1/pihole5_list_tool.egg-info/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      455 2022-10-25 14:43:28.000000 pihole5-list-tool-0.6.1/pihole5_list_tool.egg-info/SOURCES.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2022-10-25 14:43:28.000000 pihole5-list-tool-0.6.1/pihole5_list_tool.egg-info/dependency_links.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       54 2022-10-25 14:43:28.000000 pihole5-list-tool-0.6.1/pihole5_list_tool.egg-info/entry_points.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       46 2022-10-25 14:43:28.000000 pihole5-list-tool-0.6.1/pihole5_list_tool.egg-info/requires.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        6 2022-10-25 14:43:28.000000 pihole5-list-tool-0.6.1/pihole5_list_tool.egg-info/top_level.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      247 2022-10-25 14:43:28.479364 pihole5-list-tool-0.6.1/setup.cfg
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1880 2022-10-25 13:44:34.000000 pihole5-list-tool-0.6.1/setup.py
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-08 20:18:42.373634 pihole5-list-tool-0.6.2/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1064 2020-08-14 17:35:25.000000 pihole5-list-tool-0.6.2/LICENSE
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     4845 2023-05-08 20:18:42.373634 pihole5-list-tool-0.6.2/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3999 2022-10-25 14:02:24.000000 pihole5-list-tool-0.6.2/README.md
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-08 20:18:42.369634 pihole5-list-tool-0.6.2/ph5lt/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        0 2020-10-26 02:08:10.000000 pihole5-list-tool-0.6.2/ph5lt/__init__.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      228 2022-10-25 14:31:26.000000 pihole5-list-tool-0.6.2/ph5lt/__main__.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     4670 2023-05-08 19:55:59.000000 pihole5-list-tool-0.6.2/ph5lt/allowlists.py
+-rwxrwxr-x   0 jesse     (1000) jesse     (1000)     4169 2022-10-25 13:57:52.000000 pihole5-list-tool-0.6.2/ph5lt/app.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      729 2023-05-08 20:16:15.000000 pihole5-list-tool-0.6.2/ph5lt/banner.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     4789 2023-05-08 19:56:59.000000 pihole5-list-tool-0.6.2/ph5lt/blocklists.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      339 2020-10-26 02:08:10.000000 pihole5-list-tool-0.6.2/ph5lt/constants.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     7613 2023-05-08 20:11:52.000000 pihole5-list-tool-0.6.2/ph5lt/prompts.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6742 2022-10-25 13:57:52.000000 pihole5-list-tool-0.6.2/ph5lt/stats.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     4196 2022-10-25 13:57:52.000000 pihole5-list-tool-0.6.2/ph5lt/utils.py
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-08 20:18:42.373634 pihole5-list-tool-0.6.2/pihole5_list_tool.egg-info/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     4845 2023-05-08 20:18:42.000000 pihole5-list-tool-0.6.2/pihole5_list_tool.egg-info/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      455 2023-05-08 20:18:42.000000 pihole5-list-tool-0.6.2/pihole5_list_tool.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-08 20:18:42.000000 pihole5-list-tool-0.6.2/pihole5_list_tool.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       54 2023-05-08 20:18:42.000000 pihole5-list-tool-0.6.2/pihole5_list_tool.egg-info/entry_points.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       46 2023-05-08 20:18:42.000000 pihole5-list-tool-0.6.2/pihole5_list_tool.egg-info/requires.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        6 2023-05-08 20:18:42.000000 pihole5-list-tool-0.6.2/pihole5_list_tool.egg-info/top_level.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      247 2023-05-08 20:18:42.373634 pihole5-list-tool-0.6.2/setup.cfg
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1880 2022-10-25 13:44:34.000000 pihole5-list-tool-0.6.2/setup.py
```

### Comparing `pihole5-list-tool-0.6.1/LICENSE` & `pihole5-list-tool-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pihole5-list-tool-0.6.1/PKG-INFO` & `pihole5-list-tool-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pihole5-list-tool
-Version: 0.6.1
+Version: 0.6.2
 Summary: A tool for quickly and easily bulk adding allowlists and ad/blocklists to a Pi-hole 5 installation
 Home-page: https://github.com/jessedp/pihole5-list-tool
 Author: jessedp
 Author-email: jessedp@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/jessedp/pihole5-list-tool/issues
 Project-URL: Source Code, https://github.com/jessedp/pihole5-list-tool
```

### Comparing `pihole5-list-tool-0.6.1/README.md` & `pihole5-list-tool-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pihole5-list-tool-0.6.1/ph5lt/allowlists.py` & `pihole5-list-tool-0.6.2/ph5lt/allowlists.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,16 @@
     if source == constants.PASTE:
         import_list = prompts.ask_paste()
         import_list = utils.process_lines(
             import_list, "Pasted content", utils.validate_host
         )
 
     if len(import_list) == 0:
-        utils.die("No valid urls found, try again")
+        utils.warn("No valid urls found, try again")
+        return False
 
     if not prompts.confirm(f"Add {len(import_list)} white lists?"):
         return False
 
     added = 0
     exists = 0
```

### Comparing `pihole5-list-tool-0.6.1/ph5lt/app.py` & `pihole5-list-tool-0.6.2/ph5lt/app.py`

 * *Files identical despite different names*

### Comparing `pihole5-list-tool-0.6.1/ph5lt/banner.py` & `pihole5-list-tool-0.6.2/ph5lt/banner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ silly ansi banner"""
 
 from colors import color
 
 from ph5lt import utils
 
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 
 
 def display():
     """display the banner"""
     print(color("    ┌──────────────────────────────────────────┐", fg="#b61042"))
     print(
         color("    │       ", fg="#b61042")
```

### Comparing `pihole5-list-tool-0.6.1/ph5lt/blocklists.py` & `pihole5-list-tool-0.6.2/ph5lt/blocklists.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,16 @@
             import_list = utils.process_lines(import_file.read(), f"File: {fname}")
 
     if source == constants.PASTE:
         import_list = prompts.ask_paste()
         import_list = utils.process_lines(import_list, "Pasted content")
 
     if len(import_list) == 0:
-        utils.die("No valid urls found, try again")
+        utils.warn("No valid urls found, try again")
+        return False
 
     if not prompts.confirm(f"Add {len(import_list)} block lists?"):
         return False
 
     added = 0
     exists = 0
     for item in import_list:
```

### Comparing `pihole5-list-tool-0.6.1/ph5lt/prompts.py` & `pihole5-list-tool-0.6.2/ph5lt/prompts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """ prompts for inquirer """
 import os
 import sqlite3
 from InquirerPy import prompt
 from InquirerPy.separator import Separator
-from prompt_toolkit.validation import ValidationError, Validator
 
 from ph5lt import constants
 from ph5lt import utils
 
 
 def check_db(path):
     """validate we have a good file"""
@@ -26,24 +25,14 @@
         conn.close()
     except (sqlite3.DatabaseError, sqlite3.OperationalError):
         utils.warn(" IS NOT A PI-HOLE GRAVITY DB!")
         return False
     return True
 
 
-class ValidateEditor(Validator):
-    """Class to validator "editor" types since that's broken in current PyInquirer"""
-
-    def validate(self, document):
-        if document.text and len(document.text.split("\n")) <= 1:
-            raise ValidationError(
-                message="Must be at least 1 line", cursor_position=len(document.text)
-            )
-
-
 def key_prompt(questions):
     """prompt wrapper to handle ctrl+c"""
     resp = prompt(questions)
     if len(resp) != len(questions):
         raise KeyboardInterrupt
     return resp
 
@@ -219,19 +208,18 @@
 
 
 def ask_paste():
     """prompt for acquiring pasted list"""
     questions = [
         {
             "name": "content",
-            "type": "editor",
-            "message": "Opening editor",
-            # lambda text: len(text.split('\n')) >= 1 or 'Must be at least 1 line',
-            "validate": ValidateEditor,
-            "eargs": {"editor": "default", "ext": ".tmp"},
+            "type": "input",
+            "message": "Please Paste your of URLS, then:",
+            "multiline": True,
+            "instruction": "ESC + Enter to continue",
         }
     ]
     result = key_prompt(questions)
     return result["content"]
 
 
 def confirm(message, default="y"):
```

### Comparing `pihole5-list-tool-0.6.1/ph5lt/stats.py` & `pihole5-list-tool-0.6.2/ph5lt/stats.py`

 * *Files identical despite different names*

### Comparing `pihole5-list-tool-0.6.1/ph5lt/utils.py` & `pihole5-list-tool-0.6.2/ph5lt/utils.py`

 * *Files identical despite different names*

### Comparing `pihole5-list-tool-0.6.1/pihole5_list_tool.egg-info/PKG-INFO` & `pihole5-list-tool-0.6.2/pihole5_list_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pihole5-list-tool
-Version: 0.6.1
+Version: 0.6.2
 Summary: A tool for quickly and easily bulk adding allowlists and ad/blocklists to a Pi-hole 5 installation
 Home-page: https://github.com/jessedp/pihole5-list-tool
 Author: jessedp
 Author-email: jessedp@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/jessedp/pihole5-list-tool/issues
 Project-URL: Source Code, https://github.com/jessedp/pihole5-list-tool
```

### Comparing `pihole5-list-tool-0.6.1/setup.py` & `pihole5-list-tool-0.6.2/setup.py`

 * *Files identical despite different names*

