# Comparing `tmp/llsd-1.2.0.tar.gz` & `tmp/llsd-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llsd-1.2.0.tar", last modified: Wed Mar 22 20:54:54 2023, max compression
+gzip compressed data, was "llsd-1.2.1.tar", last modified: Mon May  8 14:20:23 2023, max compression
```

## Comparing `llsd-1.2.0.tar` & `llsd-1.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 20:54:54.451364 llsd-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 20:54:54.451364 llsd-1.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-22 20:53:51.000000 llsd-1.2.0/.github/dependabot.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-22 20:53:51.000000 llsd-1.2.0/.github/release.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 20:54:54.451364 llsd-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-22 20:53:51.000000 llsd-1.2.0/.github/workflows/bench.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-03-22 20:53:51.000000 llsd-1.2.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-03-22 20:53:51.000000 llsd-1.2.0/.github/workflows/cla.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-03-22 20:53:51.000000 llsd-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-03-22 20:53:51.000000 llsd-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-22 20:53:51.000000 llsd-1.2.0/CREDITS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-22 20:53:51.000000 llsd-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-03-22 20:54:54.451364 llsd-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-03-22 20:53:51.000000 llsd-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 20:54:54.451364 llsd-1.2.0/llsd/
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-03-22 20:53:51.000000 llsd-1.2.0/llsd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19387 2023-03-22 20:53:51.000000 llsd-1.2.0/llsd/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-03-22 20:53:51.000000 llsd-1.2.0/llsd/fastest_elementtree.py
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-03-22 20:53:51.000000 llsd-1.2.0/llsd/serde_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-03-22 20:53:51.000000 llsd-1.2.0/llsd/serde_notation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-03-22 20:53:51.000000 llsd-1.2.0/llsd/serde_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 20:54:54.451364 llsd-1.2.0/llsd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-03-22 20:54:54.000000 llsd-1.2.0/llsd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-22 20:54:54.000000 llsd-1.2.0/llsd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 20:54:54.000000 llsd-1.2.0/llsd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-22 20:54:54.000000 llsd-1.2.0/llsd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-22 20:54:54.000000 llsd-1.2.0/llsd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 20:54:54.451364 llsd-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-03-22 20:53:51.000000 llsd-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 20:54:54.451364 llsd-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 20:53:51.000000 llsd-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-03-22 20:53:51.000000 llsd-1.2.0/tests/bench.py
--rw-r--r--   0 runner    (1001) docker     (123)    17339 2023-03-22 20:53:51.000000 llsd-1.2.0/tests/fuzz.py
--rw-r--r--   0 runner    (1001) docker     (123)    63980 2023-03-22 20:53:51.000000 llsd-1.2.0/tests/llsd_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-22 20:53:51.000000 llsd-1.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:20:23.973150 llsd-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:20:23.969150 llsd-1.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-08 14:19:05.000000 llsd-1.2.1/.github/dependabot.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-08 14:19:05.000000 llsd-1.2.1/.github/release.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:20:23.969150 llsd-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-08 14:19:05.000000 llsd-1.2.1/.github/workflows/bench.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-08 14:19:05.000000 llsd-1.2.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-08 14:19:05.000000 llsd-1.2.1/.github/workflows/cla.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-05-08 14:19:05.000000 llsd-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-08 14:19:05.000000 llsd-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-08 14:19:05.000000 llsd-1.2.1/CREDITS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-08 14:19:05.000000 llsd-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-08 14:20:23.973150 llsd-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-08 14:19:05.000000 llsd-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:20:23.973150 llsd-1.2.1/llsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-08 14:19:05.000000 llsd-1.2.1/llsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19387 2023-05-08 14:19:05.000000 llsd-1.2.1/llsd/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-08 14:19:05.000000 llsd-1.2.1/llsd/fastest_elementtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-05-08 14:19:05.000000 llsd-1.2.1/llsd/serde_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-05-08 14:19:05.000000 llsd-1.2.1/llsd/serde_notation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11119 2023-05-08 14:19:05.000000 llsd-1.2.1/llsd/serde_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:20:23.973150 llsd-1.2.1/llsd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-08 14:20:23.000000 llsd-1.2.1/llsd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-08 14:20:23.000000 llsd-1.2.1/llsd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 14:20:23.000000 llsd-1.2.1/llsd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-08 14:20:23.000000 llsd-1.2.1/llsd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 14:20:23.000000 llsd-1.2.1/llsd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 14:20:23.973150 llsd-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-08 14:19:05.000000 llsd-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:20:23.973150 llsd-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 14:19:05.000000 llsd-1.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-08 14:19:05.000000 llsd-1.2.1/tests/bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17339 2023-05-08 14:19:05.000000 llsd-1.2.1/tests/fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64397 2023-05-08 14:19:05.000000 llsd-1.2.1/tests/llsd_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-08 14:19:05.000000 llsd-1.2.1/tox.ini
```

### Comparing `llsd-1.2.0/.github/workflows/bench.yaml` & `llsd-1.2.1/.github/workflows/bench.yaml`

 * *Files identical despite different names*

### Comparing `llsd-1.2.0/.github/workflows/ci.yaml` & `llsd-1.2.1/.github/workflows/ci.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -56,28 +56,27 @@
           name: dist-${{ matrix.python-version }}
           path: dist
 
   publish:
     name: Publish to PyPI
     needs: build
     runs-on: [ubuntu-latest]
