# Comparing `tmp/project_runpy-1.0.1.tar.gz` & `tmp/project_runpy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project_runpy-1.0.1.tar", last modified: Thu Nov 14 03:53:38 2019, max compression
+gzip compressed data, was "project_runpy-1.1.0.tar", last modified: Mon May  8 18:39:11 2023, max compression
```

## Comparing `project_runpy-1.0.1.tar` & `project_runpy-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0      139 2019-07-09 01:47:00.830983 project_runpy-1.0.1/.gitignore
--rw-r--r--   0        0        0      175 2019-07-09 05:00:42.809834 project_runpy-1.0.1/.travis.yml
--rw-r--r--   0        0        0    10905 2019-07-09 01:47:00.832260 project_runpy-1.0.1/LICENSE
--rw-r--r--   0        0        0      792 2019-11-14 03:52:49.845888 project_runpy-1.0.1/Makefile
--rw-r--r--   0        0        0     3930 2019-07-09 05:00:42.810901 project_runpy-1.0.1/README.rst
--rw-r--r--   0        0        0      145 2019-11-14 03:53:14.605586 project_runpy-1.0.1/project_runpy/__init__.py
--rw-r--r--   0        0        0     4119 2019-11-14 03:52:49.846816 project_runpy-1.0.1/project_runpy/heidi.py
--rw-r--r--   0        0        0     2443 2019-07-09 05:00:42.812054 project_runpy-1.0.1/project_runpy/tim.py
--rw-r--r--   0        0        0      663 2019-07-09 05:02:24.174702 project_runpy-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       16 2019-11-14 03:52:48.015955 project_runpy-1.0.1/requirements.txt
--rw-r--r--   0        0        0      143 2019-07-09 02:00:12.498380 project_runpy-1.0.1/setup.cfg
--rw-r--r--   0        0        0     6224 2019-11-14 03:52:49.847487 project_runpy-1.0.1/test_project_runpy.py
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 project_runpy-1.0.1/setup.py
--rw-r--r--   0        0        0      205 1970-01-01 00:00:00.000000 project_runpy-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      810 2023-03-28 15:07:21.944788 project_runpy-1.1.0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0      139 2019-07-09 01:47:00.830983 project_runpy-1.1.0/.gitignore
+-rw-r--r--   0        0        0    10905 2019-07-09 01:47:00.832260 project_runpy-1.1.0/LICENSE
+-rw-r--r--   0        0        0      792 2023-03-27 06:13:41.234491 project_runpy-1.1.0/Makefile
+-rw-r--r--   0        0        0     3996 2023-03-28 15:06:36.708875 project_runpy-1.1.0/README.rst
+-rw-r--r--   0        0        0      145 2023-05-08 18:38:18.689896 project_runpy-1.1.0/project_runpy/__init__.py
+-rw-r--r--   0        0        0     5431 2023-05-08 18:37:53.030289 project_runpy-1.1.0/project_runpy/heidi.py
+-rw-r--r--   0        0        0     2463 2023-05-08 18:37:48.685339 project_runpy-1.1.0/project_runpy/tim.py
+-rw-r--r--   0        0        0      663 2023-03-27 06:18:52.904207 project_runpy-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       16 2019-11-14 03:52:48.015955 project_runpy-1.1.0/requirements.txt
+-rw-r--r--   0        0        0      143 2019-07-09 02:00:12.498380 project_runpy-1.1.0/setup.cfg
+-rw-r--r--   0        0        0     7235 2023-05-08 18:37:53.031732 project_runpy-1.1.0/test_project_runpy.py
+-rw-r--r--   0        0        0     4681 1970-01-01 00:00:00.000000 project_runpy-1.1.0/PKG-INFO
```

### Comparing `project_runpy-1.0.1/LICENSE` & `project_runpy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `project_runpy-1.0.1/Makefile` & `project_runpy-1.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `project_runpy-1.0.1/README.rst` & `project_runpy-1.1.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 project_runpy
 =============
 
