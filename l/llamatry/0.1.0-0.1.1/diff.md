# Comparing `tmp/llamatry-0.1.0.tar.gz` & `tmp/llamatry-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamatry-0.1.0.tar", max compression
+gzip compressed data, was "llamatry-0.1.1.tar", max compression
```

## Comparing `llamatry-0.1.0.tar` & `llamatry-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2574 2023-05-08 00:03:27.807301 llamatry-0.1.0/README.md
--rw-r--r--   0        0        0     4817 2023-05-07 16:40:29.754052 llamatry-0.1.0/llamatry/__init__.py
--rw-r--r--   0        0        0      544 2023-05-07 16:40:13.340878 llamatry-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3254 1970-01-01 00:00:00.000000 llamatry-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2953 2023-05-08 05:09:01.275643 llamatry-0.1.1/README.md
+-rw-r--r--   0        0        0     4817 2023-05-07 16:40:29.754052 llamatry-0.1.1/llamatry/__init__.py
+-rw-r--r--   0        0        0      544 2023-05-08 05:09:56.106371 llamatry-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 llamatry-0.1.1/PKG-INFO
```

### Comparing `llamatry-0.1.0/README.md` & `llamatry-0.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-# Llamatry
+# [Llamatry](https://github.com/jxnl/llamatry)
 
 Llamatry is a Python package that simplifies the process of instrumenting the OpenAI API using OpenTelemetry. It allows you to monitor and trace the interactions with the OpenAI API, providing insights into the performance and behavior of your code. By leveraging OpenTelemetry, Llamatry supports various output formats, making it easy to integrate with your existing observability stack.
 
+## Why?
+
+Observability is essential for complex applications using large language models (LLMs), as it provides transparency, performance insights, and control over your data and even costs. By integrating observability into your LLM tooling, you can better understand their inner workings, optimize resource usage, and streamline your workflow. Owning your data and leveraging observability empowers you to take control of your AI application's performance.
+
 ## Features
 
 * OpenTelemetry instrumentation for OpenAI API
 * Supports tracing and monitoring of OpenAI API interactions
 * Compatible with a wide range of output formats through OpenTelemetry
 * Easy-to-use and straightforward setup process
 
@@ -20,32 +24,25 @@
 ## Usage
 
 To use Llamatry with the OpenAI API, follow these steps:
 
 Import the necessary packages:
 
 ```python
-import os
-import openai
-import logging
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import ConsoleSpanExporter, SimpleSpanProcessor
-from llamatry import OpenAICompletionInstrumentor
-```
 
-Set up OpenTelemetry:
-
-## Configure logging
+from llamatry import OpenAICompletionInstrumentor
 
-```python
-logging.basicConfig(level=logging.WARNING)
+import openai
+import os
 ```
 
-## Set up OpenTelemetry
+Set up open telemetry:
 
 ```python
 trace.set_tracer_provider(TracerProvider())
 console_exporter = ConsoleSpanExporter()
 span_processor = SimpleSpanProcessor(console_exporter)
 trace.get_tracer_provider().add_span_processor(span_processor)
 ```
```

### Comparing `llamatry-0.1.0/llamatry/__init__.py` & `llamatry-0.1.1/llamatry/__init__.py`

 * *Files identical despite different names*

### Comparing `llamatry-0.1.0/pyproject.toml` & `llamatry-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llamatry"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Jason <jason@jxnl.co>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = "^0.27.6"
```

### Comparing `llamatry-0.1.0/PKG-INFO` & `llamatry-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llamatry
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Jason
 Author-email: jason@jxnl.co
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,18 +13,22 @@
 Requires-Dist: opentelemetry-api (>=1.17.0,<2.0.0)
 Requires-Dist: opentelemetry-instrumentation (>=0.38b0,<0.39)
 Requires-Dist: opentelemetry-instrumentation-requests (>=0.38b0,<0.39)
 Requires-Dist: opentelemetry-sdk (>=1.17.0,<2.0.0)
 Requires-Dist: urllib3 (<2.0)
 Description-Content-Type: text/markdown
 
-# Llamatry
+# [Llamatry](https://github.com/jxnl/llamatry)
 
 Llamatry is a Python package that simplifies the process of instrumenting the OpenAI API using OpenTelemetry. It allows you to monitor and trace the interactions with the OpenAI API, providing insights into the performance and behavior of your code. By leveraging OpenTelemetry, Llamatry supports various output formats, making it easy to integrate with your existing observability stack.
 
+## Why?
+
+Observability is essential for complex applications using large language models (LLMs), as it provides transparency, performance insights, and control over your data and even costs. By integrating observability into your LLM tooling, you can better understand their inner workings, optimize resource usage, and streamline your workflow. Owning your data and leveraging observability empowers you to take control of your AI application's performance.
+
 ## Features
 
 * OpenTelemetry instrumentation for OpenAI API
 * Supports tracing and monitoring of OpenAI API interactions
 * Compatible with a wide range of output formats through OpenTelemetry
 * Easy-to-use and straightforward setup process
 
@@ -39,32 +43,25 @@
 ## Usage
 
 To use Llamatry with the OpenAI API, follow these steps:
 
 Import the necessary packages:
 
 ```python
-import os
-import openai
-import logging
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import ConsoleSpanExporter, SimpleSpanProcessor
-from llamatry import OpenAICompletionInstrumentor
-```
 
-Set up OpenTelemetry:
-
-## Configure logging
+from llamatry import OpenAICompletionInstrumentor
 
-```python
-logging.basicConfig(level=logging.WARNING)
+import openai
+import os
 ```
 
-## Set up OpenTelemetry
+Set up open telemetry:
 
 ```python
 trace.set_tracer_provider(TracerProvider())
 console_exporter = ConsoleSpanExporter()
 span_processor = SimpleSpanProcessor(console_exporter)
 trace.get_tracer_provider().add_span_processor(span_processor)
 ```
```

