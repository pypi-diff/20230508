# Comparing `tmp/firepup650-1.0.8.tar.gz` & `tmp/firepup650-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firepup650-1.0.8.tar", last modified: Wed Apr 26 19:03:59 2023, max compression
+gzip compressed data, was "firepup650-1.0.9.tar", last modified: Mon May  8 16:32:25 2023, max compression
```

## Comparing `firepup650-1.0.8.tar` & `firepup650-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-26 19:03:59.631296 firepup650-1.0.8/
--rw-r--r--   0 runner    (1000) runner    (1000)     1072 2021-11-16 19:34:41.000000 firepup650-1.0.8/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1764 2023-04-26 19:03:59.631296 firepup650-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      753 2023-04-26 19:03:11.000000 firepup650-1.0.8/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      310 2023-04-26 19:03:04.000000 firepup650-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)      928 2023-04-26 19:03:59.631296 firepup650-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-26 16:38:44.000000 firepup650-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-26 19:03:59.567296 firepup650-1.0.8/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-26 19:03:59.623296 firepup650-1.0.8/src/firepup650/
--rw-r--r--   0 runner    (1000) runner    (1000)    12877 2023-04-26 17:18:14.000000 firepup650-1.0.8/src/firepup650/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-26 19:03:59.627296 firepup650-1.0.8/src/firepup650.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1764 2023-04-26 19:03:59.000000 firepup650-1.0.8/src/firepup650.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      267 2023-04-26 19:03:59.000000 firepup650-1.0.8/src/firepup650.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-26 19:03:59.000000 firepup650-1.0.8/src/firepup650.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-04-26 19:03:59.000000 firepup650-1.0.8/src/firepup650.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-04-26 19:03:59.000000 firepup650-1.0.8/src/firepup650.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-08 16:32:25.015813 firepup650-1.0.9/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1072 2021-11-16 19:34:41.000000 firepup650-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1825 2023-05-08 16:32:25.015813 firepup650-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      798 2023-05-08 16:31:57.000000 firepup650-1.0.9/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      310 2023-05-08 16:31:18.000000 firepup650-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)      928 2023-05-08 16:32:25.019813 firepup650-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-26 16:38:44.000000 firepup650-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-08 16:32:25.015813 firepup650-1.0.9/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-08 16:32:25.015813 firepup650-1.0.9/src/firepup650/
+-rw-r--r--   0 runner    (1000) runner    (1000)    13143 2023-05-08 16:28:09.000000 firepup650-1.0.9/src/firepup650/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-08 16:32:25.015813 firepup650-1.0.9/src/firepup650.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1825 2023-05-08 16:32:24.000000 firepup650-1.0.9/src/firepup650.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      267 2023-05-08 16:32:24.000000 firepup650-1.0.9/src/firepup650.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-08 16:32:24.000000 firepup650-1.0.9/src/firepup650.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-05-08 16:32:24.000000 firepup650-1.0.9/src/firepup650.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-05-08 16:32:24.000000 firepup650-1.0.9/src/firepup650.egg-info/top_level.txt
```

### Comparing `firepup650-1.0.8/LICENSE` & `firepup650-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `firepup650-1.0.8/PKG-INFO` & `firepup650-1.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: firepup650
-Version: 1.0.8
+Version: 1.0.9
 Summary: Package containing various shorthand things I use, and a few imports I almost always use
 Home-page: https://github.com/F1repup650/firepup650-PYPI
 Author: Firepup650
 Author-email: firepyp650@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/F1repup650/firepup650-PYPI/issues
 Project-URL: replit, https://replit.com/@Firepup650/firepup650-PYPI-Package
 Description: # Firepup650
         Package containing various shorthand things I use, and a few imports I almost always use
         #### Change log:
+        ###### v.1.0.9:
+        Small tweaks, nothing major.
         ###### v.1.0.8:
         Can't install collections. This better fix it.
         ###### v.1.0.7:
         Adds `console` (class), `bcolors` (class), and `Color` (function). Fixes type hinting on various things (Lots of thanks to @bigminiboss!).
         ###### v.1.0.6:
         Hopefully, fixes an issue where the package doesn't install it's dependencies (Again. Hopefully.)
         ###### v.1.0.5:
```

### Comparing `firepup650-1.0.8/README.md` & `firepup650-1.0.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Firepup650
 Package containing various shorthand things I use, and a few imports I almost always use
 #### Change log:
+###### v.1.0.9:
+Small tweaks, nothing major.
 ###### v.1.0.8:
 Can't install collections. This better fix it.
 ###### v.1.0.7:
 Adds `console` (class), `bcolors` (class), and `Color` (function). Fixes type hinting on various things (Lots of thanks to @bigminiboss!).
 ###### v.1.0.6:
 Hopefully, fixes an issue where the package doesn't install it's dependencies (Again. Hopefully.)
 ###### v.1.0.5:
