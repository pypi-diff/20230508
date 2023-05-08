# Comparing `tmp/bech32m-0.0.1.tar.gz` & `tmp/bech32m-0.1.0.tar.gz`

## Comparing `bech32m-0.0.1.tar` & `bech32m-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,31 @@
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bech32m-0.0.1/bech32m/__about__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 bech32m-0.0.1/bech32m/__init__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 bech32m-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 bech32m-0.0.1/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 bech32m-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 bech32m-0.0.1/README.md
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 bech32m-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 bech32m-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bech32m-0.1.0/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bech32m-0.1.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bech32m-0.1.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 bech32m-0.1.0/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 bech32m-0.1.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 bech32m-0.1.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 bech32m-0.1.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 bech32m-0.1.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bech32m-0.1.0/.ruff_cache/content/2818dce65e936579
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 bech32m-0.1.0/.ruff_cache/content/3bf84884f50aa069
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 bech32m-0.1.0/.ruff_cache/content/54588ff63ed26071
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 bech32m-0.1.0/.ruff_cache/content/5767f150cc453ca7
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bech32m-0.1.0/.ruff_cache/content/623b5e16f9bb5e5b
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 bech32m-0.1.0/.ruff_cache/content/a2dc965ba166af70
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 bech32m-0.1.0/.ruff_cache/content/a375f84b46e2930b
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 bech32m-0.1.0/.ruff_cache/content/a4b9a522a6e7939a
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bech32m-0.1.0/.ruff_cache/content/ac68f5c6690e1746
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 bech32m-0.1.0/.ruff_cache/content/b2bf66d8dafa6d6e
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bech32m-0.1.0/.ruff_cache/content/bc471700bf78be65
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 bech32m-0.1.0/.ruff_cache/content/dc7fa9c1b9a6781b
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 bech32m-0.1.0/.ruff_cache/content/eb28e795d46c2541
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bech32m-0.1.0/.ruff_cache/content/f48550ff0b959866
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 bech32m-0.1.0/bech32m/__init__.py
+-rw-r--r--   0        0        0     5614 2020-02-02 00:00:00.000000 bech32m-0.1.0/bech32m/codecs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bech32m-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 bech32m-0.1.0/tests/test_codecs.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 bech32m-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 bech32m-0.1.0/LICENSE
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 bech32m-0.1.0/README.md
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 bech32m-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 bech32m-0.1.0/PKG-INFO
```

### Comparing `bech32m-0.0.1/LICENSE.txt` & `bech32m-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bech32m-0.0.1/PKG-INFO` & `bech32m-0.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,19 @@
 Metadata-Version: 2.1
 Name: bech32m
-Version: 0.0.1
+Version: 0.1.0
 Summary: Encoding/decoding Bech32 and Bech32m
-Project-URL: Documentation, https://github.com/unknown/bech32m#readme
-Project-URL: Issues, https://github.com/unknown/bech32m/issues
-Project-URL: Source, https://github.com/unknown/bech32m
+Project-URL: Source, https://github.com/ods/bech32m
 Author-email: Denis Otkidach <denis.otkidach@gmail.com>
 License-Expression: MIT
-License-File: LICENSE.txt
+License-File: LICENSE
+Keywords: bech32,bech32m,bitcoin,blockchain
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # bech32m
 
 [![PyPI - Version](https://img.shields.io/pypi/v/bech32m.svg)](https://pypi.org/project/bech32m)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bech32m.svg)](https://pypi.org/project/bech32m)
```