-.. image:: https://travis-ci.org/crccheck/project_runpy.svg
-    :target: https://travis-ci.org/crccheck/project_runpy
+.. image:: https://github.com/crccheck/project_runpy/actions/workflows/ci.yaml/badge.svg?branch=master
+    :target: https://github.com/crccheck/project_runpy/actions/workflows/ci.yaml
 
 Generic helpers I wish existed or am constantly copying into my Python projects.
 
 
 ``env``
 -------
```

### Comparing `project_runpy-1.0.1/project_runpy/heidi.py` & `project_runpy-1.1.0/project_runpy/heidi.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,92 +1,133 @@
 """
 Heidi: Helpers related to visuals.
 """
 import logging
+import hashlib
 
-__all__ = ['ColorizingStreamHandler', 'ReadableSqlFilter']
+__all__ = [
+    "ColorizingStreamHandler",
+    "ColorizingLevelStreamHandler",
+    "ColorizingNameStreamHandler",
+    "ReadableSqlFilter",
+]
 
 
 # Copyright (C) 2010-2012 Vinay Sajip. All rights reserved. Licensed under the new BSD license.
 # https://gist.github.com/758430
 class ColorizingStreamHandler(logging.StreamHandler):
     # color names to indices
     color_map = {
-        'black': 0,
-        'red': 1,
-        'green': 2,
-        'yellow': 3,
-        'blue': 4,
-        'magenta': 5,
-        'cyan': 6,
-        'white': 7,
+        "black": 0,
+        "red": 1,
+        "green": 2,
+        "yellow": 3,
+        "blue": 4,
+        "magenta": 5,
+        "cyan": 6,
+        "white": 7,
     }
 
     # levels to (background, foreground, bold/intense)
     level_map = {
-        logging.DEBUG: (None, 'blue', False),
-        logging.INFO: (None, 'white', False),
-        logging.WARNING: (None, 'yellow', False),
-        logging.ERROR: (None, 'red', False),
-        logging.CRITICAL: ('red', 'white', True),
+        logging.DEBUG: (None, "blue", False),
+        logging.INFO: (None, "white", False),
+        logging.WARNING: (None, "yellow", False),
+        logging.ERROR: (None, "red", False),
+        logging.CRITICAL: ("red", "white", True),
     }
-    csi = '\x1b['
-    reset = '\x1b[0m'
+    csi = "\x1b["
+    reset = "\x1b[0m"
 
     @property
     def is_tty(self):
-        isatty = getattr(self.stream, 'isatty', None)
+        isatty = getattr(self.stream, "isatty", None)
         return isatty and isatty()
 
     def emit(self, record):
         try:
             message = self.format(record)
             stream = self.stream
             if not self.is_tty:
                 stream.write(message)
             else:
                 self.output_colorized(message)
-            stream.write(getattr(self, 'terminator', '\n'))
+            stream.write(getattr(self, "terminator", "\n"))
             self.flush()
         except (KeyboardInterrupt, SystemExit):
             raise
         except:  # noqa: E722
             self.handleError(record)
 
     def output_colorized(self, message):
         self.stream.write(message)
 
-    def colorize(self, message, record):
+    def colorize(self, message: str, record: logging.LogRecord) -> str:
         if record.levelno in self.level_map:
             bg, fg, bold = self.level_map[record.levelno]
             params = []
             if bg in self.color_map:
                 params.append(str(self.color_map[bg] + 40))
             if fg in self.color_map:
                 params.append(str(self.color_map[fg] + 30))
             if bold:
-                params.append('1')
+                params.append("1")
             if params:
-                message = ''.join((self.csi, ';'.join(params),
-                                   'm', message, self.reset))
+                message = "".join(
+                    (self.csi, ";".join(params), "m", message, self.reset)
+                )
         return message
 
     def format(self, record):
         message = logging.StreamHandler.format(self, record)
         if self.is_tty:
             # Don't colorize any traceback
-            parts = message.split('\n', 1)
+            parts = message.split("\n", 1)
             parts[0] = self.colorize(parts[0], record)
