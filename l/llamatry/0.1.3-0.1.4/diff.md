# Comparing `tmp/llamatry-0.1.3.tar.gz` & `tmp/llamatry-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamatry-0.1.3.tar", max compression
+gzip compressed data, was "llamatry-0.1.4.tar", max compression
```

## Comparing `llamatry-0.1.3.tar` & `llamatry-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0     2953 2023-05-08 05:09:01.275643 llamatry-0.1.3/README.md
--rw-r--r--   0        0        0     4817 2023-05-07 16:40:29.754052 llamatry-0.1.3/llamatry/__init__.py
--rw-r--r--   0        0        0      650 2023-05-08 14:29:11.828085 llamatry-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3793 1970-01-01 00:00:00.000000 llamatry-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     4401 2023-05-08 19:30:29.882868 llamatry-0.1.4/README.md
+-rw-r--r--   0        0        0      148 2023-05-08 18:54:23.941377 llamatry-0.1.4/llamatry/__init__.py
+-rw-r--r--   0        0        0     4817 2023-05-08 18:43:18.145718 llamatry-0.1.4/llamatry/completions.py
+-rw-r--r--   0        0        0     2420 2023-05-08 19:28:40.685648 llamatry-0.1.4/llamatry/trace.py
+-rw-r--r--   0        0        0      650 2023-05-08 19:11:11.079726 llamatry-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5241 1970-01-01 00:00:00.000000 llamatry-0.1.4/PKG-INFO
```

### Comparing `llamatry-0.1.3/README.md` & `llamatry-0.1.4/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -70,14 +70,53 @@
     max_tokens=50,
     temperature=0.5,
 )
 ```
 
 Traces and other information related to the OpenAI API calls will be output to the console. By using Llamatry, you can easily switch to other exporters supported by OpenTelemetry, such as Jaeger or Zipkin, to visualize and analyze the data in different ways.
 
+## Decorator and Context Manager helpers
+
+Llamatry provides a convenient tracing utility with both decorator and context manager support. This allows you to trace your functions and code blocks easily using the provided Trace class.
+
+### Using the Trace decorator
+
+To use the `Trace` class as a decorator, you can decorate your function using `@Trace.trace`. The function's name will be used as the span name by default. If you want to set a custom span name, you can provide it as an argument: `@Trace.trace("custom_span_name")`. By default if you decorate a function all arguments that are `(str, int, float, bool)` will be set as attributes.
+
+```python
+from llamatry import Trace
+
+@Trace.trace
+def your_function():
+    # Your function implementation
+    span = Trace.get_current_span()
+    span.set_attribute("foo", "bar")
+    pass
+
+@Trace.trace("custom_span_name")
+def another_function():
+    # Your function implementation
+    pass
+```
+
+### Using the Trace context manager
+
+To use the Trace class as a context manager, use the `with` statement followed by `Trace.span("custom_span_name")`.
+
+```python
+from llamatry import Trace
+
+with Trace.span("custom_span_name") as span:
+    # Your code block here
+    span.set_attribute("foo", "bar")
+    pass
+```
+
+Using the `Trace` class in this way allows you to easily trace your functions and code blocks, providing better observability and understanding of the performance and behavior of your code.
+
 ## Documentation
 
 For more information about OpenTelemetry, visit the [official OpenTelemetry Python documentation](https://opentelemetry-python.readthedocs.io/en/stable/).
 
 For more information about the OpenAI API, visit the [official OpenAI API documentation](https://beta.openai.com/docs/).
 
 ## License
```

### Comparing `llamatry-0.1.3/llamatry/__init__.py` & `llamatry-0.1.4/llamatry/completions.py`

 * *Files identical despite different names*

### Comparing `llamatry-0.1.3/pyproject.toml` & `llamatry-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llamatry"
-version = "0.1.3"
+version = "0.1.4"
 description = "opentelemetry instrumentation for openai's completions api"
 authors = ["Jason <jason@jxnl.co>"]
 readme = "README.md"
 repository = "https://github.com/jxnl/llamatry"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

