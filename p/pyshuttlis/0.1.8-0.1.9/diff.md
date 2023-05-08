# Comparing `tmp/pyshuttlis-0.1.8.tar.gz` & `tmp/pyshuttlis-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyshuttlis-0.1.8.tar", last modified: Tue Jan  8 09:20:49 2019, max compression
+gzip compressed data, was "dist/pyshuttlis-0.1.9.tar", last modified: Mon Feb  4 14:13:58 2019, max compression
```

## Comparing `pyshuttlis-0.1.8.tar` & `pyshuttlis-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 sherub     (502) staff       (20)        0 2019-01-08 09:20:49.000000 pyshuttlis-0.1.8/
--rw-r--r--   0 sherub     (502) staff       (20)      323 2019-01-08 09:20:49.000000 pyshuttlis-0.1.8/PKG-INFO
-drwxr-xr-x   0 sherub     (502) staff       (20)        0 2019-01-08 09:20:49.000000 pyshuttlis-0.1.8/pyshuttlis.egg-info/
--rw-r--r--   0 sherub     (502) staff       (20)      323 2019-01-08 09:20:49.000000 pyshuttlis-0.1.8/pyshuttlis.egg-info/PKG-INFO
--rw-r--r--   0 sherub     (502) staff       (20)      634 2019-01-08 09:20:49.000000 pyshuttlis-0.1.8/pyshuttlis.egg-info/SOURCES.txt
--rw-r--r--   0 sherub     (502) staff       (20)       79 2019-01-08 09:20:49.000000 pyshuttlis-0.1.8/pyshuttlis.egg-info/requires.txt
--rw-r--r--   0 sherub     (502) staff       (20)       15 2019-01-08 09:20:49.000000 pyshuttlis-0.1.8/pyshuttlis.egg-info/top_level.txt
--rw-r--r--   0 sherub     (502) staff       (20)        1 2019-01-08 09:20:49.000000 pyshuttlis-0.1.8/pyshuttlis.egg-info/dependency_links.txt
-drwxr-xr-x   0 sherub     (502) staff       (20)        0 2019-01-08 09:20:49.000000 pyshuttlis-0.1.8/shuttlis/
--rw-r--r--   0 sherub     (502) staff       (20)      861 2019-01-08 09:19:57.000000 pyshuttlis-0.1.8/shuttlis/geography.py
--rw-r--r--   0 sherub     (502) staff       (20)        0 2018-11-30 13:48:20.000000 pyshuttlis-0.1.8/shuttlis/__init__.py
-drwxr-xr-x   0 sherub     (502) staff       (20)        0 2019-01-08 09:20:49.000000 pyshuttlis-0.1.8/shuttlis/time/
--rw-r--r--   0 sherub     (502) staff       (20)       92 2019-01-07 11:26:20.000000 pyshuttlis-0.1.8/shuttlis/time/__init__.py
--rw-r--r--   0 sherub     (502) staff       (20)      965 2019-01-08 09:19:57.000000 pyshuttlis-0.1.8/shuttlis/time/weekday.py
--rw-r--r--   0 sherub     (502) staff       (20)     2190 2019-01-07 11:26:20.000000 pyshuttlis-0.1.8/shuttlis/time/military_time.py
--rw-r--r--   0 sherub     (502) staff       (20)      640 2018-11-27 14:05:39.000000 pyshuttlis-0.1.8/shuttlis/utils.py
-drwxr-xr-x   0 sherub     (502) staff       (20)        0 2019-01-08 09:20:49.000000 pyshuttlis-0.1.8/shuttlis/log/
--rw-r--r--   0 sherub     (502) staff       (20)     1460 2019-01-07 11:26:20.000000 pyshuttlis-0.1.8/shuttlis/log/formatters.py
--rw-r--r--   0 sherub     (502) staff       (20)     1230 2019-01-07 11:26:20.000000 pyshuttlis-0.1.8/shuttlis/log/log.py
--rw-r--r--   0 sherub     (502) staff       (20)       49 2019-01-07 11:26:20.000000 pyshuttlis-0.1.8/shuttlis/log/__init__.py
--rw-r--r--   0 sherub     (502) staff       (20)      149 2019-01-07 11:26:20.000000 pyshuttlis-0.1.8/shuttlis/log/utils.py
--rw-r--r--   0 sherub     (502) staff       (20)      579 2019-01-07 11:26:20.000000 pyshuttlis-0.1.8/shuttlis/log/filters.py
--rw-r--r--   0 sherub     (502) staff       (20)      707 2019-01-06 20:07:29.000000 pyshuttlis-0.1.8/shuttlis/pagination.py
--rw-r--r--   0 sherub     (502) staff       (20)      769 2019-01-06 20:07:29.000000 pyshuttlis-0.1.8/shuttlis/serialization.py
-drwxr-xr-x   0 sherub     (502) staff       (20)        0 2019-01-08 09:20:49.000000 pyshuttlis-0.1.8/tests/
--rw-r--r--   0 sherub     (502) staff       (20)     1039 2019-01-06 20:07:44.000000 pyshuttlis-0.1.8/tests/test_utils.py
--rw-r--r--   0 sherub     (502) staff       (20)     3244 2019-01-08 09:19:57.000000 pyshuttlis-0.1.8/tests/test_time.py
--rw-r--r--   0 sherub     (502) staff       (20)        0 2018-11-30 13:44:31.000000 pyshuttlis-0.1.8/tests/__init__.py
--rw-r--r--   0 sherub     (502) staff       (20)      307 2019-01-07 11:26:20.000000 pyshuttlis-0.1.8/tests/test_log.py
--rw-r--r--   0 sherub     (502) staff       (20)      736 2019-01-08 09:19:57.000000 pyshuttlis-0.1.8/tests/test_geography.py
--rw-r--r--   0 sherub     (502) staff       (20)      387 2019-01-06 20:06:06.000000 pyshuttlis-0.1.8/tests/test_serialization.py
--rw-r--r--   0 sherub     (502) staff       (20)        8 2018-11-27 12:56:10.000000 pyshuttlis-0.1.8/README.md
--rw-r--r--   0 sherub     (502) staff       (20)      525 2019-01-08 09:20:07.000000 pyshuttlis-0.1.8/setup.py
--rw-r--r--   0 sherub     (502) staff       (20)      243 2019-01-08 09:20:49.000000 pyshuttlis-0.1.8/setup.cfg
+drwxr-xr-x   0 sherub     (502) staff       (20)        0 2019-02-04 14:13:58.000000 pyshuttlis-0.1.9/
+-rw-r--r--   0 sherub     (502) staff       (20)      323 2019-02-04 14:13:58.000000 pyshuttlis-0.1.9/PKG-INFO
+drwxr-xr-x   0 sherub     (502) staff       (20)        0 2019-02-04 14:13:58.000000 pyshuttlis-0.1.9/pyshuttlis.egg-info/
+-rw-r--r--   0 sherub     (502) staff       (20)      323 2019-02-04 14:13:58.000000 pyshuttlis-0.1.9/pyshuttlis.egg-info/PKG-INFO
+-rw-r--r--   0 sherub     (502) staff       (20)      682 2019-02-04 14:13:58.000000 pyshuttlis-0.1.9/pyshuttlis.egg-info/SOURCES.txt
+-rw-r--r--   0 sherub     (502) staff       (20)       90 2019-02-04 14:13:58.000000 pyshuttlis-0.1.9/pyshuttlis.egg-info/requires.txt
+-rw-r--r--   0 sherub     (502) staff       (20)       15 2019-02-04 14:13:58.000000 pyshuttlis-0.1.9/pyshuttlis.egg-info/top_level.txt
+-rw-r--r--   0 sherub     (502) staff       (20)        1 2019-02-04 14:13:58.000000 pyshuttlis-0.1.9/pyshuttlis.egg-info/dependency_links.txt
+drwxr-xr-x   0 sherub     (502) staff       (20)        0 2019-02-04 14:13:58.000000 pyshuttlis-0.1.9/shuttlis/
+-rw-r--r--   0 sherub     (502) staff       (20)      861 2019-02-04 14:10:26.000000 pyshuttlis-0.1.9/shuttlis/geography.py
+-rw-r--r--   0 sherub     (502) staff       (20)     1538 2019-02-04 14:12:08.000000 pyshuttlis-0.1.9/shuttlis/validators.py
+-rw-r--r--   0 sherub     (502) staff       (20)        0 2018-11-30 13:48:20.000000 pyshuttlis-0.1.9/shuttlis/__init__.py
+drwxr-xr-x   0 sherub     (502) staff       (20)        0 2019-02-04 14:13:58.000000 pyshuttlis-0.1.9/shuttlis/time/
+-rw-r--r--   0 sherub     (502) staff       (20)       92 2019-01-07 11:26:20.000000 pyshuttlis-0.1.9/shuttlis/time/__init__.py
+-rw-r--r--   0 sherub     (502) staff       (20)      965 2019-02-04 13:25:03.000000 pyshuttlis-0.1.9/shuttlis/time/weekday.py
+-rw-r--r--   0 sherub     (502) staff       (20)     2190 2019-02-04 13:25:03.000000 pyshuttlis-0.1.9/shuttlis/time/military_time.py
+-rw-r--r--   0 sherub     (502) staff       (20)      855 2019-02-04 13:22:36.000000 pyshuttlis-0.1.9/shuttlis/utils.py
+drwxr-xr-x   0 sherub     (502) staff       (20)        0 2019-02-04 14:13:58.000000 pyshuttlis-0.1.9/shuttlis/log/
+-rw-r--r--   0 sherub     (502) staff       (20)     1460 2019-02-04 13:25:02.000000 pyshuttlis-0.1.9/shuttlis/log/formatters.py
+-rw-r--r--   0 sherub     (502) staff       (20)     1230 2019-02-04 13:25:02.000000 pyshuttlis-0.1.9/shuttlis/log/log.py
+-rw-r--r--   0 sherub     (502) staff       (20)       49 2019-01-07 11:26:20.000000 pyshuttlis-0.1.9/shuttlis/log/__init__.py
+-rw-r--r--   0 sherub     (502) staff       (20)      149 2019-01-07 11:26:20.000000 pyshuttlis-0.1.9/shuttlis/log/utils.py
+-rw-r--r--   0 sherub     (502) staff       (20)      579 2019-02-04 13:25:02.000000 pyshuttlis-0.1.9/shuttlis/log/filters.py
+-rw-r--r--   0 sherub     (502) staff       (20)      707 2019-02-04 13:25:02.000000 pyshuttlis-0.1.9/shuttlis/pagination.py
+-rw-r--r--   0 sherub     (502) staff       (20)      769 2019-02-04 13:25:03.000000 pyshuttlis-0.1.9/shuttlis/serialization.py
+drwxr-xr-x   0 sherub     (502) staff       (20)        0 2019-02-04 14:13:58.000000 pyshuttlis-0.1.9/tests/
+-rw-r--r--   0 sherub     (502) staff       (20)     1404 2019-02-04 13:27:57.000000 pyshuttlis-0.1.9/tests/test_utils.py
+-rw-r--r--   0 sherub     (502) staff       (20)     3244 2019-01-08 09:19:57.000000 pyshuttlis-0.1.9/tests/test_time.py
+-rw-r--r--   0 sherub     (502) staff       (20)        0 2018-11-30 13:44:31.000000 pyshuttlis-0.1.9/tests/__init__.py
+-rw-r--r--   0 sherub     (502) staff       (20)      309 2019-02-04 13:25:03.000000 pyshuttlis-0.1.9/tests/test_log.py
+-rw-r--r--   0 sherub     (502) staff       (20)      736 2019-01-08 09:19:57.000000 pyshuttlis-0.1.9/tests/test_geography.py
+-rw-r--r--   0 sherub     (502) staff       (20)     1791 2019-02-04 14:12:08.000000 pyshuttlis-0.1.9/tests/test_validators.py
+-rw-r--r--   0 sherub     (502) staff       (20)      387 2019-02-04 13:25:03.000000 pyshuttlis-0.1.9/tests/test_serialization.py
+-rw-r--r--   0 sherub     (502) staff       (20)        8 2018-11-27 12:56:10.000000 pyshuttlis-0.1.9/README.md
+-rw-r--r--   0 sherub     (502) staff       (20)      539 2019-02-04 14:12:19.000000 pyshuttlis-0.1.9/setup.py
+-rw-r--r--   0 sherub     (502) staff       (20)      243 2019-02-04 14:13:58.000000 pyshuttlis-0.1.9/setup.cfg
```

### Comparing `pyshuttlis-0.1.8/pyshuttlis.egg-info/SOURCES.txt` & `pyshuttlis-0.1.9/pyshuttlis.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 pyshuttlis.egg-info/requires.txt
 pyshuttlis.egg-info/top_level.txt
 shuttlis/__init__.py
 shuttlis/geography.py
 shuttlis/pagination.py
 shuttlis/serialization.py
 shuttlis/utils.py