```

### Comparing `firepup650-1.0.8/setup.cfg` & `firepup650-1.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = firepup650
-version = 1.0.8
+version = 1.0.9
 author = Firepup650
 author_email = firepyp650@gmail.com
 description = Package containing various shorthand things I use, and a few imports I almost always use
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/F1repup650/firepup650-PYPI
 project_urls =
```

### Comparing `firepup650-1.0.8/src/firepup650/__init__.py` & `firepup650-1.0.9/src/firepup650/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,40 +149,44 @@
     # Returns:
       None
 
     # Raises:
       None"""
     r.seed(seed, version)
 
-setattr(Iterable, "__class_getitem__", lambda x:None)
+
+setattr(Iterable, "__class_getitem__", lambda x: None)
 T = TypeVar("T")
 
+
 def robj(iterable: Iterable[T]) -> T:
     """# Function: robj
       Returns a random object from the provided iterable
     # Input:
       iterable: Iterable[T] - Any valid Iterable
 
     # Returns:
       T - A random object of type `T` from the provided iterable
 
     # Raises:
       None"""
     return r.choice(iterable)
 
 
-def Color(r=0, g=0, b=0, bar=False, bcolor=False):
+def Color(r: int = 0, g: int = 0, b: int = 0, bcolor: bool = False) -> None or str:
     """# Function: Color
       Set the text to a specific color.
     # Inputs:
-      seed: any - The seed, defaults to None
-      version: int - Version of the seed (1 or 2), defaults to 2
+      r: int - The red value, range of 0-255, defaults to 0
+      g: int - The green value, range of 0-255, defaults to 0
+      b: int - The blue value, range of 0-255, defaults to 0
+      bcolor: bool - Wether to return the color as a str, defaults to False
 
     # Returns:
-      None
+      None or str - The color code if `bcolor` is True. Otherwise, returns nothing
 
     # Raises:
       None"""
     if r < 0:
         r = 0
     if r > 255:
         r = 255
@@ -190,18 +194,15 @@
         g = 0
     if g > 255:
         g = 255
     if b < 0:
         b = 0
     if b > 255:
         b = 255
-    if bar == True:
-        print("\003[0m")
-        print(f"\033[38;2;{r};{g};{b}m")
-    elif bcolor == True:
+    if bcolor == True:
         return f"\033[38;2;{r};{g};{b}m"
     else:
         print("\003[0m")
         print(f"\033[38;2;{r};{g};{b}m")
 
 
 class bcolors:
@@ -356,15 +357,15 @@
 
         Prints the values to a stream, or to sys.stdout by default.
         Optional keyword arguments:
         file:  a file-like object (stream); defaults to the current sys.stdout.
         sep:   string inserted between values, default a space.
         end:   string appended after the last value, default a newline.
         flush: whether to forcibly flush the stream."""
-        print(*args)
+        print(*args, **kwargs)
 
     def debug(*args, **kwargs) -> None:
         """print(value, ..., sep=' ', end='\n', file=sys.stdout, flush=False)
 
         Prints the values to a stream, or to sys.stdout by default.
         Optional keyword arguments:
         file:  a file-like object (stream); defaults to the current sys.stdout.
@@ -443,19 +444,19 @@
         # Returns:
           None
 
         # Raises:
           None"""
         console._counters[label] = 0
 
-    def clear() -> None:
+    def clear(ascii: bool = False) -> None:
         """# Function: console.clear
           Clears the screen
         # Inputs:
-          None
+          ascii: bool - Wether to use ASCII to clear the screen, defaults to False
 
         # Returns:
           None
 
         # Raises:
           None"""
         clear(ascii)
```

### Comparing `firepup650-1.0.8/src/firepup650.egg-info/PKG-INFO` & `firepup650-1.0.9/src/firepup650.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: firepup650
-Version: 1.0.8
+Version: 1.0.9
 Summary: Package containing various shorthand things I use, and a few imports I almost always use
 Home-page: https://github.com/F1repup650/firepup650-PYPI
 Author: Firepup650
 Author-email: firepyp650@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/F1repup650/firepup650-PYPI/issues
 Project-URL: replit, https://replit.com/@Firepup650/firepup650-PYPI-Package
 Description: # Firepup650
         Package containing various shorthand things I use, and a few imports I almost always use
         #### Change log:
+        ###### v.1.0.9:
+        Small tweaks, nothing major.
         ###### v.1.0.8:
         Can't install collections. This better fix it.
         ###### v.1.0.7:
         Adds `console` (class), `bcolors` (class), and `Color` (function). Fixes type hinting on various things (Lots of thanks to @bigminiboss!).
         ###### v.1.0.6:
         Hopefully, fixes an issue where the package doesn't install it's dependencies (Again. Hopefully.)
         ###### v.1.0.5:
```

