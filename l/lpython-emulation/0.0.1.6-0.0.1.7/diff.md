# Comparing `tmp/lpython_emulation-0.0.1.6.tar.gz` & `tmp/lpython_emulation-0.0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpython_emulation-0.0.1.6.tar", last modified: Sat May  6 13:25:42 2023, max compression
+gzip compressed data, was "lpython_emulation-0.0.1.7.tar", last modified: Mon May  8 18:25:14 2023, max compression
```

## Comparing `lpython_emulation-0.0.1.6.tar` & `lpython_emulation-0.0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-05-06 13:25:42.345970 lpython_emulation-0.0.1.6/
--rw-r--r--   0 ubaid      (501) staff       (20)     1072 2023-04-21 16:22:30.000000 lpython_emulation-0.0.1.6/LICENSE
--rw-r--r--   0 ubaid      (501) staff       (20)     1019 2023-05-06 13:25:42.345794 lpython_emulation-0.0.1.6/PKG-INFO
--rw-r--r--   0 ubaid      (501) staff       (20)      556 2023-04-30 17:58:09.000000 lpython_emulation-0.0.1.6/README.md
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-05-06 13:25:42.344902 lpython_emulation-0.0.1.6/lpython/
--rw-r--r--   0 ubaid      (501) staff       (20)        0 2023-05-06 13:19:25.000000 lpython_emulation-0.0.1.6/lpython/__init__.py
--rw-r--r--   0 ubaid      (501) staff       (20)     7587 2023-04-21 16:22:30.000000 lpython_emulation-0.0.1.6/lpython/goto.py
--rw-r--r--   0 ubaid      (501) staff       (20)    15499 2023-04-30 17:14:24.000000 lpython_emulation-0.0.1.6/lpython/lpython.py
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-05-06 13:25:42.345425 lpython_emulation-0.0.1.6/lpython_emulation.egg-info/
--rw-r--r--   0 ubaid      (501) staff       (20)     1019 2023-05-06 13:25:42.000000 lpython_emulation-0.0.1.6/lpython_emulation.egg-info/PKG-INFO
--rw-r--r--   0 ubaid      (501) staff       (20)      245 2023-05-06 13:25:42.000000 lpython_emulation-0.0.1.6/lpython_emulation.egg-info/SOURCES.txt
--rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-05-06 13:25:42.000000 lpython_emulation-0.0.1.6/lpython_emulation.egg-info/dependency_links.txt
--rw-r--r--   0 ubaid      (501) staff       (20)        8 2023-05-06 13:25:42.000000 lpython_emulation-0.0.1.6/lpython_emulation.egg-info/top_level.txt
--rw-r--r--   0 ubaid      (501) staff       (20)       38 2023-05-06 13:25:42.346016 lpython_emulation-0.0.1.6/setup.cfg
--rw-r--r--   0 ubaid      (501) staff       (20)     1779 2023-05-06 13:24:48.000000 lpython_emulation-0.0.1.6/setup.py
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-05-08 18:25:14.757469 lpython_emulation-0.0.1.7/
+-rw-r--r--   0 ubaid      (501) staff       (20)     1072 2023-05-06 13:31:30.000000 lpython_emulation-0.0.1.7/LICENSE
+-rw-r--r--   0 ubaid      (501) staff       (20)     1019 2023-05-08 18:25:14.757332 lpython_emulation-0.0.1.7/PKG-INFO
+-rw-r--r--   0 ubaid      (501) staff       (20)      556 2023-05-06 13:31:30.000000 lpython_emulation-0.0.1.7/README.md
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-05-08 18:25:14.755997 lpython_emulation-0.0.1.7/lpython/
+-rw-r--r--   0 ubaid      (501) staff       (20)      225 2023-05-06 13:44:18.000000 lpython_emulation-0.0.1.7/lpython/__init__.py
+-rw-r--r--   0 ubaid      (501) staff       (20)     7587 2023-05-06 13:44:18.000000 lpython_emulation-0.0.1.7/lpython/goto.py
+-rw-r--r--   0 ubaid      (501) staff       (20)    15500 2023-05-08 18:23:59.000000 lpython_emulation-0.0.1.7/lpython/lpython.py
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-05-08 18:25:14.757087 lpython_emulation-0.0.1.7/lpython_emulation.egg-info/
+-rw-r--r--   0 ubaid      (501) staff       (20)     1019 2023-05-08 18:25:14.000000 lpython_emulation-0.0.1.7/lpython_emulation.egg-info/PKG-INFO
+-rw-r--r--   0 ubaid      (501) staff       (20)      245 2023-05-08 18:25:14.000000 lpython_emulation-0.0.1.7/lpython_emulation.egg-info/SOURCES.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-05-08 18:25:14.000000 lpython_emulation-0.0.1.7/lpython_emulation.egg-info/dependency_links.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)        8 2023-05-08 18:25:14.000000 lpython_emulation-0.0.1.7/lpython_emulation.egg-info/top_level.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)       38 2023-05-08 18:25:14.757510 lpython_emulation-0.0.1.7/setup.cfg
+-rw-r--r--   0 ubaid      (501) staff       (20)     1794 2023-05-08 18:21:48.000000 lpython_emulation-0.0.1.7/setup.py
```

### Comparing `lpython_emulation-0.0.1.6/LICENSE` & `lpython_emulation-0.0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lpython_emulation-0.0.1.6/PKG-INFO` & `lpython_emulation-0.0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpython_emulation
-Version: 0.0.1.6
+Version: 0.0.1.7
 Summary: Package for adding type information to python
 Home-page: https://github.com/Shaikh-Ubaid/lpython_packages
 Author: Ondrej Certik
 Author-email: ondrej@certik.us
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lpython_emulation-0.0.1.6/README.md` & `lpython_emulation-0.0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `lpython_emulation-0.0.1.6/lpython/goto.py` & `lpython_emulation-0.0.1.7/lpython/goto.py`

 * *Files identical despite different names*

