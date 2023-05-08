# Comparing `tmp/fieldedge-utilities-0.9.4.tar.gz` & `tmp/fieldedge-utilities-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fieldedge-utilities-0.9.4.tar", max compression
+gzip compressed data, was "fieldedge-utilities-0.9.5.tar", max compression
```

## Comparing `fieldedge-utilities-0.9.4.tar` & `fieldedge-utilities-0.9.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2021-09-20 21:08:25.480264 fieldedge-utilities-0.9.4/LICENSE
--rw-r--r--   0        0        0      551 2022-01-06 23:17:22.524983 fieldedge-utilities-0.9.4/README.md
--rw-r--r--   0        0        0      174 2022-04-19 16:57:04.907158 fieldedge-utilities-0.9.4/fieldedge_utilities/__init__.py
--rw-r--r--   0        0        0     9750 2022-04-19 17:00:18.520569 fieldedge-utilities-0.9.4/fieldedge_utilities/hostpipe.py
--rw-r--r--   0        0        0     2400 2022-02-26 16:38:59.585139 fieldedge-utilities-0.9.4/fieldedge_utilities/ip_interfaces.py
--rw-r--r--   0        0        0     6987 2021-12-04 16:25:38.302982 fieldedge-utilities-0.9.4/fieldedge_utilities/logger.py
--rw-r--r--   0        0        0    13501 2022-04-19 17:08:36.344321 fieldedge-utilities-0.9.4/fieldedge_utilities/mqtt.py
--rw-r--r--   0        0        0     1998 2022-01-10 12:18:24.112291 fieldedge-utilities-0.9.4/fieldedge_utilities/path.py
--rw-r--r--   0        0        0     1077 2022-04-06 15:50:04.437496 fieldedge-utilities-0.9.4/fieldedge_utilities/protocols.py
--rw-r--r--   0        0        0     2183 2021-12-05 04:43:42.102918 fieldedge-utilities-0.9.4/fieldedge_utilities/serial.py
--rw-r--r--   0        0        0     7730 2022-04-19 17:06:18.992356 fieldedge-utilities-0.9.4/fieldedge_utilities/timer.py
--rw-r--r--   0        0        0      645 2022-04-19 17:09:56.637657 fieldedge-utilities-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     1369 2022-04-19 17:10:05.063400 fieldedge-utilities-0.9.4/setup.py
--rw-r--r--   0        0        0     1422 2022-04-19 17:10:05.063622 fieldedge-utilities-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-09-20 21:08:25.480264 fieldedge-utilities-0.9.5/LICENSE
+-rw-r--r--   0        0        0      551 2022-01-06 23:17:22.524983 fieldedge-utilities-0.9.5/README.md
+-rw-r--r--   0        0        0      174 2022-04-19 16:57:04.907158 fieldedge-utilities-0.9.5/fieldedge_utilities/__init__.py
+-rw-r--r--   0        0        0     9750 2022-04-19 17:00:18.520569 fieldedge-utilities-0.9.5/fieldedge_utilities/hostpipe.py
+-rw-r--r--   0        0        0     2400 2022-02-26 16:38:59.585139 fieldedge-utilities-0.9.5/fieldedge_utilities/ip_interfaces.py
+-rw-r--r--   0        0        0     8932 2022-04-19 20:37:26.071170 fieldedge-utilities-0.9.5/fieldedge_utilities/logger.py
+-rw-r--r--   0        0        0    13501 2022-04-19 17:08:36.344321 fieldedge-utilities-0.9.5/fieldedge_utilities/mqtt.py
+-rw-r--r--   0        0        0     1998 2022-01-10 12:18:24.112291 fieldedge-utilities-0.9.5/fieldedge_utilities/path.py
+-rw-r--r--   0        0        0     1077 2022-04-06 15:50:04.437496 fieldedge-utilities-0.9.5/fieldedge_utilities/protocols.py
+-rw-r--r--   0        0        0     2183 2021-12-05 04:43:42.102918 fieldedge-utilities-0.9.5/fieldedge_utilities/serial.py
+-rw-r--r--   0        0        0     7699 2022-04-19 21:05:32.689763 fieldedge-utilities-0.9.5/fieldedge_utilities/timer.py
+-rw-r--r--   0        0        0      711 2022-04-19 21:13:21.874121 fieldedge-utilities-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     1369 2022-04-19 21:13:28.913392 fieldedge-utilities-0.9.5/setup.py
+-rw-r--r--   0        0        0     1422 2022-04-19 21:13:28.913628 fieldedge-utilities-0.9.5/PKG-INFO
```

### Comparing `fieldedge-utilities-0.9.4/LICENSE` & `fieldedge-utilities-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fieldedge-utilities-0.9.4/README.md` & `fieldedge-utilities-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `fieldedge-utilities-0.9.4/fieldedge_utilities/hostpipe.py` & `fieldedge-utilities-0.9.5/fieldedge_utilities/hostpipe.py`

 * *Files identical despite different names*

