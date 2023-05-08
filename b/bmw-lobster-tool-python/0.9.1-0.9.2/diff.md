# Comparing `tmp/bmw-lobster-tool-python-0.9.1.tar.gz` & `tmp/bmw-lobster-tool-python-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-tool-python-0.9.1.tar", last modified: Wed May  3 14:22:58 2023, max compression
+gzip compressed data, was "bmw-lobster-tool-python-0.9.2.tar", last modified: Mon May  8 15:06:40 2023, max compression
```

## Comparing `bmw-lobster-tool-python-0.9.1.tar` & `bmw-lobster-tool-python-0.9.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:58.772386 bmw-lobster-tool-python-0.9.1/
--rw-r--r--   0 florian   (1000) florian   (1000)     1542 2023-05-03 14:22:58.772386 bmw-lobster-tool-python-0.9.1/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      609 2023-05-03 14:09:11.000000 bmw-lobster-tool-python-0.9.1/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:58.772386 bmw-lobster-tool-python-0.9.1/bmw_lobster_tool_python.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     1542 2023-05-03 14:22:58.000000 bmw-lobster-tool-python-0.9.1/bmw_lobster_tool_python.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      366 2023-05-03 14:22:58.000000 bmw-lobster-tool-python-0.9.1/bmw_lobster_tool_python.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-03 14:22:58.000000 bmw-lobster-tool-python-0.9.1/bmw_lobster_tool_python.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       68 2023-05-03 14:22:58.000000 bmw-lobster-tool-python-0.9.1/bmw_lobster_tool_python.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-03 14:22:58.000000 bmw-lobster-tool-python-0.9.1/bmw_lobster_tool_python.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-05-03 14:22:58.000000 bmw-lobster-tool-python-0.9.1/bmw_lobster_tool_python.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:58.768386 bmw-lobster-tool-python-0.9.1/lobster/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:58.768386 bmw-lobster-tool-python-0.9.1/lobster/tools/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:58.772386 bmw-lobster-tool-python-0.9.1/lobster/tools/python/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-03 14:09:11.000000 bmw-lobster-tool-python-0.9.1/lobster/tools/python/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)    12329 2023-05-03 14:09:11.000000 bmw-lobster-tool-python-0.9.1/lobster/tools/python/python.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-03 14:22:58.772386 bmw-lobster-tool-python-0.9.1/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2273 2023-05-03 14:09:11.000000 bmw-lobster-tool-python-0.9.1/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:40.645497 bmw-lobster-tool-python-0.9.2/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1542 2023-05-08 15:06:40.645497 bmw-lobster-tool-python-0.9.2/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      609 2023-05-08 15:03:18.000000 bmw-lobster-tool-python-0.9.2/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:40.641497 bmw-lobster-tool-python-0.9.2/bmw_lobster_tool_python.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1542 2023-05-08 15:06:40.000000 bmw-lobster-tool-python-0.9.2/bmw_lobster_tool_python.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      366 2023-05-08 15:06:40.000000 bmw-lobster-tool-python-0.9.2/bmw_lobster_tool_python.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-08 15:06:40.000000 bmw-lobster-tool-python-0.9.2/bmw_lobster_tool_python.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       68 2023-05-08 15:06:40.000000 bmw-lobster-tool-python-0.9.2/bmw_lobster_tool_python.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-08 15:06:40.000000 bmw-lobster-tool-python-0.9.2/bmw_lobster_tool_python.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-05-08 15:06:40.000000 bmw-lobster-tool-python-0.9.2/bmw_lobster_tool_python.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:40.641497 bmw-lobster-tool-python-0.9.2/lobster/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:40.641497 bmw-lobster-tool-python-0.9.2/lobster/tools/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:40.641497 bmw-lobster-tool-python-0.9.2/lobster/tools/python/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:40.000000 bmw-lobster-tool-python-0.9.2/lobster/tools/python/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)    12276 2023-05-08 15:06:40.000000 bmw-lobster-tool-python-0.9.2/lobster/tools/python/python.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-08 15:06:40.645497 bmw-lobster-tool-python-0.9.2/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2273 2023-05-08 15:03:18.000000 bmw-lobster-tool-python-0.9.2/setup.py
```

### Comparing `bmw-lobster-tool-python-0.9.1/PKG-INFO` & `bmw-lobster-tool-python-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-python
-Version: 0.9.1
+Version: 0.9.2
 Summary: LOBSTER Tool for Python3
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-tool-python-0.9.1/README.md` & `bmw-lobster-tool-python-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `bmw-lobster-tool-python-0.9.1/bmw_lobster_tool_python.egg-info/PKG-INFO` & `bmw-lobster-tool-python-0.9.2/bmw_lobster_tool_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-python
-Version: 0.9.1
+Version: 0.9.2
 Summary: LOBSTER Tool for Python3
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-tool-python-0.9.1/lobster/tools/python/python.py` & `bmw-lobster-tool-python-0.9.2/lobster/tools/python/python.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,16 +112,14 @@
         # If all functions in the class have a tag, then this class
         # doesn't require tracing, as everything in it is. First lets
         # generate the tracing for the items.
         # TODO
         class_contents = []
         for node in self.children:
             node.to_lobster(class_contents)
-        for item in class_contents:
-            pass
         items += class_contents
 
         l_item = Implementation(tag      = Tracing_Tag("python",
                                                        self.fqn()),
                                 location = self.location,
                                 language = "Python",
                                 kind     = self.kind,
```

### Comparing `bmw-lobster-tool-python-0.9.1/setup.py` & `bmw-lobster-tool-python-0.9.2/setup.py`

 * *Files identical despite different names*

