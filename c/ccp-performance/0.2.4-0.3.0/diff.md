# Comparing `tmp/ccp-performance-0.2.4.tar.gz` & `tmp/ccp-performance-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/ccp/ccp/dist/.tmp-fr8bc0me/ccp-performance-0.2.4.tar", last modified: Mon Apr 17 13:16:56 2023, max compression
+gzip compressed data, was "/home/runner/work/ccp/ccp/dist/.tmp-hlzohd_b/ccp-performance-0.3.0.tar", last modified: Mon May  8 15:36:37 2023, max compression
```

## Comparing `ccp-performance-0.2.4.tar` & `ccp-performance-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-04-17 13:16:43.000000 ccp-performance-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 13:16:43.000000 ccp-performance-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-17 13:16:43.000000 ccp-performance-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/ccp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/ccp/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/ccp/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   288892 2023-04-17 13:16:43.000000 ccp-performance-0.2.4/ccp/tests/data/UTGCA_1231_A_1s.csv
--rw-r--r--   0 runner    (1001) docker     (123)   502046 2023-04-17 13:16:43.000000 ccp-performance-0.2.4/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-17 13:16:43.000000 ccp-performance-0.2.4/ccp/tests/data/lp-sec1-caso-a-eff.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-17 13:16:43.000000 ccp-performance-0.2.4/ccp/tests/data/lp-sec1-caso-a-head.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-17 13:16:43.000000 ccp-performance-0.2.4/ccp/tests/data/normal-eff.csv
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-17 13:16:43.000000 ccp-performance-0.2.4/ccp/tests/data/normal-head.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/ccp_performance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/ccp_performance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/ccp_performance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/ccp_performance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/ccp_performance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/ccp_performance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-17 13:16:43.000000 ccp-performance-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-08 15:36:28.000000 ccp-performance-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-08 15:36:28.000000 ccp-performance-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-08 15:36:28.000000 ccp-performance-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/ccp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/ccp/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/ccp/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   288892 2023-05-08 15:36:28.000000 ccp-performance-0.3.0/ccp/tests/data/UTGCA_1231_A_1s.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   502046 2023-05-08 15:36:28.000000 ccp-performance-0.3.0/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-08 15:36:28.000000 ccp-performance-0.3.0/ccp/tests/data/lp-sec1-caso-a-eff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-08 15:36:28.000000 ccp-performance-0.3.0/ccp/tests/data/lp-sec1-caso-a-head.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-08 15:36:28.000000 ccp-performance-0.3.0/ccp/tests/data/normal-eff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-08 15:36:28.000000 ccp-performance-0.3.0/ccp/tests/data/normal-head.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/ccp_performance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/ccp_performance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/ccp_performance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/ccp_performance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/ccp_performance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/ccp_performance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:36:37.000000 ccp-performance-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-08 15:36:28.000000 ccp-performance-0.3.0/setup.py
```

### Comparing `ccp-performance-0.2.4/LICENSE` & `ccp-performance-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.2.4/PKG-INFO` & `ccp-performance-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccp-performance
-Version: 0.2.4
+Version: 0.3.0
 Summary: Centrifugal Compressor Performance calculation.
 Author: Raphael Timbó
 Author-email: raphaelts@petrobras.com.br
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ccp-performance-0.2.4/README.md` & `ccp-performance-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.2.4/ccp/tests/data/UTGCA_1231_A_1s.csv` & `ccp-performance-0.3.0/ccp/tests/data/UTGCA_1231_A_1s.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.2.4/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h` & `ccp-performance-0.3.0/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.2.4/ccp/tests/data/lp-sec1-caso-a-eff.csv` & `ccp-performance-0.3.0/ccp/tests/data/lp-sec1-caso-a-eff.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.2.4/ccp/tests/data/lp-sec1-caso-a-head.csv` & `ccp-performance-0.3.0/ccp/tests/data/lp-sec1-caso-a-head.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.2.4/ccp/tests/data/normal-eff.csv` & `ccp-performance-0.3.0/ccp/tests/data/normal-eff.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.2.4/ccp/tests/data/normal-head.csv` & `ccp-performance-0.3.0/ccp/tests/data/normal-head.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.2.4/ccp_performance.egg-info/PKG-INFO` & `ccp-performance-0.3.0/ccp_performance.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccp-performance
-Version: 0.2.4
+Version: 0.3.0
 Summary: Centrifugal Compressor Performance calculation.
 Author: Raphael Timbó
 Author-email: raphaelts@petrobras.com.br
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ccp-performance-0.2.4/setup.py` & `ccp-performance-0.3.0/setup.py`

 * *Files identical despite different names*