+    permissions:
+      id-token: write
     if: github.event_name != 'pull_request'
     steps:
       - uses: actions/download-artifact@v3
 
       - name: Organize files for upload
         run: |
           mkdir dist
           mv dist-3.8/* dist/
           mv dist-2.7/*.whl dist/
 
       - name: Test Publish package
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          password: ${{ secrets.SHARED_PYPI_TEST_TOKEN }}
-          repository_url: https://test.pypi.org/legacy/
+          repository-url: https://test.pypi.org/legacy/
 
       - name: Publish package
         uses: pypa/gh-action-pypi-publish@release/v1
         if: startsWith(github.event.ref, 'refs/tags/v')
-        with:
-          password: ${{ secrets.SHARED_PYPI_TOKEN }}
```

### Comparing `llsd-1.2.0/.github/workflows/cla.yaml` & `llsd-1.2.1/.github/workflows/cla.yaml`

 * *Files identical despite different names*

### Comparing `llsd-1.2.0/.gitignore` & `llsd-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `llsd-1.2.0/LICENSE` & `llsd-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llsd-1.2.0/PKG-INFO` & `llsd-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llsd
-Version: 1.2.0
+Version: 1.2.1
 Summary: Linden Lab Structured Data (LLSD) serialization library
 Home-page: https://github.com/secondlife/python-llsd
 Author: Linden Research, Inc.
 Author-email: opensource-dev@lists.secondlife.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `llsd-1.2.0/README.md` & `llsd-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `llsd-1.2.0/llsd/__init__.py` & `llsd-1.2.1/llsd/__init__.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.0/llsd/base.py` & `llsd-1.2.1/llsd/base.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.0/llsd/fastest_elementtree.py` & `llsd-1.2.1/llsd/fastest_elementtree.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.0/llsd/serde_binary.py` & `llsd-1.2.1/llsd/serde_binary.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.0/llsd/serde_notation.py` & `llsd-1.2.1/llsd/serde_notation.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.0/llsd/serde_xml.py` & `llsd-1.2.1/llsd/serde_xml.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,25 +40,21 @@
     def _elt(self, name, contents=None):
         """
         Serialize a single element.
 
         If 'contents' is omitted, write <name/>.
         If 'contents' is bytes, write <name>contents</name>.
         If 'contents' is str, write <name>contents.encode('utf8')</name>.
-        If 'contents' is callable, write <name>, call contents(), write </name>.
         """
         if not contents:
             self.stream.writelines([b"<", name, b" />"])
         else:
-            self.stream.writelines([b"<", name, b">"])
-            if callable(contents):
-                contents()
-            else:
-                self.stream.write(_str_to_bytes(contents))
-            self.stream.writelines([b"</", name, b">"])
+            self.stream.writelines([b"<", name, b">",
+                                    _str_to_bytes(contents),
+                                    b"</", name, b">"])
 
     def xml_esc(self, v):
         "Escape string or unicode object v for xml output"
 
         # Use is_unicode() instead of is_string() because in python 2, str is
         # bytes, not unicode, and should not be "encode()"d. Attempts to
         # encode("utf-8") a bytes type will result in an implicit
@@ -96,23 +92,24 @@
     def _STRING(self, v):
         return self._elt(b'string', self.xml_esc(v))
     def _URI(self, v):
         return self._elt(b'uri', self.xml_esc(str(v)))
     def _DATE(self, v):
         return self._elt(b'date', _format_datestr(v))
     def _ARRAY(self, v):
-        return self._elt(
-            b'array',
-            lambda: [self._generate(item) for item in v])
+        self.stream.write(b'<array>')
+        for item in v:
+            self._generate(item)
+        self.stream.write(b'</array>')
     def _MAP(self, v):
-        return self._elt(
-            b'map',
-            lambda: [(self._elt(b'key', self.xml_esc(UnicodeType(key))),
-                      self._generate(value))
-                     for key, value in v.items()])
+        self.stream.write(b'<map>')
+        for key, value in v.items():
+            self._elt(b'key', self.xml_esc(UnicodeType(key)))
+            self._generate(value)
+        self.stream.write(b'</map>')
 
     def _generate(self, something):
         "Generate xml from a single python object."
         t = type(something)
         if t in self.type_map:
             return self.type_map[t](something)
         elif isinstance(something, _LLSD):
@@ -123,16 +120,18 @@
 
     def _write(self, something):
         """
         Serialize a python object to self.stream as application/llsd+xml.
 
         :param something: A python object (typically a dict) to be serialized.
         """
-        self.stream.write(b'<?xml version="1.0" ?>')
-        self._elt(b"llsd", lambda: self._generate(something))
+        self.stream.write(b'<?xml version="1.0" ?>'
+                          b'<llsd>')
+        self._generate(something)
+        self.stream.write(b'</llsd>')
 
 
 class LLSDXMLPrettyFormatter(LLSDXMLFormatter):
     """
     Class which implements 'pretty' LLSD XML serialization..
 
     See http://wiki.secondlife.com/wiki/LLSD#XML_Serialization
```

### Comparing `llsd-1.2.0/llsd.egg-info/PKG-INFO` & `llsd-1.2.1/llsd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llsd
-Version: 1.2.0
+Version: 1.2.1
 Summary: Linden Lab Structured Data (LLSD) serialization library
 Home-page: https://github.com/secondlife/python-llsd
 Author: Linden Research, Inc.
 Author-email: opensource-dev@lists.secondlife.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `llsd-1.2.0/llsd.egg-info/SOURCES.txt` & `llsd-1.2.1/llsd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llsd-1.2.0/setup.py` & `llsd-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.0/tests/bench.py` & `llsd-1.2.1/tests/bench.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.0/tests/fuzz.py` & `llsd-1.2.1/tests/fuzz.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.0/tests/llsd_test.py` & `llsd-1.2.1/tests/llsd_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1341,14 +1341,28 @@
         python_map_within_map = {"foo":"bar", "doo":{"goo":"poo"}}
 
         self.assertXMLRoundtrip(python_map, map_xml)
         self.assertXMLRoundtrip(python_map_within_map,
                                   map_within_map_xml)
         self.assertXMLRoundtrip({}, blank_map_xml)
 
+    def testDeepMap(self):
+        """
+        Test that formatting a deeply nested map does not cause a RecursionError
+        """
+
+        test_map = {"foo":"bar", "depth":0, "next":None}
+        max_depth = 200
+        for depth in range(max_depth):
+            test_map = {"foo":"bar", "depth":depth, "next":test_map}
+
+        # this should not throw an exception.
+        test_xml = self.llsd.as_xml(test_map)
+
+
     def testBinary(self):
         """
         Test the parse and serialization of input type : binary.
         Maps to test scenarios module:llsd:test#64
         """
         base64_binary_xml = b"\
 <?xml version=\"1.0\" ?>\
```

