# Comparing `tmp/bs_python_utils-0.0.4.tar.gz` & `tmp/bs_python_utils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_python_utils-0.0.4.tar", max compression
+gzip compressed data, was "bs_python_utils-0.0.5.tar", max compression
```

## Comparing `bs_python_utils-0.0.4.tar` & `bs_python_utils-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1073 2023-04-21 14:06:07.415664 bs_python_utils-0.0.4/LICENSE
--rw-r--r--   0        0        0     1210 2023-05-02 17:34:41.331375 bs_python_utils-0.0.4/README.md
--rw-r--r--   0        0        0     1799 2023-04-24 19:42:58.427840 bs_python_utils-0.0.4/bs_python_utils/Timer.py
--rw-r--r--   0        0        0        0 2023-04-24 19:42:58.429294 bs_python_utils-0.0.4/bs_python_utils/__init__.py
--rw-r--r--   0        0        0    28473 2023-04-24 22:57:44.859499 bs_python_utils-0.0.4/bs_python_utils/bs_altair.py
--rw-r--r--   0        0        0     2976 2023-04-24 20:25:24.489951 bs_python_utils-0.0.4/bs_python_utils/bs_logging.py
--rw-r--r--   0        0        0     3577 2023-04-24 19:42:58.433666 bs_python_utils-0.0.4/bs_python_utils/bs_mathstr.py
--rw-r--r--   0        0        0     4338 2023-04-24 21:45:53.142922 bs_python_utils-0.0.4/bs_python_utils/bs_mem.py
--rw-r--r--   0        0        0    13696 2023-04-24 22:48:26.403984 bs_python_utils-0.0.4/bs_python_utils/bs_opt.py
--rw-r--r--   0        0        0       36 2023-04-24 19:42:58.438686 bs_python_utils-0.0.4/bs_python_utils/bs_plots.py
--rw-r--r--   0        0        0     4507 2023-04-24 20:32:13.556809 bs_python_utils-0.0.4/bs_python_utils/bs_seaborn.py
--rw-r--r--   0        0        0     1391 2023-04-24 22:48:26.302214 bs_python_utils-0.0.4/bs_python_utils/bs_sparse_gaussian.py
--rw-r--r--   0        0        0      905 2023-04-24 19:42:58.441367 bs_python_utils-0.0.4/bs_python_utils/bsmplutils.py
--rw-r--r--   0        0        0    31781 2023-05-02 17:31:44.506884 bs_python_utils-0.0.4/bs_python_utils/bsnputils.py
--rw-r--r--   0        0        0     2132 2023-04-24 20:25:24.253141 bs_python_utils-0.0.4/bs_python_utils/bssputils.py
--rw-r--r--   0        0        0    15489 2023-04-24 20:25:24.644930 bs_python_utils-0.0.4/bs_python_utils/bsstats.py
--rw-r--r--   0        0        0     9199 2023-04-24 20:25:24.587557 bs_python_utils-0.0.4/bs_python_utils/bsutils.py
--rw-r--r--   0        0        0     7801 2023-04-24 21:45:53.165270 bs_python_utils-0.0.4/bs_python_utils/distance_covariances.py
--rw-r--r--   0        0        0     1350 2023-04-24 22:36:28.733299 bs_python_utils-0.0.4/bs_python_utils/example_opt.py
--rw-r--r--   0        0        0     3833 2023-04-24 22:48:26.344134 bs_python_utils-0.0.4/bs_python_utils/examples_altair.py
--rw-r--r--   0        0        0     1013 2023-04-24 22:36:28.733372 bs_python_utils-0.0.4/bs_python_utils/examples_distance_covariances.py
--rw-r--r--   0        0        0      552 2023-04-24 22:36:28.733335 bs_python_utils-0.0.4/bs_python_utils/examples_mem.py
--rw-r--r--   0        0        0      771 2023-04-24 21:45:53.146924 bs_python_utils-0.0.4/bs_python_utils/examples_seaborn.py
--rw-r--r--   0        0        0      786 2023-04-24 22:36:28.733292 bs_python_utils-0.0.4/bs_python_utils/examples_sklearn.py
--rw-r--r--   0        0        0     7426 2023-04-24 20:25:24.576148 bs_python_utils-0.0.4/bs_python_utils/pandas_utils.py
--rw-r--r--   0        0        0     1872 2023-04-24 21:46:50.361114 bs_python_utils-0.0.4/bs_python_utils/sklearn_utils.py
--rw-r--r--   0        0        0     1871 2023-05-02 17:33:54.399911 bs_python_utils-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2182 1970-01-01 00:00:00.000000 bs_python_utils-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-21 14:06:07.415664 bs_python_utils-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1371 2023-05-08 18:46:21.795283 bs_python_utils-0.0.5/README.md
+-rw-r--r--   0        0        0     1799 2023-04-24 19:42:58.427840 bs_python_utils-0.0.5/bs_python_utils/Timer.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:42:58.429294 bs_python_utils-0.0.5/bs_python_utils/__init__.py
+-rw-r--r--   0        0        0    28473 2023-04-24 22:57:44.859499 bs_python_utils-0.0.5/bs_python_utils/bs_altair.py
+-rw-r--r--   0        0        0     2976 2023-04-24 20:25:24.489951 bs_python_utils-0.0.5/bs_python_utils/bs_logging.py
+-rw-r--r--   0        0        0     3577 2023-04-24 19:42:58.433666 bs_python_utils-0.0.5/bs_python_utils/bs_mathstr.py
+-rw-r--r--   0        0        0     4338 2023-04-24 21:45:53.142922 bs_python_utils-0.0.5/bs_python_utils/bs_mem.py
+-rw-r--r--   0        0        0    13696 2023-04-24 22:48:26.403984 bs_python_utils-0.0.5/bs_python_utils/bs_opt.py
+-rw-r--r--   0        0        0       36 2023-04-24 19:42:58.438686 bs_python_utils-0.0.5/bs_python_utils/bs_plots.py
+-rw-r--r--   0        0        0     4507 2023-04-24 20:32:13.556809 bs_python_utils-0.0.5/bs_python_utils/bs_seaborn.py
+-rw-r--r--   0        0        0     1391 2023-04-24 22:48:26.302214 bs_python_utils-0.0.5/bs_python_utils/bs_sparse_gaussian.py
+-rw-r--r--   0        0        0      905 2023-04-24 19:42:58.441367 bs_python_utils-0.0.5/bs_python_utils/bsmplutils.py
+-rw-r--r--   0        0        0    31781 2023-05-02 17:31:44.506884 bs_python_utils-0.0.5/bs_python_utils/bsnputils.py
+-rw-r--r--   0        0        0     2132 2023-04-24 20:25:24.253141 bs_python_utils-0.0.5/bs_python_utils/bssputils.py
+-rw-r--r--   0        0        0    15489 2023-04-24 20:25:24.644930 bs_python_utils-0.0.5/bs_python_utils/bsstats.py
+-rw-r--r--   0        0        0     9471 2023-05-08 18:43:13.753098 bs_python_utils-0.0.5/bs_python_utils/bsutils.py
+-rw-r--r--   0        0        0     7801 2023-04-24 21:45:53.165270 bs_python_utils-0.0.5/bs_python_utils/distance_covariances.py
+-rw-r--r--   0        0        0     1350 2023-04-24 22:36:28.733299 bs_python_utils-0.0.5/bs_python_utils/example_opt.py
+-rw-r--r--   0        0        0     3833 2023-04-24 22:48:26.344134 bs_python_utils-0.0.5/bs_python_utils/examples_altair.py
+-rw-r--r--   0        0        0     1013 2023-04-24 22:36:28.733372 bs_python_utils-0.0.5/bs_python_utils/examples_distance_covariances.py
+-rw-r--r--   0        0        0      552 2023-04-24 22:36:28.733335 bs_python_utils-0.0.5/bs_python_utils/examples_mem.py
+-rw-r--r--   0        0        0      771 2023-04-24 21:45:53.146924 bs_python_utils-0.0.5/bs_python_utils/examples_seaborn.py
+-rw-r--r--   0        0        0      786 2023-04-24 22:36:28.733292 bs_python_utils-0.0.5/bs_python_utils/examples_sklearn.py
+-rw-r--r--   0        0        0     7426 2023-04-24 20:25:24.576148 bs_python_utils-0.0.5/bs_python_utils/pandas_utils.py
+-rw-r--r--   0        0        0     1872 2023-04-24 21:46:50.361114 bs_python_utils-0.0.5/bs_python_utils/sklearn_utils.py
+-rw-r--r--   0        0        0     1871 2023-05-08 18:45:42.703018 bs_python_utils-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2343 1970-01-01 00:00:00.000000 bs_python_utils-0.0.5/PKG-INFO
```

### Comparing `bs_python_utils-0.0.4/LICENSE` & `bs_python_utils-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/README.md` & `bs_python_utils-0.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 # bs-python-utils
 
