# Comparing `tmp/SAPsim-1.0.6.tar.gz` & `tmp/SAPsim-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAPsim-1.0.6.tar", last modified: Mon May  8 03:02:07 2023, max compression
+gzip compressed data, was "SAPsim-1.0.7.tar", last modified: Mon May  8 03:22:36 2023, max compression
```

## Comparing `SAPsim-1.0.6.tar` & `SAPsim-1.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:02:07.307944 SAPsim-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-08 03:01:58.000000 SAPsim-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-08 03:02:07.307944 SAPsim-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-08 03:01:58.000000 SAPsim-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:02:07.303944 SAPsim-1.0.6/SAPsim/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-08 03:01:58.000000 SAPsim-1.0.6/SAPsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:02:07.307944 SAPsim-1.0.6/SAPsim/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 03:01:58.000000 SAPsim-1.0.6/SAPsim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-05-08 03:01:58.000000 SAPsim-1.0.6/SAPsim/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-05-08 03:01:58.000000 SAPsim-1.0.6/SAPsim/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-08 03:01:58.000000 SAPsim-1.0.6/SAPsim/utils/global_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-05-08 03:01:58.000000 SAPsim-1.0.6/SAPsim/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-08 03:01:58.000000 SAPsim-1.0.6/SAPsim/utils/instructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-08 03:01:58.000000 SAPsim-1.0.6/SAPsim/utils/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:02:07.307944 SAPsim-1.0.6/SAPsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-08 03:02:07.000000 SAPsim-1.0.6/SAPsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-08 03:02:07.000000 SAPsim-1.0.6/SAPsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 03:02:07.000000 SAPsim-1.0.6/SAPsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 03:02:07.000000 SAPsim-1.0.6/SAPsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-08 03:02:07.000000 SAPsim-1.0.6/SAPsim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-08 03:01:58.000000 SAPsim-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 03:02:07.307944 SAPsim-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-08 03:01:58.000000 SAPsim-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:02:07.307944 SAPsim-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 03:01:58.000000 SAPsim-1.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-08 03:01:58.000000 SAPsim-1.0.6/tests/test_example_progs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-08 03:01:58.000000 SAPsim-1.0.6/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-08 03:01:58.000000 SAPsim-1.0.6/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-08 03:01:58.000000 SAPsim-1.0.6/tests/test_instructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-08 03:01:58.000000 SAPsim-1.0.6/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:22:36.414992 SAPsim-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-08 03:22:21.000000 SAPsim-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-08 03:22:36.414992 SAPsim-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-08 03:22:21.000000 SAPsim-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:22:36.402992 SAPsim-1.0.7/SAPsim/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-08 03:22:21.000000 SAPsim-1.0.7/SAPsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:22:36.410992 SAPsim-1.0.7/SAPsim/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 03:22:21.000000 SAPsim-1.0.7/SAPsim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-05-08 03:22:21.000000 SAPsim-1.0.7/SAPsim/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-05-08 03:22:21.000000 SAPsim-1.0.7/SAPsim/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-08 03:22:21.000000 SAPsim-1.0.7/SAPsim/utils/global_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-05-08 03:22:21.000000 SAPsim-1.0.7/SAPsim/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-08 03:22:21.000000 SAPsim-1.0.7/SAPsim/utils/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-08 03:22:21.000000 SAPsim-1.0.7/SAPsim/utils/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:22:36.406992 SAPsim-1.0.7/SAPsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-08 03:22:36.000000 SAPsim-1.0.7/SAPsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-08 03:22:36.000000 SAPsim-1.0.7/SAPsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 03:22:36.000000 SAPsim-1.0.7/SAPsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 03:22:36.000000 SAPsim-1.0.7/SAPsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-08 03:22:36.000000 SAPsim-1.0.7/SAPsim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-08 03:22:21.000000 SAPsim-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 03:22:36.414992 SAPsim-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-08 03:22:21.000000 SAPsim-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:22:36.414992 SAPsim-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 03:22:21.000000 SAPsim-1.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-08 03:22:21.000000 SAPsim-1.0.7/tests/test_example_progs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-08 03:22:21.000000 SAPsim-1.0.7/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-08 03:22:21.000000 SAPsim-1.0.7/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-08 03:22:21.000000 SAPsim-1.0.7/tests/test_instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-08 03:22:21.000000 SAPsim-1.0.7/tests/test_run.py
```

### Comparing `SAPsim-1.0.6/LICENSE` & `SAPsim-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.6/PKG-INFO` & `SAPsim-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAPsim
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC
 Home-page: https://github.com/jesse-wei/SAPsim
 Download-URL: https://github.com/jesse-wei/SAPsim/releases
 Author: Jesse Wei
 Author-email: Jesse Wei <jesse@cs.unc.edu>
 Project-URL: Homepage, https://github.com/jesse-wei/SAPsim
 Project-URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SAPsim Version: 1.0.6 Summary: Simulation of SAP
