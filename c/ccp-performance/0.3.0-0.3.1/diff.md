# Comparing `tmp/ccp-performance-0.3.0.tar.gz` & `tmp/ccp-performance-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/ccp/ccp/dist/.tmp-hlzohd_b/ccp-performance-0.3.0.tar", last modified: Mon May  8 15:36:37 2023, max compression
+gzip compressed data, was "/home/runner/work/ccp/ccp/dist/.tmp-3nffs68v/ccp-performance-0.3.1.tar", last modified: Mon May  8 16:12:37 2023, max compression
```

## Comparing `ccp-performance-0.3.0.tar` & `ccp-performance-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-08 15:36:28.000000 ccp-performance-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-08 15:36:28.000000 ccp-performance-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-08 15:36:28.000000 ccp-performance-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/ccp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/ccp/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/ccp/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   288892 2023-05-08 15:36:28.000000 ccp-performance-0.3.0/ccp/tests/data/UTGCA_1231_A_1s.csv
--rw-r--r--   0 runner    (1001) docker     (123)   502046 2023-05-08 15:36:28.000000 ccp-performance-0.3.0/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-08 15:36:28.000000 ccp-performance-0.3.0/ccp/tests/data/lp-sec1-caso-a-eff.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-08 15:36:28.000000 ccp-performance-0.3.0/ccp/tests/data/lp-sec1-caso-a-head.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-08 15:36:28.000000 ccp-performance-0.3.0/ccp/tests/data/normal-eff.csv
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-08 15:36:28.000000 ccp-performance-0.3.0/ccp/tests/data/normal-head.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/ccp_performance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/ccp_performance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/ccp_performance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/ccp_performance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/ccp_performance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/ccp_performance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-08 15:36:28.000000 ccp-performance-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-08 16:12:26.000000 ccp-performance-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-08 16:12:26.000000 ccp-performance-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-08 16:12:26.000000 ccp-performance-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/ccp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/ccp/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/ccp/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   288892 2023-05-08 16:12:26.000000 ccp-performance-0.3.1/ccp/tests/data/UTGCA_1231_A_1s.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   502046 2023-05-08 16:12:26.000000 ccp-performance-0.3.1/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-08 16:12:26.000000 ccp-performance-0.3.1/ccp/tests/data/lp-sec1-caso-a-eff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-08 16:12:26.000000 ccp-performance-0.3.1/ccp/tests/data/lp-sec1-caso-a-head.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-08 16:12:26.000000 ccp-performance-0.3.1/ccp/tests/data/normal-eff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-08 16:12:26.000000 ccp-performance-0.3.1/ccp/tests/data/normal-head.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/ccp_performance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/ccp_performance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/ccp_performance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/ccp_performance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/ccp_performance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/ccp_performance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:12:37.000000 ccp-performance-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-08 16:12:26.000000 ccp-performance-0.3.1/setup.py
```

### Comparing `ccp-performance-0.3.0/LICENSE` & `ccp-performance-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.0/PKG-INFO` & `ccp-performance-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: ccp-performance
-Version: 0.3.0
+Version: 0.3.1
 Summary: Centrifugal Compressor Performance calculation.
 Author: Raphael Timbó
 Author-email: raphaelts@petrobras.com.br
 License: Apache License 2.0
