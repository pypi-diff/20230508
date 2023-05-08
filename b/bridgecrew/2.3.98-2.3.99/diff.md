# Comparing `tmp/bridgecrew-2.3.98.tar.gz` & `tmp/bridgecrew-2.3.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bridgecrew-2.3.98.tar", last modified: Sun Mar 19 15:07:12 2023, max compression
+gzip compressed data, was "dist/bridgecrew-2.3.99.tar", last modified: Sun Mar 19 16:11:49 2023, max compression
```

## Comparing `bridgecrew-2.3.98.tar` & `bridgecrew-2.3.99.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 15:07:12.768148 bridgecrew-2.3.98/
--rw-r--r--   0 root         (0) root         (0)     1129 2023-03-19 15:07:12.768148 bridgecrew-2.3.98/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      258 2023-03-19 15:05:55.000000 bridgecrew-2.3.98/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 15:07:12.764148 bridgecrew-2.3.98/bin/
--rwxr-xr-x   0 root         (0) root         (0)       93 2023-03-19 15:05:55.000000 bridgecrew-2.3.98/bin/bridgecrew
--rw-r--r--   0 root         (0) root         (0)     1368 2023-03-19 15:05:55.000000 bridgecrew-2.3.98/bin/bridgecrew.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 15:07:12.768148 bridgecrew-2.3.98/bridgecrew/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-19 15:05:55.000000 bridgecrew-2.3.98/bridgecrew/__init__.py
--rw-r--r--   0 root         (0) root         (0)      481 2023-03-19 15:05:55.000000 bridgecrew-2.3.98/bridgecrew/banner.py
--rw-r--r--   0 root         (0) root         (0)      248 2023-03-19 15:05:55.000000 bridgecrew-2.3.98/bridgecrew/main.py
--rw-r--r--   0 root         (0) root         (0)       19 2023-03-19 15:05:55.000000 bridgecrew-2.3.98/bridgecrew/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 15:07:12.768148 bridgecrew-2.3.98/bridgecrew.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1129 2023-03-19 15:07:12.000000 bridgecrew-2.3.98/bridgecrew.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      306 2023-03-19 15:07:12.000000 bridgecrew-2.3.98/bridgecrew.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-19 15:07:12.000000 bridgecrew-2.3.98/bridgecrew.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-03-19 15:07:12.000000 bridgecrew-2.3.98/bridgecrew.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-03-19 15:07:12.000000 bridgecrew-2.3.98/bridgecrew.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-19 15:07:12.768148 bridgecrew-2.3.98/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1773 2023-03-19 15:05:55.000000 bridgecrew-2.3.98/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 16:11:49.387554 bridgecrew-2.3.99/
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-03-19 16:11:49.387554 bridgecrew-2.3.99/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      258 2023-03-19 16:10:32.000000 bridgecrew-2.3.99/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 16:11:49.383554 bridgecrew-2.3.99/bin/
+-rwxr-xr-x   0 root         (0) root         (0)       93 2023-03-19 16:10:32.000000 bridgecrew-2.3.99/bin/bridgecrew
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-03-19 16:10:32.000000 bridgecrew-2.3.99/bin/bridgecrew.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 16:11:49.387554 bridgecrew-2.3.99/bridgecrew/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-19 16:10:32.000000 bridgecrew-2.3.99/bridgecrew/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      481 2023-03-19 16:10:32.000000 bridgecrew-2.3.99/bridgecrew/banner.py
+-rw-r--r--   0 root         (0) root         (0)      248 2023-03-19 16:10:32.000000 bridgecrew-2.3.99/bridgecrew/main.py
+-rw-r--r--   0 root         (0) root         (0)       19 2023-03-19 16:10:32.000000 bridgecrew-2.3.99/bridgecrew/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 16:11:49.387554 bridgecrew-2.3.99/bridgecrew.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-03-19 16:11:49.000000 bridgecrew-2.3.99/bridgecrew.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      306 2023-03-19 16:11:49.000000 bridgecrew-2.3.99/bridgecrew.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-19 16:11:49.000000 bridgecrew-2.3.99/bridgecrew.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-03-19 16:11:49.000000 bridgecrew-2.3.99/bridgecrew.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-03-19 16:11:49.000000 bridgecrew-2.3.99/bridgecrew.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-19 16:11:49.387554 bridgecrew-2.3.99/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-03-19 16:10:32.000000 bridgecrew-2.3.99/setup.py
```

### Comparing `bridgecrew-2.3.98/PKG-INFO` & `bridgecrew-2.3.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bridgecrew
-Version: 2.3.98
+Version: 2.3.99
 Summary: Infrastructure as code static analysis
 Home-page: https://github.com/bridgecrewio/bridgecrew
 Author: bridgecrew
 Author-email: meet@bridgecrew.io
 License: Apache License 2.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `bridgecrew-2.3.98/bin/bridgecrew.cmd` & `bridgecrew-2.3.99/bin/bridgecrew.cmd`

 * *Files identical despite different names*

### Comparing `bridgecrew-2.3.98/bridgecrew.egg-info/PKG-INFO` & `bridgecrew-2.3.99/bridgecrew.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bridgecrew
-Version: 2.3.98
+Version: 2.3.99
 Summary: Infrastructure as code static analysis
 Home-page: https://github.com/bridgecrewio/bridgecrew
 Author: bridgecrew
 Author-email: meet@bridgecrew.io
 License: Apache License 2.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `bridgecrew-2.3.98/setup.py` & `bridgecrew-2.3.99/setup.py`

 * *Files identical despite different names*

