# Comparing `tmp/troncos-3.2.0.tar.gz` & `tmp/troncos-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troncos-3.2.0.tar", max compression
+gzip compressed data, was "troncos-3.2.1.tar", max compression
```

## Comparing `troncos-3.2.0.tar` & `troncos-3.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1077 2023-05-05 08:29:22.517858 troncos-3.2.0/LICENSE
--rw-r--r--   0        0        0    15620 2023-05-05 08:29:22.517858 troncos-3.2.0/README.md
--rw-r--r--   0        0        0     2273 2023-05-05 08:29:22.517858 troncos-3.2.0/pyproject.toml
--rw-r--r--   0        0        0      291 2023-05-05 08:29:22.517858 troncos-3.2.0/troncos/__init__.py
--rw-r--r--   0        0        0     1214 2023-05-05 08:29:22.521858 troncos-3.2.0/troncos/_ddlazy/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 08:29:22.521858 troncos-3.2.0/troncos/frameworks/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 08:29:22.521858 troncos-3.2.0/troncos/frameworks/asgi/__init__.py
--rw-r--r--   0        0        0     2595 2023-05-05 08:29:22.521858 troncos-3.2.0/troncos/frameworks/asgi/middleware.py
--rw-r--r--   0        0        0     3367 2023-05-05 08:29:22.521858 troncos-3.2.0/troncos/frameworks/asgi/utils.py
--rw-r--r--   0        0        0      993 2023-05-05 08:29:22.521858 troncos-3.2.0/troncos/frameworks/gunicorn/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 08:29:22.521858 troncos-3.2.0/troncos/frameworks/starlette/__init__.py
--rw-r--r--   0        0        0     4488 2023-05-05 08:29:22.521858 troncos-3.2.0/troncos/frameworks/starlette/uvicorn.py
--rw-r--r--   0        0        0        0 2023-05-05 08:29:22.521858 troncos-3.2.0/troncos/frameworks/structlog/__init__.py
--rw-r--r--   0        0        0     2044 2023-05-05 08:29:22.521858 troncos-3.2.0/troncos/frameworks/structlog/processors.py
--rw-r--r--   0        0        0     5589 2023-05-05 08:29:22.521858 troncos-3.2.0/troncos/frameworks/structlog/setup.py
--rw-r--r--   0        0        0     4922 2023-05-05 08:29:22.521858 troncos-3.2.0/troncos/logs/__init__.py
--rw-r--r--   0        0        0     3430 2023-05-05 08:29:22.521858 troncos-3.2.0/troncos/logs/filters.py
--rw-r--r--   0        0        0     9364 2023-05-05 08:29:22.521858 troncos-3.2.0/troncos/logs/formatters.py
--rw-r--r--   0        0        0     3090 2023-05-05 08:29:22.521858 troncos-3.2.0/troncos/profiling/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 08:29:22.521858 troncos-3.2.0/troncos/py.typed
--rw-r--r--   0        0        0    10656 2023-05-05 08:29:22.521858 troncos-3.2.0/troncos/traces/__init__.py
--rw-r--r--   0        0        0     6585 2023-05-05 08:29:22.521858 troncos-3.2.0/troncos/traces/dd_shim.py
--rw-r--r--   0        0        0     8351 2023-05-05 08:29:22.521858 troncos-3.2.0/troncos/traces/decorate.py
--rw-r--r--   0        0        0     1459 2023-05-05 08:29:22.521858 troncos-3.2.0/troncos/traces/propagation.py
--rw-r--r--   0        0        0    16694 1970-01-01 00:00:00.000000 troncos-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-08 12:26:19.531825 troncos-3.2.1/LICENSE
+-rw-r--r--   0        0        0    15818 2023-05-08 12:26:19.531825 troncos-3.2.1/README.md
+-rw-r--r--   0        0        0     2278 2023-05-08 12:26:19.535825 troncos-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/__init__.py
+-rw-r--r--   0        0        0     1214 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/_ddlazy/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/frameworks/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/frameworks/asgi/__init__.py
+-rw-r--r--   0        0        0     3049 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/frameworks/asgi/middleware.py
+-rw-r--r--   0        0        0     3367 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/frameworks/asgi/utils.py
+-rw-r--r--   0        0        0      993 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/frameworks/gunicorn/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/frameworks/starlette/__init__.py
+-rw-r--r--   0        0        0     4488 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/frameworks/starlette/uvicorn.py
+-rw-r--r--   0        0        0        0 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/frameworks/structlog/__init__.py
+-rw-r--r--   0        0        0     2222 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/frameworks/structlog/processors.py
+-rw-r--r--   0        0        0     5589 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/frameworks/structlog/setup.py
+-rw-r--r--   0        0        0     4922 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/logs/__init__.py
+-rw-r--r--   0        0        0     3710 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/logs/filters.py
+-rw-r--r--   0        0        0     9364 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/logs/formatters.py
+-rw-r--r--   0        0        0     3090 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/profiling/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/py.typed
+-rw-r--r--   0        0        0    10656 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/traces/__init__.py
+-rw-r--r--   0        0        0     6585 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/traces/dd_shim.py
+-rw-r--r--   0        0        0     8351 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/traces/decorate.py
+-rw-r--r--   0        0        0     1459 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/traces/propagation.py
+-rw-r--r--   0        0        0    16888 1970-01-01 00:00:00.000000 troncos-3.2.1/PKG-INFO
```

### Comparing `troncos-3.2.0/LICENSE` & `troncos-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `troncos-3.2.0/README.md` & `troncos-3.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -300,34 +300,44 @@
 ```
 
 ### Structlog
 
 You can substitute `init_logging_basic` with `init_logging_structlog` to setup structlog:
 
 ```python
+import structlog
 from os import environ
 from troncos.frameworks.structlog.setup import init_logging_structlog
 
 init_logging_structlog(
     level=environ.get("LOG_LEVEL", "INFO"),
     formatter=environ.get("LOG_FORMATTER", "cli"),  # Use "logfmt" in production
 )
+
+log = structlog.get_logger()
+log.info("Some Message")
 ```
 
 Alternatively you can add trace injection into your own structlog setup:
 
 ```python
 import structlog
+from structlog.dev import ConsoleRenderer
+
 from troncos.frameworks.structlog.processors import trace_injection_processor
 
 structlog.configure(
     processors=[
-       trace_injection_processor,
+        trace_injection_processor,
+        ConsoleRenderer(),
     ],
 )
+
+log = structlog.get_logger()
+log.info("Some Message")
 ```
 
 ## Tracing
 
 ### Tracing your code
 
 After initializing tracing in your project you can use different methods to trace your code.
