# Comparing `tmp/cttd-0.0.1a3.tar.gz` & `tmp/cttd-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cttd-0.0.1a3.tar", max compression
+gzip compressed data, was "cttd-0.0.2a0.tar", max compression
```

## Comparing `cttd-0.0.1a3.tar` & `cttd-0.0.2a0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1108 2023-05-03 17:25:05.122292 cttd-0.0.1a3/LICENSE
--rw-r--r--   0        0        0     2025 2023-05-03 18:54:09.035294 cttd-0.0.1a3/README.md
--rw-r--r--   0        0        0       28 2023-05-03 18:15:09.070117 cttd-0.0.1a3/cttd/__init__.py
--rw-r--r--   0        0        0       55 2023-05-03 18:26:42.187993 cttd-0.0.1a3/cttd/factory.py
--rw-r--r--   0        0        0     2175 2023-05-03 18:28:56.276959 cttd-0.0.1a3/cttd/tester.py
--rw-r--r--   0        0        0      738 2023-05-03 19:53:57.721984 cttd-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 cttd-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-05-03 17:25:05.122292 cttd-0.0.2a0/LICENSE
+-rw-r--r--   0        0        0     2025 2023-05-03 18:54:09.035294 cttd-0.0.2a0/README.md
+-rw-r--r--   0        0        0       28 2023-05-03 18:15:09.070117 cttd-0.0.2a0/cttd/__init__.py
+-rw-r--r--   0        0        0       55 2023-05-03 18:26:42.187993 cttd-0.0.2a0/cttd/factory.py
+-rw-r--r--   0        0        0     2450 2023-05-08 00:41:47.727104 cttd-0.0.2a0/cttd/tester.py
+-rw-r--r--   0        0        0      738 2023-05-08 00:51:43.905579 cttd-0.0.2a0/pyproject.toml
+-rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 cttd-0.0.2a0/PKG-INFO
```

### Comparing `cttd-0.0.1a3/LICENSE` & `cttd-0.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `cttd-0.0.1a3/README.md` & `cttd-0.0.2a0/README.md`

 * *Files identical despite different names*

### Comparing `cttd-0.0.1a3/cttd/tester.py` & `cttd-0.0.2a0/cttd/tester.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,16 +68,27 @@
     @property
     def _state(self):
         return self.__class__._state
 
     @property
     def sut(self):
         return self._state.ensure_sut()
+    
+    @property
+    def null_pointer(self):
+        return self.sut.null_pointer
 
     def register_mock(self, sig: str) -> None:
         if not self._state.sut:
             self._state.externs.append(sig)
 
     def attach_mock(self, func):
         def_extern_decorator = self._state.tube._ffi.def_extern()
         def_extern_decorator(func)
         return getattr(self._state.tube._lib, func.__name__)
+    
+    def assertStrEqual(self, expected, actual):
+        if not isinstance(actual, str):
+            actual = self.sut.str(actual)
+
+        self.assertEqual(actual, expected)
+
```

### Comparing `cttd-0.0.1a3/pyproject.toml` & `cttd-0.0.2a0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cttd"
-version = "0.0.1a3"
+version = "0.0.2a0"
 description = "C test-driven development framework implemented in Python"
 authors = [
   "WideOpenTech <fossie@wideopentech.co.uk>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `cttd-0.0.1a3/PKG-INFO` & `cttd-0.0.2a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cttd
-Version: 0.0.1a3
+Version: 0.0.2a0
 Summary: C test-driven development framework implemented in Python
 Home-page: https://github.com/wideopensource/cttd
 Author: WideOpenTech
 Author-email: fossie@wideopentech.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

