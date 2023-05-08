# Comparing `tmp/datarec-0.3.0.tar.gz` & `tmp/datarec-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datarec-0.3.0.tar", last modified: Sat May  6 05:33:00 2023, max compression
+gzip compressed data, was "datarec-0.3.1.tar", last modified: Mon May  8 00:25:18 2023, max compression
```

## Comparing `datarec-0.3.0.tar` & `datarec-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 05:33:00.467098 datarec-0.3.0/
--rw-rw-rw-   0        0        0    35285 2023-05-06 05:33:00.465094 datarec-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    34721 2023-05-06 04:35:32.000000 datarec-0.3.0/README.md
--rw-rw-rw-   0        0        0     1083 2023-05-06 04:35:32.000000 datarec-0.3.0/license
--rw-rw-rw-   0        0        0      666 2023-05-06 05:31:36.000000 datarec-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 05:33:00.468098 datarec-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-06 05:33:00.371102 datarec-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-06 05:33:00.397100 datarec-0.3.0/src/datarec/
--rw-rw-rw-   0        0        0      106 2023-05-06 04:35:32.000000 datarec-0.3.0/src/datarec/__init__.py
--rw-rw-rw-   0        0        0     5991 2023-05-06 05:30:21.000000 datarec-0.3.0/src/datarec/data.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:33:00.438100 datarec-0.3.0/src/datarec/tables/
--rw-rw-rw-   0        0        0      207 2023-05-06 04:35:32.000000 datarec-0.3.0/src/datarec/tables/__init__.py
--rw-rw-rw-   0        0        0     3467 2023-05-06 04:35:32.000000 datarec-0.3.0/src/datarec/tables/_is_close_numeric.py
--rw-rw-rw-   0        0        0     2449 2023-05-06 04:35:32.000000 datarec-0.3.0/src/datarec/tables/_is_equal.py
--rw-rw-rw-   0        0        0     2474 2023-05-06 04:35:32.000000 datarec-0.3.0/src/datarec/tables/_method_base.py
--rw-rw-rw-   0        0        0     3928 2023-05-06 04:35:32.000000 datarec-0.3.0/src/datarec/tables/_reconciler.py
--rw-rw-rw-   0        0        0     4567 2023-05-06 05:21:50.000000 datarec-0.3.0/src/datarec/tables/_summarizer.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:33:00.452099 datarec-0.3.0/src/datarec/utils/
--rw-rw-rw-   0        0        0      150 2023-05-06 04:35:32.000000 datarec-0.3.0/src/datarec/utils/__init__.py
--rw-rw-rw-   0        0        0      333 2023-05-06 04:35:32.000000 datarec-0.3.0/src/datarec/utils/_get_suffixed.py
--rw-rw-rw-   0        0        0      319 2023-05-06 04:35:32.000000 datarec-0.3.0/src/datarec/utils/_set_case.py
--rw-rw-rw-   0        0        0     5821 2023-05-06 04:35:32.000000 datarec-0.3.0/src/datarec/utils/functions.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:33:00.417103 datarec-0.3.0/src/datarec.egg-info/
--rw-rw-rw-   0        0        0    35285 2023-05-06 05:33:00.000000 datarec-0.3.0/src/datarec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      654 2023-05-06 05:33:00.000000 datarec-0.3.0/src/datarec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 05:33:00.000000 datarec-0.3.0/src/datarec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-06 05:33:00.000000 datarec-0.3.0/src/datarec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-06 05:33:00.000000 datarec-0.3.0/src/datarec.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 05:33:00.462095 datarec-0.3.0/tests/
--rw-rw-rw-   0        0        0     1756 2023-05-06 04:35:32.000000 datarec-0.3.0/tests/test_is_close.py
--rw-rw-rw-   0        0        0     1319 2023-05-06 04:35:32.000000 datarec-0.3.0/tests/test_is_equal.py
--rw-rw-rw-   0        0        0     3585 2023-05-06 05:26:02.000000 datarec-0.3.0/tests/test_summarizer.py
+drwxrwxrwx   0        0        0        0 2023-05-08 00:25:18.363357 datarec-0.3.1/
+-rw-rw-rw-   0        0        0    35285 2023-05-08 00:25:18.361360 datarec-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    34721 2023-05-08 00:15:57.000000 datarec-0.3.1/README.md
+-rw-rw-rw-   0        0        0     1083 2023-05-08 00:15:57.000000 datarec-0.3.1/license
+-rw-rw-rw-   0        0        0      666 2023-05-08 00:17:02.000000 datarec-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 00:25:18.364361 datarec-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 00:25:18.268359 datarec-0.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 00:25:18.289359 datarec-0.3.1/src/datarec/
+-rw-rw-rw-   0        0        0      106 2023-05-08 00:15:57.000000 datarec-0.3.1/src/datarec/__init__.py
+-rw-rw-rw-   0        0        0     5991 2023-05-08 00:15:57.000000 datarec-0.3.1/src/datarec/data.py
+drwxrwxrwx   0        0        0        0 2023-05-08 00:25:18.328357 datarec-0.3.1/src/datarec/tables/
+-rw-rw-rw-   0        0        0      207 2023-05-08 00:15:57.000000 datarec-0.3.1/src/datarec/tables/__init__.py
+-rw-rw-rw-   0        0        0     3764 2023-05-08 00:19:22.000000 datarec-0.3.1/src/datarec/tables/_is_close_numeric.py
+-rw-rw-rw-   0        0        0     2449 2023-05-08 00:15:57.000000 datarec-0.3.1/src/datarec/tables/_is_equal.py
+-rw-rw-rw-   0        0        0     2474 2023-05-08 00:15:57.000000 datarec-0.3.1/src/datarec/tables/_method_base.py
+-rw-rw-rw-   0        0        0     3928 2023-05-08 00:15:57.000000 datarec-0.3.1/src/datarec/tables/_reconciler.py
+-rw-rw-rw-   0        0        0     4567 2023-05-08 00:15:57.000000 datarec-0.3.1/src/datarec/tables/_summarizer.py
+drwxrwxrwx   0        0        0        0 2023-05-08 00:25:18.344361 datarec-0.3.1/src/datarec/utils/
+-rw-rw-rw-   0        0        0      150 2023-05-08 00:15:57.000000 datarec-0.3.1/src/datarec/utils/__init__.py
+-rw-rw-rw-   0        0        0      333 2023-05-08 00:15:57.000000 datarec-0.3.1/src/datarec/utils/_get_suffixed.py
+-rw-rw-rw-   0        0        0      319 2023-05-08 00:15:57.000000 datarec-0.3.1/src/datarec/utils/_set_case.py
+-rw-rw-rw-   0        0        0     5821 2023-05-08 00:15:57.000000 datarec-0.3.1/src/datarec/utils/functions.py
+drwxrwxrwx   0        0        0        0 2023-05-08 00:25:18.306359 datarec-0.3.1/src/datarec.egg-info/
+-rw-rw-rw-   0        0        0    35285 2023-05-08 00:25:18.000000 datarec-0.3.1/src/datarec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      654 2023-05-08 00:25:18.000000 datarec-0.3.1/src/datarec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 00:25:18.000000 datarec-0.3.1/src/datarec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-08 00:25:18.000000 datarec-0.3.1/src/datarec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-08 00:25:18.000000 datarec-0.3.1/src/datarec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 00:25:18.356358 datarec-0.3.1/tests/
+-rw-rw-rw-   0        0        0     1756 2023-05-08 00:15:58.000000 datarec-0.3.1/tests/test_is_close.py
+-rw-rw-rw-   0        0        0     1319 2023-05-08 00:15:58.000000 datarec-0.3.1/tests/test_is_equal.py
+-rw-rw-rw-   0        0        0     3585 2023-05-08 00:15:58.000000 datarec-0.3.1/tests/test_summarizer.py
```

### Comparing `datarec-0.3.0/PKG-INFO` & `datarec-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarec
-Version: 0.3.0
+Version: 0.3.1
 Summary: utilities for reconciling data
 Author-email: Chris Mamon <chrisam1993@live.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `datarec-0.3.0/README.md` & `datarec-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `datarec-0.3.0/license` & `datarec-0.3.1/license`

 * *Files identical despite different names*

### Comparing `datarec-0.3.0/pyproject.toml` & `datarec-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires      = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "datarec"
 description = "utilities for reconciling data"