+![GitHub last commit](https://img.shields.io/github/last-commit/bsalanie/bs-python-utils)
+
 <!-- [![Release](https://img.shields.io/github/v/release/bsalanie/bs-python-utils)](https://img.shields.io/github/v/release/bsalanie/bs-python-utils) -->
-[![Build status](https://img.shields.io/github/actions/workflow/status/bsalanie/bs-python-utils/main.yml?branch=main)](https://github.com/bsalanie/bs-python-utils/actions/workflows/main.yml?query=branch%3Amain)
-<!-- [![codecov](https://codecov.io/gh/bsalanie/bs-python-utils/branch/main/graph/badge.svg)](https://codecov.io/gh/bsalanie/bs-python-utils) -->
-[![Commit activity](https://img.shields.io/github/commit-activity/m/bsalanie/bs-python-utils)](https://img.shields.io/github/commit-activity/m/bsalanie/bs-python-utils)
-[![License](https://img.shields.io/github/license/bsalanie/bs-python-utils)](https://img.shields.io/github/license/bsalanie/bs-python-utils)
 
-My Python utilities.
+[![Build status](https://img.shields.io/github/actions/workflow/status/bsalanie/bs-python-utils/main.yml?branch=main)](https://github.com/bsalanie/bs-python-utils/actions/workflows/main.yml?query=branch%3Amain) <!-- [![codecov](https://codecov.io/gh/bsalanie/bs-python-utils/branch/main/graph/badge.svg)](https://codecov.io/gh/bsalanie/bs-python-utils) --> <!-- [![Commit activity](https://img.shields.io/github/commit-activity/m/bsalanie/bs-python-utils)](https://img.shields.io/github/commit-activity/m/bsalanie/bs-python-utils) --> [![License](https://img.shields.io/github/license/bsalanie/bs-python-utils)](https://img.shields.io/github/license/bsalanie/bs-python-utils)
 
-- **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
-- **Documentation** <https://bsalanie.github.io/bs-python-utils/>
+My Python utilities.
 
+-   **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
+-   **Documentation** <https://bsalanie.github.io/bs-python-utils/>
 
 ### Release notes
 
+#### 0.0.5 (May 8, 2023)
+
+Added `final_s` in `bsutils`.
+
 #### 0.0.4 (May 2, 2023)
+
 Added Legendre polynomials and quantile routines in `bsnputils`.
 
-#### 0.0.3  (April 24, 2023)
+#### 0.0.3 (April 24, 2023)
+
 Satisfied mypy.
 
-#### 0.0.2  (April 24, 2023)
-Fixed main PyPI page.
+#### 0.0.2 (April 24, 2023)
+
+Fixed main PyPI page.
```

### Comparing `bs_python_utils-0.0.4/bs_python_utils/Timer.py` & `bs_python_utils-0.0.5/bs_python_utils/Timer.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/bs_python_utils/bs_altair.py` & `bs_python_utils-0.0.5/bs_python_utils/bs_altair.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/bs_python_utils/bs_logging.py` & `bs_python_utils-0.0.5/bs_python_utils/bs_logging.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/bs_python_utils/bs_mathstr.py` & `bs_python_utils-0.0.5/bs_python_utils/bs_mathstr.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/bs_python_utils/bs_mem.py` & `bs_python_utils-0.0.5/bs_python_utils/bs_mem.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/bs_python_utils/bs_opt.py` & `bs_python_utils-0.0.5/bs_python_utils/bs_opt.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/bs_python_utils/bs_seaborn.py` & `bs_python_utils-0.0.5/bs_python_utils/bs_seaborn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/bs_python_utils/bs_sparse_gaussian.py` & `bs_python_utils-0.0.5/bs_python_utils/bs_sparse_gaussian.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/bs_python_utils/bsmplutils.py` & `bs_python_utils-0.0.5/bs_python_utils/bsmplutils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/bs_python_utils/bsnputils.py` & `bs_python_utils-0.0.5/bs_python_utils/bsnputils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/bs_python_utils/bssputils.py` & `bs_python_utils-0.0.5/bs_python_utils/bssputils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/bs_python_utils/bsstats.py` & `bs_python_utils-0.0.5/bs_python_utils/bsstats.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/bs_python_utils/bsutils.py` & `bs_python_utils-0.0.5/bs_python_utils/bsutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,29 @@
     Returns:
         prints the message and exits with code 1
     """
     print_stars(f"{bs_name_func(3)}: {msg}")
     sys.exit(1)
 
 
+def final_s(n: int, word: str) -> str:
+    """
+    pluralizes word if n > 1
+
+    Args:
+        n: how many times
+        word: to be pluralized, maybe
+
+    Returns:
+        `1 word` or `n words`
+    """
+    suffix = "s" if n > 1 else ""
+    return f"{n} {word}{suffix}"
+
+
 def bs_switch(
     match: str, dico: dict, strict: bool = True, default: Any = "no match"
 ) -> Any:
     """
     a switch statement that allows for partial matches if strict is False
 
     Args:
```

### Comparing `bs_python_utils-0.0.4/bs_python_utils/distance_covariances.py` & `bs_python_utils-0.0.5/bs_python_utils/distance_covariances.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/bs_python_utils/example_opt.py` & `bs_python_utils-0.0.5/bs_python_utils/example_opt.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/bs_python_utils/examples_altair.py` & `bs_python_utils-0.0.5/bs_python_utils/examples_altair.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/bs_python_utils/examples_distance_covariances.py` & `bs_python_utils-0.0.5/bs_python_utils/examples_distance_covariances.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/bs_python_utils/examples_mem.py` & `bs_python_utils-0.0.5/bs_python_utils/examples_mem.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/bs_python_utils/examples_seaborn.py` & `bs_python_utils-0.0.5/bs_python_utils/examples_seaborn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/bs_python_utils/examples_sklearn.py` & `bs_python_utils-0.0.5/bs_python_utils/examples_sklearn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/bs_python_utils/pandas_utils.py` & `bs_python_utils-0.0.5/bs_python_utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/bs_python_utils/sklearn_utils.py` & `bs_python_utils-0.0.5/bs_python_utils/sklearn_utils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.4/pyproject.toml` & `bs_python_utils-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bs_python_utils"
-version = "0.0.4"
+version = "0.0.5"
 description = "my Python utilities"
 authors = ["Bernard Salanie <fbsalanie@columbia.edu>"]
 repository = "https://github.com/bsalanie/bs-python-utils"
 documentation = "https://bsalanie.github.io/bs-python-utils/"
 readme = "README.md"
 packages = [
   {include = "bs_python_utils"}
```

### Comparing `bs_python_utils-0.0.4/PKG-INFO` & `bs_python_utils-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bs-python-utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: my Python utilities
 Home-page: https://github.com/bsalanie/bs-python-utils
 Author: Bernard Salanie
 Author-email: fbsalanie@columbia.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -20,30 +20,35 @@
 Requires-Dist: vega-datasets (>=0.9.0,<0.10.0)
 Project-URL: Documentation, https://bsalanie.github.io/bs-python-utils/
 Project-URL: Repository, https://github.com/bsalanie/bs-python-utils
 Description-Content-Type: text/markdown
 
 # bs-python-utils
 
+![GitHub last commit](https://img.shields.io/github/last-commit/bsalanie/bs-python-utils)
+
 <!-- [![Release](https://img.shields.io/github/v/release/bsalanie/bs-python-utils)](https://img.shields.io/github/v/release/bsalanie/bs-python-utils) -->
-[![Build status](https://img.shields.io/github/actions/workflow/status/bsalanie/bs-python-utils/main.yml?branch=main)](https://github.com/bsalanie/bs-python-utils/actions/workflows/main.yml?query=branch%3Amain)
-<!-- [![codecov](https://codecov.io/gh/bsalanie/bs-python-utils/branch/main/graph/badge.svg)](https://codecov.io/gh/bsalanie/bs-python-utils) -->
-[![Commit activity](https://img.shields.io/github/commit-activity/m/bsalanie/bs-python-utils)](https://img.shields.io/github/commit-activity/m/bsalanie/bs-python-utils)
-[![License](https://img.shields.io/github/license/bsalanie/bs-python-utils)](https://img.shields.io/github/license/bsalanie/bs-python-utils)
 
-My Python utilities.
+[![Build status](https://img.shields.io/github/actions/workflow/status/bsalanie/bs-python-utils/main.yml?branch=main)](https://github.com/bsalanie/bs-python-utils/actions/workflows/main.yml?query=branch%3Amain) <!-- [![codecov](https://codecov.io/gh/bsalanie/bs-python-utils/branch/main/graph/badge.svg)](https://codecov.io/gh/bsalanie/bs-python-utils) --> <!-- [![Commit activity](https://img.shields.io/github/commit-activity/m/bsalanie/bs-python-utils)](https://img.shields.io/github/commit-activity/m/bsalanie/bs-python-utils) --> [![License](https://img.shields.io/github/license/bsalanie/bs-python-utils)](https://img.shields.io/github/license/bsalanie/bs-python-utils)
 
-- **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
-- **Documentation** <https://bsalanie.github.io/bs-python-utils/>
+My Python utilities.
 
+-   **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
+-   **Documentation** <https://bsalanie.github.io/bs-python-utils/>
 
 ### Release notes
 
+#### 0.0.5 (May 8, 2023)
+
+Added `final_s` in `bsutils`.
+
 #### 0.0.4 (May 2, 2023)
+
 Added Legendre polynomials and quantile routines in `bsnputils`.
 
-#### 0.0.3  (April 24, 2023)
+#### 0.0.3 (April 24, 2023)
+
 Satisfied mypy.
 
-#### 0.0.2  (April 24, 2023)
-Fixed main PyPI page.
+#### 0.0.2 (April 24, 2023)
 
+Fixed main PyPI page.
```

