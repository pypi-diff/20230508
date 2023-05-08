# Comparing `tmp/serverless-sdk-schema-0.2.1.tar.gz` & `tmp/serverless-sdk-schema-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk-schema/dist/.tmp-t5i1vddo/serverless-sdk-schema-0.2.1.tar", last modified: Tue Apr 11 20:27:52 2023, max compression
+gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk-schema/dist/.tmp-mw0ijzp7/serverless-sdk-schema-0.2.2.tar", last modified: Mon May  8 14:27:35 2023, max compression
```

## Comparing `serverless-sdk-schema-0.2.1.tar` & `serverless-sdk-schema-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-11 20:27:30.000000 serverless-sdk-schema-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-11 20:27:30.000000 serverless-sdk-schema-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-11 20:27:30.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/aws_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/error_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/notice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/tags_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/warning_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/dev_mode_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/event_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/metric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/request_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/trace_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-11 20:27:30.000000 serverless-sdk-schema-0.2.1/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:27:35.000000 serverless-sdk-schema-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-08 14:27:35.000000 serverless-sdk-schema-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-08 14:27:04.000000 serverless-sdk-schema-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-08 14:27:04.000000 serverless-sdk-schema-0.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:27:35.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 14:27:04.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 14:27:04.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:27:35.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:27:35.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:27:35.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:27:35.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/tags/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:27:35.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-05-08 14:27:14.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/aws_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-08 14:27:14.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-08 14:27:14.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/error_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-08 14:27:14.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/notice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-08 14:27:14.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/tags_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-08 14:27:14.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/warning_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:27:35.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-08 14:27:14.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/v1/dev_mode_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-08 14:27:14.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/v1/event_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-08 14:27:14.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/v1/log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-08 14:27:14.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/v1/metric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-08 14:27:14.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/v1/request_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-08 14:27:14.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/v1/trace_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:27:35.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-08 14:27:34.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-08 14:27:35.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 14:27:34.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-08 14:27:34.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 14:27:34.000000 serverless-sdk-schema-0.2.2/serverless_sdk_schema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 14:27:35.000000 serverless-sdk-schema-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:27:35.000000 serverless-sdk-schema-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-08 14:27:04.000000 serverless-sdk-schema-0.2.2/tests/test_schema.py
```

### Comparing `serverless-sdk-schema-0.2.1/PKG-INFO` & `serverless-sdk-schema-0.2.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 Metadata-Version: 2.1
 Name: serverless-sdk-schema
-Version: 0.2.1
+Version: 0.2.2
 Summary: The protobuf generated Serverless SDK Schema
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk-schema/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk-schema
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # Serverless SDK Schema
 
 This is the auto generated Python package from the Serverless Protobufs. Serverless uses Protobufs as the required format for all instrumentation libraries that communicate with the Serverless Platform.
```

### Comparing `serverless-sdk-schema-0.2.1/README.md` & `serverless-sdk-schema-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/aws_pb2.py` & `serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/aws_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/common_pb2.py` & `serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/error_pb2.py` & `serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/error_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/notice_pb2.py` & `serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/notice_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/tags_pb2.py` & `serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/tags_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/warning_pb2.py` & `serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/warning_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/dev_mode_pb2.py` & `serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/v1/dev_mode_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/event_pb2.py` & `serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/v1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/log_pb2.py` & `serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/v1/log_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/metric_pb2.py` & `serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/v1/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/request_response_pb2.py` & `serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/v1/request_response_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/trace_pb2.py` & `serverless-sdk-schema-0.2.2/serverless_sdk_schema/schema/serverless/instrumentation/v1/trace_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.1/serverless_sdk_schema.egg-info/PKG-INFO` & `serverless-sdk-schema-0.2.2/serverless_sdk_schema.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 Metadata-Version: 2.1
 Name: serverless-sdk-schema
-Version: 0.2.1
+Version: 0.2.2
 Summary: The protobuf generated Serverless SDK Schema
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk-schema/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk-schema
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # Serverless SDK Schema
 
 This is the auto generated Python package from the Serverless Protobufs. Serverless uses Protobufs as the required format for all instrumentation libraries that communicate with the Serverless Platform.
```

### Comparing `serverless-sdk-schema-0.2.1/serverless_sdk_schema.egg-info/SOURCES.txt` & `serverless-sdk-schema-0.2.2/serverless_sdk_schema.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 pyproject.toml
 serverless_sdk_schema/__init__.py
+serverless_sdk_schema/py.typed
 serverless_sdk_schema.egg-info/PKG-INFO
 serverless_sdk_schema.egg-info/SOURCES.txt
 serverless_sdk_schema.egg-info/dependency_links.txt
 serverless_sdk_schema.egg-info/requires.txt
 serverless_sdk_schema.egg-info/top_level.txt
 serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/aws_pb2.py
 serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/common_pb2.py
```

### Comparing `serverless-sdk-schema-0.2.1/tests/test_schema.py` & `serverless-sdk-schema-0.2.2/tests/test_schema.py`

 * *Files identical despite different names*