### Comparing `lpython_emulation-0.0.1.6/lpython/lpython.py` & `lpython_emulation-0.0.1.7/lpython/lpython.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from inspect import getfullargspec, getcallargs, isclass
 import os
 import ctypes
 import platform
 from dataclasses import dataclass as py_dataclass, is_dataclass as py_is_dataclass
-from goto import with_goto
+from .goto import with_goto
 
 # TODO: this does not seem to restrict other imports
 __slots__ = ["i8", "i16", "i32", "i64", "f32", "f64", "c32", "c64", "CPtr",
         "overload", "ccall", "TypeVar", "pointer", "c_p_pointer", "Pointer",
         "p_c_pointer", "vectorize", "inline", "Union", "static", "with_goto",
         "packed", "Const", "sizeof", "ccallable"]
```

### Comparing `lpython_emulation-0.0.1.6/lpython_emulation.egg-info/PKG-INFO` & `lpython_emulation-0.0.1.7/lpython_emulation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpython-emulation
-Version: 0.0.1.6
+Version: 0.0.1.7
 Summary: Package for adding type information to python
 Home-page: https://github.com/Shaikh-Ubaid/lpython_packages
 Author: Ondrej Certik
 Author-email: ondrej@certik.us
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lpython_emulation-0.0.1.6/setup.py` & `lpython_emulation-0.0.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 import setuptools
 
 # Define required packages. Alternatively, these could be defined in a separate
 # file and read in here.
 REQUIRED_PACKAGES=[]
 
-VERSION="0.0.1.6"
+VERSION="0.0.1.7"
 
 # Read in the project description. We define this in the README file.
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lpython_emulation",                                   # name of project
-    packages=["lpython"],
+    packages=setuptools.find_packages(),
     install_requires=REQUIRED_PACKAGES,                         # all requirements used by this package
     version=VERSION,                                            # project version, read from version.py
     author="Ondrej Certik",                                     # Author, shown on PyPI
     author_email="ondrej@certik.us",                            # Author email
     description="Package for adding type information to python",# Short description of project
     long_description=long_description,                          # Long description, shown on PyPI
     long_description_content_type="text/markdown",              # Content type. Here, we used a markdown file.
```