+Project-URL: Documentation, https://ccp-centrifugal-compressor-performance.readthedocs.io/en/stable/
+Project-URL: Bug Tracker, https://github.com/petrobras/ccp/issues
+Project-URL: Source Code, https://github.com/petrobras/ccp
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -18,17 +21,15 @@
 
 # <img src="https://ccp-centrifugal-compressor-performance.readthedocs.io/en/latest/_static/ccp.png" alt="drawing" width="40"/> Centrifugal Compressor Performance
 
 [![PyPI Version](https://img.shields.io/pypi/v/ccp-performance.svg)](https://pypi.org/project/ccp-performance/)
 [![License](https://img.shields.io/pypi/l/ccp-performance.svg)](https://github.com/raphaeltimbo/ccp/blob/master/LICENSE)
 [![code style black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-ccp is a python library for calculation of centrifugal compressor performance. It is based on the book of [Ludtke04] and uses CoolProp REFPROP for the gas properties calculations.
-
-Online documentation is available at [here](https://ccp-centrifugal-compressor-performance.readthedocs.io/en/latest/).
+ccp is a python library for calculation of centrifugal compressor performance. It uses CoolProp/REFPROP for the gas properties calculations.
 
 ```python
 import ccp
 
 # ccp uses pint to handle units. Q_ is a pint quantity.
 # If a pint quantity is not provided, SI units are assumed.
 Q_ = ccp.Q_
@@ -70,7 +71,17 @@
 
 imp = ccp.Impeller([point0, point1])
 
 # Get results from the Impeller with methods such as
 imp.head_plot()
 imp.disch.T_plot()
 ```
+
+# Documentation 
+Access the documentation [here](https://ccp-centrifugal-compressor-performance.readthedocs.io/en/stable/).
+
+# Questions
+If you have any questions, you can use the [Discussions](https://github.com/petrobras/ccp/discussions) area in the repository.
+
+# Contributing to ccp
+ROSS is a community-driven project. If you want to contribute to the project, please
+check [CONTRIBUTING.md](https://github.com/petrobras/ccp/blob/master/CONTRIBUTING.md).
```

### Comparing `ccp-performance-0.3.0/README.md` & `ccp-performance-0.3.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # <img src="https://ccp-centrifugal-compressor-performance.readthedocs.io/en/latest/_static/ccp.png" alt="drawing" width="40"/> Centrifugal Compressor Performance
 
 [![PyPI Version](https://img.shields.io/pypi/v/ccp-performance.svg)](https://pypi.org/project/ccp-performance/)
 [![License](https://img.shields.io/pypi/l/ccp-performance.svg)](https://github.com/raphaeltimbo/ccp/blob/master/LICENSE)
 [![code style black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-ccp is a python library for calculation of centrifugal compressor performance. It is based on the book of [Ludtke04] and uses CoolProp REFPROP for the gas properties calculations.
-
-Online documentation is available at [here](https://ccp-centrifugal-compressor-performance.readthedocs.io/en/latest/).
+ccp is a python library for calculation of centrifugal compressor performance. It uses CoolProp/REFPROP for the gas properties calculations.
 
 ```python
 import ccp
 
 # ccp uses pint to handle units. Q_ is a pint quantity.
 # If a pint quantity is not provided, SI units are assumed.
 Q_ = ccp.Q_
@@ -51,8 +49,18 @@
 # Create an impeller with those points:
 
 imp = ccp.Impeller([point0, point1])
 
 # Get results from the Impeller with methods such as
 imp.head_plot()
 imp.disch.T_plot()
-```
+```
+
+# Documentation 
+Access the documentation [here](https://ccp-centrifugal-compressor-performance.readthedocs.io/en/stable/).
+
+# Questions
+If you have any questions, you can use the [Discussions](https://github.com/petrobras/ccp/discussions) area in the repository.
+
+# Contributing to ccp
+ROSS is a community-driven project. If you want to contribute to the project, please
+check [CONTRIBUTING.md](https://github.com/petrobras/ccp/blob/master/CONTRIBUTING.md).
```

### Comparing `ccp-performance-0.3.0/ccp/tests/data/UTGCA_1231_A_1s.csv` & `ccp-performance-0.3.1/ccp/tests/data/UTGCA_1231_A_1s.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.0/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h` & `ccp-performance-0.3.1/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.0/ccp/tests/data/lp-sec1-caso-a-eff.csv` & `ccp-performance-0.3.1/ccp/tests/data/lp-sec1-caso-a-eff.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.0/ccp/tests/data/lp-sec1-caso-a-head.csv` & `ccp-performance-0.3.1/ccp/tests/data/lp-sec1-caso-a-head.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.0/ccp/tests/data/normal-eff.csv` & `ccp-performance-0.3.1/ccp/tests/data/normal-eff.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.0/ccp/tests/data/normal-head.csv` & `ccp-performance-0.3.1/ccp/tests/data/normal-head.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.0/ccp_performance.egg-info/PKG-INFO` & `ccp-performance-0.3.1/ccp_performance.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: ccp-performance
-Version: 0.3.0
+Version: 0.3.1
 Summary: Centrifugal Compressor Performance calculation.
 Author: Raphael Timbó
 Author-email: raphaelts@petrobras.com.br
 License: Apache License 2.0
+Project-URL: Documentation, https://ccp-centrifugal-compressor-performance.readthedocs.io/en/stable/
+Project-URL: Bug Tracker, https://github.com/petrobras/ccp/issues
+Project-URL: Source Code, https://github.com/petrobras/ccp
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -18,17 +21,15 @@
 
 # <img src="https://ccp-centrifugal-compressor-performance.readthedocs.io/en/latest/_static/ccp.png" alt="drawing" width="40"/> Centrifugal Compressor Performance
 
 [![PyPI Version](https://img.shields.io/pypi/v/ccp-performance.svg)](https://pypi.org/project/ccp-performance/)
 [![License](https://img.shields.io/pypi/l/ccp-performance.svg)](https://github.com/raphaeltimbo/ccp/blob/master/LICENSE)
 [![code style black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-ccp is a python library for calculation of centrifugal compressor performance. It is based on the book of [Ludtke04] and uses CoolProp REFPROP for the gas properties calculations.
-
-Online documentation is available at [here](https://ccp-centrifugal-compressor-performance.readthedocs.io/en/latest/).
+ccp is a python library for calculation of centrifugal compressor performance. It uses CoolProp/REFPROP for the gas properties calculations.
 
 ```python
 import ccp
 
 # ccp uses pint to handle units. Q_ is a pint quantity.
 # If a pint quantity is not provided, SI units are assumed.
 Q_ = ccp.Q_
@@ -70,7 +71,17 @@
 
 imp = ccp.Impeller([point0, point1])
 
 # Get results from the Impeller with methods such as
 imp.head_plot()
 imp.disch.T_plot()
 ```
+
+# Documentation 
+Access the documentation [here](https://ccp-centrifugal-compressor-performance.readthedocs.io/en/stable/).
+
+# Questions
+If you have any questions, you can use the [Discussions](https://github.com/petrobras/ccp/discussions) area in the repository.
+
+# Contributing to ccp
+ROSS is a community-driven project. If you want to contribute to the project, please
+check [CONTRIBUTING.md](https://github.com/petrobras/ccp/blob/master/CONTRIBUTING.md).
```

### Comparing `ccp-performance-0.3.0/setup.py` & `ccp-performance-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,14 +51,19 @@
     name="ccp-performance",
     version=VERSION,
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Raphael Timbó",
     author_email="raphaelts@petrobras.com.br",
+    project_urls={
+        "Documentation": "https://ccp-centrifugal-compressor-performance.readthedocs.io/en/stable/",
+        "Bug Tracker": "https://github.com/petrobras/ccp/issues",
+        "Source Code": "https://github.com/petrobras/ccp",
+    },
     package_data={"ccp.config": ["new_units.txt"], "ccp.tests.data": ["*"]},
     python_requires=">=3.6",
     install_requires=REQUIRES,
     extras_require={
         "dev": [
             "pytest",
             "pytest-cov",
```

