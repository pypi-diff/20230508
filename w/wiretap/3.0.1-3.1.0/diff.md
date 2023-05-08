# Comparing `tmp/wiretap-3.0.1-py3-none-any.whl.zip` & `tmp/wiretap-3.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4707 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      201 b- defN 23-Apr-07 12:05 wiretap/__init__.py
+Zip file size: 4627 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      199 b- defN 23-May-08 08:36 wiretap/__init__.py
 -rw-rw-rw-  2.0 fat      620 b- defN 23-Feb-08 09:16 wiretap/layers.py
--rw-rw-rw-  2.0 fat    10812 b- defN 23-Apr-28 12:28 wiretap/wiretap.py
--rw-rw-rw-  2.0 fat      223 b- defN 23-May-03 11:19 wiretap-3.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-03 11:19 wiretap-3.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-03 11:19 wiretap-3.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      520 b- defN 23-May-03 11:19 wiretap-3.0.1.dist-info/RECORD
-7 files, 12476 bytes uncompressed, 3789 bytes compressed:  69.6%
+-rw-rw-rw-  2.0 fat    10667 b- defN 23-May-08 08:49 wiretap/wiretap.py
+-rw-rw-rw-  2.0 fat      244 b- defN 23-May-08 08:57 wiretap-3.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-08 08:57 wiretap-3.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-08 08:57 wiretap-3.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      520 b- defN 23-May-08 08:57 wiretap-3.1.0.dist-info/RECORD
+7 files, 12350 bytes uncompressed, 3709 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: wiretap/layers.py
 Comment: 
 
 Filename: wiretap/wiretap.py
 Comment: 
 
-Filename: wiretap-3.0.1.dist-info/METADATA
+Filename: wiretap-3.1.0.dist-info/METADATA
 Comment: 
 
-Filename: wiretap-3.0.1.dist-info/WHEEL
+Filename: wiretap-3.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: wiretap-3.0.1.dist-info/top_level.txt
+Filename: wiretap-3.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: wiretap-3.0.1.dist-info/RECORD
+Filename: wiretap-3.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wiretap/__init__.py

```diff
@@ -1,12 +1,11 @@
 from .wiretap import (
     Logger,
-    telemetry,
     OnStarted,
     OnCompleted,
-    CannotContinue,
-    begin_telemetry,
+    FormatStartDetails,
+    FormatResultDetails,
     SerializeDetails,
     MultiFormatter,
+    telemetry,
+    collect,
 )
-
-from . import layers
```

## wiretap/wiretap.py

