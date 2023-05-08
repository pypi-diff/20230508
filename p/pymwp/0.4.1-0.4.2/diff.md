# Comparing `tmp/pymwp-0.4.1.tar.gz` & `tmp/pymwp-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymwp-0.4.1.tar", last modified: Sun Apr 30 04:52:45 2023, max compression
+gzip compressed data, was "pymwp-0.4.2.tar", last modified: Mon May  8 15:41:55 2023, max compression
```

## Comparing `pymwp-0.4.1.tar` & `pymwp-0.4.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:52:45.978363 pymwp-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-30 04:52:13.000000 pymwp-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-30 04:52:13.000000 pymwp-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-04-30 04:52:45.978363 pymwp-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-30 04:52:13.000000 pymwp-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:52:45.974363 pymwp-0.4.1/pymwp/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18891 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/bound.py
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/delta_graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/monomial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    18771 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/polynomial.py
--rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/relation_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-30 04:52:13.000000 pymwp-0.4.1/pymwp/semiring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:52:45.974363 pymwp-0.4.1/pymwp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-04-30 04:52:45.000000 pymwp-0.4.1/pymwp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-30 04:52:45.000000 pymwp-0.4.1/pymwp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 04:52:45.000000 pymwp-0.4.1/pymwp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-30 04:52:45.000000 pymwp-0.4.1/pymwp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-30 04:52:45.000000 pymwp-0.4.1/pymwp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 04:52:45.000000 pymwp-0.4.1/pymwp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-30 04:52:13.000000 pymwp-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 04:52:45.978363 pymwp-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-30 04:52:13.000000 pymwp-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:52:45.978363 pymwp-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:52:45.978363 pymwp-0.4.1/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/mocks/ast_mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_bound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_choices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_delta_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_monomial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_polynomial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-30 04:52:13.000000 pymwp-0.4.1/tests/test_relation_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:41:55.379270 pymwp-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 15:40:58.000000 pymwp-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-08 15:40:58.000000 pymwp-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-08 15:41:55.379270 pymwp-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-08 15:40:58.000000 pymwp-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:41:55.379270 pymwp-0.4.2/pymwp/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-08 15:40:58.000000 pymwp-0.4.2/pymwp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-08 15:40:58.000000 pymwp-0.4.2/pymwp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18680 2023-05-08 15:40:58.000000 pymwp-0.4.2/pymwp/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-08 15:40:58.000000 pymwp-0.4.2/pymwp/bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-05-08 15:40:58.000000 pymwp-0.4.2/pymwp/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-08 15:40:58.000000 pymwp-0.4.2/pymwp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-05-08 15:40:58.000000 pymwp-0.4.2/pymwp/delta_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-08 15:40:58.000000 pymwp-0.4.2/pymwp/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-05-08 15:40:58.000000 pymwp-0.4.2/pymwp/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-08 15:40:58.000000 pymwp-0.4.2/pymwp/monomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-08 15:40:58.000000 pymwp-0.4.2/pymwp/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18771 2023-05-08 15:40:58.000000 pymwp-0.4.2/pymwp/polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-05-08 15:40:58.000000 pymwp-0.4.2/pymwp/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-05-08 15:40:58.000000 pymwp-0.4.2/pymwp/relation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-05-08 15:40:58.000000 pymwp-0.4.2/pymwp/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-08 15:40:58.000000 pymwp-0.4.2/pymwp/semiring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:41:55.379270 pymwp-0.4.2/pymwp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-08 15:41:55.000000 pymwp-0.4.2/pymwp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-08 15:41:55.000000 pymwp-0.4.2/pymwp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:41:55.000000 pymwp-0.4.2/pymwp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-08 15:41:55.000000 pymwp-0.4.2/pymwp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 15:41:55.000000 pymwp-0.4.2/pymwp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 15:41:55.000000 pymwp-0.4.2/pymwp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-08 15:40:58.000000 pymwp-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:41:55.379270 pymwp-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-08 15:40:58.000000 pymwp-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:41:55.379270 pymwp-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 15:40:58.000000 pymwp-0.4.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:41:55.379270 pymwp-0.4.2/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-08 15:40:58.000000 pymwp-0.4.2/tests/mocks/ast_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-05-08 15:40:58.000000 pymwp-0.4.2/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-08 15:40:58.000000 pymwp-0.4.2/tests/test_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-08 15:40:58.000000 pymwp-0.4.2/tests/test_choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-08 15:40:58.000000 pymwp-0.4.2/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-08 15:40:58.000000 pymwp-0.4.2/tests/test_delta_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-08 15:40:58.000000 pymwp-0.4.2/tests/test_file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-05-08 15:40:58.000000 pymwp-0.4.2/tests/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-08 15:40:58.000000 pymwp-0.4.2/tests/test_monomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-08 15:40:58.000000 pymwp-0.4.2/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-05-08 15:40:58.000000 pymwp-0.4.2/tests/test_polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-08 15:40:58.000000 pymwp-0.4.2/tests/test_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-08 15:40:58.000000 pymwp-0.4.2/tests/test_relation_list.py
```

### Comparing `pymwp-0.4.1/LICENSE` & `pymwp-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/PKG-INFO` & `pymwp-0.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: pymwp
-Version: 0.4.1
+Version: 0.4.2
 Summary: Implementation of MWP analysis on C code in Python.
 Home-page: https://github.com/statycc/pymwp
 Author: Clément Aubert, Thomas Rubiano, Neea Rusch, Thomas Seiller
 Author-email: nrusch@augusta.edu
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/statycc/pymwp/issues
 Project-URL: Documentation, https://statycc.github.io/pymwp/
