# Comparing `tmp/exondb-0.3.6.tar.gz` & `tmp/exondb-0.3.7.tar.gz`

## Comparing `exondb-0.3.6.tar` & `exondb-0.3.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 exondb-0.3.6/Makefile
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 exondb-0.3.6/exondb/__about__.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 exondb-0.3.6/exondb/__init__.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 exondb-0.3.6/exondb/cli.py
--rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 exondb-0.3.6/exondb/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 exondb-0.3.6/tests/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 exondb-0.3.6/tests/test_load.py
--rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 exondb-0.3.6/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 exondb-0.3.6/LICENSE.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 exondb-0.3.6/README.md
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 exondb-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 exondb-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 exondb-0.3.7/Makefile
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 exondb-0.3.7/exondb/__about__.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 exondb-0.3.7/exondb/__init__.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 exondb-0.3.7/exondb/cli.py
+-rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 exondb-0.3.7/exondb/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 exondb-0.3.7/tests/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 exondb-0.3.7/tests/test_load.py
+-rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 exondb-0.3.7/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 exondb-0.3.7/LICENSE.txt
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 exondb-0.3.7/README.md
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 exondb-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 exondb-0.3.7/PKG-INFO
```

### Comparing `exondb-0.3.6/exondb/cli.py` & `exondb-0.3.7/exondb/cli.py`

 * *Files identical despite different names*

### Comparing `exondb-0.3.6/exondb/main.py` & `exondb-0.3.7/exondb/main.py`

 * *Files identical despite different names*

### Comparing `exondb-0.3.6/tests/test_load.py` & `exondb-0.3.7/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `exondb-0.3.6/.gitignore` & `exondb-0.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `exondb-0.3.6/LICENSE.txt` & `exondb-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `exondb-0.3.6/pyproject.toml` & `exondb-0.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `exondb-0.3.6/PKG-INFO` & `exondb-0.3.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: exondb
-Version: 0.3.6
+Version: 0.3.7
 Author-email: Trent Hauck <thauck@wheretrue.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: duckdb==0.7.1
 Description-Content-Type: text/markdown
 
-# WTT 01
+# ExonDB
 
 **Table of Contents**
 
 - [Installation](#installation)
 
 ## Installation
 
 ```console
 pip install exondb
 ```
+
+Please see [wheretrue.com](https://www.wheretrue.com) for more information.
```