+shuttlis/validators.py
 shuttlis/log/__init__.py
 shuttlis/log/filters.py
 shuttlis/log/formatters.py
 shuttlis/log/log.py
 shuttlis/log/utils.py
 shuttlis/time/__init__.py
 shuttlis/time/military_time.py
 shuttlis/time/weekday.py
 tests/__init__.py
 tests/test_geography.py
 tests/test_log.py
 tests/test_serialization.py
 tests/test_time.py
-tests/test_utils.py
+tests/test_utils.py
+tests/test_validators.py
```

### Comparing `pyshuttlis-0.1.8/shuttlis/geography.py` & `pyshuttlis-0.1.9/shuttlis/geography.py`

 * *Files identical despite different names*

### Comparing `pyshuttlis-0.1.8/shuttlis/time/weekday.py` & `pyshuttlis-0.1.9/shuttlis/time/weekday.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from datetime import datetime, date
 from enum import Enum
 from functools import total_ordering
 
 
 @total_ordering
 class WeekDay(Enum):
-    MONDAY = 'MONDAY'
-    TUESDAY = 'TUESDAY'
-    WEDNESDAY = 'WEDNESDAY'
-    THURSDAY = 'THURSDAY'
-    FRIDAY = 'FRIDAY'
-    SATURDAY = 'SATURDAY'
-    SUNDAY = 'SUNDAY'
+    MONDAY = "MONDAY"
+    TUESDAY = "TUESDAY"
+    WEDNESDAY = "WEDNESDAY"
+    THURSDAY = "THURSDAY"
+    FRIDAY = "FRIDAY"
+    SATURDAY = "SATURDAY"
+    SUNDAY = "SUNDAY"
 
     @classmethod
     def extract_from_datetime(cls, dt: datetime):
         return cls[calendar.day_name[dt.weekday()].upper()]
 
     @classmethod
     def extract_from_date(cls, dt: date):
