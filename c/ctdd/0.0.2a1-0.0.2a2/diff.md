# Comparing `tmp/ctdd-0.0.2a1.tar.gz` & `tmp/ctdd-0.0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctdd-0.0.2a1.tar", max compression
+gzip compressed data, was "ctdd-0.0.2a2.tar", max compression
```

## Comparing `ctdd-0.0.2a1.tar` & `ctdd-0.0.2a2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1108 2023-05-03 17:25:05.122292 ctdd-0.0.2a1/LICENSE
--rw-r--r--   0        0        0     2025 2023-05-03 18:54:09.035294 ctdd-0.0.2a1/README.md
--rw-r--r--   0        0        0       28 2023-05-03 18:15:09.070117 ctdd-0.0.2a1/ctdd/__init__.py
--rw-r--r--   0        0        0       55 2023-05-03 18:26:42.187993 ctdd-0.0.2a1/ctdd/factory.py
--rw-r--r--   0        0        0     2450 2023-05-08 00:41:47.727104 ctdd-0.0.2a1/ctdd/tester.py
--rw-r--r--   0        0        0      738 2023-05-08 00:57:22.154407 ctdd-0.0.2a1/pyproject.toml
--rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 ctdd-0.0.2a1/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-05-03 17:25:05.122292 ctdd-0.0.2a2/LICENSE
+-rw-r--r--   0        0        0     2025 2023-05-08 01:05:44.511002 ctdd-0.0.2a2/README.md
+-rw-r--r--   0        0        0       28 2023-05-03 18:15:09.070117 ctdd-0.0.2a2/ctdd/__init__.py
+-rw-r--r--   0        0        0       55 2023-05-03 18:26:42.187993 ctdd-0.0.2a2/ctdd/factory.py
+-rw-r--r--   0        0        0     2450 2023-05-08 00:41:47.727104 ctdd-0.0.2a2/ctdd/tester.py
+-rw-r--r--   0        0        0      738 2023-05-08 01:12:56.336365 ctdd-0.0.2a2/pyproject.toml
+-rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 ctdd-0.0.2a2/PKG-INFO
```

### Comparing `ctdd-0.0.2a1/LICENSE` & `ctdd-0.0.2a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.2a1/README.md` & `ctdd-0.0.2a2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# cttd
+# ctdd
 
 ## tl:dr
 
 C test-driven development framework implemented in Python.
 
 ## Info
 
 The testing framework is Python's native unittest, with a few extra asserts ans stuff provided by John. The tester looks for a .c and .h pair with the same name as the .py test file. It builds them into a Python extension using Crelm (which in turn uses cffi) and runs the Python tests as if it were testing Python code. C callbacks are mocked in Python (demo to follow..), meaning that there is exactly zero C code involved in the testing.
 
 ## Example
 
-There is a demo of a TTD'd `add3` function in \_\_main\_\_.py, \_\_main\_\_.c and \_\_main\_\_.h in the root of the repo, run with `python3 .`. The silly filenames are to suit the Python auto-run mechanism.
+There is a demo of a TDD'd `add3` function in \_\_main\_\_.py, \_\_main\_\_.c and \_\_main\_\_.h in the root of the repo, run with `python3 .`. The silly filenames are to suit the Python auto-run mechanism.
 
 The files are reproduced here (possibly out of date) with original filenames:
 
 __add3.py__
 
 ```
-from cttd import Tester
+from ctdd import Tester
 
 class Add3Tests(Tester):
 
     def test_sut_compiles(self):
         with self.assertDoesNotRaise():
             self.sut
 
@@ -59,15 +59,15 @@
 
 int add3(int a, int b, int c)
 {
     return a + b + c;
 }
 ```
 
-To use this in real life install the package with `pip install cttd` (in a virtualenv if you prefer), and run `python add3.py` after each add test or add code iteration.
+To use this in real life install the package with `pip install ctdd` (in a virtualenv if you prefer), and run `python add3.py` after each add test or add code iteration.
 
 Test output is exactly what unittest said (with distutils deprecation warning removed):
 
 ```
 ...........
 ----------------------------------------------------------------------
 Ran 11 tests in 2.104s
```

### Comparing `ctdd-0.0.2a1/ctdd/tester.py` & `ctdd-0.0.2a2/ctdd/tester.py`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.2a1/pyproject.toml` & `ctdd-0.0.2a2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ctdd"
-version = "0.0.2a1"
+version = "0.0.2a2"
 description = "C test-driven development framework implemented in Python"
 authors = [
   "WideOpenTech <fossie@wideopentech.co.uk>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ctdd-0.0.2a1/PKG-INFO` & `ctdd-0.0.2a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctdd
-Version: 0.0.2a1
+Version: 0.0.2a2
 Summary: C test-driven development framework implemented in Python
 Home-page: https://github.com/wideopensource/ctdd
 Author: WideOpenTech
 Author-email: fossie@wideopentech.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,34 +15,34 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: crelm (>=0.0.32,<0.0.33)
 Requires-Dist: john (>=0.1.5,<0.2.0)
 Project-URL: Repository, https://github.com/wideopensource/ctdd
 Description-Content-Type: text/markdown
 
-# cttd
+# ctdd
 
 ## tl:dr
 
 C test-driven development framework implemented in Python.
 
 ## Info
 
 The testing framework is Python's native unittest, with a few extra asserts ans stuff provided by John. The tester looks for a .c and .h pair with the same name as the .py test file. It builds them into a Python extension using Crelm (which in turn uses cffi) and runs the Python tests as if it were testing Python code. C callbacks are mocked in Python (demo to follow..), meaning that there is exactly zero C code involved in the testing.
 
 ## Example
 
-There is a demo of a TTD'd `add3` function in \_\_main\_\_.py, \_\_main\_\_.c and \_\_main\_\_.h in the root of the repo, run with `python3 .`. The silly filenames are to suit the Python auto-run mechanism.
+There is a demo of a TDD'd `add3` function in \_\_main\_\_.py, \_\_main\_\_.c and \_\_main\_\_.h in the root of the repo, run with `python3 .`. The silly filenames are to suit the Python auto-run mechanism.
 
 The files are reproduced here (possibly out of date) with original filenames:
 
 __add3.py__
 
 ```
-from cttd import Tester
+from ctdd import Tester
 
 class Add3Tests(Tester):
 
     def test_sut_compiles(self):
         with self.assertDoesNotRaise():
             self.sut
 
@@ -80,15 +80,15 @@
 
 int add3(int a, int b, int c)
 {
     return a + b + c;
 }
 ```
 
-To use this in real life install the package with `pip install cttd` (in a virtualenv if you prefer), and run `python add3.py` after each add test or add code iteration.
+To use this in real life install the package with `pip install ctdd` (in a virtualenv if you prefer), and run `python add3.py` after each add test or add code iteration.
 
 Test output is exactly what unittest said (with distutils deprecation warning removed):
 
 ```
 ...........
 ----------------------------------------------------------------------
 Ran 11 tests in 2.104s
```

