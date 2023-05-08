# Comparing `tmp/kopia-0.1.0.tar.gz` & `tmp/kopia-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kopia-0.1.0.tar", max compression
+gzip compressed data, was "kopia-0.1.1.tar", max compression
```

## Comparing `kopia-0.1.0.tar` & `kopia-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      620 2023-04-04 18:20:36.405728 kopia-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-04 18:02:27.415137 kopia-0.1.0/kopia/__init__.py
--rw-r--r--   0        0        0      238 2023-04-04 18:02:57.290510 kopia-0.1.0/kopia/main.py
--rw-r--r--   0        0        0        0 2023-04-04 14:14:07.117800 kopia-0.1.0/kopia/mysqlc/__init__.py
--rw-r--r--   0        0        0     1357 2023-04-04 17:39:40.192600 kopia-0.1.0/kopia/mysqlc/app.py
--rw-r--r--   0        0        0        0 2023-04-04 14:15:33.606873 kopia-0.1.0/kopia/sqlite/__init__.py
--rw-r--r--   0        0        0      926 2023-04-04 17:31:21.841989 kopia-0.1.0/kopia/sqlite/app.py
--rw-r--r--   0        0        0      540 2023-04-04 17:46:32.351611 kopia-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 kopia-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      715 2023-05-08 10:15:22.340948 kopia-0.1.1/README.md
+-rw-r--r--   0        0        0       22 2023-05-08 11:04:48.720463 kopia-0.1.1/kopia/__init__.py
+-rw-r--r--   0        0        0      238 2023-04-04 18:02:57.290510 kopia-0.1.1/kopia/main.py
+-rw-r--r--   0        0        0        0 2023-04-04 14:14:07.117800 kopia-0.1.1/kopia/mysqlc/__init__.py
+-rw-r--r--   0        0        0     1511 2023-05-08 10:57:32.843791 kopia-0.1.1/kopia/mysqlc/app.py
+-rw-r--r--   0        0        0        0 2023-04-04 14:15:33.606873 kopia-0.1.1/kopia/sqlite/__init__.py
+-rw-r--r--   0        0        0      986 2023-05-08 11:04:11.247165 kopia-0.1.1/kopia/sqlite/app.py
+-rw-r--r--   0        0        0      590 2023-05-08 11:04:52.018872 kopia-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 kopia-0.1.1/PKG-INFO
```

### Comparing `kopia-0.1.0/README.md` & `kopia-0.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -11,11 +11,16 @@
 `kopia mysql dump <db_name> <username> <password>`
 
 ### Creating a SQLite dump
 To create a SQLite dump, use the sqlite command followed by the dump subcommand:
 
 `kopia sqlite dump <db_path>`
 
+## Development
+
+### Running tests
+To run the tests, use the following command: `pytest tests`
+
 ## Contributing
 If you'd like to contribute to Kopia, please submit a pull request on GitHub:
 
 https://github.com/weactivist/kopia
```

### Comparing `kopia-0.1.0/PKG-INFO` & `kopia-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: kopia
-Version: 0.1.0
+Version: 0.1.1
 Summary: CLI for creating database dumps
 Author: Rasmus Nathanson
 Author-email: rasmus.nathanson@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: mysql-connector-python (>=8.0.32,<9.0.0)
+Requires-Dist: pytest (>=7.3.1,<8.0.0)
+Requires-Dist: pytest-mock (>=3.10.0,<4.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # Kopia
 Kopia is a command-line tool for creating database dumps. It supports both MySQL and SQLite databases.
 
 ## Installation
@@ -29,12 +28,17 @@
 `kopia mysql dump <db_name> <username> <password>`
 
 ### Creating a SQLite dump
 To create a SQLite dump, use the sqlite command followed by the dump subcommand:
 
 `kopia sqlite dump <db_path>`
 
+## Development
+
+### Running tests
+To run the tests, use the following command: `pytest tests`
+
 ## Contributing
 If you'd like to contribute to Kopia, please submit a pull request on GitHub:
 
 https://github.com/weactivist/kopia
```

