# Comparing `tmp/bmw-lobster-core-0.9.1.tar.gz` & `tmp/bmw-lobster-core-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-core-0.9.1.tar", last modified: Wed May  3 14:22:57 2023, max compression
+gzip compressed data, was "bmw-lobster-core-0.9.2.tar", last modified: Mon May  8 15:06:38 2023, max compression
```

## Comparing `bmw-lobster-core-0.9.1.tar` & `bmw-lobster-core-0.9.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:57.492379 bmw-lobster-core-0.9.1/
--rw-r--r--   0 florian   (1000) florian   (1000)     2692 2023-05-03 14:22:57.492379 bmw-lobster-core-0.9.1/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1733 2023-05-03 14:09:11.000000 bmw-lobster-core-0.9.1/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:57.488379 bmw-lobster-core-0.9.1/bmw_lobster_core.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     2692 2023-05-03 14:22:57.000000 bmw-lobster-core-0.9.1/bmw_lobster_core.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      679 2023-05-03 14:22:57.000000 bmw-lobster-core-0.9.1/bmw_lobster_core.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-03 14:22:57.000000 bmw-lobster-core-0.9.1/bmw_lobster_core.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      240 2023-05-03 14:22:57.000000 bmw-lobster-core-0.9.1/bmw_lobster_core.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-05-03 14:22:57.000000 bmw-lobster-core-0.9.1/bmw_lobster_core.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:57.492379 bmw-lobster-core-0.9.1/lobster/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-03 14:09:11.000000 bmw-lobster-core-0.9.1/lobster/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:57.492379 bmw-lobster-core-0.9.1/lobster/config/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-03 14:09:11.000000 bmw-lobster-core-0.9.1/lobster/config/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4154 2023-05-03 14:09:11.000000 bmw-lobster-core-0.9.1/lobster/config/lexer.py
--rw-r--r--   0 florian   (1000) florian   (1000)     8992 2023-05-03 14:09:11.000000 bmw-lobster-core-0.9.1/lobster/config/parser.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2500 2023-05-03 14:09:11.000000 bmw-lobster-core-0.9.1/lobster/errors.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1243 2023-05-03 14:09:11.000000 bmw-lobster-core-0.9.1/lobster/exceptions.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:57.492379 bmw-lobster-core-0.9.1/lobster/html/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-03 14:09:11.000000 bmw-lobster-core-0.9.1/lobster/html/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2682 2023-05-03 14:22:57.000000 bmw-lobster-core-0.9.1/lobster/html/assets.py
--rw-r--r--   0 florian   (1000) florian   (1000)     9677 2023-05-03 14:09:11.000000 bmw-lobster-core-0.9.1/lobster/html/htmldoc.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4401 2023-05-03 14:09:11.000000 bmw-lobster-core-0.9.1/lobster/io.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11204 2023-05-03 14:09:11.000000 bmw-lobster-core-0.9.1/lobster/items.py
--rw-r--r--   0 florian   (1000) florian   (1000)     7161 2023-05-03 14:09:11.000000 bmw-lobster-core-0.9.1/lobster/location.py
--rw-r--r--   0 florian   (1000) florian   (1000)     8157 2023-05-03 14:09:11.000000 bmw-lobster-core-0.9.1/lobster/report.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:57.488379 bmw-lobster-core-0.9.1/lobster/tools/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-03 14:22:57.492379 bmw-lobster-core-0.9.1/lobster/tools/core/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-03 14:09:11.000000 bmw-lobster-core-0.9.1/lobster/tools/core/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     1917 2023-05-03 14:09:11.000000 bmw-lobster-core-0.9.1/lobster/tools/core/ci_report.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)    15949 2023-05-03 14:09:11.000000 bmw-lobster-core-0.9.1/lobster/tools/core/html_report.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     3797 2023-05-03 14:09:11.000000 bmw-lobster-core-0.9.1/lobster/tools/core/online_report.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     1647 2023-05-03 14:09:11.000000 bmw-lobster-core-0.9.1/lobster/tools/core/report.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1025 2023-05-03 14:09:11.000000 bmw-lobster-core-0.9.1/lobster/version.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-03 14:22:57.492379 bmw-lobster-core-0.9.1/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2513 2023-05-03 14:09:11.000000 bmw-lobster-core-0.9.1/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.505486 bmw-lobster-core-0.9.2/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2692 2023-05-08 15:06:38.505486 bmw-lobster-core-0.9.2/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1733 2023-05-08 15:03:18.000000 bmw-lobster-core-0.9.2/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.497486 bmw-lobster-core-0.9.2/bmw_lobster_core.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2692 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/bmw_lobster_core.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      679 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/bmw_lobster_core.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/bmw_lobster_core.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      240 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/bmw_lobster_core.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/bmw_lobster_core.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.501486 bmw-lobster-core-0.9.2/lobster/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.501486 bmw-lobster-core-0.9.2/lobster/config/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/config/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4160 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/config/lexer.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     9086 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/config/parser.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2500 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/errors.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1243 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/exceptions.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.501486 bmw-lobster-core-0.9.2/lobster/html/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/html/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2682 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/html/assets.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     9667 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/html/htmldoc.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4401 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/io.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11204 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/items.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     7161 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/location.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     8157 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/report.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.497486 bmw-lobster-core-0.9.2/lobster/tools/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.501486 bmw-lobster-core-0.9.2/lobster/tools/core/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/tools/core/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     1917 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/tools/core/ci_report.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)    15949 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/tools/core/html_report.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     3707 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/tools/core/online_report.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     1817 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/tools/core/report.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1025 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/version.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-08 15:06:38.505486 bmw-lobster-core-0.9.2/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2513 2023-05-08 15:03:18.000000 bmw-lobster-core-0.9.2/setup.py
```

### Comparing `bmw-lobster-core-0.9.1/PKG-INFO` & `bmw-lobster-core-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-core
-Version: 0.9.1
+Version: 0.9.2
 Summary: Lightweight Open BMW Software Tracability Evidence Report
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-core-0.9.1/README.md` & `bmw-lobster-core-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.1/bmw_lobster_core.egg-info/PKG-INFO` & `bmw-lobster-core-0.9.2/bmw_lobster_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-core
-Version: 0.9.1
+Version: 0.9.2
 Summary: Lightweight Open BMW Software Tracability Evidence Report
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-core-0.9.1/bmw_lobster_core.egg-info/SOURCES.txt` & `bmw-lobster-core-0.9.2/bmw_lobster_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.1/lobster/config/lexer.py` & `bmw-lobster-core-0.9.2/lobster/config/lexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 # You should have received a copy of the GNU Affero General Public
 # License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
 import sys
 import os.path
 