### Comparing `fieldedge-utilities-0.9.4/fieldedge_utilities/ip_interfaces.py` & `fieldedge-utilities-0.9.5/fieldedge_utilities/ip_interfaces.py`

 * *Files identical despite different names*

### Comparing `fieldedge-utilities-0.9.4/fieldedge_utilities/logger.py` & `fieldedge-utilities-0.9.5/fieldedge_utilities/logger.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,88 +23,193 @@
 """
 import logging
 from logging.handlers import RotatingFileHandler
 import os
 import sys
 from time import gmtime
 
-from fieldedge_utilities.path import clean_path, get_caller_name
+from fieldedge_utilities.path import clean_path
 
 FORMAT_CSV = ('%(asctime)s.%(msecs)03dZ,[%(levelname)s],(%(threadName)s),'
               '%(module)s.%(funcName)s:%(lineno)d,%(message)s')
 FORMAT_JSON = ('{'
                 '"datetime":"%(asctime)s.%(msecs)03dZ"'
                 ',"level":"%(levelname)s"'
                 ',"thread":"%(threadName)s"'
                 ',"module":"%(module)s"'
                 ',"function":"%(funcName)s"'
                 ',"line":%(lineno)d'
                 ',"message":"%(message)s"'
                 '}')
+DATEFMT = '%Y-%m-%dT%H:%M:%S'
 
 
-# Logging to STDOUT or STDERR
-class _LessThanFilter(logging.Filter):
-    """Filters logs below a specified level for routing to a given handler."""
+class LogFilterLessThan(logging.Filter):
+    """Filters logs below a specified level for routing to a given handler.
+    
+    Intended to route `WARNING` and higher to `STDERR` and lower to `STDOUT`.
+
+    """
     def __init__(self,
                  exclusive_maximum: int = logging.WARNING,
                  name: str = None):
         if name is None:
             name = f'LessThan{logging.getLevelName(exclusive_maximum)}'
-        # super(_LessThanFilter, self).__init__(name)
         super().__init__(name)
         self.max_level = exclusive_maximum
 
     def filter(self, record):
         #non-zero return means we log this message
         return 1 if record.levelno < self.max_level else 0
 
 
-class _OneLineExceptionFormatter(logging.Formatter):
-    """Formats exceptions into a single line stack trace."""
+class LogFormatterOneLineException(logging.Formatter):
+    """Formats exceptions into a single line stack trace.
+    
+    Also replaces the record message with the error type.
+
+    """
     def formatException(self, exc_info):
         original = super().formatException(exc_info)
-        lines = original.splitlines()
-        result = ''
-        for i, line in enumerate(lines):
-            result += (' -> ' if i > 0 else '') + line.strip()
-        return result
+        return ' -> '.join([x.strip() for x in original.splitlines()])
 
     def format(self, record):
         result = super().format(record)
         if record.exc_text:
             err_type = type(record.msg).__name__
             result = result.replace(f'{record.msg}\n', f'{err_type}: ')
         return result
 
 
 def get_logfile_name(logger: logging.Logger) -> str:
-    """Returns the logger's RotatingFileHandler name."""
+    """Returns the logger's RotatingFileHandler name.
+    
+    Args:
+        logger: The Logger to retrieve its file name from.
+
+    Raises:
+        TypeError if Logger is invalid
+
+    """
+    if not isinstance(logger, logging.Logger):
+        raise TypeError('Invalid Logger')
     for h in logger.handlers:
         if isinstance(h, RotatingFileHandler):
             return h.baseFilename