```

### Comparing `pyshuttlis-0.1.8/shuttlis/time/military_time.py` & `pyshuttlis-0.1.9/shuttlis/time/military_time.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,18 @@
     def to_time(self, tzinfo) -> time:
         return time(hour=self.hr, minute=self.min, tzinfo=tzinfo)
 
     def __eq__(self, other):
         return (self.hr, self.min, self.tz.zone) == (other.hr, other.min, other.tz.zone)
 
     def __str__(self):
-        return f'{self.hr:02}{self.min:02}:{self.tz.zone}'
+        return f"{self.hr:02}{self.min:02}:{self.tz.zone}"
 
     def __repr__(self):
-        return f'<MilitaryTime: {str(self)}>'
+        return f"<MilitaryTime: {str(self)}>"
 
     def __add__(self, other: TimeDelta):
         min = (self.min + other.min) % 60
         additional_hrs = (self.min + other.min) // 60
         hr = (self.hr + other.hr + additional_hrs) % 24
         return MilitaryTime.from_hr_min(hr, min, self.tz)
 
@@ -71,11 +71,11 @@
 
     def __hash__(self):
         return hash((self.hr, self.min))
 
     def __lt__(self, other):
         if self.tz.zone != other.tz.zone:
             raise TimezoneMismatch(
-                f'Recieved different timezones as {self.tz.zone} and {other.tz.zone}'
+                f"Recieved different timezones as {self.tz.zone} and {other.tz.zone}"
             )
 
         return (self.hr * 100, self.min) < (other.hr * 100, other.min)
