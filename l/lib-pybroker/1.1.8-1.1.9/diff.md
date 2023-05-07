# Comparing `tmp/lib-pybroker-1.1.8.tar.gz` & `tmp/lib-pybroker-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-pybroker-1.1.8.tar", last modified: Fri May  5 23:09:48 2023, max compression
+gzip compressed data, was "lib-pybroker-1.1.9.tar", last modified: Sat May  6 00:00:08 2023, max compression
```

## Comparing `lib-pybroker-1.1.8.tar` & `lib-pybroker-1.1.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:09:48.595905 lib-pybroker-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-05 23:09:48.595905 lib-pybroker-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-05 23:09:48.595905 lib-pybroker-1.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:09:48.583904 lib-pybroker-1.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:09:48.587904 lib-pybroker-1.1.8/src/lib_pybroker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-05 23:09:48.000000 lib-pybroker-1.1.8/src/lib_pybroker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-05 23:09:48.000000 lib-pybroker-1.1.8/src/lib_pybroker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 23:09:48.000000 lib-pybroker-1.1.8/src/lib_pybroker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-05 23:09:48.000000 lib-pybroker-1.1.8/src/lib_pybroker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 23:09:48.000000 lib-pybroker-1.1.8/src/lib_pybroker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:09:48.591904 lib-pybroker-1.1.8/src/pybroker/
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    46093 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    34553 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    38568 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25908 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    58375 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/vect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:09:48.595905 lib-pybroker-1.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    21990 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    18142 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    18876 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)    17300 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    76914 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_vect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:00:08.172451 lib-pybroker-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-06 00:00:08.172451 lib-pybroker-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-06 00:00:08.172451 lib-pybroker-1.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:00:08.164451 lib-pybroker-1.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:00:08.168451 lib-pybroker-1.1.9/src/lib_pybroker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-06 00:00:08.000000 lib-pybroker-1.1.9/src/lib_pybroker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-06 00:00:08.000000 lib-pybroker-1.1.9/src/lib_pybroker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:00:08.000000 lib-pybroker-1.1.9/src/lib_pybroker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-06 00:00:08.000000 lib-pybroker-1.1.9/src/lib_pybroker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 00:00:08.000000 lib-pybroker-1.1.9/src/lib_pybroker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:00:08.168451 lib-pybroker-1.1.9/src/pybroker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/src/pybroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/src/pybroker/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/src/pybroker/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/src/pybroker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46093 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/src/pybroker/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/src/pybroker/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34553 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/src/pybroker/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/src/pybroker/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/src/pybroker/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/src/pybroker/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38568 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/src/pybroker/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/src/pybroker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25908 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/src/pybroker/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58375 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/src/pybroker/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/src/pybroker/vect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:00:08.172451 lib-pybroker-1.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21990 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18142 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18876 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/tests/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/tests/test_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/tests/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17300 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/tests/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76914 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/tests/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-05 23:59:59.000000 lib-pybroker-1.1.9/tests/test_vect.py
```

### Comparing `lib-pybroker-1.1.8/LICENSE` & `lib-pybroker-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/PKG-INFO` & `lib-pybroker-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-pybroker
-Version: 1.1.8
+Version: 1.1.9
 Summary: Algorithmic trading with machine learning
 Home-page: http://www.pybroker.com
 Author: Edward West
 Author-email: edwest@pybroker.com
 License: Apache License 2.0 with Commons Clause
 Classifier: License :: Free for non-commercial use
 Description-Content-Type: text/markdown
```

### Comparing `lib-pybroker-1.1.8/README.md` & `lib-pybroker-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/setup.cfg` & `lib-pybroker-1.1.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 [options]
 package_dir = 
 	=src
 packages = find:
 include_package_data = True
 install_requires = 
 	alpaca-py>=0.7.2,<1
-	alpaca-trade-api>=2.3.0,<3
 	diskcache>=5.4.0,<6
 	joblib>=1.2.0,<2
 	numba>=0.56.3,<1
 	numpy>=1.23.4,<2
 	pandas>=1.5.1,<2
 	progressbar2>=4.1.1,<5
 	yfinance>=0.1.84,<1