-    return None
 
 
-def _is_log_handler(logger: logging.Logger, handler: object) -> bool:
-    """Returns true if the handler is found in the logger.
+def add_handler(logger: logging.Logger, handler: logging.Handler) -> None:
+    """Adds a handler to a logger if one of the same name is not present.
     
     Args:
-        logger (logging.Logger)
-        handler (logging handler)
+        logger: The logger to add the handler to.
+        handler: The handler to add to the logger.
     
-    Returns:
-        True if the handler is in the logger.
+    Raises:
+        TypeError if Logger or Handler are invalid
+        ValueError if a handler with the same name is already in the logger.
 
     """
     if not isinstance(logger, logging.Logger):
-        return False
+        raise TypeError('Invalid Logger')
+    if not isinstance(handler, logging.Handler):
+        raise TypeError('Invalid Handler')
     for h in logger.handlers:
         if h.name == handler.name:
-            return True
+            raise ValueError(f'Logger already has a handler named {h.name}')
+    logger.addHandler(handler)
+
+
+def apply_formatter(logger: logging.Logger,
+                    formatter: logging.Formatter) -> None:
+    """Applies the log formatter to all handlers in the logger.
+    
+    Args:
+        logger: The logger with the handler targets.
+        formatter: The formatter to apply.
+
+    Raises:
+        TypeError if Logger or Handler are invalid
+    
+    """
+    if not isinstance(logger, logging.Logger):
+        raise TypeError('Invalid Logger')
+    if not isinstance(formatter, logging.Formatter):
+        raise TypeError('Invalid Formatter')
+    for h in logger.handlers:
+        h.setFormatter(formatter)
+
+
+def apply_loglevel(logger: logging.Logger, level: int) -> None:
+    """Sets the log level on all handlers except stderr (always WARNING).
+    
+    Args:
+        logger: The logger whose handlers to apply the level to.
+        level: The logging level to apply
+
+    Raises:
+        TypeError if Logger is invalid
+    
+    """
+    if not isinstance(logger, logging.Logger):
+        raise TypeError('Invalid Logger')
+    for h in logger.handlers:
+        if 'stderr' not in h.name:
+            h.setLevel(level)
+
+
+def get_formatter(format: str = 'csv') -> logging.Formatter:
+    """Returns a standardized log formatter.
+    
+    Args:
+        format: `csv` or `json` are supported.
+    
+    Returns:
+        A logging.Formatter
+
+    """
+    fmt = FORMAT_JSON if format == 'json' else FORMAT_CSV
+    log_formatter = LogFormatterOneLineException(fmt, DATEFMT)
+    log_formatter.converter = gmtime
+    return log_formatter
+
+
+def get_handler_file(filename: str,
+                     file_size: int = 5,
+                     **kwargs) -> RotatingFileHandler:
+    if not filename:
+        raise ValueError('Missing filename')
+    filename = clean_path(filename)
+    if not os.path.isdir(os.path.dirname(filename)):
+        raise FileNotFoundError('Invalid logfile path'
+            f' {os.path.dirname(filename)}')
+    handler = RotatingFileHandler(
+        filename=filename,
+        mode=kwargs.pop('mode', 'a'),
+        maxBytes=kwargs.pop('maxBytes', int(file_size * 1024 * 1024)),
+        backupCount=kwargs.pop('backupCount', 2),
+        encoding=kwargs.pop('encoding', None),
+        delay=kwargs.pop('delay', 0),
+    )
+    handler.name = f'{kwargs.pop("name", __name__)}_file_handler'
+    return handler
+
+
+def get_handler_stdout(**kwargs) -> logging.StreamHandler:
+    handler_stdout = logging.StreamHandler(sys.stdout)
+    handler_stdout.name = f'{kwargs.pop("name", __name__)}_stdout_handler'
+    handler_stdout.addFilter(LogFilterLessThan(logging.WARNING))
+    return handler_stdout
+
+
+def get_handler_stderr(**kwargs) -> logging.StreamHandler:
+    handler_stderr = logging.StreamHandler(sys.stderr)
+    handler_stderr.name = f'{kwargs.pop("name", __name__)}_stderr_handler'
+    handler_stderr.setLevel(logging.WARNING)
+    return handler_stderr
 
 
 def get_wrapping_logger(name: str = None,
                         filename: str = None,
                         file_size: int = 5,
                         log_level: int = logging.INFO,
                         format: str = 'csv',
@@ -127,64 +232,31 @@
         format: `csv` or `json`
         kwargs: Optional overrides for RotatingFileHandler
             mode (str): defaults to `a` (append)
             maxBytes (int): overrides file_size
             backupCount (int): defaults to 2
     
     Returns:
-        A logger with console stream handler and (optional) file handler.
+        A `Logger` with console `StreamHandler` and (optional)
+            `RotatingFileHandler`.
     
     Raises:
-        FileNotFoundError if a logfile name is specified with an invalid
-            directory.
+        `FileNotFoundError` if a logfile name is specified with an invalid path.
     
     """