```

### Comparing `pyshuttlis-0.1.8/shuttlis/utils.py` & `pyshuttlis-0.1.9/shuttlis/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,21 +2,27 @@
 
 from typing import List, Callable, Any, Optional, Dict
 
 
 def one_or_none(lizt: List[Any], key: Callable[[Any], bool]) -> Optional[Any]:
     gen = (x for x in lizt if key(x))
     elm = next(gen, None)
-    if not None:
+    if elm:
         assert next(gen, None) is None
     return elm
 
 
 def one(lizt: List[Any], key: Callable[[Any], bool]) -> Any:
     maybe_elm = one_or_none(lizt, key)
     assert maybe_elm is not None
     return maybe_elm
 
 
 def group_by(lizt: List[Any], key: Callable[[Any], Any]) -> Dict[Any, List[Any]]:
     sorted_list = sorted(lizt, key=key)
     return {k: list(v) for k, v in it.groupby(sorted_list, key)}
+
+
+def id_map(lizt: List[Any], key: Callable[[Any], Any]) -> Dict[Any, Any]:
+    list_map = group_by(lizt, key=key)
+    assert all(len(v) == 1 for v in list_map.values())
+    return {k: v[0] for k, v in list_map.items()}
```

### Comparing `pyshuttlis-0.1.8/shuttlis/log/formatters.py` & `pyshuttlis-0.1.9/shuttlis/log/formatters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 import json
 import logging
 
 from .utils import _sanitize_stacktrace_for_json_fields
 
 
 default_formatter = logging.Formatter(
-    '[%(levelname)s -- %(asctime)s] :: (%(module)s.%(funcName)s) :: %(message)s',
+    "[%(levelname)s -- %(asctime)s] :: (%(module)s.%(funcName)s) :: %(message)s",
     "%H:%M:%S",
 )
 
 
 class JSONFormatter(logging.Formatter):
     def format(self, record: logging.LogRecord) -> str:
         json_dict = {}
 
         if record.exc_info:
