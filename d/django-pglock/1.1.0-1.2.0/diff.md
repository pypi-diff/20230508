# Comparing `tmp/django-pglock-1.1.0.tar.gz` & `tmp/django_pglock-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pglock-1.1.0.tar", max compression
+gzip compressed data, was "django_pglock-1.2.0.tar", max compression
```

## Comparing `django-pglock-1.1.0.tar` & `django_pglock-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1456 2022-11-04 00:12:02.709763 django-pglock-1.1.0/LICENSE
--rw-r--r--   0        0        0     5017 2022-11-04 00:12:02.713763 django-pglock-1.1.0/README.rst
--rw-r--r--   0        0        0      877 2022-11-04 00:12:02.713763 django-pglock-1.1.0/pglock/__init__.py
--rw-r--r--   0        0        0     1766 2022-11-04 00:12:02.713763 django-pglock-1.1.0/pglock/config.py
--rw-r--r--   0        0        0    19826 2022-11-04 00:12:02.713763 django-pglock-1.1.0/pglock/core.py
--rw-r--r--   0        0        0        0 2022-11-04 00:12:02.713763 django-pglock-1.1.0/pglock/management/__init__.py
--rw-r--r--   0        0        0        0 2022-11-04 00:12:02.713763 django-pglock-1.1.0/pglock/management/commands/__init__.py
--rw-r--r--   0        0        0     5490 2022-11-04 00:12:02.713763 django-pglock-1.1.0/pglock/management/commands/pglock.py
--rw-r--r--   0        0        0     9520 2022-11-04 00:12:02.713763 django-pglock-1.1.0/pglock/models.py
--rw-r--r--   0        0        0      151 2022-11-04 00:12:02.713763 django-pglock-1.1.0/pglock/version.py
--rw-r--r--   0        0        0     2414 2022-11-04 00:12:54.710109 django-pglock-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6060 1970-01-01 00:00:00.000000 django-pglock-1.1.0/setup.py
--rw-r--r--   0        0        0     6473 1970-01-01 00:00:00.000000 django-pglock-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2023-05-08 13:18:27.576763 django_pglock-1.2.0/LICENSE
+-rw-r--r--   0        0        0     5017 2023-05-08 13:18:27.576763 django_pglock-1.2.0/README.rst
+-rw-r--r--   0        0        0      877 2023-05-08 13:18:27.576763 django_pglock-1.2.0/pglock/__init__.py
+-rw-r--r--   0        0        0     1766 2023-05-08 13:18:27.576763 django_pglock-1.2.0/pglock/config.py
+-rw-r--r--   0        0        0    19826 2023-05-08 13:18:27.576763 django_pglock-1.2.0/pglock/core.py
+-rw-r--r--   0        0        0        0 2023-05-08 13:18:27.576763 django_pglock-1.2.0/pglock/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 13:18:27.576763 django_pglock-1.2.0/pglock/management/commands/__init__.py
+-rw-r--r--   0        0        0     5490 2023-05-08 13:18:27.576763 django_pglock-1.2.0/pglock/management/commands/pglock.py
+-rw-r--r--   0        0        0     9526 2023-05-08 13:18:27.576763 django_pglock-1.2.0/pglock/models.py
+-rw-r--r--   0        0        0      151 2023-05-08 13:18:27.576763 django_pglock-1.2.0/pglock/version.py
+-rw-r--r--   0        0        0     2414 2023-05-08 13:19:12.992488 django_pglock-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6525 1970-01-01 00:00:00.000000 django_pglock-1.2.0/PKG-INFO
```

### Comparing `django-pglock-1.1.0/LICENSE` & `django_pglock-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pglock-1.1.0/README.rst` & `django_pglock-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-pglock-1.1.0/pglock/__init__.py` & `django_pglock-1.2.0/pglock/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pglock-1.1.0/pglock/config.py` & `django_pglock-1.2.0/pglock/config.py`

 * *Files identical despite different names*

### Comparing `django-pglock-1.1.0/pglock/core.py` & `django_pglock-1.2.0/pglock/core.py`

 * *Files identical despite different names*

### Comparing `django-pglock-1.1.0/pglock/management/commands/pglock.py` & `django_pglock-1.2.0/pglock/management/commands/pglock.py`

 * *Files identical despite different names*

### Comparing `django-pglock-1.1.0/pglock/models.py` & `django_pglock-1.2.0/pglock/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                         WHEN 't' THEN 'TOAST'::text
                         WHEN 'v' THEN 'VIEW'::text
                         WHEN 'm' THEN 'MATERIALIZED_VIEW'::text
                         WHEN 'c' THEN 'COMPOSITE_TYPE'::text
                         WHEN 'f' THEN 'FOREIGN_TABLE'::text
                         WHEN 'p' THEN 'PARTITIONED_TABLE'::text
                         WHEN 'I' THEN 'PARTITIONED_INDEX'::text
-                        ELSE pg_class.relkind
+                        ELSE pg_class.relkind::text
                     END AS rel_kind,
                     UPPER(locktype) as type,
                     pg_class.relname as rel_name,
                     granted,
                     {wait_start_clause}
                 FROM pg_locks
                 JOIN pg_database ON pg_database.oid = pg_locks.database
```

### Comparing `django-pglock-1.1.0/pyproject.toml` & `django_pglock-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 name = "django-pglock"
 packages = [
   { include = "pglock" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "1.1.0"
+version = "1.2.0"
 description = "Postgres locking routines and lock table access."
 authors = ["Opus 10 Engineering"]
 classifiers = [
   "Framework :: Django",
   "Framework :: Django :: 2.2",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
@@ -67,15 +67,15 @@
 django-extensions = "3.2.1"
 flake8 = "3.9.2"
 flake8-bugbear = "22.1.11"
 flake8-comprehensions = "3.8.0"
 flake8-import-order = "0.18.1"
 flake8-logging-format = "0.6.0"
 flake8-mutable = "1.2.0"
-git-tidy = "1.1.2"
+git-tidy = "1.2.0"
 ipython = { version = "8.5.0", python = ">=3.8" }
 myst-parser = "0.18.0"
 packaging = ">=19.2"
 pip = "*"
 poetry-core = "1.3.2"
 pre-commit = "2.13.0"
 psycopg2-binary = "2.9.3"
```

### Comparing `django-pglock-1.1.0/PKG-INFO` & `django_pglock-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pglock
-Version: 1.1.0
+Version: 1.2.0
 Summary: Postgres locking routines and lock table access.
 Home-page: https://github.com/Opus10/django-pglock
 License: BSD-3-Clause
 Author: Opus 10 Engineering
 Requires-Python: >=3.7.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
@@ -16,22 +16,23 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: django (>=2)
 Requires-Dist: django-pgactivity (>=1.1,<2)
-Requires-Dist: importlib_metadata (>=4); python_version >= "3.7" and python_version < "3.8"
+Requires-Dist: importlib_metadata (>=4) ; python_version >= "3.7" and python_version < "3.8"
 Project-URL: Documentation, https://django-pglock.readthedocs.io
 Project-URL: Repository, https://github.com/Opus10/django-pglock
 Description-Content-Type: text/x-rst
 
 django-pglock
 #############
```