+Metadata-Version: 2.1 Name: SAPsim Version: 1.0.7 Summary: Simulation of SAP
 (Simple As Possible) computer programs from COMP311 (Computer Organization) @
 UNC Home-page: https://github.com/jesse-wei/SAPsim Download-URL: https://
 github.com/jesse-wei/SAPsim/releases Author: Jesse Wei Author-email: Jesse Wei
 cs.unc.edu> Project-URL: Homepage, https://github.com/jesse-wei/SAPsim Project-
 URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues Keywords:
 SAP,SAPsim,simple as possible,UNC,COMP311 Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
```

### Comparing `SAPsim-1.0.6/README.md` & `SAPsim-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.6/SAPsim/__init__.py` & `SAPsim-1.0.7/SAPsim/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
+from typing import Union, Any
 from SAPsim.utils.helpers import is_documented_by
 import SAPsim.utils.execute as execute
 
 
 # Weird glitch, passing in the function doesn't actually get its docstring? Just append then
 @is_documented_by(execute.run, 0, "", execute.run.__doc__)
-def run(prog_path: str, **kwargs) -> None:
-    execute.run(prog_path, **kwargs)
+def run(prog_path: str, **kwargs) -> Union[None, dict[str, Any]]:
+    return execute.run(prog_path, **kwargs)
 
 
 def create_template() -> None:
     r"""
     Create blank ``template.csv`` file in SAPsim format in current directory.
     """
     # This will rarely be used so doesn't need to be imported at top level
```

### Comparing `SAPsim-1.0.6/SAPsim/utils/exceptions.py` & `SAPsim-1.0.7/SAPsim/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.6/SAPsim/utils/execute.py` & `SAPsim-1.0.7/SAPsim/utils/execute.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.6/SAPsim/utils/global_vars.py` & `SAPsim-1.0.7/SAPsim/utils/global_vars.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.6/SAPsim/utils/helpers.py` & `SAPsim-1.0.7/SAPsim/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.6/SAPsim/utils/instructions.py` & `SAPsim-1.0.7/SAPsim/utils/instructions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.6/SAPsim/utils/parser.py` & `SAPsim-1.0.7/SAPsim/utils/parser.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.6/SAPsim.egg-info/PKG-INFO` & `SAPsim-1.0.7/SAPsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAPsim
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC
 Home-page: https://github.com/jesse-wei/SAPsim
 Download-URL: https://github.com/jesse-wei/SAPsim/releases
 Author: Jesse Wei
 Author-email: Jesse Wei <jesse@cs.unc.edu>
 Project-URL: Homepage, https://github.com/jesse-wei/SAPsim
 Project-URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SAPsim Version: 1.0.6 Summary: Simulation of SAP
+Metadata-Version: 2.1 Name: SAPsim Version: 1.0.7 Summary: Simulation of SAP
 (Simple As Possible) computer programs from COMP311 (Computer Organization) @
 UNC Home-page: https://github.com/jesse-wei/SAPsim Download-URL: https://
 github.com/jesse-wei/SAPsim/releases Author: Jesse Wei Author-email: Jesse Wei
 cs.unc.edu> Project-URL: Homepage, https://github.com/jesse-wei/SAPsim Project-
 URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues Keywords:
 SAP,SAPsim,simple as possible,UNC,COMP311 Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
```

### Comparing `SAPsim-1.0.6/SAPsim.egg-info/SOURCES.txt` & `SAPsim-1.0.7/SAPsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.6/pyproject.toml` & `SAPsim-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.6/setup.py` & `SAPsim-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """All required (i.e., for functionality) dependencies that are installed when running `pip install SAPsim`.
 
 Non-functional (e.g., formatting, documentation) dependencies listed in requirements.txt."""
 
 setup(
     name="SAPsim",
     # Check https://pypi.org/project/SAPsim/ for latest version number
-    version="1.0.6",
+    version="1.0.7",
     description="Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC.",
     author="Jesse Wei",
     author_email="jesse@cs.unc.edu",
     url="https://github.com/jesse-wei/SAPsim",
     download_url="https://github.com/jesse-wei/SAPsim/releases",
     keywords=[
         "SAP",
```

### Comparing `SAPsim-1.0.6/tests/test_example_progs.py` & `SAPsim-1.0.7/tests/test_example_progs.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.6/tests/test_exceptions.py` & `SAPsim-1.0.7/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.6/tests/test_helpers.py` & `SAPsim-1.0.7/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.6/tests/test_instructions.py` & `SAPsim-1.0.7/tests/test_instructions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.6/tests/test_run.py` & `SAPsim-1.0.7/tests/test_run.py`

 * *Files identical despite different names*