-            json_dict['stack_trace'] = _sanitize_stacktrace_for_json_fields(
+            json_dict["stack_trace"] = _sanitize_stacktrace_for_json_fields(
                 *record.exc_info
             )
 
             # mark exception info as none to consume the exception here and stop propogation
             # where it might get logged to sys.stderr.
             # If we need to reraise it we can log it as an exception on the root logger
             record.exc_info = None
 
         json_dict.update(record.__dict__)
 
         # Already replaced this with 'stack_trace', no longer needed
-        assert json_dict['exc_info'] is None
-        del json_dict['exc_info']
+        assert json_dict["exc_info"] is None
+        del json_dict["exc_info"]
 
         # We don't need these 2 fields as message field has msg % args now
-        json_dict['message'] = record.getMessage()
-        del json_dict['msg']
-        del json_dict['args']
+        json_dict["message"] = record.getMessage()
+        del json_dict["msg"]
+        del json_dict["args"]
 
-        json_dict['level'] = json_dict['levelname']
-        del json_dict['levelname']
+        json_dict["level"] = json_dict["levelname"]
+        del json_dict["levelname"]
 
         try:
             return json.dumps(json_dict)
         except (TypeError, OverflowError):
             return json.dumps(
                 {"message": "An unrecoverable exception occured while logging"}
             )
```

### Comparing `pyshuttlis-0.1.8/shuttlis/log/log.py` & `pyshuttlis-0.1.9/shuttlis/log/log.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 ):
     exception_string = _sanitize_stacktrace_for_json_fields(type, exc, traceback)
     # raise to root logger where it will be consumed by the formatter attached to our handler
     logging.getLogger().error(exception_string)
 
 
 def configure_logging(
-    logger_name: str, level: str, log_format: str = 'json'
+    logger_name: str, level: str, log_format: str = "json"
 ) -> logging.Logger:
     logger = logging.getLogger()
     logger.addHandler(logging.StreamHandler())
     logger.setLevel(level)
 
     assert logger.hasHandlers()
     for handler in logger.handlers:
-        if log_format != 'console':
+        if log_format != "console":
             handler.setFormatter(JSONFormatter())
         else:
             handler.setFormatter(default_formatter)
         handler.addFilter(MaskPasswordsInLogs())
-        handler.addFilter(AddContextualFieldFilter('service', logger_name))
+        handler.addFilter(AddContextualFieldFilter("service", logger_name))
 
     sys.excepthook = _uncaught_exception_logger
 
     return logging.getLogger(logger_name)
```

### Comparing `pyshuttlis-0.1.8/shuttlis/log/filters.py` & `pyshuttlis-0.1.9/shuttlis/log/filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,10 +9,10 @@
     def filter(self, record: logging.LogRecord) -> bool:
         record.__dict__[self._field_name] = self._field_value
         return True
 
 
 class MaskPasswordsInLogs(logging.Filter):
     def filter(self, record: logging.LogRecord) -> bool:
-        if record.__dict__.get('password') is not None:
-            record.__dict__['password'] = "******"
+        if record.__dict__.get("password") is not None:
+            record.__dict__["password"] = "******"
         return True