@@ -44,15 +43,15 @@
 per-file-ignores = 
 	src/pybroker/*.py:E203,E402
 	src/pybroker/__init__.py:F401,E402
 	tests/*.py:E203,E402
 	tests/test_*:E203,E402,F403,F405
 
 [tox:tox]
-envlist = py39,py310
+envlist = py39,py310,py311
 isolated_build = True
 
 [testenv]
 deps = 
 	pytest
 	pytest-cov
 	pytest-instafail
```

### Comparing `lib-pybroker-1.1.8/src/lib_pybroker.egg-info/PKG-INFO` & `lib-pybroker-1.1.9/src/lib_pybroker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-pybroker
-Version: 1.1.8
+Version: 1.1.9
 Summary: Algorithmic trading with machine learning
 Home-page: http://www.pybroker.com
 Author: Edward West
 Author-email: edwest@pybroker.com
 License: Apache License 2.0 with Commons Clause
 Classifier: License :: Free for non-commercial use
 Description-Content-Type: text/markdown
```

### Comparing `lib-pybroker-1.1.8/src/lib_pybroker.egg-info/SOURCES.txt` & `lib-pybroker-1.1.9/src/lib_pybroker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/src/pybroker/__init__.py` & `lib-pybroker-1.1.9/src/pybroker/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,8 +47,8 @@
 from .strategy import Strategy, TestResult
 from .vect import cross, highv, lowv, sumv
 
 # Temporary fix for regression in Numba 0.57.0
 # https://github.com/numba/numba/issues/8940
 from numba.np.unsafe import ndarray
 
-__version__ = "1.1.8"
+__version__ = "1.1.9"
```

### Comparing `lib-pybroker-1.1.8/src/pybroker/cache.py` & `lib-pybroker-1.1.9/src/pybroker/cache.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/src/pybroker/common.py` & `lib-pybroker-1.1.9/src/pybroker/common.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/src/pybroker/config.py` & `lib-pybroker-1.1.9/src/pybroker/config.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/src/pybroker/context.py` & `lib-pybroker-1.1.9/src/pybroker/context.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/src/pybroker/data.py` & `lib-pybroker-1.1.9/src/pybroker/data.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/src/pybroker/eval.py` & `lib-pybroker-1.1.9/src/pybroker/eval.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/src/pybroker/indicator.py` & `lib-pybroker-1.1.9/src/pybroker/indicator.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/src/pybroker/log.py` & `lib-pybroker-1.1.9/src/pybroker/log.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/src/pybroker/model.py` & `lib-pybroker-1.1.9/src/pybroker/model.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/src/pybroker/portfolio.py` & `lib-pybroker-1.1.9/src/pybroker/portfolio.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/src/pybroker/scope.py` & `lib-pybroker-1.1.9/src/pybroker/scope.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/src/pybroker/strategy.py` & `lib-pybroker-1.1.9/src/pybroker/strategy.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/src/pybroker/vect.py` & `lib-pybroker-1.1.9/src/pybroker/vect.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/tests/test_cache.py` & `lib-pybroker-1.1.9/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/tests/test_common.py` & `lib-pybroker-1.1.9/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/tests/test_context.py` & `lib-pybroker-1.1.9/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/tests/test_data.py` & `lib-pybroker-1.1.9/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/tests/test_eval.py` & `lib-pybroker-1.1.9/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/tests/test_indicator.py` & `lib-pybroker-1.1.9/tests/test_indicator.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/tests/test_log.py` & `lib-pybroker-1.1.9/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/tests/test_model.py` & `lib-pybroker-1.1.9/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/tests/test_portfolio.py` & `lib-pybroker-1.1.9/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/tests/test_scope.py` & `lib-pybroker-1.1.9/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/tests/test_strategy.py` & `lib-pybroker-1.1.9/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.8/tests/test_vect.py` & `lib-pybroker-1.1.9/tests/test_vect.py`

 * *Files identical despite different names*