-            message = '\n'.join(parts)
+            message = "\n".join(parts)
+        return message
+
+
+class ColorizingLevelStreamHandler(ColorizingStreamHandler):
+    pass
+
+
+class ColorizingNameStreamHandler(ColorizingStreamHandler):
+    per_logger_colors = [
+        (None, "red", False),
+        (None, "green", False),
+        (None, "yellow", False),
+        (None, "blue", False),
+        (None, "magenta", False),
+        (None, "cyan", False),
+    ]
+
+    def colorize(self, message: str, record: logging.LogRecord) -> str:
+        bg, fg, bold = self.per_logger_colors[
+            int.from_bytes(
+                hashlib.blake2s(record.name.encode()).digest()[:8], byteorder="big"
+            )
+            % len(self.per_logger_colors)
+        ]
+        params = []
+        if bg in self.color_map:
+            params.append(str(self.color_map[bg] + 40))
+        if fg in self.color_map:
+            params.append(str(self.color_map[fg] + 30))
+        if bold:
+            params.append("1")
+        if params:
+            message = "".join((self.csi, ";".join(params), "m", message, self.reset))
         return message
 
 
 # LOGGING FILTERS
 #################
 
+
 class ReadableSqlFilter(logging.Filter):
     """
     A filter for more readable sql by stripping out the SELECT ... columns.
 
     Modeled after how debug toolbar displays SQL. This code should be optimized
     for performance. For example, I don't check to make sure record.name is
     'django.db.backends' because I assume you put this filter alongside it.
@@ -108,24 +149,27 @@
                 ...
             },
         }
     """
 
     def filter(self, record):
         # https://github.com/django/django/blob/febe136d4c3310ec8901abecca3ea5ba2be3952c/django/db/backends/utils.py#L106-L131
-        duration, sql, *__ = record.args
-        if not sql or 'SELECT' not in sql[:28]:
+        duration, sql, *record_args = record.args
+        if sql and "\n" in sql[:28]:
+            sql = " ".join(sql.strip().split())
+            record.args = (duration, sql, *record_args)
+        if not sql or "SELECT" not in sql[:28]:
             # WISHLIST what's the most performant way to see if 'SELECT' was
             # used?
             return super().filter(record)
 
-        begin = sql.index('SELECT')
+        begin = sql.index("SELECT")
         try:
-            end = sql.index('FROM', begin + 6)
+            end = sql.index("FROM", begin + 6)
         except ValueError:  # not all SELECT statements also have a FROM
             return super().filter(record)
 
-        sql = '{0}...{1}'.format(sql[:begin + 6], sql[end:])
+        sql = "{0}...{1}".format(sql[: begin + 6], sql[end:])
         # Drop "; args=%s" to shorten logging output
-        record.msg = '(%.3f) %s'
+        record.msg = "(%.3f) %s"
         record.args = (duration, sql)
         return super().filter(record)
```

### Comparing `project_runpy-1.0.1/project_runpy/tim.py` & `project_runpy-1.1.0/project_runpy/tim.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 """
 Tim: Helpers related to functionality.
 """
 import os
 
 
-__all__ = ['ImproperlyConfigured', 'env', ]
+__all__ = [
+    "ImproperlyConfigured",
+    "env",
+]
 
 
 class ImproperlyConfigured(Exception):
     """ForgotPantsException"""
+
     pass
 
 
 class _Env(dict):
     """A wrapper around os.environ that supports environments and `Boolean`."""
+
     def __init__(self):
         self.update(os.environ.copy())
 
     def parse_bool(self, value):
-        return str(value).lower() not in ('false', '0', 'f')
+        return str(value).lower() not in ("false", "0", "f")
 
     def get(self, key, default=None, type_func=None, **defaults):
         """
         Get information from your environment.
 
         If additional kwargs are specified, they will become the default if
         ENVIRONMENT matches the key.
@@ -34,20 +39,20 @@
             env.get('DEBUG', True)  # default can be bool
             env.get('WORKERS', 10)  # default can be other types too, like int
             env.get('WORKERS', 10, DEV=1)  # if ENVIRONMENT == DEV: default = 1
             env.get('DEBUG', True, type_func=bool)  # explicitly get bool
             env.get('DEBUG', FALSE, type_func=bool, TEST=False)  # combine it
 
         """
