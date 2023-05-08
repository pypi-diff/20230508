# Comparing `tmp/kopia-0.1.1.tar.gz` & `tmp/kopia-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kopia-0.1.1.tar", max compression
+gzip compressed data, was "kopia-0.1.2.tar", max compression
```

## Comparing `kopia-0.1.1.tar` & `kopia-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      715 2023-05-08 10:15:22.340948 kopia-0.1.1/README.md
--rw-r--r--   0        0        0       22 2023-05-08 11:04:48.720463 kopia-0.1.1/kopia/__init__.py
--rw-r--r--   0        0        0      238 2023-04-04 18:02:57.290510 kopia-0.1.1/kopia/main.py
--rw-r--r--   0        0        0        0 2023-04-04 14:14:07.117800 kopia-0.1.1/kopia/mysqlc/__init__.py
--rw-r--r--   0        0        0     1511 2023-05-08 10:57:32.843791 kopia-0.1.1/kopia/mysqlc/app.py
--rw-r--r--   0        0        0        0 2023-04-04 14:15:33.606873 kopia-0.1.1/kopia/sqlite/__init__.py
--rw-r--r--   0        0        0      986 2023-05-08 11:04:11.247165 kopia-0.1.1/kopia/sqlite/app.py
--rw-r--r--   0        0        0      590 2023-05-08 11:04:52.018872 kopia-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 kopia-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      715 2023-05-08 10:15:22.340948 kopia-0.1.2/README.md
+-rw-r--r--   0        0        0       22 2023-05-08 11:16:32.548889 kopia-0.1.2/kopia/__init__.py
+-rw-r--r--   0        0        0      238 2023-04-04 18:02:57.290510 kopia-0.1.2/kopia/main.py
+-rw-r--r--   0        0        0        0 2023-04-04 14:14:07.117800 kopia-0.1.2/kopia/mysqlc/__init__.py
+-rw-r--r--   0        0        0     1511 2023-05-08 10:57:32.843791 kopia-0.1.2/kopia/mysqlc/app.py
+-rw-r--r--   0        0        0        0 2023-04-04 14:15:33.606873 kopia-0.1.2/kopia/sqlite/__init__.py
+-rw-r--r--   0        0        0      986 2023-05-08 11:15:44.717579 kopia-0.1.2/kopia/sqlite/app.py
+-rw-r--r--   0        0        0      619 2023-05-08 11:16:34.651055 kopia-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1376 1970-01-01 00:00:00.000000 kopia-0.1.2/PKG-INFO
```

### Comparing `kopia-0.1.1/README.md` & `kopia-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kopia-0.1.1/kopia/mysqlc/app.py` & `kopia-0.1.2/kopia/mysqlc/app.py`

 * *Files identical despite different names*

### Comparing `kopia-0.1.1/kopia/sqlite/app.py` & `kopia-0.1.2/kopia/sqlite/app.py`

 * *Files identical despite different names*

### Comparing `kopia-0.1.1/PKG-INFO` & `kopia-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: kopia
-Version: 0.1.1
+Version: 0.1.2
 Summary: CLI for creating database dumps
 Author: Rasmus Nathanson
 Author-email: rasmus.nathanson@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: mysql-connector-python (>=8.0.32,<9.0.0)
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: pytest-mock (>=3.10.0,<4.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Kopia
 Kopia is a command-line tool for creating database dumps. It supports both MySQL and SQLite databases.
 
 ## Installation
 You can install kopia using pip: `pip install kopia`
```

