# Comparing `tmp/py_fumen_py-0.0.4.tar.gz` & `tmp/py_fumen_py-0.0.5.tar.gz`

## Comparing `py_fumen_py-0.0.4.tar` & `py_fumen_py-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 py_fumen_py-0.0.4/src/py_fumen_py/__init__.py
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 py_fumen_py-0.0.4/src/py_fumen_py/action.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 py_fumen_py-0.0.4/src/py_fumen_py/comment.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 py_fumen_py-0.0.4/src/py_fumen_py/constant.py
--rw-r--r--   0        0        0     6991 2020-02-02 00:00:00.000000 py_fumen_py-0.0.4/src/py_fumen_py/field.py
--rw-r--r--   0        0        0     6579 2020-02-02 00:00:00.000000 py_fumen_py-0.0.4/src/py_fumen_py/fumen_buffer.py
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 py_fumen_py-0.0.4/src/py_fumen_py/fumen_codec.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 py_fumen_py-0.0.4/src/py_fumen_py/js_escape.py
--rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 py_fumen_py-0.0.4/src/py_fumen_py/operation.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 py_fumen_py-0.0.4/src/py_fumen_py/page.py
--rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 py_fumen_py-0.0.4/src/py_fumen_py/quiz.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 py_fumen_py-0.0.4/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 py_fumen_py-0.0.4/LICENSE
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 py_fumen_py-0.0.4/README.md
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 py_fumen_py-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 py_fumen_py-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 py_fumen_py-0.0.5/src/py_fumen_py/__init__.py
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 py_fumen_py-0.0.5/src/py_fumen_py/action.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 py_fumen_py-0.0.5/src/py_fumen_py/comment.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 py_fumen_py-0.0.5/src/py_fumen_py/constant.py
+-rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 py_fumen_py-0.0.5/src/py_fumen_py/field.py
+-rw-r--r--   0        0        0     8437 2020-02-02 00:00:00.000000 py_fumen_py-0.0.5/src/py_fumen_py/fumen_buffer.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 py_fumen_py-0.0.5/src/py_fumen_py/fumen_codec.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 py_fumen_py-0.0.5/src/py_fumen_py/js_escape.py
+-rw-r--r--   0        0        0     6723 2020-02-02 00:00:00.000000 py_fumen_py-0.0.5/src/py_fumen_py/operation.py
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 py_fumen_py-0.0.5/src/py_fumen_py/page.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 py_fumen_py-0.0.5/src/py_fumen_py/quiz.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 py_fumen_py-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 py_fumen_py-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 py_fumen_py-0.0.5/README.md
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 py_fumen_py-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 py_fumen_py-0.0.5/PKG-INFO
```

### Comparing `py_fumen_py-0.0.4/src/py_fumen_py/action.py` & `py_fumen_py-0.0.5/src/py_fumen_py/action.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,22 +3,32 @@
 from dataclasses import dataclass
 
 from .constant import FieldConstants
 from .operation import Mino, Rotation, Operation
 
 @dataclass
 class Action():
+    """A dataclass for storing encoded Fumen page flags and field changes.
+    Keyword arguments:
+    operation: the operation applied to the field.
+    rise: if the garbage in the field rises.
+    mirror: if the field is mirrored.
+    colorize: if the page is using SRS coloring. (only valid on page 0.)
+    lock: if the operation is locked and filled field lines are cleared.
+    """
     operation: Operation
     rise: bool
     mirror: bool
     colorize: bool
     comment: bool
     lock: bool
 
 class ActionCodec() :
+    """Codec of the dataclass Action, from/to fumen data (int).
+    """
     _DECODING_OFFSET = {
         Mino.I: {
             Rotation.REVERSE: (1, 0),
             Rotation.LEFT: (0, -1),
         },
         Mino.O: {
             Rotation.SPAWN: (0, -1),
```

### Comparing `py_fumen_py-0.0.4/src/py_fumen_py/comment.py` & `py_fumen_py-0.0.5/src/py_fumen_py/comment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # -*- coding: utf-8 -*-
 
 class CommentCodec:
+    """Codec of comment string segment, from/to fumen data (int).
+    """
     _ENCODING_TABLE = (' !"#$%&\'()*+,-./0123456789:;<=>?@'
                       'ABCDEFGHIJKLMNOPQRSTUVWXYZ[\\]^_`'
                       'abcdefghijklmnopqrstuvwxyz{|}~')
     _DECODING_TABLE = {char: i for i, char in enumerate(_ENCODING_TABLE)}
     _TABLE_LENGTH = len(_ENCODING_TABLE) + 1
 
     @classmethod
```

### Comparing `py_fumen_py-0.0.4/src/py_fumen_py/fumen_codec.py` & `py_fumen_py-0.0.5/src/py_fumen_py/fumen_codec.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .fumen_buffer import FumenBufferReader, FumenBufferWriter
 from .js_escape import escape, escaped_compare
 from .operation import Mino, Rotation, Operation
 from .page import Page, Flags, Refs
 from .quiz import Quiz
 
 def _get_reader(string):
+    # Initially parse the given input, and preapre the FumenBufferReader.
     string = string.split('&')[0]
     data = None
     for version in ['115', '110']:
         for prefix in 'vmd':
             match = string.find(prefix+version)
             if match != -1:
                 data = string[match+5:].strip().replace('?', '')
@@ -24,14 +25,15 @@
 
     if version == '110':
         return FumenBufferReader(FieldConstants110, data)
     else:
         return FumenBufferReader(FieldConstants, data)
 
 def decode(string):
+    """Decode the given fumen string into usable data."""
     fumen_reader = _get_reader(string)
     pages = []
     prev_comment = ''
     prev_lock = False
     prev_mino = Mino._
     field_ref_index = None
     comment_ref_index = None
@@ -69,14 +71,15 @@
         prev_comment = comment
         prev_lock = action.lock
         prev_mino = action.operation.mino
 
     return pages
 
 def encode(pages):
+    """Encode the given pages into a fumen string."""
     fumen_writer = FumenBufferWriter()
     prev_comment = ''
     prev_lock = False
     prev_mino = Mino._
 
     for page in pages:
         page.flags = Flags() if page.flags is None else page.flags
```

### Comparing `py_fumen_py-0.0.4/.gitignore` & `py_fumen_py-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.4/LICENSE` & `py_fumen_py-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.4/README.md` & `py_fumen_py-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.4/pyproject.toml` & `py_fumen_py-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "py_fumen_py"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
 	{ name="Octupus Tea" },
 ]
 description = "Python implementation of the JavaScript package 'tetris-fumen'"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `py_fumen_py-0.0.4/PKG-INFO` & `py_fumen_py-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_fumen_py
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python implementation of the JavaScript package 'tetris-fumen'
 Project-URL: Source, https://github.com/OctupusTea/py-fumen-py
 Author: Octupus Tea
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

