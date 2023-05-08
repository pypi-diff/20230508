# Comparing `tmp/llamatry-0.1.2.tar.gz` & `tmp/llamatry-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamatry-0.1.2.tar", max compression
+gzip compressed data, was "llamatry-0.1.3.tar", max compression
```

## Comparing `llamatry-0.1.2.tar` & `llamatry-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2953 2023-05-08 05:09:01.275643 llamatry-0.1.2/README.md
--rw-r--r--   0        0        0     4817 2023-05-07 16:40:29.754052 llamatry-0.1.2/llamatry/__init__.py
--rw-r--r--   0        0        0      602 2023-05-08 14:27:45.871638 llamatry-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3691 1970-01-01 00:00:00.000000 llamatry-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2953 2023-05-08 05:09:01.275643 llamatry-0.1.3/README.md
+-rw-r--r--   0        0        0     4817 2023-05-07 16:40:29.754052 llamatry-0.1.3/llamatry/__init__.py
+-rw-r--r--   0        0        0      650 2023-05-08 14:29:11.828085 llamatry-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3793 1970-01-01 00:00:00.000000 llamatry-0.1.3/PKG-INFO
```

### Comparing `llamatry-0.1.2/README.md` & `llamatry-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `llamatry-0.1.2/llamatry/__init__.py` & `llamatry-0.1.3/llamatry/__init__.py`

 * *Files identical despite different names*

### Comparing `llamatry-0.1.2/pyproject.toml` & `llamatry-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "llamatry"
-version = "0.1.2"
+version = "0.1.3"
 description = "opentelemetry instrumentation for openai's completions api"
 authors = ["Jason <jason@jxnl.co>"]
 readme = "README.md"
+repository = "https://github.com/jxnl/llamatry"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = "^0.27.6"
 opentelemetry-api = "^1.17.0"
 opentelemetry-sdk = "^1.17.0"
 opentelemetry-instrumentation = "^0.38b0"
```

### Comparing `llamatry-0.1.2/PKG-INFO` & `llamatry-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: llamatry
-Version: 0.1.2
+Version: 0.1.3
 Summary: opentelemetry instrumentation for openai's completions api
+Home-page: https://github.com/jxnl/llamatry
 Author: Jason
 Author-email: jason@jxnl.co
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: opentelemetry-api (>=1.17.0,<2.0.0)
 Requires-Dist: opentelemetry-instrumentation (>=0.38b0,<0.39)
 Requires-Dist: opentelemetry-instrumentation-requests (>=0.38b0,<0.39)
 Requires-Dist: opentelemetry-sdk (>=1.17.0,<2.0.0)
 Requires-Dist: urllib3 (<2.0)
+Project-URL: Repository, https://github.com/jxnl/llamatry
 Description-Content-Type: text/markdown
 
 # [Llamatry](https://github.com/jxnl/llamatry)
 
 Llamatry is a Python package that simplifies the process of instrumenting the OpenAI API using OpenTelemetry. It allows you to monitor and trace the interactions with the OpenAI API, providing insights into the performance and behavior of your code. By leveraging OpenTelemetry, Llamatry supports various output formats, making it easy to integrate with your existing observability stack.
 
 ## Why?
```