-version     = "0.3.0"
+version     = "0.3.1"
 readme      = "README.md"
 dependencies = [
   "polars",
 ]
 authors         = [
   { name = "Chris Mamon", email = "chrisam1993@live.com" },
 ]
```

### Comparing `datarec-0.3.0/src/datarec/data.py` & `datarec-0.3.1/src/datarec/data.py`

 * *Files identical despite different names*

### Comparing `datarec-0.3.0/src/datarec/tables/_is_close_numeric.py` & `datarec-0.3.1/src/datarec/tables/_is_close_numeric.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,34 @@
         a_tol = kwargs["a_tol"]
         r_tol = kwargs["r_tol"]
 
         validation = merged.with_columns(
             [
                 (
                     (
-                        (pl.col(get_left(c)) - pl.col(get_right(c))).abs()
-                        < a_tol
-                    )
-                    | (
                         (
-                            (pl.col(get_left(c)) - pl.col(get_right(c)))
-                            / (
-                                (pl.col(get_left(c)) + pl.col(get_right(c)))
-                                / 2
-                                + 1e-20
-                            )
-                        ).abs()
-                        < r_tol
+                            (pl.col(get_left(c)) - pl.col(get_right(c))).abs()
+                            < a_tol
+                        )
+                        | (
+                            (
+                                (pl.col(get_left(c)) - pl.col(get_right(c)))
+                                / (
+                                    (
+                                        pl.col(get_left(c))
+                                        + pl.col(get_right(c))
+                                    )
+                                    / 2
+                                    + 1e-20
+                                )
+                            ).abs()
+                            < r_tol
+                        )
                     )
+                    | (pl.col(get_left(c)).eq(pl.col(get_right(c))))
                 )
                 .fill_null(pl.lit(False))
                 .alias("%s ~*%s*~" % (c, setcase("validation")))
                 for c in test_columns
             ]
         )
         return validation