-        environment = os.environ.get('ENVIRONMENT')
+        environment = os.environ.get("ENVIRONMENT")
         default = defaults.get(environment, default)
         value = os.environ.get(key, default)
         if value is None and type_func is None:
             # return early to prevent returning 'None'
-            return ''
+            return ""
         if type_func is None:
             # guess the type_func
             type_func = str if default is None else default.__class__
         if type_func is bool:
             # strings will cast as `True` so don't use bool, use parse_bool.
             type_func = self.parse_bool
         return type_func(value)
@@ -61,14 +66,15 @@
 
         Example::
 
             env.require('SECRET_KEY')
         """
         # yeah, I could check the inputs and do stuff, but I feel like wrapping.
         result = self.get(key, default, *args, **kwargs)
-        if result == '':
+        if result == "":
             raise ImproperlyConfigured(
-                    'Environment variable not found: {0}'.format(key))
+                "Environment variable not found: {0}".format(key)
+            )
         return result
 
 
 env = _Env()
```

### Comparing `project_runpy-1.0.1/pyproject.toml` & `project_runpy-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `project_runpy-1.0.1/test_project_runpy.py` & `project_runpy-1.1.0/test_project_runpy.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,175 +7,202 @@
     ColorizingStreamHandler,
     env,
     ImproperlyConfigured,
     ReadableSqlFilter,
 )
 
 
-VERY_LONG_STRING = '*' * 512
+VERY_LONG_STRING = "*" * 512
 
 
 class TestTimEnv(TestCase):
     def setUp(self):
-        self.key = '_tim_test'
+        self.key = "_tim_test"
 
     def tearDown(self):
         if self.key in os.environ:
             os.environ.pop(self.key)
-        if 'ENVIRONMENT' in os.environ:
-            os.environ.pop('ENVIRONMENT')
+        if "ENVIRONMENT" in os.environ:
+            os.environ.pop("ENVIRONMENT")
 
     def set_val(self, value):
         """Shortcut for setting the environment variable."""
         os.environ[self.key] = str(value)
 
     def test_gets_value(self):
-        self.set_val('foobar')
+        self.set_val("foobar")
         result = env.get(self.key)
-        self.assertEqual(result, 'foobar')
+        self.assertEqual(result, "foobar")
 
     def test_geting_empty_is_null_string(self):
         result = env.get(self.key)
-        self.assertIs(result, '')
+        self.assertIs(result, "")
 
     def test_reads_from_default(self):
-        result = env.get(self.key, 'qwerty')
-        self.assertEqual(result, 'qwerty')
+        result = env.get(self.key, "qwerty")
+        self.assertEqual(result, "qwerty")
 
     def test_gets_as_bool_if_default_is_bool(self):
-        self.set_val('1')
+        self.set_val("1")
         result = env.get(self.key, True)
         self.assertIs(result, True)
 
     def test_get_bool_coerced_version_true(self):
-        self.set_val('1')
-        result = env.get(self.key, 'True', type_func=bool)
+        self.set_val("1")
+        result = env.get(self.key, "True", type_func=bool)
         self.assertIs(result, True)
 
     def test_get_bool_coerced_version_false(self):
-        self.set_val('0')
-        result = env.get(self.key, 'True', type_func=bool)
+        self.set_val("0")
+        result = env.get(self.key, "True", type_func=bool)
         self.assertIs(result, False)
 
     def test_coerced_bool_no_default_no_value_is_true(self):
         result = env.get(self.key, type_func=bool)
         self.assertIs(result, True)
 
     def test_zero_gives_false(self):
-        self.set_val('0')
+        self.set_val("0")
         result = env.get(self.key, True)
         self.assertIs(result, False)
 
     def test_f_gives_false(self):
-        self.set_val('f')
+        self.set_val("f")
         result = env.get(self.key, True)
         self.assertIs(result, False)
 
     def test_false_gives_false(self):
-        self.set_val('fAlsE')
+        self.set_val("fAlsE")
         result = env.get(self.key, True)
         self.assertIs(result, False)
 
     def test_can_coerce_to_other_types(self):
-        self.set_val('20')
+        self.set_val("20")
         result = env.get(self.key, 10)
         self.assertIs(result, 20)
 
     def test_reads_from_environment_if_set(self):
-        result = env.get(self.key, 'qwerty', DEV='dvorak')
-        self.assertEqual(result, 'qwerty')
-        os.environ['ENVIRONMENT'] = 'DEV'
-        result = env.get(self.key, 'qwerty', DEV='dvorak')
-        self.assertEqual(result, 'dvorak')
-        del os.environ['ENVIRONMENT']  # teardown
+        result = env.get(self.key, "qwerty", DEV="dvorak")
+        self.assertEqual(result, "qwerty")
+        os.environ["ENVIRONMENT"] = "DEV"
+        result = env.get(self.key, "qwerty", DEV="dvorak")
+        self.assertEqual(result, "dvorak")
+        del os.environ["ENVIRONMENT"]  # teardown
 
     def test_no_default_unless_in_environment(self):
-        result = env.get(self.key, DEV='dvorak')
-        self.assertEqual(result, '')
-        os.environ['ENVIRONMENT'] = 'DEV'
-        result = env.get(self.key, DEV='dvorak')
-        self.assertEqual(result, 'dvorak')
-        del os.environ['ENVIRONMENT']  # teardown
+        result = env.get(self.key, DEV="dvorak")
+        self.assertEqual(result, "")
+        os.environ["ENVIRONMENT"] = "DEV"
+        result = env.get(self.key, DEV="dvorak")
+        self.assertEqual(result, "dvorak")
+        del os.environ["ENVIRONMENT"]  # teardown
 
     def test_no_default_unless_in_environment_and_bool(self):
         result = env.get(self.key, DEV=False)
-        self.assertEqual(result, '')
-        os.environ['ENVIRONMENT'] = 'DEV'
+        self.assertEqual(result, "")
+        os.environ["ENVIRONMENT"] = "DEV"
         result = env.get(self.key, DEV=False)
         self.assertEqual(result, False)
-        del os.environ['ENVIRONMENT']  # teardown
+        del os.environ["ENVIRONMENT"]  # teardown
 
     def test_require_raises_exception(self):
         with self.assertRaises(ImproperlyConfigured):
-            env.require('FOO')
+            env.require("FOO")
 
     def test_require_raises_exception_with_stupid_default(self):
         with self.assertRaises(ImproperlyConfigured):
-            env.require('FOO', default='')
+            env.require("FOO", default="")
 
         with self.assertRaises(ImproperlyConfigured):
-            env.require('FOO', default='')
+            env.require("FOO", default="")
 
     def test_require_acts_like_get(self):
-        os.environ['FOO'] = 'BAR'
-        self.assertEqual(env.require('FOO'), 'BAR')
-        del os.environ['FOO']  # teardown
+        os.environ["FOO"] = "BAR"
+        self.assertEqual(env.require("FOO"), "BAR")
+        del os.environ["FOO"]  # teardown
 
 
 class HeidiColorizingStreamHandler(TestCase):
     def test_it_can_be_added_to_logger(self):
-        logger = logging.getLogger('test')
+        logger = logging.getLogger("test")
         logger.addHandler(ColorizingStreamHandler())
+        with self.assertLogs(logger, logging.CRITICAL):
+            logger.critical("hello")
+
+    def test_it_handles_unicode_loggers(self):
+        logger = logging.getLogger("¡tést!")
+        logger.addHandler(ColorizingStreamHandler())
+        with self.assertLogs(logger, logging.CRITICAL):
+            logger.critical("héllø")
 
 
 class HeidiReadableSqlFilter(TestCase):
     def test_it_can_be_added_to_logger(self):
-        logger = logging.getLogger('foo.sql')
+        logger = logging.getLogger("foo.sql")
         logger.addHandler(logging.NullHandler())
         logger.addFilter(ReadableSqlFilter())
         with self.assertRaises(ValueError):
             # Sanity check
-            logger.warning('original msg %s %s %s')
-        logger.warning('original msg %s %s %s', '0.1', 'NOT SQL', ())
+            logger.warning("original msg %s %s %s")
+        logger.warning("original msg %s %s %s", "0.1", "NOT SQL", ())
 
     def test_filter_trivial_case(self):
         logging_filter = ReadableSqlFilter()
         record = mock.MagicMock(args=())
-        record = mock.MagicMock(args=(1.0, 'foo', ()))
+        record = mock.MagicMock(args=(1.0, "foo", ()))
         self.assertTrue(logging_filter.filter(record))
-        self.assertEqual('foo', record.args[1])
+        self.assertEqual("foo", record.args[1])
 
     def test_filter_runs_when_no_sql_exists(self):
         logging_filter = ReadableSqlFilter()
         record = mock.MagicMock(args=(0.07724404335021973, None, ()))
         self.assertTrue(logging_filter.filter(record))
 
     def test_filter_params_is_optional(self):
         logging_filter = ReadableSqlFilter()
         record = mock.MagicMock(args=())
-        record = mock.MagicMock(args=(1.0, 'foo'))
+        record = mock.MagicMock(args=(1.0, "foo"))
         self.assertTrue(logging_filter.filter(record))
-        self.assertEqual('foo', record.args[1])
+        self.assertEqual("foo", record.args[1])
 
     def test_filter_formats_select_from(self):
         logging_filter = ReadableSqlFilter()
-        record = mock.MagicMock(args=(1.0, '(yolo) SELECT foo FROM moo'))
+        record = mock.MagicMock(args=(1.0, "(yolo) SELECT foo FROM moo"))
         self.assertTrue(logging_filter.filter(record))
-        self.assertIn('SELECT...FROM moo', record.args[1])
+        self.assertIn("SELECT...FROM moo", record.args[1])
 
     def test_filter_formats_select_from_long(self):
         logging_filter = ReadableSqlFilter()
-        original_sql = '(yolo) SELECT {0} FROM moo'.format(VERY_LONG_STRING)
+        original_sql = "(yolo) SELECT {0} FROM moo".format(VERY_LONG_STRING)
         record = mock.MagicMock(args=(1.0, original_sql))
         self.assertTrue(logging_filter.filter(record))
-        self.assertIn('SELECT...FROM moo', record.args[1])
+        self.assertIn("SELECT...FROM moo", record.args[1])
 
     def test_filter_formats_ignores_select_without_from(self):
         logging_filter = ReadableSqlFilter()
-        original_sql = '(yolo) SELECT {0} moo'.format(VERY_LONG_STRING)
+        original_sql = "(yolo) SELECT {0} moo".format(VERY_LONG_STRING)
         record = mock.MagicMock(args=(1.0, original_sql))
         self.assertTrue(logging_filter.filter(record))
         self.assertEqual(original_sql, record.args[1])
 
+    def test_filter_collapses_multiline_sql(self):
+        long_sql = """
+            (0.002)
+                SELECT VERSION(),
+                       @@sql_mode,
+                       @@default_storage_engine,
+                       @@sql_auto_is_null,
+                       @@lower_case_table_names,
+                       CONVERT_TZ('2001-01-01 01:00:00', 'UTC', 'UTC') IS NOT NULL
+            ; args=None
+            """
+        logging_filter = ReadableSqlFilter()
+        record = mock.MagicMock(args=(1.0, long_sql))
+        self.assertIn("\n", record.args[1])
+
+        self.assertTrue(logging_filter.filter(record))
+
+        self.assertNotIn("\n", record.args[1])
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

