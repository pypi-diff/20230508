# Comparing `tmp/osim_utils-0.4.0.tar.gz` & `tmp/osim_utils-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osim_utils-0.4.0.tar", max compression
+gzip compressed data, was "osim_utils-0.4.1.tar", max compression
```

## Comparing `osim_utils-0.4.0.tar` & `osim_utils-0.4.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      232 2023-05-03 10:56:19.733098 osim_utils-0.4.0/README.md
--rw-r--r--   0        0        0     6886 2023-05-03 10:56:19.733447 osim_utils-0.4.0/osim_utils/clients/epmc.py
--rw-r--r--   0        0        0     4130 2023-05-03 16:19:44.648513 osim_utils-0.4.0/osim_utils/clients/openalex.py
--rw-r--r--   0        0        0     2282 2023-05-05 17:12:19.978124 osim_utils-0.4.0/osim_utils/clients/sherpa.py
--rw-r--r--   0        0        0      271 2023-05-03 13:04:39.071567 osim_utils-0.4.0/osim_utils/common.py
--rw-r--r--   0        0        0      311 2023-05-03 13:04:39.071765 osim_utils-0.4.0/osim_utils/constants.py
--rw-r--r--   0        0        0     1515 2023-05-03 13:04:39.071924 osim_utils-0.4.0/osim_utils/decorators.py
--rw-r--r--   0        0        0      716 2023-05-05 17:07:41.792972 osim_utils-0.4.0/osim_utils/exceptions.py
--rw-r--r--   0        0        0     2532 2023-01-12 14:22:33.188019 osim_utils-0.4.0/osim_utils/logger.py
--rw-r--r--   0        0        0      408 2023-05-05 17:07:41.793319 osim_utils-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 osim_utils-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      232 2023-05-03 10:56:19.733098 osim_utils-0.4.1/README.md
+-rw-r--r--   0        0        0     1446 2023-05-08 15:29:46.880844 osim_utils-0.4.1/osim_utils/clients/crossref.py
+-rw-r--r--   0        0        0     6886 2023-05-03 10:56:19.733447 osim_utils-0.4.1/osim_utils/clients/epmc.py
+-rw-r--r--   0        0        0     4130 2023-05-03 16:19:44.648513 osim_utils-0.4.1/osim_utils/clients/openalex.py
+-rw-r--r--   0        0        0     2282 2023-05-05 17:12:19.978124 osim_utils-0.4.1/osim_utils/clients/sherpa.py
+-rw-r--r--   0        0        0      271 2023-05-03 13:04:39.071567 osim_utils-0.4.1/osim_utils/common.py
+-rw-r--r--   0        0        0      311 2023-05-03 13:04:39.071765 osim_utils-0.4.1/osim_utils/constants.py
+-rw-r--r--   0        0        0     1515 2023-05-03 13:04:39.071924 osim_utils-0.4.1/osim_utils/decorators.py
+-rw-r--r--   0        0        0      716 2023-05-05 17:07:41.792972 osim_utils-0.4.1/osim_utils/exceptions.py
+-rw-r--r--   0        0        0     2532 2023-01-12 14:22:33.188019 osim_utils-0.4.1/osim_utils/logger.py
+-rw-r--r--   0        0        0      408 2023-05-08 15:32:44.051158 osim_utils-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 osim_utils-0.4.1/PKG-INFO
```

### Comparing `osim_utils-0.4.0/osim_utils/clients/epmc.py` & `osim_utils-0.4.1/osim_utils/clients/epmc.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.4.0/osim_utils/clients/openalex.py` & `osim_utils-0.4.1/osim_utils/clients/openalex.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.4.0/osim_utils/clients/sherpa.py` & `osim_utils-0.4.1/osim_utils/clients/sherpa.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.4.0/osim_utils/decorators.py` & `osim_utils-0.4.1/osim_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.4.0/osim_utils/exceptions.py` & `osim_utils-0.4.1/osim_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.4.0/osim_utils/logger.py` & `osim_utils-0.4.1/osim_utils/logger.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.4.0/PKG-INFO` & `osim_utils-0.4.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osim-utils
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