```

### Comparing `pyshuttlis-0.1.8/shuttlis/serialization.py` & `pyshuttlis-0.1.9/shuttlis/serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 primitive = (int, float, str, bool)
 
 
 def is_primitive(thing):
     return isinstance(thing, primitive)
 
 
-def serialize(obj, decoder='utf8'):
+def serialize(obj, decoder="utf8"):
     if obj is None:
         return None
     if is_primitive(obj):
         return obj
     if isinstance(obj, Enum):
         return obj.value
     if isinstance(obj, datetime):
```

### Comparing `pyshuttlis-0.1.8/tests/test_utils.py` & `pyshuttlis-0.1.9/tests/test_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,52 @@
 import pytest
 
-from shuttlis.utils import one_or_none, one
+from shuttlis.utils import one_or_none, one, id_map
 
 
-@pytest.mark.parametrize('lizt,key,expected', [
-    ([1, 2, 3], lambda x: x == 2, 2),
-    (['a', 'b', 'c'], lambda x: x == 'c', 'c'),
-    (['a', 'b', 'c'], lambda x: x == 'd', None),
-])
+@pytest.mark.parametrize(
+    "lizt,key,expected",
+    [
+        ([1, 2, 3], lambda x: x == 2, 2),
+        (["a", "b", "c"], lambda x: x == "c", "c"),
+        (["a", "b", "c"], lambda x: x == "d", None),
+    ],
+)
 def test_one_or_none(lizt, key, expected):
     actual = one_or_none(lizt, key)
     assert expected == actual
 
 
 def test_one_or_none_raises_assertion_error_if_more_than_one_match():
     with pytest.raises(AssertionError):
         one_or_none([1, 2, 2, 2], lambda x: x == 2)
 
 
-@pytest.mark.parametrize('lizt,key,expected', [
-    ([1, 2, 3], lambda x: x == 2, 2),
-    (['a', 'b', 'c'], lambda x: x == 'c', 'c'),
-])
+@pytest.mark.parametrize(
+    "lizt,key,expected",
+    [([1, 2, 3], lambda x: x == 2, 2), (["a", "b", "c"], lambda x: x == "c", "c")],
+)
 def test_one(lizt, key, expected):
     actual = one(lizt, key)
     assert expected == actual
 
 
 def test_one_raises_assertion_error_if_more_than_one_match():
     with pytest.raises(AssertionError):
         one([1, 2, 2, 2], lambda x: x == 2)
 
 
 def test_one_raises_assertion_error_if_none_match():
     with pytest.raises(AssertionError):
         one([1, 2, 2, 2], lambda x: x == 4)
+
+
+@pytest.mark.parametrize(
+    "lizt,key,expected", [(["a", "ab", "abc"], len, {1: "a", 2: "ab", 3: "abc"})]
+)
+def test_id_map(lizt, key, expected):
+    assert expected == id_map(lizt, key=key)
+
+
+def test_id_map_with_multiple_items_raises_error():
+    with pytest.raises(AssertionError):
+        id_map(["a", "b", "c"], key=len)
```

### Comparing `pyshuttlis-0.1.8/tests/test_time.py` & `pyshuttlis-0.1.9/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `pyshuttlis-0.1.8/tests/test_geography.py` & `pyshuttlis-0.1.9/tests/test_geography.py`

 * *Files identical despite different names*

### Comparing `pyshuttlis-0.1.8/setup.py` & `pyshuttlis-0.1.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='pyshuttlis',
-    version='0.1.8',
-    description='Utilities',
-    url='https://github.com/shuttl-tech/pyshuttlis',
-    author='Shuttl',
-    author_email='sherub.thakur@shuttl.com',
-    license='MIT',
+    name="pyshuttlis",
+    version="0.1.9",
+    description="Utilities",
+    url="https://github.com/shuttl-tech/pyshuttlis",
+    author="Shuttl",
+    author_email="sherub.thakur@shuttl.com",
+    license="MIT",
     packages=find_packages(),
     classifiers=["Programming Language :: Python :: 3.7"],
-    install_requires=['shapely', 'pytz'],
+    install_requires=["shapely", "pytz", "voluptuous"],
     extras_require={
-        'test': ['pytest', 'pytest-runner', 'pytest-cov', 'pytest-pep8'],
-        'dev': ['flake8'],
+        "test": ["pytest", "pytest-runner", "pytest-cov", "pytest-pep8"],
+        "dev": ["flake8"],
     },
 )
```

