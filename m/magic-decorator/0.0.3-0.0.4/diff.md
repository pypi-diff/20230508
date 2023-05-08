# Comparing `tmp/magic_decorator-0.0.3.tar.gz` & `tmp/magic_decorator-0.0.4.tar.gz`

## Comparing `magic_decorator-0.0.3.tar` & `magic_decorator-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 magic_decorator-0.0.3/magic_decorator.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 magic_decorator-0.0.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 magic_decorator-0.0.3/LICENSE
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 magic_decorator-0.0.3/README.md
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 magic_decorator-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 magic_decorator-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 magic_decorator-0.0.4/magic_decorator.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 magic_decorator-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 magic_decorator-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 magic_decorator-0.0.4/README.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 magic_decorator-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 magic_decorator-0.0.4/PKG-INFO
```

### Comparing `magic_decorator-0.0.3/.gitignore` & `magic_decorator-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `magic_decorator-0.0.3/LICENSE` & `magic_decorator-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `magic_decorator-0.0.3/README.md` & `magic_decorator-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `magic_decorator-0.0.3/PKG-INFO` & `magic_decorator-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: magic-decorator
-Version: 0.0.3
+Version: 0.0.4
 Summary: A magic function decorator using OpenAI ChatCompletion
 Author-email: Kim Minjong <make.dirty.code@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.1
 Requires-Dist: openai>0.27
+Requires-Dist: sick-json
 Description-Content-Type: text/markdown
 
 # Simple demo function using OpenAI's ChatComplete
 
 The only function implemented in this module is magic.
 
 `magic` works as a decorator. It simply sends the function's signature and docstring to the GPT and expects to get a result.
```