-import lobster.errors as errors
-import lobster.location as location
+from lobster import errors
+from lobster import location
 
 
 class Token:
     def __init__(self, kind, text, loc):
         self.kind = kind
         self.text = text
         self.loc  = loc
@@ -47,15 +47,15 @@
         assert isinstance(mh, errors.Message_Handler)
         assert isinstance(file_name, str)
         assert os.path.isfile(file_name)
 
         self.file_name = file_name
         self.mh        = mh
 
-        with open(file_name, "r") as fd:
+        with open(file_name, "r", encoding="UTF-8") as fd:
             self.content = fd.read()
             self.length  = len(self.content)
 
         self.lexpos = -1
         self.line_nr = 1
         self.cc = None
         self.nc = self.content[0] if self.length > 0 else None
```

### Comparing `bmw-lobster-core-0.9.1/lobster/config/parser.py` & `bmw-lobster-core-0.9.2/lobster/config/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 # License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
 import sys
 import os.path
 import collections
 
-import lobster.config.lexer as lexer
-import lobster.errors as errors
-import lobster.location as location
+from lobster.config import lexer
+from lobster import errors
+from lobster import location
 
 
 class Parser:
     def __init__(self, mh, file_name):
         assert isinstance(mh, errors.Message_Handler)
         assert isinstance(file_name, str)
         assert os.path.isfile(file_name)
@@ -57,25 +57,28 @@
             return False
 
     def match(self, kind, value=None):
         if self.peek(kind, value):
             self.advance()
         elif self.nt is None:
             self.error(
-                errors.File_Reference(filename = self.lexer.file_name),
+                location.File_Reference(filename = self.lexer.file_name),
                 "expected %s, found EOF" % kind)
         elif value is None:
             self.error(self.nt.loc,
                        "expected %s, found %s %s" % (kind,
                                                      self.nt.kind,
                                                      self.nt.value()))
         else:
             self.error(self.nt.loc,
                        "expected %s, found %s" % (value, self.nt.value()))
 
+    def warning(self, loc, message):
+        self.lexer.mh.warning(loc, message)
+
     def error(self, loc, message):
         self.lexer.mh.error(loc, message)
 
     def parse(self):
         while self.nt:
             if self.peek("KEYWORD", "requirements") or \
                self.peek("KEYWORD", "implementation") or \
@@ -205,32 +208,32 @@
                 self.error(self.nt.loc,
                            "unexpected directive %s" % self.nt.value())
 
         self.match("C_KET")
 
 
 def load(mh, file_name):
-    p = Parser(mh, file_name)
-    ast = p.parse()
+    parser = Parser(mh, file_name)
+    ast = parser.parse()
 
     # Resolve requires links now
     for item in ast.values():
         item["breakdown_requirements"] = []
         if len(item["raw_trace_requirements"]) > 0:
             for chain in item["raw_trace_requirements"]:
                 new_chain = []
