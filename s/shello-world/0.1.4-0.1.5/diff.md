# Comparing `tmp/shello_world-0.1.4.tar.gz` & `tmp/shello_world-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shello_world-0.1.4.tar", max compression
+gzip compressed data, was "shello_world-0.1.5.tar", max compression
```

## Comparing `shello_world-0.1.4.tar` & `shello_world-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      666 2023-05-07 20:19:36.842148 shello_world-0.1.4/LICENSE
--rw-r--r--   0        0        0     1204 2023-05-07 21:18:59.996740 shello_world-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1187 2023-05-07 21:18:46.241686 shello_world-0.1.4/README.md
--rw-r--r--   0        0        0       52 2023-05-07 20:19:36.842148 shello_world-0.1.4/shello_world/__init__.py
--rw-r--r--   0        0        0     1197 2023-05-07 20:19:36.842148 shello_world-0.1.4/shello_world/shello_world.py
--rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 shello_world-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      666 2023-05-07 20:19:36.842148 shello_world-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1204 2023-05-08 20:50:23.507672 shello_world-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1200 2023-05-08 20:49:19.906290 shello_world-0.1.5/README.md
+-rw-r--r--   0        0        0       52 2023-05-07 20:19:36.842148 shello_world-0.1.5/shello_world/__init__.py
+-rw-r--r--   0        0        0     1197 2023-05-07 20:19:36.842148 shello_world-0.1.5/shello_world/shello_world.py
+-rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 shello_world-0.1.5/PKG-INFO
```

### Comparing `shello_world-0.1.4/LICENSE` & `shello_world-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shello_world-0.1.4/pyproject.toml` & `shello_world-0.1.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shello-world"
-version = "0.1.4"
+version = "0.1.5"
 description = "A few simple Python functions allow you to run shell commands from your Python code"
 authors = ["numericmaestro <re5lyltx@duck.com>"]
 readme = "README.md"
 license = "0BSD"
 homepage = "https://github.com/numericmaestro/shello-world"
 repository = "https://github.com/numericmaestro/shello-world"
 keywords = ["shell"]
```

### Comparing `shello_world-0.1.4/shello_world/shello_world.py` & `shello_world-0.1.5/shello_world/shello_world.py`

 * *Files identical despite different names*

### Comparing `shello_world-0.1.4/PKG-INFO` & `shello_world-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shello-world
-Version: 0.1.4
+Version: 0.1.5
 Summary: A few simple Python functions allow you to run shell commands from your Python code
 Home-page: https://github.com/numericmaestro/shello-world
 License: 0BSD
 Keywords: shell
 Author: numericmaestro
 Author-email: re5lyltx@duck.com
 Requires-Python: >=3.11,<4.0
@@ -22,41 +22,54 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: System :: System Shells
 Classifier: Topic :: System :: Systems Administration
 Project-URL: Repository, https://github.com/numericmaestro/shello-world
 Description-Content-Type: text/markdown
 
-# Shello-world: run shell commands from your Python code via simple functions
+
+# Shello-world: simple Python functions to run shell commands
 A few simple Python functions allow you to run shell commands from your Python code.
 
 ## Why shello-world?
-It isn't a big library or framework. If you want a quick solution, you could prefer shello-world.
+It is a simple and quick solution if you don't want to use a big library or framework.
 
 ## Usage
 Let's take a look at a simple example below:
 ```python
 from shello_world import shell_execute, shell_run
 
 # Both functions work similarly
 
-# shell_run runs a command directly in your shell
-# Change color to green
-shell_run("color a")
-# You will see executing ipconfig in your shell just like you'd enter it
-ipconfig = shell_run("ipconfig")
-# But the function doesn't return anything
-print(ipconfig is None) # True
-
-# shell_execute doesn't print executing in your shell by default
-systeminfo = shell_execute("systeminfo") # This line doesn't print anything
+# Use shell_run if you want to run a command
+# directly in your shell, like you'd enter it
+shell_run("color a") # Change font color to green
+# But shell_run doesn't return anything
+output = shell_run("echo 'This text is printed in the shell'")
+print(output is None) # True
+
+# Use shell_execute to get output to use it in your code
+# shell_execute doesn't print anything
+systeminfo = shell_execute("systeminfo")
 # But it always returns result as a string
 print(systeminfo.upper())
-print(systeminfo.split())
+#
+# HOST NAME:
+# OS NAME:
+# OS VERSION:
+# ...
+#
 ```
 
 ## Installation
-You can install this library with ```pip install shello-world``` command.
+### pip
+```
+pip install shello-world
+```
+### poetry
+```
+poetry add shello-world
+```
 
 ## Links
 [PyPI](https://pypi.org/project/shello-world/)  
 [GitHub](https://github.com/numericmaestro/shello-world)
```

