# Comparing `tmp/sampling-constraints-0.0.3.tar.gz` & `tmp/sampling-constraints-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sampling-constraints-0.0.3.tar", last modified: Sun May  7 22:10:08 2023, max compression
+gzip compressed data, was "sampling-constraints-0.0.4.tar", last modified: Sun May  7 22:29:26 2023, max compression
```

## Comparing `sampling-constraints-0.0.3.tar` & `sampling-constraints-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:10:08.191511 sampling-constraints-0.0.3/
--rw-r--r--   0 isaac     (1000) isaac     (1000)     1067 2023-05-07 21:44:12.000000 sampling-constraints-0.0.3/LICENSE
--rw-r--r--   0 isaac     (1000) isaac     (1000)      402 2023-05-07 22:10:08.191511 sampling-constraints-0.0.3/PKG-INFO
--rw-r--r--   0 isaac     (1000) isaac     (1000)       57 2023-05-07 20:35:15.000000 sampling-constraints-0.0.3/README.md
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:10:08.191511 sampling-constraints-0.0.3/scs/
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:10:08.191511 sampling-constraints-0.0.3/scs/constraint/
--rw-r--r--   0 isaac     (1000) isaac     (1000)      582 2023-05-07 20:17:09.000000 sampling-constraints-0.0.3/scs/constraint/__init__.py
--rw-r--r--   0 isaac     (1000) isaac     (1000)      162 2023-05-07 21:01:04.000000 sampling-constraints-0.0.3/scs/constraint/json.py
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:10:08.191511 sampling-constraints-0.0.3/scs/incremental_parse/
--rw-r--r--   0 isaac     (1000) isaac     (1000)     1240 2023-05-07 21:11:34.000000 sampling-constraints-0.0.3/scs/incremental_parse/__init__.py
--rw-r--r--   0 isaac     (1000) isaac     (1000)    11185 2023-05-07 21:21:55.000000 sampling-constraints-0.0.3/scs/incremental_parse/json.py
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:10:08.191511 sampling-constraints-0.0.3/scs/sampling_constraints.egg-info/
--rw-r--r--   0 isaac     (1000) isaac     (1000)      402 2023-05-07 22:10:08.000000 sampling-constraints-0.0.3/scs/sampling_constraints.egg-info/PKG-INFO
--rw-r--r--   0 isaac     (1000) isaac     (1000)      351 2023-05-07 22:10:08.000000 sampling-constraints-0.0.3/scs/sampling_constraints.egg-info/SOURCES.txt
--rw-r--r--   0 isaac     (1000) isaac     (1000)        1 2023-05-07 22:10:08.000000 sampling-constraints-0.0.3/scs/sampling_constraints.egg-info/dependency_links.txt
--rw-r--r--   0 isaac     (1000) isaac     (1000)        1 2023-05-07 22:10:08.000000 sampling-constraints-0.0.3/scs/sampling_constraints.egg-info/top_level.txt
--rw-r--r--   0 isaac     (1000) isaac     (1000)       38 2023-05-07 22:10:08.191511 sampling-constraints-0.0.3/setup.cfg
--rw-r--r--   0 isaac     (1000) isaac     (1000)      530 2023-05-07 22:09:54.000000 sampling-constraints-0.0.3/setup.py
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:10:08.191511 sampling-constraints-0.0.3/tests/
--rw-r--r--   0 isaac     (1000) isaac     (1000)     4413 2023-05-07 21:17:28.000000 sampling-constraints-0.0.3/tests/test_json.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:29:26.963963 sampling-constraints-0.0.4/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)     1067 2023-05-07 21:44:12.000000 sampling-constraints-0.0.4/LICENSE
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      402 2023-05-07 22:29:26.963963 sampling-constraints-0.0.4/PKG-INFO
+-rw-r--r--   0 isaac     (1000) isaac     (1000)       57 2023-05-07 20:35:15.000000 sampling-constraints-0.0.4/README.md
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:29:26.953963 sampling-constraints-0.0.4/scs/
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:29:26.963963 sampling-constraints-0.0.4/scs/constraint/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      582 2023-05-07 20:17:09.000000 sampling-constraints-0.0.4/scs/constraint/__init__.py
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      162 2023-05-07 21:01:04.000000 sampling-constraints-0.0.4/scs/constraint/json.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:29:26.963963 sampling-constraints-0.0.4/scs/incremental_parse/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)     1240 2023-05-07 21:11:34.000000 sampling-constraints-0.0.4/scs/incremental_parse/__init__.py
+-rw-r--r--   0 isaac     (1000) isaac     (1000)    11411 2023-05-07 22:27:06.000000 sampling-constraints-0.0.4/scs/incremental_parse/json.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:29:26.963963 sampling-constraints-0.0.4/scs/sampling_constraints.egg-info/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      402 2023-05-07 22:29:26.000000 sampling-constraints-0.0.4/scs/sampling_constraints.egg-info/PKG-INFO
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      351 2023-05-07 22:29:26.000000 sampling-constraints-0.0.4/scs/sampling_constraints.egg-info/SOURCES.txt
+-rw-r--r--   0 isaac     (1000) isaac     (1000)        1 2023-05-07 22:29:26.000000 sampling-constraints-0.0.4/scs/sampling_constraints.egg-info/dependency_links.txt
+-rw-r--r--   0 isaac     (1000) isaac     (1000)        1 2023-05-07 22:29:26.000000 sampling-constraints-0.0.4/scs/sampling_constraints.egg-info/top_level.txt
+-rw-r--r--   0 isaac     (1000) isaac     (1000)       38 2023-05-07 22:29:26.963963 sampling-constraints-0.0.4/setup.cfg
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      530 2023-05-07 22:29:22.000000 sampling-constraints-0.0.4/setup.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-07 22:29:26.963963 sampling-constraints-0.0.4/tests/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)     4660 2023-05-07 22:28:41.000000 sampling-constraints-0.0.4/tests/test_json.py
```

### Comparing `sampling-constraints-0.0.3/LICENSE` & `sampling-constraints-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sampling-constraints-0.0.3/scs/constraint/__init__.py` & `sampling-constraints-0.0.4/scs/constraint/__init__.py`

 * *Files identical despite different names*

### Comparing `sampling-constraints-0.0.3/scs/incremental_parse/__init__.py` & `sampling-constraints-0.0.4/scs/incremental_parse/__init__.py`

 * *Files identical despite different names*

### Comparing `sampling-constraints-0.0.3/scs/incremental_parse/json.py` & `sampling-constraints-0.0.4/scs/incremental_parse/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from enum import Enum
 from typing import Dict, Union, Optional
 from copy import deepcopy
 
