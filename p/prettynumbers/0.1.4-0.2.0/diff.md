# Comparing `tmp/prettynumbers-0.1.4.tar.gz` & `tmp/prettynumbers-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettynumbers-0.1.4.tar", last modified: Sat May  6 15:08:36 2023, max compression
+gzip compressed data, was "prettynumbers-0.2.0.tar", last modified: Mon May  8 12:33:58 2023, max compression
```

## Comparing `prettynumbers-0.1.4.tar` & `prettynumbers-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-06 15:08:36.832995 prettynumbers-0.1.4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14849 2023-05-06 15:08:32.000000 prettynumbers-0.1.4/LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-06 15:08:32.000000 prettynumbers-0.1.4/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1049 2023-05-06 15:08:36.832995 prettynumbers-0.1.4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1199 2023-05-06 15:08:32.000000 prettynumbers-0.1.4/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      500 2023-05-06 15:08:32.000000 prettynumbers-0.1.4/README.rst
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1976 2023-05-06 15:08:32.000000 prettynumbers-0.1.4/pretty_numbers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-06 15:08:36.832995 prettynumbers-0.1.4/prettynumbers.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1049 2023-05-06 15:08:36.000000 prettynumbers-0.1.4/prettynumbers.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      244 2023-05-06 15:08:36.000000 prettynumbers-0.1.4/prettynumbers.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-06 15:08:36.000000 prettynumbers-0.1.4/prettynumbers.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-05-06 15:08:36.000000 prettynumbers-0.1.4/prettynumbers.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2023-05-06 15:08:32.000000 prettynumbers-0.1.4/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2023-05-06 15:08:36.832995 prettynumbers-0.1.4/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      949 2023-05-06 15:08:32.000000 prettynumbers-0.1.4/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 12:33:58.455289 prettynumbers-0.2.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14849 2023-05-08 12:33:52.000000 prettynumbers-0.2.0/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-08 12:33:52.000000 prettynumbers-0.2.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1049 2023-05-08 12:33:58.455289 prettynumbers-0.2.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1199 2023-05-08 12:33:52.000000 prettynumbers-0.2.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      500 2023-05-08 12:33:52.000000 prettynumbers-0.2.0/README.rst
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1981 2023-05-08 12:33:52.000000 prettynumbers-0.2.0/pretty_numbers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 12:33:58.455289 prettynumbers-0.2.0/prettynumbers.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1049 2023-05-08 12:33:58.000000 prettynumbers-0.2.0/prettynumbers.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      244 2023-05-08 12:33:58.000000 prettynumbers-0.2.0/prettynumbers.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-08 12:33:58.000000 prettynumbers-0.2.0/prettynumbers.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-05-08 12:33:58.000000 prettynumbers-0.2.0/prettynumbers.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2023-05-08 12:33:52.000000 prettynumbers-0.2.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2023-05-08 12:33:58.459288 prettynumbers-0.2.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2023-05-08 12:33:52.000000 prettynumbers-0.2.0/setup.py
```

### Comparing `prettynumbers-0.1.4/LICENSE.txt` & `prettynumbers-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.1.4/PKG-INFO` & `prettynumbers-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: prettynumbers
-Version: 0.1.4
+Version: 0.2.0
 Summary: Display a range of numbers in a human readable way
 Home-page: https://github.com/vfxGer/pretty-numbers
 Author: Gerard Keating
 Author-email: gerardk@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
-Download-URL: https://pypi.python.org/packages/source/d/pretty_numbers-0.1.4.tar.gz?raw=true
+Download-URL: https://pypi.python.org/packages/source/d/pretty_numbers-0.2.0.tar.gz?raw=true
 Description: |Build Status| |codecov.io| |Code Climate|
         
         .. |Build Status| image:: https://travis-ci.org/vfxGer/pretty-numbers.svg?branch=master
            :target: https://travis-ci.org/vfxGer/pretty-numbers
         .. |codecov.io| image:: https://codecov.io/gh/vfxGer/pretty-numbers/coverage.svg?branch=master
            :target: https://codecov.io/gh/vfxGer/pretty-numbers
         .. |Code Climate| image:: https://codeclimate.com/github/vfxGer/pretty-numbers/badges/gpa.svg
```

### Comparing `prettynumbers-0.1.4/README.md` & `prettynumbers-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.1.4/pretty_numbers.py` & `prettynumbers-0.2.0/pretty_numbers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 ########################################################
 __author__ = "Gerard Keating vfxger.com"
 ########################################################
-from typing import Set, Sequence
+from typing import Any, Sequence, Set
 
 
 def getPrettyTextFromSet(frames: Set[int]) -> str:
     """
     Given a set of integers returns a more human readable string
     """
     if not frames:
@@ -36,15 +36,15 @@
     """
     Given iterable of integers returns a more human readable string
     """
     framesSet = set(frames)
     return getPrettyTextFromSet(framesSet)
 
 
-def getPrettyNumbersText(list_of_strings: Sequence[str]) -> str:
+def getPrettyNumbersText(list_of_strings: Sequence[Any]) -> str:
     nums = set()
     text_result = set()
     for i in list_of_strings:
         try:
             is_digit = i.isdigit()
         except AttributeError:
             is_digit = True
```

### Comparing `prettynumbers-0.1.4/prettynumbers.egg-info/PKG-INFO` & `prettynumbers-0.2.0/prettynumbers.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: prettynumbers
-Version: 0.1.4
+Version: 0.2.0
 Summary: Display a range of numbers in a human readable way
 Home-page: https://github.com/vfxGer/pretty-numbers
 Author: Gerard Keating
 Author-email: gerardk@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
-Download-URL: https://pypi.python.org/packages/source/d/pretty_numbers-0.1.4.tar.gz?raw=true
+Download-URL: https://pypi.python.org/packages/source/d/pretty_numbers-0.2.0.tar.gz?raw=true
 Description: |Build Status| |codecov.io| |Code Climate|
         
         .. |Build Status| image:: https://travis-ci.org/vfxGer/pretty-numbers.svg?branch=master
            :target: https://travis-ci.org/vfxGer/pretty-numbers
         .. |codecov.io| image:: https://codecov.io/gh/vfxGer/pretty-numbers/coverage.svg?branch=master
            :target: https://codecov.io/gh/vfxGer/pretty-numbers
         .. |Code Climate| image:: https://codeclimate.com/github/vfxGer/pretty-numbers/badges/gpa.svg
```

### Comparing `prettynumbers-0.1.4/pyproject.toml` & `prettynumbers-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.1.4/setup.py` & `prettynumbers-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # based on https://github.com/pypa/sampleproject/blob/master/setup.py
 from os import path
 
 from setuptools import setup
 
 here = path.abspath(path.dirname(__file__))
 
-version = "0.1.4"
+version = "0.2.0"
 
 # Get the long description from the README file
 with open(path.join(here, "README.rst"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="prettynumbers",
@@ -23,8 +23,9 @@
     url="https://github.com/vfxGer/pretty-numbers",
     py_modules=["pretty_numbers"],
     download_url=f"https://pypi.python.org/packages/"
     f"source/d/"
     f"pretty_numbers-{version}.tar.gz?raw=true",
     platforms="Cross-platform",
     classifiers=["Programming Language :: Python :: 3"],
+    package_data={"prettynumbers": ["py.typed"]},
 )
```

