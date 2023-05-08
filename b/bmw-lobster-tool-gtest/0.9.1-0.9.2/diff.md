# Comparing `tmp/bmw-lobster-tool-gtest-0.9.1.tar.gz` & `tmp/bmw-lobster-tool-gtest-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-tool-gtest-0.9.1.tar", last modified: Wed May  3 14:22:58 2023, max compression
+gzip compressed data, was "bmw-lobster-tool-gtest-0.9.2.tar", last modified: Mon May  8 15:06:39 2023, max compression
```

## Comparing `bmw-lobster-tool-gtest-0.9.1.tar` & `bmw-lobster-tool-gtest-0.9.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:58.456384 bmw-lobster-tool-gtest-0.9.1/
--rw-r--r--   0 florian   (1000) florian   (1000)     1801 2023-05-03 14:22:58.452384 bmw-lobster-tool-gtest-0.9.1/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      804 2023-05-03 14:09:11.000000 bmw-lobster-tool-gtest-0.9.1/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:58.452384 bmw-lobster-tool-gtest-0.9.1/bmw_lobster_tool_gtest.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     1801 2023-05-03 14:22:58.000000 bmw-lobster-tool-gtest-0.9.1/bmw_lobster_tool_gtest.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      357 2023-05-03 14:22:58.000000 bmw-lobster-tool-gtest-0.9.1/bmw_lobster_tool_gtest.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-03 14:22:58.000000 bmw-lobster-tool-gtest-0.9.1/bmw_lobster_tool_gtest.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       65 2023-05-03 14:22:58.000000 bmw-lobster-tool-gtest-0.9.1/bmw_lobster_tool_gtest.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       24 2023-05-03 14:22:58.000000 bmw-lobster-tool-gtest-0.9.1/bmw_lobster_tool_gtest.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-05-03 14:22:58.000000 bmw-lobster-tool-gtest-0.9.1/bmw_lobster_tool_gtest.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:58.452384 bmw-lobster-tool-gtest-0.9.1/lobster/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:58.452384 bmw-lobster-tool-gtest-0.9.1/lobster/tools/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:58.452384 bmw-lobster-tool-gtest-0.9.1/lobster/tools/gtest/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-03 14:09:11.000000 bmw-lobster-tool-gtest-0.9.1/lobster/tools/gtest/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     5529 2023-05-03 14:09:11.000000 bmw-lobster-tool-gtest-0.9.1/lobster/tools/gtest/gtest.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-03 14:22:58.456384 bmw-lobster-tool-gtest-0.9.1/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2231 2023-05-03 14:09:11.000000 bmw-lobster-tool-gtest-0.9.1/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:39.905493 bmw-lobster-tool-gtest-0.9.2/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1823 2023-05-08 15:06:39.905493 bmw-lobster-tool-gtest-0.9.2/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      826 2023-05-08 15:03:18.000000 bmw-lobster-tool-gtest-0.9.2/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:39.905493 bmw-lobster-tool-gtest-0.9.2/bmw_lobster_tool_gtest.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1823 2023-05-08 15:06:39.000000 bmw-lobster-tool-gtest-0.9.2/bmw_lobster_tool_gtest.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      357 2023-05-08 15:06:39.000000 bmw-lobster-tool-gtest-0.9.2/bmw_lobster_tool_gtest.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-08 15:06:39.000000 bmw-lobster-tool-gtest-0.9.2/bmw_lobster_tool_gtest.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       65 2023-05-08 15:06:39.000000 bmw-lobster-tool-gtest-0.9.2/bmw_lobster_tool_gtest.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       24 2023-05-08 15:06:39.000000 bmw-lobster-tool-gtest-0.9.2/bmw_lobster_tool_gtest.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-05-08 15:06:39.000000 bmw-lobster-tool-gtest-0.9.2/bmw_lobster_tool_gtest.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:39.901493 bmw-lobster-tool-gtest-0.9.2/lobster/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:39.901493 bmw-lobster-tool-gtest-0.9.2/lobster/tools/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:39.905493 bmw-lobster-tool-gtest-0.9.2/lobster/tools/gtest/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:39.000000 bmw-lobster-tool-gtest-0.9.2/lobster/tools/gtest/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     5529 2023-05-08 15:06:39.000000 bmw-lobster-tool-gtest-0.9.2/lobster/tools/gtest/gtest.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-08 15:06:39.905493 bmw-lobster-tool-gtest-0.9.2/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2231 2023-05-08 15:03:18.000000 bmw-lobster-tool-gtest-0.9.2/setup.py
```

### Comparing `bmw-lobster-tool-gtest-0.9.1/PKG-INFO` & `bmw-lobster-tool-gtest-0.9.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-gtest
-Version: 0.9.1
+Version: 0.9.2
 Summary: LOBSTER Tool for GoogleTest
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
@@ -27,16 +27,17 @@
 
 This package contains a tool and helper header for GoogleTest.
 
 ## Tools
 
 * `lobster-gtest`: Extrat tracing data from GoogleTest XML files
 
-* [lobster_gtest.h](https://github.com/bmw-software-engineering/lobster/blob/main/include/lobster_gtest.h): A public domain header
-  with a C/C++ macro to embed tracing tags or justifications
+* [lobster_gtest.h](https://github.com/bmw-software-engineering/lobster/blob/main/../../support/gtest/include/lobster_gtest.h): A
+  public domain header with a C/C++ macro to embed tracing tags or
+  justifications
 
 ## Copyright & License information
 
 The copyright holder of LOBSTER is the Bayerische Motoren Werke
 Aktiengesellschaft (BMW AG), and LOBSTER is published under the [GNU
 Affero General Public License, Version 3](../LICENSE.md).
```

### Comparing `bmw-lobster-tool-gtest-0.9.1/bmw_lobster_tool_gtest.egg-info/PKG-INFO` & `bmw-lobster-tool-gtest-0.9.2/bmw_lobster_tool_gtest.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-gtest
-Version: 0.9.1
+Version: 0.9.2
 Summary: LOBSTER Tool for GoogleTest
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
@@ -27,16 +27,17 @@
 
 This package contains a tool and helper header for GoogleTest.
 
 ## Tools
 
 * `lobster-gtest`: Extrat tracing data from GoogleTest XML files
 
-* [lobster_gtest.h](https://github.com/bmw-software-engineering/lobster/blob/main/include/lobster_gtest.h): A public domain header
-  with a C/C++ macro to embed tracing tags or justifications
+* [lobster_gtest.h](https://github.com/bmw-software-engineering/lobster/blob/main/../../support/gtest/include/lobster_gtest.h): A
+  public domain header with a C/C++ macro to embed tracing tags or
+  justifications
 
 ## Copyright & License information
 
 The copyright holder of LOBSTER is the Bayerische Motoren Werke
 Aktiengesellschaft (BMW AG), and LOBSTER is published under the [GNU
 Affero General Public License, Version 3](../LICENSE.md).
```

### Comparing `bmw-lobster-tool-gtest-0.9.1/lobster/tools/gtest/gtest.py` & `bmw-lobster-tool-gtest-0.9.2/lobster/tools/gtest/gtest.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-tool-gtest-0.9.1/setup.py` & `bmw-lobster-tool-gtest-0.9.2/setup.py`

 * *Files identical despite different names*