+Project-URL: Source Code, https://github.com/statycc/pymwp
+Project-URL: Archive, https://doi.org/10.5281/zenodo.7879822
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -30,29 +32,30 @@
 
 # pymwp: MWP analysis in Python
 
 [![build](https://github.com/statycc/pymwp/actions/workflows/build.yaml/badge.svg)](https://github.com/statycc/pymwp/actions/workflows/build.yaml)
 [![codecov](https://codecov.io/gh/statycc/pymwp/branch/main/graph/badge.svg?token=4v3zRbkAjM)](https://codecov.io/gh/statycc/pymwp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pymwp)](https://pypi.org/project/pymwp/)
 [![PyPI](https://img.shields.io/pypi/v/pymwp)](https://pypi.org/project/pymwp/)
+[![DOI](https://zenodo.org/badge/355822953.svg)](https://zenodo.org/badge/latestdoi/355822953)
+
 
 <!--
     do not remove start and end comments (e.g. "include-start", "include-end").
     They are markers for what to include in the docs, but feel free to edit 
     the inner content.
 -->
 
 <!--desc-start-->
 
 pymwp is a tool for automatically performing static analysis on programs written in C.
 It is inspired by [_"A Flow Calculus of mwp-Bounds for Complexity Analysis"_](https://doi.org/10.1145/1555746.1555752).
 It analyzes resource usage and determines if a program's variables growth rates are no more than polynomially related to their inputs sizes.
 Try our online [demo](https://statycc.github.io/pymwp/demo/) to see it action.
 For more details on usage and behavior, see pymwp [documentation](https://statycc.github.io/pymwp/), particularly [supported C language features](https://statycc.github.io/pymwp/features/).
-See latest [profiling results](https://github.com/statycc/pymwp/releases/tag/profile-latest) for interesting performance metrics. 
 
 <!--desc-end--> 
 
 ## Documentation and Demo
 
 Refer to **[statycc.github.io/pymwp](https://statycc.github.io/pymwp/)** for a documentation, an [online demo](https://statycc.github.io/pymwp/demo/), and a presentation of [examples](https://statycc.github.io/pymwp/examples/).
 
@@ -93,14 +96,17 @@
 matrix[2][1] = Polynomial('p')
 
 show(matrix)
 ```
 
 See [modules documentation](https://statycc.github.io/pymwp/analysis/) for available methods.
 
+
+
+
 ## Running from source
 
 If you want to use the latest stable version (possibly ahead of 
 latest release), use the version from source following these steps.
 
 1. Clone the repository
```

### Comparing `pymwp-0.4.1/README.md` & `pymwp-0.4.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # pymwp: MWP analysis in Python
 
 [![build](https://github.com/statycc/pymwp/actions/workflows/build.yaml/badge.svg)](https://github.com/statycc/pymwp/actions/workflows/build.yaml)
 [![codecov](https://codecov.io/gh/statycc/pymwp/branch/main/graph/badge.svg?token=4v3zRbkAjM)](https://codecov.io/gh/statycc/pymwp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pymwp)](https://pypi.org/project/pymwp/)
 [![PyPI](https://img.shields.io/pypi/v/pymwp)](https://pypi.org/project/pymwp/)
+[![DOI](https://zenodo.org/badge/355822953.svg)](https://zenodo.org/badge/latestdoi/355822953)
+
 
 <!--
     do not remove start and end comments (e.g. "include-start", "include-end").
     They are markers for what to include in the docs, but feel free to edit 
     the inner content.
 -->
 
 <!--desc-start-->
 
 pymwp is a tool for automatically performing static analysis on programs written in C.
 It is inspired by [_"A Flow Calculus of mwp-Bounds for Complexity Analysis"_](https://doi.org/10.1145/1555746.1555752).
 It analyzes resource usage and determines if a program's variables growth rates are no more than polynomially related to their inputs sizes.
 Try our online [demo](https://statycc.github.io/pymwp/demo/) to see it action.
 For more details on usage and behavior, see pymwp [documentation](https://statycc.github.io/pymwp/), particularly [supported C language features](https://statycc.github.io/pymwp/features/).
-See latest [profiling results](https://github.com/statycc/pymwp/releases/tag/profile-latest) for interesting performance metrics. 
 
 <!--desc-end--> 
 
 ## Documentation and Demo
 
 Refer to **[statycc.github.io/pymwp](https://statycc.github.io/pymwp/)** for a documentation, an [online demo](https://statycc.github.io/pymwp/demo/), and a presentation of [examples](https://statycc.github.io/pymwp/examples/).
 
@@ -63,14 +64,17 @@
 matrix[2][1] = Polynomial('p')
 
 show(matrix)
 ```
 
 See [modules documentation](https://statycc.github.io/pymwp/analysis/) for available methods.
 
+
+
+
 ## Running from source
 
 If you want to use the latest stable version (possibly ahead of 
 latest release), use the version from source following these steps.
 
 1. Clone the repository
```

### Comparing `pymwp-0.4.1/pymwp/__init__.py` & `pymwp-0.4.2/pymwp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 pymwp: implementation of MWP analysis on C code in Python.
 """
 
 __title__ = "pymwp"
 __author__ = "Clément Aubert, Thomas Rubiano, Neea Rusch, Thomas Seiller"
 __license__ = "GPLv3"
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 from pymwp.parser import Parser
 from pymwp.delta_graphs import DeltaGraph
 from pymwp.choice import Choices
 from pymwp.monomial import Monomial
 from pymwp.polynomial import Polynomial
 from pymwp.relation_list import RelationList
```

### Comparing `pymwp-0.4.1/pymwp/__main__.py` & `pymwp-0.4.2/pymwp/__main__.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/pymwp/analysis.py` & `pymwp-0.4.2/pymwp/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,25 +342,18 @@
             relation_list: current relation list state
             dg: [DeltaGraph instance](delta_graphs.md#pymwp.delta_graphs)
 
         Returns:
             Updated index value, relation list, and an exit flag.
         """
         if node is not None:
-            # when branch has braces
-            if hasattr(node, 'block_items'):
-                for child in node.block_items:
-                    index, rel_list, exit_ = Analysis.compute_relation(
-                        index, child, dg)
-                    if exit_:
-                        return index, exit_
-                    relation_list.composition(rel_list)
-            else:
-                index, rel_list, exit_ = Analysis.compute_relation(
-                    index, node, dg)
+            for child in node.block_items \
+                    if hasattr(node, 'block_items') else [node]:
+                index, rel_list, exit_ = Analysis \
+                    .compute_relation(index, child, dg)
                 if exit_:
                     return index, exit_
                 relation_list.composition(rel_list)
         return index, False
 
     @staticmethod
     def while_(index: int, node: pr.While, dg: DeltaGraph) \
@@ -374,15 +367,16 @@
 
         Returns:
             Updated index value, relation list, and an exit flag.
         """
         logger.debug("analysing While")
 
         relations = RelationList()
-        for child in node.stmt.block_items:
+        for child in node.stmt.block_items \
+                if hasattr(node, 'block_items') else [node.stmt]:
             index, rel_list, exit_ = Analysis.compute_relation(
                 index, child, dg)
             if exit_:
                 return index, rel_list, exit_
             relations.composition(rel_list)
 
         logger.debug('while loop fixpoint')
@@ -442,14 +436,15 @@
             node: compound AST node
             dg: [DeltaGraph instance](delta_graphs.md#pymwp.delta_graphs)
 
         Returns:
             Updated index value, relation list, and an exit flag.
         """
         relations = RelationList()
+
         if node.block_items:
             for node in node.block_items:
                 index, rel_list, exit_ = Analysis.compute_relation(
                     index, node, dg)
                 relations.composition(rel_list)
                 if exit_:
                     return index, relations, True
```

### Comparing `pymwp-0.4.1/pymwp/bound.py` & `pymwp-0.4.2/pymwp/bound.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,20 +51,42 @@
         self.z = HonestPoly('*', *z)
 
     def __str__(self):
         return self.bound_poly(self)
 
     @property
     def bound_triple(self) -> Tuple[Tuple[str], Tuple[str], Tuple[str]]:
-        """Alternative bounds representation"""
+        """Alternative bounds representation.
+
+        Example:
+            ```
+            (X1,) (,) (X4, X5)
+            ```
+
+        Returns:
+            Current bound as $(m_1,...m_n), (w_1,...w_n), (p_1,...p_n)$
+                where the first contains list of variables in m,
+                second contains variables in w, and last in p (if any).
+        """
         return tuple(self.x.vars), tuple(self.y.vars), tuple(self.z.vars)
 
     @property
     def bound_triple_str(self) -> str:
-        """Alternative bounds representation"""
+        """Alternative bounds representation.
+
+        Example:
+            ```
+            X1;;X4,X5
+            ```
+
+        Returns:
+            Current bound as `m;w;p` where the first section contains
+                list of variables in m, second contains variables in w,
+                and last in p (if any).
+        """
         return f'{";".join([",".join(v) for v in self.bound_triple])}'
 
     @staticmethod
     def parse_triple_str(value: str = None):
         """Restore bound from triple format"""
         return [v.split(',') if v else [] for v in value.split(";")] \
             if value else ([], [], [])
@@ -100,35 +122,44 @@
     """
 
     def __init__(self, bounds: dict = None):
         self.bound_dict = dict([
             (k, MwpBound(triple=v)) for k, v in bounds.items()]) \
             if bounds else {}
 
-    def calculate(self, relation: SimpleRelation):
-        """Calculate bound from a simple-valued matrix"""
+    def calculate(self, relation: SimpleRelation) -> Bound:
+        """Calculate bound from a simple-valued matrix.
+
+        Arguments
+            relation: a simple-valued relation.
+
+        Returns:
+            The bound for the relation.
+        """
         vars_, matrix = relation.variables, relation.matrix
         for col_id, name in enumerate(vars_):
             var_bound = MwpBound()
             for row_id in range(len(matrix)):
                 var_bound.append(matrix[row_id][col_id], vars_[row_id])
             self.bound_dict[name] = var_bound
         return self
 
     def to_dict(self) -> dict:
         """Get serializable dictionary representation of a bound."""
         return dict([(k, v.bound_triple_str)
                      for k, v in self.bound_dict.items()])
 
-    def show_poly(self, compact=False, significant=False) -> str:
+    def show_poly(
+            self, compact: bool = False, significant: bool = False
+    ) -> str:
         """Format a nice display string of bounds.
 
         Arguments:
-            compact - reduce whitespace in the output
-            significant - omit bounds that depend only on self
+            compact: reduce whitespace in the output
+            significant: omit bounds that depend only on self
 
         Returns:
             A formatted string of the bound.
         """
         return ' ∧ '.join([
             f'{k}′{"≤" if compact else " ≤ "}{v}'
             for k, v in self.bound_dict.items()
```

### Comparing `pymwp-0.4.1/pymwp/choice.py` & `pymwp-0.4.2/pymwp/choice.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/pymwp/delta_graphs.py` & `pymwp-0.4.2/pymwp/delta_graphs.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/pymwp/file_io.py` & `pymwp-0.4.2/pymwp/file_io.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/pymwp/matrix.py` & `pymwp-0.4.2/pymwp/matrix.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/pymwp/monomial.py` & `pymwp-0.4.2/pymwp/monomial.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/pymwp/parser.py` & `pymwp-0.4.2/pymwp/parser.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/pymwp/polynomial.py` & `pymwp-0.4.2/pymwp/polynomial.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/pymwp/relation.py` & `pymwp-0.4.2/pymwp/relation.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,16 +290,16 @@
 
     def infty_vars(self) -> Dict[str, List[str]]:
         """Identify all variable pairs that for some choices, can raise
         infinity result.
 
         Returns:
             Dictionary of potentially infinite dependencies, where
-            the key is source variable and value is list of targets;
-            All entries are non-empty.
+                the key is source variable and value is list of targets.
+                All entries are non-empty.
         """
         vars_ = self.variables
         return dict([(x, y) for x, y in [
             (src, [tgt for tgt, p in zip(vars_, polys) if p.some_infty])
             for src, polys in zip(vars_, self.matrix)] if len(y) != 0])
 
     def infty_pairs(self) -> str:
@@ -389,12 +389,12 @@
 
         # generate valid choices
         return Choices.generate(choices, index, infinity_deltas)
 
 
 class SimpleRelation(Relation):
     """Specialized instance of relation, where matrix contains only
-       scalar values, no Polynomials."""
+       scalar values, no polynomials."""
 
     def __init__(self, variables: Optional[List[str]] = None,
                  matrix: Optional[List[List[str]]] = None):
         super().__init__(variables, matrix)
```

### Comparing `pymwp-0.4.1/pymwp/relation_list.py` & `pymwp-0.4.2/pymwp/relation_list.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/pymwp/semiring.py` & `pymwp-0.4.2/pymwp/semiring.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/pymwp.egg-info/PKG-INFO` & `pymwp-0.4.2/pymwp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: pymwp
-Version: 0.4.1
+Version: 0.4.2
 Summary: Implementation of MWP analysis on C code in Python.
 Home-page: https://github.com/statycc/pymwp
 Author: Clément Aubert, Thomas Rubiano, Neea Rusch, Thomas Seiller
 Author-email: nrusch@augusta.edu
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/statycc/pymwp/issues
 Project-URL: Documentation, https://statycc.github.io/pymwp/
+Project-URL: Source Code, https://github.com/statycc/pymwp
+Project-URL: Archive, https://doi.org/10.5281/zenodo.7879822
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -30,29 +32,30 @@
 
 # pymwp: MWP analysis in Python
 
 [![build](https://github.com/statycc/pymwp/actions/workflows/build.yaml/badge.svg)](https://github.com/statycc/pymwp/actions/workflows/build.yaml)
 [![codecov](https://codecov.io/gh/statycc/pymwp/branch/main/graph/badge.svg?token=4v3zRbkAjM)](https://codecov.io/gh/statycc/pymwp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pymwp)](https://pypi.org/project/pymwp/)
 [![PyPI](https://img.shields.io/pypi/v/pymwp)](https://pypi.org/project/pymwp/)
+[![DOI](https://zenodo.org/badge/355822953.svg)](https://zenodo.org/badge/latestdoi/355822953)
+
 
 <!--
     do not remove start and end comments (e.g. "include-start", "include-end").
     They are markers for what to include in the docs, but feel free to edit 
     the inner content.
 -->
 
 <!--desc-start-->
 
 pymwp is a tool for automatically performing static analysis on programs written in C.
 It is inspired by [_"A Flow Calculus of mwp-Bounds for Complexity Analysis"_](https://doi.org/10.1145/1555746.1555752).
 It analyzes resource usage and determines if a program's variables growth rates are no more than polynomially related to their inputs sizes.
 Try our online [demo](https://statycc.github.io/pymwp/demo/) to see it action.
 For more details on usage and behavior, see pymwp [documentation](https://statycc.github.io/pymwp/), particularly [supported C language features](https://statycc.github.io/pymwp/features/).
-See latest [profiling results](https://github.com/statycc/pymwp/releases/tag/profile-latest) for interesting performance metrics. 
 
 <!--desc-end--> 
 
 ## Documentation and Demo
 
 Refer to **[statycc.github.io/pymwp](https://statycc.github.io/pymwp/)** for a documentation, an [online demo](https://statycc.github.io/pymwp/demo/), and a presentation of [examples](https://statycc.github.io/pymwp/examples/).
 
@@ -93,14 +96,17 @@
 matrix[2][1] = Polynomial('p')
 
 show(matrix)
 ```
 
 See [modules documentation](https://statycc.github.io/pymwp/analysis/) for available methods.
 
+
+
+
 ## Running from source
 
 If you want to use the latest stable version (possibly ahead of 
 latest release), use the version from source following these steps.
 
 1. Clone the repository
```

### Comparing `pymwp-0.4.1/pymwp.egg-info/SOURCES.txt` & `pymwp-0.4.2/pymwp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/setup.py` & `pymwp-0.4.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 __title__ = "pymwp"
 __author__ = "Clément Aubert, Thomas Rubiano, Neea Rusch, Thomas Seiller"
 __desc__ = "Implementation of MWP analysis on C code in Python."
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name=__title__,
     version=__version__,
@@ -19,21 +19,23 @@
     description=__desc__,
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/statycc/pymwp',
     project_urls={
         'Bug Tracker': 'https://github.com/statycc/pymwp/issues',
         'Documentation': 'https://statycc.github.io/pymwp/',
+        'Source Code': 'https://github.com/statycc/pymwp',
+        'Archive': 'https://doi.org/10.5281/zenodo.7879822'
     },
     package_data={"": ["LICENSE"], },
     include_package_data=True,
     classifiers=[
         'Natural Language :: English',
         'Intended Audience :: Science/Research',
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
```

### Comparing `pymwp-0.4.1/tests/mocks/ast_mocks.py` & `pymwp-0.4.2/tests/mocks/ast_mocks.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/tests/test_analysis.py` & `pymwp-0.4.2/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/tests/test_bound.py` & `pymwp-0.4.2/tests/test_bound.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/tests/test_choices.py` & `pymwp-0.4.2/tests/test_choices.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/tests/test_compare.py` & `pymwp-0.4.2/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/tests/test_delta_graph.py` & `pymwp-0.4.2/tests/test_delta_graph.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/tests/test_file_io.py` & `pymwp-0.4.2/tests/test_file_io.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/tests/test_matrix.py` & `pymwp-0.4.2/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/tests/test_monomial.py` & `pymwp-0.4.2/tests/test_monomial.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/tests/test_parser.py` & `pymwp-0.4.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/tests/test_polynomial.py` & `pymwp-0.4.2/tests/test_polynomial.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/tests/test_relation.py` & `pymwp-0.4.2/tests/test_relation.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.4.1/tests/test_relation_list.py` & `pymwp-0.4.2/tests/test_relation_list.py`

 * *Files identical despite different names*