+from scs.incremental_parse import IncrementalParser
+
 from . import IncrementalParser, ParseFailure, SpecialToken
 
 
 class JSONParser(IncrementalParser):
     
     def __init__(self):
         super().__init__()
         self._subparser = None
         self._complete = False
+
+    def _copy_from(self, other: "JSONParser"):
+        super()._copy_from(other)
+        self._subparser = other._subparser.copy()
+        self._complete = other._complete
     
     def _append(self, char: Union[str, SpecialToken]) -> bool:
         if self._subparser is None:
             if char == SpecialChar.OPEN_ARRAY.value:
                 self._subparser = ArrayParser()
             elif char == SpecialChar.OPEN_OBJECT.value:
                 self._subparser = ObjectParser()
```

### Comparing `sampling-constraints-0.0.3/setup.py` & `sampling-constraints-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='sampling-constraints',
-    version='0.0.3',
+    version='0.0.4',
     url='https://github.com/IsaacRe/Syntactically-Constrained-Sampling',
     description='Library of incremental parsers used to force syntax constraints on next-token predictions during language model generation',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license="MIT",
     packages=find_packages("scs", include=["scs", "scs.*"]),
     package_dir={"": "scs"},
```

### Comparing `sampling-constraints-0.0.3/tests/test_json.py` & `sampling-constraints-0.0.4/tests/test_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,17 +110,24 @@
     def test_update_parser(self):
         test_data = '{"name": "John Smith", "ag', 'e": 35, "city": "New York"}'
         constraint = valid_json()
         constraint.update_parser(test_data[0])
         self.assertEqual(constraint.parser.get_parsed(), test_data[0])
 
     def test_check_next(self):
-        test_data = '{"name": "John Smith", "age": 35, "city": "New York"}'
+        test_data = '{"name": "John Smith", "ag', 'e": 35, "city": "New York"}'
         constraint = valid_json()
         constraint.update_parser(test_data[0])
 
-        constraint.check_next(test_data[1])
+        self.assertTrue(constraint.check_next(test_data[1]))
         self.assertEqual(constraint.parser.get_parsed(), test_data[0])
 
+    def test_check_next_with_extra(self):
+        test_data = '{}', 'extra data'
+        constraint = valid_json()
+        constraint.update_parser(test_data[0])
+
+        self.assertFalse(constraint.check_next(test_data[1]))
+
 
 if __name__ == '__main__':
     unittest.main()
```