```diff
@@ -1,21 +1,22 @@
-import sys
 import asyncio
 import contextlib
 import functools
 import inspect
 import json
 import logging
 import sys
 import uuid
+import collections.abc
+import abc
 from collections.abc import Generator
 from contextvars import ContextVar
 from datetime import datetime, date
 from timeit import default_timer as timer
-from typing import Dict, Callable, Any, Protocol, Optional, Iterator
+from typing import Dict, Callable, Any, Protocol, Optional, Iterator, TypeVar
 
 _scope: ContextVar[Optional["Logger"]] = ContextVar("_scope", default=None)
 
 
 class SerializeDetails(Protocol):
     def __call__(self, value: Optional[Dict[str, Any]]) -> str | None: ...
 
@@ -59,14 +60,81 @@
         if hasattr(record, "format"):
             self._style._fmt = record.format
 
         self.formats = DEFAULT_FORMATS | self.formats
         return super().format(record)
 
 
+class OnStarted(Protocol):
+    """Allows you to create details from function arguments."""
+
+    def __call__(self, params: Dict[str, Any]) -> Dict[str, Any]: ...
+
+
+class OnCompleted(Protocol):
+    """Allows you to create details from function result."""
+
+    def __call__(self, result: Optional[Any]) -> Dict[str, Any]: ...
+
+
+class EmptyOnStarted:
+    def __call__(self, params: Dict[str, Any]) -> Dict[str, Any]:
+        return {}
+
+
+class EmptyOnCompleted(OnCompleted):
+    def __call__(self, result: Optional[Any]) -> Dict[str, Any]:
+        return {}
+
+
+def _format_detail(value: Any, formats: Optional[str | Callable[[Any], Any]]) -> Optional[Any]:
+    if not value:
+        return None
+
+    if not formats:
+        return None
+
+    if isinstance(formats, str):
+        return format(value, formats)
+
+    if callable(formats):
+        return formats(value)
+
+    raise ValueError(f"Details format supports only [str | Callable[[Any], Any] not {type(formats)}")
+
+
+class FormatStartDetails(OnStarted):
+    def __init__(self, **details):
+        self.details = details
+
+    def __call__(self, params: Dict[str, Any]) -> Dict[str, Any]:
+        return {key: _format_detail(params.get(key, None), self.details[key]) for key in self.details}
+
+
+class FormatResultDetails(OnCompleted):
+    def __init__(self, formats: Optional[str | Callable[[Any], Any]] = None, **details):
+        self.formats = formats
+        self.details = details
+
+    def __call__(self, value: Optional[Any]) -> Dict[str, Any]:
+        if not value:
+            return dict(result=None)
+
+        if self.formats:
+            return dict(result=_format_detail(value, self.formats))
+
+        if self.details:
+            return {key: _format_detail(value, self.details[key]) for key in self.details}
+
+        return dict(result=value)
+
+
+TResult = TypeVar("TResult")
+
+
 class Logger:
 
     def __init__(self, module: Optional[str], scope: str, parent: Optional["Logger"] = None):
         self.id = uuid.uuid4()
         self.module = module
         self.scope = scope
         self.parent = parent
@@ -75,49 +143,51 @@
         self._finalized = False
         self._logger = logging.getLogger(f"{module}.{scope}")
 
     @property
     def elapsed(self) -> float:
         return round(timer() - self._start, 3)
 
-    def started(self, **kwargs):
+    def started(self, **details):
         self._logger.setLevel(logging.INFO)
         self._start = timer()
-        self._log(**kwargs)
+        self._log(**details)
 
-    def running(self, **kwargs):
+    def running(self, **details):
         self._logger.setLevel(logging.DEBUG)
-        self._log(**kwargs)
+        self._log(**details)
 
-    def completed(self, **kwargs):
+    def completed(self, result: Optional[TResult] = None, details_factory: OnCompleted = EmptyOnCompleted(), **details) -> Optional[TResult]:
         self._logger.setLevel(logging.INFO)
-        self._log(**kwargs)
+        self._log(**(details_factory(result) | details))
+        return result
 
-    def canceled(self, **kwargs):
+    def canceled(self, result: Optional[TResult] = None, details_factory: OnCompleted = EmptyOnCompleted(), **details) -> Optional[TResult]:
         self._logger.setLevel(logging.WARNING)
-        self._log(**kwargs)
+        self._log(**(details_factory(result) | details))
+        return result
 
-    def faulted(self, **kwargs):
+    def faulted(self, result: Optional[TResult] = None, details_factory: OnCompleted = EmptyOnCompleted(), **details) -> Optional[TResult]:
         self._logger.setLevel(logging.ERROR)
-        self._log(**kwargs)
+        self._log(**(details_factory(result) | details))
+        return result
 
     def _log(self, **kwargs):
         if self._finalized:
             return
 
         status = inspect.stack()[1][3]
         with _use_custom_log_record_factory(
                 _set_exc_text,
                 functools.partial(_set_module_name, name=self.module),
                 functools.partial(_set_func_name, name=self.scope),
                 functools.partial(_set_attachment, value=kwargs.pop("attachment", None)),
         ):
-            # Exceptions must be logged with the exception method or otherwise the exception will be missing.
-            is_error = all(sys.exc_info()) and sys.exc_info()[0] is not CannotContinue
-            self._logger.log(level=self._logger.level, msg=None, exc_info=is_error, extra={
+            exc_info = all(sys.exc_info())
+            self._logger.log(level=self._logger.level, msg=None, exc_info=exc_info, extra={
                 "parent": self.parent.id if self.parent else None,
                 "node": self.id,
                 "status": status,
                 "elapsed": self.elapsed,
                 "details": kwargs | {"depth": self.depth}
             })
 
@@ -126,156 +196,79 @@
     def __iter__(self):
         current = self
         while current:
             yield current
             current = current.parent
 
 
-class AttachDetails(Protocol):
-    def __call__(self, details: Dict[str, Any]) -> None: ...
-
-
-class OnStarted(Protocol):
-    """Allows you to create details from function arguments."""
-
-    def __call__(self, params: Dict[str, Any]) -> Optional[Dict[str, Any]]: ...
-
-
-class OnCompleted(Protocol):
-    """Allows you to create details from function result."""
-
-    def __call__(self, result: Any) -> Optional[Dict[str, Any]]: ...
-
-
-class CannotContinue(Exception):
-    """Raise this error to gracefully handle a cancellation."""
-
-    details: Dict[str, Any] = dict()
-    result: Optional[Any] = None
-
-    def __new__(cls, reason: str, result: Optional[Any] = None, **details) -> "CannotContinue":
-        instance = super().__new__(cls)
-        details["reason"] = reason
-        instance.details = details
-        instance.result = result
-        return instance
-
-    def __init__(self, reason: str, result: Optional[Any] = None, **details):
-        super().__init__(reason)
-
-
-class ReturnValueMissing(Exception):
-
-    def __init__(self, name: str):
-        super().__init__(f"Function '{name}' expects a return value, but it wasn't provided.")
-
-
-def _default_on_started(params: Dict[str, Any]) -> Optional[Dict[str, Any]]:
-    return None
-
-
-def _default_on_completed(result: Any) -> Optional[Dict[str, Any]]:
-    return None
+@contextlib.contextmanager
+def collect(module: Optional[str], name: str, **kwargs) -> Iterator[Logger]:
+    """Begins a new telemetry scope."""
+    logger = Logger(module, name, _scope.get())
+    token = _scope.set(logger)
+    try:
+        logger.started(**kwargs)
+        yield logger
+        logger.completed(test="blub!")
+    except:  # noqa
+        logger.faulted()
+        raise
+    finally:
+        _scope.reset(token)
 
 
-def telemetry(on_started: OnStarted = _default_on_started, on_completed: OnCompleted = _default_on_completed, attachment: Optional[Any] = None):
-    """Provides flow telemetry for the decorated function. Use named args to provide more static data."""
+def telemetry(on_started: OnStarted = EmptyOnStarted(), on_completed: OnCompleted = EmptyOnCompleted(), attachment: Optional[Any] = None):
+    """Provides telemetry for the decorated function."""
 
     def factory(decoratee):
         module = inspect.getmodule(decoratee)
-
-        @contextlib.contextmanager
-        def logger_scope() -> Iterator[Logger]:
-            logger = Logger(
-                module=module.__name__ if module else None,
-                scope=decoratee.__name__,
-                parent=_scope.get()
-            )
-
-            token = _scope.set(logger)
-            try:
-                yield logger
-            except Exception:
-                logger.faulted()
-                raise
-            finally:
-                _scope.reset(token)
+        module_name = module.__name__ if module else None
+        scope_name = decoratee.__name__
 
         def inject_logger(logger: Logger, d: Dict):
-            """ Injects Logger if required. """
+            """Injects Logger if required."""
             for n, t in inspect.getfullargspec(decoratee).annotations.items():
                 if t is Logger:
                     d[n] = logger
 
         def params(*decoratee_args, **decoratee_kwargs) -> Dict[str, Any]:
             # Zip arg names and their indexes up to the number of args of the decoratee_args.
             arg_pairs = zip(inspect.getfullargspec(decoratee).args, range(len(decoratee_args)))
             # Turn arg_pairs into a dictionary and combine it with decoratee_kwargs.
             return {t[0]: decoratee_args[t[1]] for t in arg_pairs} | decoratee_kwargs
 
-        # returns = inspect.getfullargspec(decoratee).annotations.get("return", None) is not None
-
         if asyncio.iscoroutinefunction(decoratee):
             @functools.wraps(decoratee)
             async def decorator(*decoratee_args, **decoratee_kwargs):
-                if attachment:
-                    decoratee_kwargs["attachment"] = attachment
-                with logger_scope() as scope:
+                start_details = on_started(params(*decoratee_args, **decoratee_kwargs)) | dict(attachment=attachment)
+                with collect(module_name, scope_name, **start_details) as scope:
                     inject_logger(scope, decoratee_kwargs)
                     scope.started(**(on_started(params(*decoratee_args, **decoratee_kwargs)) or {}))
-                    try:
-                        result = await decoratee(*decoratee_args, **decoratee_kwargs)
-                        scope.completed(**(on_completed(result) or {}))
-                        return result
-                    except CannotContinue as e:
-                        scope.canceled(**((on_completed(result) or {}) | e.details))
-                        return e.result
+                    result = await decoratee(*decoratee_args, **decoratee_kwargs)
+                    return scope.completed(result, on_completed)
 
             decorator.__signature__ = inspect.signature(decoratee)
             return decorator
 
         else:
             @functools.wraps(decoratee)
             def decorator(*decoratee_args, **decoratee_kwargs):
-                if attachment:
-                    decoratee_kwargs["attachment"] = attachment
-                with logger_scope() as scope:
+                start_details = on_started(params(*decoratee_args, **decoratee_kwargs)) | dict(attachment=attachment)
+                with collect(module_name, scope_name, **start_details) as scope:
                     inject_logger(scope, decoratee_kwargs)
-                    scope.started(**(on_started(params(*decoratee_args, **decoratee_kwargs)) or {}))
-                    try:
-                        result = decoratee(*decoratee_args, **decoratee_kwargs)
-                        scope.completed(**(on_completed(result) or {}))
-                        return result
-                    except CannotContinue as e:
-                        scope.canceled(**((on_completed(result) or {}) | e.details))
-                        return e.result
+                    result = decoratee(*decoratee_args, **decoratee_kwargs)
+                    return scope.completed(result, on_completed)
 
             decorator.__signature__ = inspect.signature(decoratee)
             return decorator
 
     return factory
 
 
 @contextlib.contextmanager
-def begin_telemetry(name: str, **kwargs) -> Iterator[Logger]:
-    """Begins a new telemetry scope."""
-    logger = Logger(None, name, _scope.get())
-    token = _scope.set(logger)
-    try:
-        logger.started(**kwargs)
-        yield logger
-        logger.completed()
-    except:  # noqa
-        logger.faulted()
-        raise
-    finally:
-        _scope.reset(token)
-
-
-@contextlib.contextmanager
 def _use_custom_log_record_factory(*actions: Callable[[logging.LogRecord], None]) -> Generator[None, None, None]:
     default = logging.getLogRecordFactory()
 
     def custom(*args, **kwargs):
         record = default(*args, **kwargs)
         for action in actions:
             action(record)
```