-    if format == 'json':
-        fmt = FORMAT_JSON
-    else:
-        fmt = FORMAT_CSV
-    log_formatter = _OneLineExceptionFormatter(fmt=fmt,
-                                               datefmt='%Y-%m-%dT%H:%M:%S')
-    log_formatter.converter = gmtime
-    if name is None:
-        name = get_caller_name()
+    if not name:
+        name = __name__
     logger = logging.getLogger(name)
-    if logger.getEffectiveLevel() == logging.DEBUG:
-        log_level = logging.DEBUG
-    #: Set up log file
     if filename is not None:
-        try:
-            filename = clean_path(filename)
-            if not os.path.isdir(os.path.dirname(filename)):
-                raise FileNotFoundError('Invalid logfile path'
-                    f' {os.path.dirname(filename)}')
-            handler_file = RotatingFileHandler(
-                filename=filename,
-                mode=kwargs.pop('mode', 'a'),
-                maxBytes=kwargs.pop('maxBytes', int(file_size * 1024 * 1024)),
-                backupCount=kwargs.pop('backupCount', 2),
-                encoding=kwargs.pop('encoding', None),
-                delay=kwargs.pop('delay', 0))
-            handler_file.name = name + '_file_handler'
-            handler_file.setFormatter(log_formatter)
-            handler_file.setLevel(log_level)
-            if not _is_log_handler(logger, handler_file):
-                logger.addHandler(handler_file)
-        except Exception as e:
-            logger.exception(f'Could not create RotatingFileHandler {filename}'
-                f' ({e})')
-            raise e
+        filename = clean_path(filename)
+        if not os.path.isdir(os.path.dirname(filename)):
+            raise FileNotFoundError('Invalid logfile path'
+                f' {os.path.dirname(filename)}')
+        add_handler(logger, get_handler_file(filename,
+                                             name=name,
+                                             file_size=file_size,
+                                             **kwargs))
+    add_handler(logger, get_handler_stdout(name=name))
+    add_handler(logger, get_handler_stderr(name=name))
+    apply_formatter(logger, get_formatter(format))
     logger.setLevel(log_level)
-    handler_stdout = logging.StreamHandler(sys.stdout)
-    handler_stdout.name = name + '_stdout_handler'
-    handler_stdout.setFormatter(log_formatter)
-    handler_stdout.setLevel(log_level)
-    handler_stdout.addFilter(_LessThanFilter(logging.WARNING))
-    if not _is_log_handler(logger, handler_stdout):
-        logger.addHandler(handler_stdout)
-    handler_stderr = logging.StreamHandler(sys.stderr)
-    handler_stderr.name = name + '_stderr_handler'
-    handler_stderr.setFormatter(log_formatter)
-    handler_stderr.setLevel(logging.WARNING)
-    if not _is_log_handler(logger, handler_stderr):
-        logger.addHandler(handler_stderr)
     return logger
```

### Comparing `fieldedge-utilities-0.9.4/fieldedge_utilities/mqtt.py` & `fieldedge-utilities-0.9.5/fieldedge_utilities/mqtt.py`

 * *Files identical despite different names*

### Comparing `fieldedge-utilities-0.9.4/fieldedge_utilities/path.py` & `fieldedge-utilities-0.9.5/fieldedge_utilities/path.py`

 * *Files identical despite different names*

### Comparing `fieldedge-utilities-0.9.4/fieldedge_utilities/protocols.py` & `fieldedge-utilities-0.9.5/fieldedge_utilities/protocols.py`

 * *Files identical despite different names*

### Comparing `fieldedge-utilities-0.9.4/fieldedge_utilities/serial.py` & `fieldedge-utilities-0.9.5/fieldedge_utilities/serial.py`

 * *Files identical despite different names*

### Comparing `fieldedge-utilities-0.9.4/fieldedge_utilities/timer.py` & `fieldedge-utilities-0.9.5/fieldedge_utilities/timer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import threading
 from time import time