```

### Comparing `datarec-0.3.0/src/datarec/tables/_is_equal.py` & `datarec-0.3.1/src/datarec/tables/_is_equal.py`

 * *Files identical despite different names*

### Comparing `datarec-0.3.0/src/datarec/tables/_method_base.py` & `datarec-0.3.1/src/datarec/tables/_method_base.py`

 * *Files identical despite different names*

### Comparing `datarec-0.3.0/src/datarec/tables/_reconciler.py` & `datarec-0.3.1/src/datarec/tables/_reconciler.py`

 * *Files identical despite different names*

### Comparing `datarec-0.3.0/src/datarec/tables/_summarizer.py` & `datarec-0.3.1/src/datarec/tables/_summarizer.py`

 * *Files identical despite different names*

### Comparing `datarec-0.3.0/src/datarec/utils/functions.py` & `datarec-0.3.1/src/datarec/utils/functions.py`

 * *Files identical despite different names*

### Comparing `datarec-0.3.0/src/datarec.egg-info/PKG-INFO` & `datarec-0.3.1/src/datarec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarec
-Version: 0.3.0
+Version: 0.3.1
 Summary: utilities for reconciling data
 Author-email: Chris Mamon <chrisam1993@live.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `datarec-0.3.0/src/datarec.egg-info/SOURCES.txt` & `datarec-0.3.1/src/datarec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datarec-0.3.0/tests/test_is_close.py` & `datarec-0.3.1/tests/test_is_close.py`

 * *Files identical despite different names*

### Comparing `datarec-0.3.0/tests/test_is_equal.py` & `datarec-0.3.1/tests/test_is_equal.py`

 * *Files identical despite different names*

### Comparing `datarec-0.3.0/tests/test_summarizer.py` & `datarec-0.3.1/tests/test_summarizer.py`

 * *Files identical despite different names*