```

#### html2text {}

```diff
@@ -109,89 +109,91 @@
 post_request(worker, req, environ, resp): duration = time.time() -
 req._gunicorn_start_time trace_id = next(iter([v for k, v in req.headers if k
 == "X-B3-TRACEID"]), None) worker.log.info( "[status=%s] %s %s duration=%s
 traceID=%s", resp.status, req.method, req.path, duration, trace_id, ) ``` Then
 when running gunicorn, specify what config file to use: ```console gunicorn
 myapp.wsgi:application --config python:myapp.gunicorn.config ... ``` ###
 Structlog You can substitute `init_logging_basic` with `init_logging_structlog`
-to setup structlog: ```python from os import environ from
+to setup structlog: ```python import structlog from os import environ from
 troncos.frameworks.structlog.setup import init_logging_structlog
 init_logging_structlog( level=environ.get("LOG_LEVEL", "INFO"),
 formatter=environ.get("LOG_FORMATTER", "cli"), # Use "logfmt" in production )
-``` Alternatively you can add trace injection into your own structlog setup:
-```python import structlog from troncos.frameworks.structlog.processors import
-trace_injection_processor structlog.configure( processors=
-[ trace_injection_processor, ], ) ``` ## Tracing ### Tracing your code After
-initializing tracing in your project you can use different methods to trace
-your code. #### trace_function This decorator adds tracing to a function. You
-can supply a tracer provider, if none is supplied, the global tracer provider
-will be used: ```python from troncos.traces.decorate import trace_function
-@trace_function def myfunc1(): return "This will be traced" @trace_function
-(service="my_custom_service") def myfunc2(): return "This will be traced as
-my_custom_service" ``` #### trace_block Trace using a with statement. You can
-supply a tracer provider, if none is supplied, the global tracer provider will
-be used. ```python from troncos.traces.decorate import trace_block with
-trace_block(name="action", resource="thing", attributes={"some": "attribute"}):
-print("... do an action to a thing...") ``` #### trace_class This decorator
-adds a tracing decorator to every method of the decorated class. If you don't
-want some methods to be traced, you can add the [trace_ignore](#traceignore)
+log = structlog.get_logger() log.info("Some Message") ``` Alternatively you can
+add trace injection into your own structlog setup: ```python import structlog
+from structlog.dev import ConsoleRenderer from
+troncos.frameworks.structlog.processors import trace_injection_processor
+structlog.configure( processors=[ trace_injection_processor, ConsoleRenderer(),
+], ) log = structlog.get_logger() log.info("Some Message") ``` ## Tracing ###
+Tracing your code After initializing tracing in your project you can use
+different methods to trace your code. #### trace_function This decorator adds
+tracing to a function. You can supply a tracer provider, if none is supplied,
+the global tracer provider will be used: ```python from troncos.traces.decorate
+import trace_function @trace_function def myfunc1(): return "This will be
+traced" @trace_function(service="my_custom_service") def myfunc2(): return
+"This will be traced as my_custom_service" ``` #### trace_block Trace using a
+with statement. You can supply a tracer provider, if none is supplied, the
+global tracer provider will be used. ```python from troncos.traces.decorate
+import trace_block with trace_block(name="action", resource="thing",
+attributes={"some": "attribute"}): print("... do an action to a thing...") ```
+#### trace_class This decorator adds a tracing decorator to every method of the
+decorated class. If you don't want some methods to be traced, you can add the
+[trace_ignore](#traceignore) decorator to them. You can supply a tracer
+provider, if none is supplied, the global tracer provider will be used:
+```python from troncos.traces.decorate import trace_class, trace_ignore
+@trace_class class MyClass1: def m1(self): return "This will be traced"
+@trace_ignore def m2(self): return "This will not traced" @trace_class
+(service="my_custom_service") class MyClass2: def m3(self): return "This will
+be traced as my_custom_service" ``` #### trace_module This function adds a
+tracing decorator to every function of the calling module. If you don't want
+some functions to be traced, you can add the [trace_ignore](#traceignore)
 decorator to them. You can supply a tracer provider, if none is supplied, the
 global tracer provider will be used: ```python from troncos.traces.decorate
-import trace_class, trace_ignore @trace_class class MyClass1: def m1(self):
-return "This will be traced" @trace_ignore def m2(self): return "This will not
-traced" @trace_class(service="my_custom_service") class MyClass2: def m3(self):
-return "This will be traced as my_custom_service" ``` #### trace_module This
-function adds a tracing decorator to every function of the calling module. If
-you don't want some functions to be traced, you can add the [trace_ignore]
-(#traceignore) decorator to them. You can supply a tracer provider, if none is
-supplied, the global tracer provider will be used: ```python from
-troncos.traces.decorate import trace_ignore, trace_module def my_function():
-return "This func will be traced" @trace_ignore def my_function(): return "This
-func will not be traced" trace_module() ``` #### trace_ignore A decorator that
-will make [trace_class](#traceclass) and [trace_module](#tracemodule) ignore
-the decorated function/method. ### Trace Propagation > **Warning**: Traces with
-IDs bigger than `64` bits are not propagated correctly because of limitations
-of [ddtrace](https://github.com/DataDog/dd-trace-py/blob/
-1e1de001d3fd694d3bcf0fff604a927ef891b19e/ddtrace/propagation/http.py#L102-
-L108). Default trace ID size for OTEL is `128` bits. If you want to propagate
-your trace to the next service, you need to send/receive special headers with
-your request/message. If you are using plain `requests` that should be handled
-automatically by troncos. Here is how you do this manually: #### Send context
-```python from troncos.traces.propagation import get_propagation_value # Get
-header value value = get_propagation_value() # Send it somewhere ``` or
-```python from troncos.traces.propagation import add_context_to_dict some_dict
-= {} # Add propagation headers to dict add_context_to_dict(some_dict) # Send it
-somewhere ``` #### Receive context Again, troncos should in most cases do this
-automatically for you, but here is how you do it manually: ```python from
-troncos.traces.propagation import activate_context_from_dict from
-troncos.traces.decorate import trace_block some_dict = {}
-activate_context_from_dict(some_dict) with trace_block("my_block"): print("...
-do something ...") ``` ### Trace sampling Set these variables to turn on trace
-sampling: ```console OTEL_TRACES_SAMPLER=parentbased_traceidratio
-OTEL_TRACES_SAMPLER_ARG=0.05 DD_TRACE_SAMPLE_RATE=0.05 ``` ### Trace debugging
-You can enable trace debugging by setting the environmental variable
-`OTEL_TRACE_DEBUG=true`. That will print all spans to the console. If you would
-rather get the spans in a file you can also provide the variable
-`OTEL_TRACE_DEBUG_FILE=/tmp/traces`. ## Profiling > **Warning**: Profiling
-while using Python 3.11 is [not yet fully supported](https://github.com/
-DataDog/dd-trace-py/issues/4149). ### Setup endpoint Simply add a `/debug/
-pprof` endpoint that returns the profile: ```python from fastapi import FastAPI
-from starlette.responses import Response from troncos.profiling import
-init_profiling_basic profiler = init_profiling_basic() app = FastAPI
-(title="my_service") @app.get("/debug/pprof", response_model=str) async def
-debug_pprof() -> Response: content, headers = profiler() return Response
-(content=content, headers=headers) ``` You can verify that your setup works
-with the [pprof](https://github.com/google/pprof) cli: ```console $ pprof -http
-:6060 "http://localhost:8080/debug/pprof" ``` > **Note**: You will get an empty
-string from `profiler()` until the first profile has been collected. ### Enable
-scraping When you deploy your application, be sure to use the custom oda
-annotation for scraping: ```yaml annotations: phlare.oda.com/port: "8080"
-phlare.oda.com/scrape: "true" ``` ## Development When developing troncos you
-should be constantly aware of the fact that under no circumstances should you
-import `ddtrace` into your module. That would cause the tracer to initialize
-with default values that would not change when the user initializes the tracer.
-For this reason, if you need to use any parts of `ddtrace` in your code,
-consider using the `_ddlazy` module, that gives you access lazily. If that does
-not satisfy your requirements you can always import `ddtrace` in your functions
-(not at the top of your module). You can compare performance of your local
-version, to some older version of troncos using the [performance test setup](./
-perf).
+import trace_ignore, trace_module def my_function(): return "This func will be
+traced" @trace_ignore def my_function(): return "This func will not be traced"
+trace_module() ``` #### trace_ignore A decorator that will make [trace_class]
+(#traceclass) and [trace_module](#tracemodule) ignore the decorated function/
+method. ### Trace Propagation > **Warning**: Traces with IDs bigger than `64`
+bits are not propagated correctly because of limitations of [ddtrace](https://
+github.com/DataDog/dd-trace-py/blob/1e1de001d3fd694d3bcf0fff604a927ef891b19e/
+ddtrace/propagation/http.py#L102-L108). Default trace ID size for OTEL is `128`
+bits. If you want to propagate your trace to the next service, you need to
+send/receive special headers with your request/message. If you are using plain
+`requests` that should be handled automatically by troncos. Here is how you do
+this manually: #### Send context ```python from troncos.traces.propagation
+import get_propagation_value # Get header value value = get_propagation_value()
+# Send it somewhere ``` or ```python from troncos.traces.propagation import
+add_context_to_dict some_dict = {} # Add propagation headers to dict
+add_context_to_dict(some_dict) # Send it somewhere ``` #### Receive context
+Again, troncos should in most cases do this automatically for you, but here is
+how you do it manually: ```python from troncos.traces.propagation import
+activate_context_from_dict from troncos.traces.decorate import trace_block
+some_dict = {} activate_context_from_dict(some_dict) with trace_block
+("my_block"): print("... do something ...") ``` ### Trace sampling Set these
+variables to turn on trace sampling: ```console
+OTEL_TRACES_SAMPLER=parentbased_traceidratio OTEL_TRACES_SAMPLER_ARG=0.05
+DD_TRACE_SAMPLE_RATE=0.05 ``` ### Trace debugging You can enable trace
+debugging by setting the environmental variable `OTEL_TRACE_DEBUG=true`. That
+will print all spans to the console. If you would rather get the spans in a
+file you can also provide the variable `OTEL_TRACE_DEBUG_FILE=/tmp/traces`. ##
+Profiling > **Warning**: Profiling while using Python 3.11 is [not yet fully
+supported](https://github.com/DataDog/dd-trace-py/issues/4149). ### Setup
+endpoint Simply add a `/debug/pprof` endpoint that returns the profile:
+```python from fastapi import FastAPI from starlette.responses import Response
+from troncos.profiling import init_profiling_basic profiler =
+init_profiling_basic() app = FastAPI(title="my_service") @app.get("/debug/
+pprof", response_model=str) async def debug_pprof() -> Response: content,
+headers = profiler() return Response(content=content, headers=headers) ``` You
+can verify that your setup works with the [pprof](https://github.com/google/
+pprof) cli: ```console $ pprof -http :6060 "http://localhost:8080/debug/pprof"
+``` > **Note**: You will get an empty string from `profiler()` until the first
+profile has been collected. ### Enable scraping When you deploy your
+application, be sure to use the custom oda annotation for scraping: ```yaml
+annotations: phlare.oda.com/port: "8080" phlare.oda.com/scrape: "true" ``` ##
+Development When developing troncos you should be constantly aware of the fact
+that under no circumstances should you import `ddtrace` into your module. That
+would cause the tracer to initialize with default values that would not change
+when the user initializes the tracer. For this reason, if you need to use any
+parts of `ddtrace` in your code, consider using the `_ddlazy` module, that
+gives you access lazily. If that does not satisfy your requirements you can
+always import `ddtrace` in your functions (not at the top of your module). You
+can compare performance of your local version, to some older version of troncos
+using the [performance test setup](./perf).
```

### Comparing `troncos-3.2.0/pyproject.toml` & `troncos-3.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troncos"
-version = "3.2.0"
+version = "3.2.1"
 description = "Collection of Python logging, tracing and profiling tools"
 authors = [
     "Guðmundur Björn Birkisson <gudmundur.birkisson@oda.com>",
     "Karl Fredrik Haugland <karlfredrik.haugland@oda.com>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -15,15 +15,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 ddtrace = "1.12.4"
 opentelemetry-sdk = "1.17.0"
 opentelemetry-exporter-otlp-proto-http = {version = "1.17.0", optional = true}
 opentelemetry-exporter-otlp-proto-grpc = {version = "1.17.0", optional = true}
-structlog = {version = "^22.3.0", optional = true}
+structlog = {version = ">=22.3,<24.0", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.1"
 pytest = "^7.2.1"
```

### Comparing `troncos-3.2.0/troncos/_ddlazy/__init__.py` & `troncos-3.2.1/troncos/_ddlazy/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.0/troncos/frameworks/asgi/middleware.py` & `troncos-3.2.1/troncos/frameworks/asgi/middleware.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import time
 from typing import Any, Awaitable, Callable
 
+from troncos._ddlazy import ddlazy
 from troncos.frameworks.asgi.utils import guarantee_single_callable
 
 
 class AsgiLoggingMiddleware:
     """
     ASGI application middleware that logs requests.
     """
@@ -25,14 +26,22 @@
         scope: dict[str, Any],
         receive: Callable[[Any], Any],
         send: Callable[[dict[str, Any]], Awaitable[Any]],
     ) -> Any:
         if scope["type"] != "http":
             return await self._app(scope, receive, send)
 
+        # Extract tracing context now, because it is not available
+        # when we create the log records!
+        dd_context = (
+            ddlazy.dd_tracer().current_trace_context()
+            if ddlazy.dd_initialized()
+            else None
+        )
+
         client_ip, client_port = scope.get("client", ("NO_IP", -1))
         method = scope.get("method")
         path = scope.get("path")
         http_version = scope.get("http_version")
         status = [0]
         start_time = time.time()
 
@@ -43,35 +52,41 @@
             await send(message)
 
             # "more_body" is used if there is still data to send. Log the request
             # when "http.response.body" has no more data left to send in the response.
             if message.get("type") == "http.response.body" and not message.get(
                 "more_body", False
             ):
+                extra = {
+                    "http_client_addr": f"{client_ip}:{client_port}",
+                    "http_method": method,
+                    "http_path": path,
+                    "http_version": http_version,
+                    "http_status_code": status[0],
+                    "duration": f"{time.time()-start_time:.6f}",
+                }
+                if dd_context:
+                    extra["dd_context"] = dd_context
                 self._access.info(
                     "",
-                    extra={
-                        "http_client_addr": f"{client_ip}:{client_port}",
-                        "http_method": method,
-                        "http_path": path,
-                        "http_version": http_version,
-                        "http_status_code": status[0],
-                        "duration": f"{time.time()-start_time:.6f}",
-                    },
+                    extra=extra,
                 )
 
         try:
             return await self._app(scope, receive, wrapped_send)
         except Exception as e:
+            extra = {
+                "http_client_addr": f"{client_ip}:{client_port}",
+                "http_method": method,
+                "http_path": path,
+                "http_version": http_version,
+                "http_status_code": 500,
+                "duration": f"{time.time()-start_time:.6f}",
+            }
+            if dd_context:
+                extra["dd_context"] = dd_context
             self._error.error(
                 "",
                 exc_info=e,
-                extra={
-                    "http_client_addr": f"{client_ip}:{client_port}",
-                    "http_method": method,
-                    "http_path": path,
-                    "http_version": http_version,
-                    "http_status_code": 500,
-                    "duration": f"{time.time()-start_time:.6f}",
-                },
+                extra=extra,
             )
             raise e
```

### Comparing `troncos-3.2.0/troncos/frameworks/asgi/utils.py` & `troncos-3.2.1/troncos/frameworks/asgi/utils.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.0/troncos/frameworks/gunicorn/__init__.py` & `troncos-3.2.1/troncos/frameworks/gunicorn/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.0/troncos/frameworks/starlette/uvicorn.py` & `troncos-3.2.1/troncos/frameworks/starlette/uvicorn.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.0/troncos/frameworks/structlog/processors.py` & `troncos-3.2.1/troncos/frameworks/structlog/processors.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,18 +47,23 @@
 def trace_injection_processor(
     _logger: WrappedLogger, _log_method: str, event_dict: EventDict
 ) -> EventDict:
     """
     Simple logging processor that adds a trace_id to the log record if available.
     """
 
-    if not ddlazy.dd_initialized():
-        return event_dict
+    # Try to get context from log record
+    dd_context = event_dict.pop("dd_context", None)
 
-    dd_context = ddlazy.dd_tracer().current_trace_context()
+    # Try to get context from tracer
+    if not dd_context:
+        if ddlazy.dd_initialized():
+            dd_context = ddlazy.dd_tracer().current_trace_context()
+
+    # Add context to log record if exists
     if dd_context:
         event_dict["trace_id"] = f"{dd_context.trace_id:x}".zfill(32)
         event_dict["span_id"] = f"{dd_context.span_id:x}"
 
         if ddlazy.dd_trace_export_enabled():
             event_dict["dd_trace_id"] = dd_context.trace_id
             event_dict["dd_span_id"] = dd_context.span_id
```

### Comparing `troncos-3.2.0/troncos/frameworks/structlog/setup.py` & `troncos-3.2.1/troncos/frameworks/structlog/setup.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.0/troncos/logs/__init__.py` & `troncos-3.2.1/troncos/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.0/troncos/logs/filters.py` & `troncos-3.2.1/troncos/logs/filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,18 +15,26 @@
     https://docs.python.org/3/howto/logging-cookbook.html#using-filters-to-impart-contextual-information
     """
 
     def __init__(self, name: str = "TraceIdFilter") -> None:
         super().__init__(name)
 
     def filter(self, record: logging.LogRecord) -> bool:
-        if not ddlazy.dd_initialized():
-            return True
+        dd_context = None
 
-        dd_context = ddlazy.dd_tracer().current_trace_context()
+        # Try to get context from log record
+        if hasattr(record, "dd_context"):
+            dd_context = record.dd_context
+            del record.dd_context
+        else:
+            # Try to get context from tracer
+            if ddlazy.dd_initialized():
+                dd_context = ddlazy.dd_tracer().current_trace_context()
+
+        # Add context to log record if exists
         if dd_context:
             record.trace_id = f"{dd_context.trace_id:x}".zfill(32)
             record.span_id = f"{dd_context.span_id:x}"
 
             if ddlazy.dd_trace_export_enabled():
                 record.dd_trace_id = dd_context.trace_id
                 record.dd_span_id = dd_context.span_id
```

### Comparing `troncos-3.2.0/troncos/logs/formatters.py` & `troncos-3.2.1/troncos/logs/formatters.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.0/troncos/profiling/__init__.py` & `troncos-3.2.1/troncos/profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.0/troncos/traces/__init__.py` & `troncos-3.2.1/troncos/traces/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.0/troncos/traces/dd_shim.py` & `troncos-3.2.1/troncos/traces/dd_shim.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.0/troncos/traces/decorate.py` & `troncos-3.2.1/troncos/traces/decorate.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.0/troncos/traces/propagation.py` & `troncos-3.2.1/troncos/traces/propagation.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.0/PKG-INFO` & `troncos-3.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troncos
-Version: 3.2.0
+Version: 3.2.1
 Summary: Collection of Python logging, tracing and profiling tools
 Home-page: https://github.com/kolonialno/troncos
 License: MIT
 Keywords: logs,traces,opentelemetry
 Author: Guðmundur Björn Birkisson
 Author-email: gudmundur.birkisson@oda.com
 Requires-Python: >=3.10,<4.0
@@ -15,15 +15,15 @@
 Provides-Extra: grpc
 Provides-Extra: http
 Provides-Extra: structlog
 Requires-Dist: ddtrace (==1.12.4)
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc (==1.17.0) ; extra == "grpc"
 Requires-Dist: opentelemetry-exporter-otlp-proto-http (==1.17.0) ; extra == "http"
 Requires-Dist: opentelemetry-sdk (==1.17.0)
-Requires-Dist: structlog (>=22.3.0,<23.0.0) ; extra == "structlog"
+Requires-Dist: structlog (>=22.3,<24.0) ; extra == "structlog"
 Project-URL: Documentation, https://github.com/kolonialno/troncos
 Project-URL: Repository, https://github.com/kolonialno/troncos
 Description-Content-Type: text/markdown
 
 <h1 align="center" style="border-bottom: 0">
   🪵<br>
   Troncos <br/>
@@ -326,34 +326,44 @@
 ```
 
 ### Structlog
 
 You can substitute `init_logging_basic` with `init_logging_structlog` to setup structlog:
 
 ```python
+import structlog
 from os import environ
 from troncos.frameworks.structlog.setup import init_logging_structlog
 
 init_logging_structlog(
     level=environ.get("LOG_LEVEL", "INFO"),
     formatter=environ.get("LOG_FORMATTER", "cli"),  # Use "logfmt" in production
 )
+
+log = structlog.get_logger()
+log.info("Some Message")
 ```
 
 Alternatively you can add trace injection into your own structlog setup:
 
 ```python
 import structlog
+from structlog.dev import ConsoleRenderer
+
 from troncos.frameworks.structlog.processors import trace_injection_processor
 
 structlog.configure(
     processors=[
-       trace_injection_processor,
+        trace_injection_processor,
+        ConsoleRenderer(),
     ],
 )
+
+log = structlog.get_logger()
+log.info("Some Message")
 ```
 
 ## Tracing
 
 ### Tracing your code
 
 After initializing tracing in your project you can use different methods to trace your code.
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: troncos Version: 3.2.0 Summary: Collection of
+Metadata-Version: 2.1 Name: troncos Version: 3.2.1 Summary: Collection of
 Python logging, tracing and profiling tools Home-page: https://github.com/
 kolonialno/troncos License: MIT Keywords: logs,traces,opentelemetry Author:
 GuÃ°mundur BjÃ¶rn Birkisson Author-email: gudmundur.birkisson@oda.com Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: grpc Provides-Extra: http Provides-Extra: structlog Requires-
 Dist: ddtrace (==1.12.4) Requires-Dist: opentelemetry-exporter-otlp-proto-grpc
 (==1.17.0) ; extra == "grpc" Requires-Dist: opentelemetry-exporter-otlp-proto-
 http (==1.17.0) ; extra == "http" Requires-Dist: opentelemetry-sdk (==1.17.0)
-Requires-Dist: structlog (>=22.3.0,<23.0.0) ; extra == "structlog" Project-URL:
+Requires-Dist: structlog (>=22.3,<24.0) ; extra == "structlog" Project-URL:
 Documentation, https://github.com/kolonialno/troncos Project-URL: Repository,
 https://github.com/kolonialno/troncos Description-Content-Type: text/markdown
                                   ****** ðªµ
                                    Troncos
                                      ******
           Collection of Python logging, tracing and profiling tools
        [CI_status] [https://img.shields.io/pypi/v/troncos.svg] [https://
@@ -123,89 +123,91 @@
 post_request(worker, req, environ, resp): duration = time.time() -
 req._gunicorn_start_time trace_id = next(iter([v for k, v in req.headers if k
 == "X-B3-TRACEID"]), None) worker.log.info( "[status=%s] %s %s duration=%s
 traceID=%s", resp.status, req.method, req.path, duration, trace_id, ) ``` Then
 when running gunicorn, specify what config file to use: ```console gunicorn
 myapp.wsgi:application --config python:myapp.gunicorn.config ... ``` ###
 Structlog You can substitute `init_logging_basic` with `init_logging_structlog`
-to setup structlog: ```python from os import environ from
+to setup structlog: ```python import structlog from os import environ from
 troncos.frameworks.structlog.setup import init_logging_structlog
 init_logging_structlog( level=environ.get("LOG_LEVEL", "INFO"),
 formatter=environ.get("LOG_FORMATTER", "cli"), # Use "logfmt" in production )
-``` Alternatively you can add trace injection into your own structlog setup:
-```python import structlog from troncos.frameworks.structlog.processors import
-trace_injection_processor structlog.configure( processors=
-[ trace_injection_processor, ], ) ``` ## Tracing ### Tracing your code After
-initializing tracing in your project you can use different methods to trace
-your code. #### trace_function This decorator adds tracing to a function. You
-can supply a tracer provider, if none is supplied, the global tracer provider
-will be used: ```python from troncos.traces.decorate import trace_function
-@trace_function def myfunc1(): return "This will be traced" @trace_function
-(service="my_custom_service") def myfunc2(): return "This will be traced as
-my_custom_service" ``` #### trace_block Trace using a with statement. You can
-supply a tracer provider, if none is supplied, the global tracer provider will
-be used. ```python from troncos.traces.decorate import trace_block with
-trace_block(name="action", resource="thing", attributes={"some": "attribute"}):
-print("... do an action to a thing...") ``` #### trace_class This decorator
-adds a tracing decorator to every method of the decorated class. If you don't
-want some methods to be traced, you can add the [trace_ignore](#traceignore)
+log = structlog.get_logger() log.info("Some Message") ``` Alternatively you can
+add trace injection into your own structlog setup: ```python import structlog
+from structlog.dev import ConsoleRenderer from
+troncos.frameworks.structlog.processors import trace_injection_processor
+structlog.configure( processors=[ trace_injection_processor, ConsoleRenderer(),
+], ) log = structlog.get_logger() log.info("Some Message") ``` ## Tracing ###
+Tracing your code After initializing tracing in your project you can use
+different methods to trace your code. #### trace_function This decorator adds
+tracing to a function. You can supply a tracer provider, if none is supplied,
+the global tracer provider will be used: ```python from troncos.traces.decorate
+import trace_function @trace_function def myfunc1(): return "This will be
+traced" @trace_function(service="my_custom_service") def myfunc2(): return
+"This will be traced as my_custom_service" ``` #### trace_block Trace using a
+with statement. You can supply a tracer provider, if none is supplied, the
+global tracer provider will be used. ```python from troncos.traces.decorate
+import trace_block with trace_block(name="action", resource="thing",
+attributes={"some": "attribute"}): print("... do an action to a thing...") ```
+#### trace_class This decorator adds a tracing decorator to every method of the
+decorated class. If you don't want some methods to be traced, you can add the
+[trace_ignore](#traceignore) decorator to them. You can supply a tracer
+provider, if none is supplied, the global tracer provider will be used:
+```python from troncos.traces.decorate import trace_class, trace_ignore
+@trace_class class MyClass1: def m1(self): return "This will be traced"
+@trace_ignore def m2(self): return "This will not traced" @trace_class
+(service="my_custom_service") class MyClass2: def m3(self): return "This will
+be traced as my_custom_service" ``` #### trace_module This function adds a
+tracing decorator to every function of the calling module. If you don't want
+some functions to be traced, you can add the [trace_ignore](#traceignore)
 decorator to them. You can supply a tracer provider, if none is supplied, the
 global tracer provider will be used: ```python from troncos.traces.decorate
-import trace_class, trace_ignore @trace_class class MyClass1: def m1(self):
-return "This will be traced" @trace_ignore def m2(self): return "This will not
-traced" @trace_class(service="my_custom_service") class MyClass2: def m3(self):
-return "This will be traced as my_custom_service" ``` #### trace_module This
-function adds a tracing decorator to every function of the calling module. If
-you don't want some functions to be traced, you can add the [trace_ignore]
-(#traceignore) decorator to them. You can supply a tracer provider, if none is
-supplied, the global tracer provider will be used: ```python from
-troncos.traces.decorate import trace_ignore, trace_module def my_function():
-return "This func will be traced" @trace_ignore def my_function(): return "This
-func will not be traced" trace_module() ``` #### trace_ignore A decorator that
-will make [trace_class](#traceclass) and [trace_module](#tracemodule) ignore
-the decorated function/method. ### Trace Propagation > **Warning**: Traces with
-IDs bigger than `64` bits are not propagated correctly because of limitations
-of [ddtrace](https://github.com/DataDog/dd-trace-py/blob/
-1e1de001d3fd694d3bcf0fff604a927ef891b19e/ddtrace/propagation/http.py#L102-
-L108). Default trace ID size for OTEL is `128` bits. If you want to propagate
-your trace to the next service, you need to send/receive special headers with
-your request/message. If you are using plain `requests` that should be handled
-automatically by troncos. Here is how you do this manually: #### Send context
-```python from troncos.traces.propagation import get_propagation_value # Get
-header value value = get_propagation_value() # Send it somewhere ``` or
-```python from troncos.traces.propagation import add_context_to_dict some_dict
-= {} # Add propagation headers to dict add_context_to_dict(some_dict) # Send it
-somewhere ``` #### Receive context Again, troncos should in most cases do this
-automatically for you, but here is how you do it manually: ```python from
-troncos.traces.propagation import activate_context_from_dict from
-troncos.traces.decorate import trace_block some_dict = {}
-activate_context_from_dict(some_dict) with trace_block("my_block"): print("...
-do something ...") ``` ### Trace sampling Set these variables to turn on trace
-sampling: ```console OTEL_TRACES_SAMPLER=parentbased_traceidratio
-OTEL_TRACES_SAMPLER_ARG=0.05 DD_TRACE_SAMPLE_RATE=0.05 ``` ### Trace debugging
-You can enable trace debugging by setting the environmental variable
-`OTEL_TRACE_DEBUG=true`. That will print all spans to the console. If you would
-rather get the spans in a file you can also provide the variable
-`OTEL_TRACE_DEBUG_FILE=/tmp/traces`. ## Profiling > **Warning**: Profiling
-while using Python 3.11 is [not yet fully supported](https://github.com/
-DataDog/dd-trace-py/issues/4149). ### Setup endpoint Simply add a `/debug/
-pprof` endpoint that returns the profile: ```python from fastapi import FastAPI
-from starlette.responses import Response from troncos.profiling import
-init_profiling_basic profiler = init_profiling_basic() app = FastAPI
-(title="my_service") @app.get("/debug/pprof", response_model=str) async def
-debug_pprof() -> Response: content, headers = profiler() return Response
-(content=content, headers=headers) ``` You can verify that your setup works
-with the [pprof](https://github.com/google/pprof) cli: ```console $ pprof -http
-:6060 "http://localhost:8080/debug/pprof" ``` > **Note**: You will get an empty
-string from `profiler()` until the first profile has been collected. ### Enable
-scraping When you deploy your application, be sure to use the custom oda
-annotation for scraping: ```yaml annotations: phlare.oda.com/port: "8080"
-phlare.oda.com/scrape: "true" ``` ## Development When developing troncos you
-should be constantly aware of the fact that under no circumstances should you
-import `ddtrace` into your module. That would cause the tracer to initialize
-with default values that would not change when the user initializes the tracer.
-For this reason, if you need to use any parts of `ddtrace` in your code,
-consider using the `_ddlazy` module, that gives you access lazily. If that does
-not satisfy your requirements you can always import `ddtrace` in your functions
-(not at the top of your module). You can compare performance of your local
-version, to some older version of troncos using the [performance test setup](./
-perf).
+import trace_ignore, trace_module def my_function(): return "This func will be
+traced" @trace_ignore def my_function(): return "This func will not be traced"
+trace_module() ``` #### trace_ignore A decorator that will make [trace_class]
+(#traceclass) and [trace_module](#tracemodule) ignore the decorated function/
+method. ### Trace Propagation > **Warning**: Traces with IDs bigger than `64`
+bits are not propagated correctly because of limitations of [ddtrace](https://
+github.com/DataDog/dd-trace-py/blob/1e1de001d3fd694d3bcf0fff604a927ef891b19e/
+ddtrace/propagation/http.py#L102-L108). Default trace ID size for OTEL is `128`
+bits. If you want to propagate your trace to the next service, you need to
+send/receive special headers with your request/message. If you are using plain
+`requests` that should be handled automatically by troncos. Here is how you do
+this manually: #### Send context ```python from troncos.traces.propagation
+import get_propagation_value # Get header value value = get_propagation_value()
+# Send it somewhere ``` or ```python from troncos.traces.propagation import
+add_context_to_dict some_dict = {} # Add propagation headers to dict
+add_context_to_dict(some_dict) # Send it somewhere ``` #### Receive context
+Again, troncos should in most cases do this automatically for you, but here is
+how you do it manually: ```python from troncos.traces.propagation import
+activate_context_from_dict from troncos.traces.decorate import trace_block
+some_dict = {} activate_context_from_dict(some_dict) with trace_block
+("my_block"): print("... do something ...") ``` ### Trace sampling Set these
+variables to turn on trace sampling: ```console
+OTEL_TRACES_SAMPLER=parentbased_traceidratio OTEL_TRACES_SAMPLER_ARG=0.05
+DD_TRACE_SAMPLE_RATE=0.05 ``` ### Trace debugging You can enable trace
+debugging by setting the environmental variable `OTEL_TRACE_DEBUG=true`. That
+will print all spans to the console. If you would rather get the spans in a
+file you can also provide the variable `OTEL_TRACE_DEBUG_FILE=/tmp/traces`. ##
+Profiling > **Warning**: Profiling while using Python 3.11 is [not yet fully
+supported](https://github.com/DataDog/dd-trace-py/issues/4149). ### Setup
+endpoint Simply add a `/debug/pprof` endpoint that returns the profile:
+```python from fastapi import FastAPI from starlette.responses import Response
+from troncos.profiling import init_profiling_basic profiler =
+init_profiling_basic() app = FastAPI(title="my_service") @app.get("/debug/
+pprof", response_model=str) async def debug_pprof() -> Response: content,
+headers = profiler() return Response(content=content, headers=headers) ``` You
+can verify that your setup works with the [pprof](https://github.com/google/
+pprof) cli: ```console $ pprof -http :6060 "http://localhost:8080/debug/pprof"
+``` > **Note**: You will get an empty string from `profiler()` until the first
+profile has been collected. ### Enable scraping When you deploy your
+application, be sure to use the custom oda annotation for scraping: ```yaml
+annotations: phlare.oda.com/port: "8080" phlare.oda.com/scrape: "true" ``` ##
+Development When developing troncos you should be constantly aware of the fact
+that under no circumstances should you import `ddtrace` into your module. That
+would cause the tracer to initialize with default values that would not change
+when the user initializes the tracer. For this reason, if you need to use any
+parts of `ddtrace` in your code, consider using the `_ddlazy` module, that
+gives you access lazily. If that does not satisfy your requirements you can
+always import `ddtrace` in your functions (not at the top of your module). You
+can compare performance of your local version, to some older version of troncos
+using the [performance test setup](./perf).
```