-from typing import Callable, Tuple
 
 _log = logging.getLogger(__name__)
 
 
 class RepeatingTimer(threading.Thread):
     """A repeating thread to call a function, can be stopped/restarted/changed.
     
@@ -21,16 +20,16 @@
         name (str): An optional descriptive name for the Thread.
         interval (int): Repeating timer interval in seconds (0=disabled).
         sleep_chunk (float): The fraction of seconds between processing ticks.
 
     """
     def __init__(self,
                  seconds: int,
-                 target: Callable,
-                 args: Tuple = (),
+                 target: callable,
+                 args: tuple = (),
                  kwargs: dict = {},
                  name: str = None,
                  sleep_chunk: float = 0.25,
                  max_drift: int = None,
                  auto_start: bool = False,
                  defer: bool = True,
                  daemon: bool = True,
@@ -54,15 +53,15 @@
         Raises:
             ValueError if seconds is not an integer.
         """
         if not (isinstance(seconds, int) and seconds >= 0):
             err_str = 'RepeatingTimer seconds must be integer >= 0'
             raise ValueError(err_str)
         super().__init__(daemon=daemon)
-        self.name = name or f'{str(target)}_timer_thread'
+        self.name = name or f'{target.__name__}_timer_thread'
         self.interval = seconds
         if target is None:
             _log.warning(f'No target specified for RepeatingTimer {self.name}')
         self.target = target
         self._exception = None
         self.args = args
         self.kwargs = kwargs
```

### Comparing `fieldedge-utilities-0.9.4/pyproject.toml` & `fieldedge-utilities-0.9.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fieldedge-utilities"
-version = "0.9.4"
+version = "0.9.5"
 description = "Utilities package for the FieldEdge project."
 authors = ["geoffbrucepayne <geoff.bruce-payne@inmarsat.com>"]
 license = "Apache2.0"
 readme = "README.md"
 repository = "https://github.com/inmarsat-enterprise/fieldedge-utilities"
 keywords = ["Inmarsat", "FieldEdge"]
 
@@ -16,10 +16,14 @@
 ifaddr = "^0.1.7"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2.11.1"
 pytest = "^6.2.5"
 pdoc3 = "^0.10.0"
 
+[tool.pytest.ini_options]
+log_cli = true
+log_cli_level = "DEBUG"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fieldedge-utilities-0.9.4/setup.py` & `fieldedge-utilities-0.9.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['ifaddr>=0.1.7,<0.2.0',
  'paho-mqtt>=1.6.1,<2.0.0',
  'pyserial>=3.5,<4.0',
  'python-dotenv>=0.19.1,<0.20.0']
 
 setup_kwargs = {
     'name': 'fieldedge-utilities',
-    'version': '0.9.4',
+    'version': '0.9.5',
     'description': 'Utilities package for the FieldEdge project.',
     'long_description': '# Inmarsat FieldEdge Utilities\n\nInmarsat FieldEdge project supports *Internet of Things* (**IoT**) using\nsatellite communications technology.\n\nThis library available on **PyPI** provides:\n\n* A common **`logger`** format and wrapping file facility.\n* A simplified **`mqtt`** client that automatically connects\n(to a `fieldedge-broker`).\n* Helper functions for managing files and **`path`** on different OS.\n* An interface for **`hostpipe`** service interacting via a logfile.\n\n[Docmentation](https://inmarsat-enterprise.github.io/fieldedge-utilities/)\n',
     'author': 'geoffbrucepayne',
     'author_email': 'geoff.bruce-payne@inmarsat.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/inmarsat-enterprise/fieldedge-utilities',
```

### Comparing `fieldedge-utilities-0.9.4/PKG-INFO` & `fieldedge-utilities-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fieldedge-utilities
-Version: 0.9.4
+Version: 0.9.5
 Summary: Utilities package for the FieldEdge project.
 Home-page: https://github.com/inmarsat-enterprise/fieldedge-utilities
 License: Apache2.0
 Keywords: Inmarsat,FieldEdge
 Author: geoffbrucepayne
 Author-email: geoff.bruce-payne@inmarsat.com
 Requires-Python: >=3.7,<4.0
```