-                for t in chain:
-                    if t.value() not in ast:
-                        mh.error(t.loc, "unknown level %s" % t.value())
-                    if item["name"] not in ast[t.value()]["traces"]:
-                        mh.error(t.loc,
+                for tok in chain:
+                    if tok.value() not in ast:
+                        mh.error(tok.loc, "unknown level %s" % tok.value())
+                    if item["name"] not in ast[tok.value()]["traces"]:
+                        mh.error(tok.loc,
                                  "%s cannot trace to %s items" %
-                                 (t.value(),
+                                 (tok.value(),
                                   item["name"]))
-                    new_chain.append(t.value())
+                    new_chain.append(tok.value())
                 item["breakdown_requirements"].append(new_chain)
         else:
             for src in ast.values():
                 if item["name"] in src["traces"]:
                     item["breakdown_requirements"].append([src["name"]])
         del item["raw_trace_requirements"]
```

### Comparing `bmw-lobster-core-0.9.1/lobster/errors.py` & `bmw-lobster-core-0.9.2/lobster/errors.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.1/lobster/exceptions.py` & `bmw-lobster-core-0.9.2/lobster/exceptions.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.1/lobster/html/assets.py` & `bmw-lobster-core-0.9.2/lobster/html/assets.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.1/lobster/html/htmldoc.py` & `bmw-lobster-core-0.9.2/lobster/html/htmldoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
         if len(self.body) == 0:
             self.body.append('<div class="content">')
         self.body.append(line)
 
     def add_heading(self, level, text, anchor=None):
         assert isinstance(level, int)
         assert isinstance(text, str)
-        assert level >= 2 and level <= 7
+        assert 2 <= level <= 7
         assert anchor is None or isinstance(anchor, str)
 
         if level == 2 and self.body:
             self.body.append("</div>")
 
         if anchor is None:
             self.body.append("<h%u>%s</h%u>" % (level,
```

### Comparing `bmw-lobster-core-0.9.1/lobster/io.py` & `bmw-lobster-core-0.9.2/lobster/io.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.1/lobster/items.py` & `bmw-lobster-core-0.9.2/lobster/items.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.1/lobster/location.py` & `bmw-lobster-core-0.9.2/lobster/location.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.1/lobster/report.py` & `bmw-lobster-core-0.9.2/lobster/report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.1/lobster/tools/core/ci_report.py` & `bmw-lobster-core-0.9.2/lobster/tools/core/ci_report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.1/lobster/tools/core/html_report.py` & `bmw-lobster-core-0.9.2/lobster/tools/core/html_report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.1/lobster/tools/core/online_report.py` & `bmw-lobster-core-0.9.2/lobster/tools/core/online_report.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 
 import re
 import sys
 import os
 import argparse
 import configparser
 
-from lobster.exceptions import LOBSTER_Exception
-from lobster.errors import LOBSTER_Error
 from lobster.report import Report
 from lobster.location import File_Reference, Github_Reference
 
 
 def main():
     ap = argparse.ArgumentParser()
     ap.add_argument("lobster_report",
```

### Comparing `bmw-lobster-core-0.9.1/lobster/tools/core/report.py` & `bmw-lobster-core-0.9.2/lobster/tools/core/report.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public
 # License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
+import os
 import sys
 import argparse
 
 from lobster.exceptions import LOBSTER_Exception
 from lobster.errors import LOBSTER_Error
 from lobster.report import Report
 
@@ -29,25 +30,30 @@
     ap = argparse.ArgumentParser()
     ap.add_argument("--lobster-config",
                     metavar="FILE",
                     default="lobster.conf")
 
     options = ap.parse_args()
 
+    if not os.path.isfile(options.lobster_config):
+        print("error: cannot read config file '%s'" % options.lobster_config)
+        return 0
+
     report = Report()
 
     try:
         report.parse_config(options.lobster_config)
     except LOBSTER_Error:
         print("lobster: aborting due to earlier errors.")
         return 1
     except LOBSTER_Exception as err:
         print("lobster: aborting due to earlier errors.")
         print("lobster: Additional data for debugging:")
         err.dump()
         return 1
 
     report.write_report("report.lobster")
+    return 0
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `bmw-lobster-core-0.9.1/lobster/version.py` & `bmw-lobster-core-0.9.2/lobster/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public
 # License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-VERSION_TUPLE = (0, 9, 1)
+VERSION_TUPLE = (0, 9, 2)
 VERSION_SUFFIX = ""
 
 LOBSTER_VERSION = ("%u.%u.%u" % VERSION_TUPLE) + \
     ("-%s" % VERSION_SUFFIX if VERSION_SUFFIX else "")
 
 FULL_NAME = "LOBSTER %s" % LOBSTER_VERSION
```

### Comparing `bmw-lobster-core-0.9.1/setup.py` & `bmw-lobster-core-0.9.2/setup.py`

 * *Files identical despite different names*

