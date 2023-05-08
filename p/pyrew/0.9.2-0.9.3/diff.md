# Comparing `tmp/pyrew-0.9.2.tar.gz` & `tmp/pyrew-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrew-0.9.2.tar", last modified: Sat Apr 22 09:09:07 2023, max compression
+gzip compressed data, was "pyrew-0.9.3.tar", last modified: Sat Apr 22 09:36:53 2023, max compression
```

## Comparing `pyrew-0.9.2.tar` & `pyrew-0.9.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:09:07.918482 pyrew-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-22 09:09:07.918482 pyrew-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-22 09:08:54.000000 pyrew-0.9.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-22 09:08:54.000000 pyrew-0.9.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:09:07.914482 pyrew-0.9.2/pyrew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-22 09:09:07.000000 pyrew-0.9.2/pyrew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-22 09:09:07.000000 pyrew-0.9.2/pyrew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:09:07.000000 pyrew-0.9.2/pyrew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-22 09:09:07.000000 pyrew-0.9.2/pyrew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-04-22 09:08:54.000000 pyrew-0.9.2/pyrew.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 09:09:07.918482 pyrew-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-22 09:08:54.000000 pyrew-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:36:53.617206 pyrew-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-22 09:36:53.617206 pyrew-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-22 09:36:35.000000 pyrew-0.9.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-22 09:36:35.000000 pyrew-0.9.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:36:53.617206 pyrew-0.9.3/pyrew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-22 09:36:53.000000 pyrew-0.9.3/pyrew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-22 09:36:53.000000 pyrew-0.9.3/pyrew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:36:53.000000 pyrew-0.9.3/pyrew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-22 09:36:53.000000 pyrew-0.9.3/pyrew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-22 09:36:35.000000 pyrew-0.9.3/pyrew.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 09:36:53.617206 pyrew-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-22 09:36:35.000000 pyrew-0.9.3/setup.py
```

### Comparing `pyrew-0.9.2/PKG-INFO` & `pyrew-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrew
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Python library for writing shorter and more efficient Python code.
 Home-page: https://github.com/AquaQuokka/pyrew
 Author: AquaQuokka
 License: BSD-3-Clause
 
 =============
 Pyrew
```

### Comparing `pyrew-0.9.2/pyrew.egg-info/PKG-INFO` & `pyrew-0.9.3/pyrew.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrew
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Python library for writing shorter and more efficient Python code.
 Home-page: https://github.com/AquaQuokka/pyrew
 Author: AquaQuokka
 License: BSD-3-Clause
 
 =============
 Pyrew
```

### Comparing `pyrew-0.9.2/pyrew.py` & `pyrew-0.9.3/pyrew.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,16 +13,26 @@
 try:
     import colorama
     colorama.init()
 
 except ImportError:
     pass
 
+class FailureReturnValueError(ValueError):
+    def __init__(self, value):
+        self.value = value
+        super().__init__(f"\"{value}\" is not a valid return value for a failure")
+
+class SuccessReturnValueError(ValueError):
+    def __init__(self, value):
+        self.value = value
+        super().__init__(f"\"{value}\" is not a valid return value for a success")
+
 class MultiException(Exception):
-    def __init__(self, exceptions):
+    def __init__(self, exceptions: int):
         self.exceptions = exceptions
         super().__init__(f"{len(exceptions)} exceptions occurred")
 
 class Pyrew:
     @staticmethod
     def write(*args, end='\n'):
 
@@ -256,14 +266,46 @@
                     
                     else:
                         return False
                 
                 results.append(validate_email(email))
 
             return results
+        
+    @staticmethod
+    def success(*ids):
+
+        if ids:
+            if len(ids) != 1:
+                raise ValueError("Invalid number of return values: %d" % len(ids))
+        
+        for i in ids:
+            if i != 0:
+                raise SuccessReturnValueError(value=int(i))
+
+        else:
+            return 0
+            
+
+    
+    @staticmethod
+    def failure(*ids):
+
+        if ids:
+            for i in ids:
+                if i != 0:
+                    return int(i)
+                
+            else:
+                raise FailureReturnValueError(value=int(i))
+            
+        else:
+            return int(1)
+
+
 
 builtins.print = Pyrew().write
 
 builtins.__dict__['true'] = True
 builtins.__dict__['false'] = False
 builtins.__dict__['string'] = str
 builtins.__dict__['integer'] = int
```

