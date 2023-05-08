# Comparing `tmp/mysql-to-sqlite3-1.4.8.tar.gz` & `tmp/mysql-to-sqlite3-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mysql-to-sqlite3-1.4.8.tar", last modified: Sun Oct 10 11:34:57 2021, max compression
+gzip compressed data, was "mysql-to-sqlite3-1.4.9.tar", last modified: Sun Oct 10 12:25:33 2021, max compression
```

## Comparing `mysql-to-sqlite3-1.4.8.tar` & `mysql-to-sqlite3-1.4.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 11:34:57.872741 mysql-to-sqlite3-1.4.8/
--rw-r--r--   0 klemen     (501) staff       (20)     5513 2021-09-19 12:14:51.000000 mysql-to-sqlite3-1.4.8/CODE-OF-CONDUCT.md
--rw-r--r--   0 klemen     (501) staff       (20)     1069 2021-02-13 10:59:16.000000 mysql-to-sqlite3-1.4.8/LICENSE
--rw-r--r--   0 klemen     (501) staff       (20)      166 2020-07-19 22:16:56.000000 mysql-to-sqlite3-1.4.8/MANIFEST.in
--rw-r--r--   0 klemen     (501) staff       (20)     6650 2021-10-10 11:34:57.874568 mysql-to-sqlite3-1.4.8/PKG-INFO
--rw-r--r--   0 klemen     (501) staff       (20)     4735 2021-10-10 11:20:53.000000 mysql-to-sqlite3-1.4.8/README.md
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 11:34:57.823253 mysql-to-sqlite3-1.4.8/mysql_to_sqlite3/
--rw-r--r--   0 klemen     (501) staff       (20)       95 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.8/mysql_to_sqlite3/__init__.py
--rw-r--r--   0 klemen     (501) staff       (20)      363 2021-10-10 11:34:12.000000 mysql-to-sqlite3-1.4.8/mysql_to_sqlite3/__version__.py
--rw-r--r--   0 klemen     (501) staff       (20)     4740 2021-10-10 11:20:53.000000 mysql-to-sqlite3-1.4.8/mysql_to_sqlite3/cli.py
--rw-r--r--   0 klemen     (501) staff       (20)     2598 2021-08-07 15:18:45.000000 mysql-to-sqlite3-1.4.8/mysql_to_sqlite3/click_utils.py
--rw-r--r--   0 klemen     (501) staff       (20)     3451 2020-11-05 17:57:09.000000 mysql-to-sqlite3-1.4.8/mysql_to_sqlite3/debug_info.py
--rw-r--r--   0 klemen     (501) staff       (20)      175 2020-08-31 13:42:08.000000 mysql-to-sqlite3-1.4.8/mysql_to_sqlite3/sixeptions.py
--rw-r--r--   0 klemen     (501) staff       (20)     1183 2021-08-01 13:08:36.000000 mysql-to-sqlite3-1.4.8/mysql_to_sqlite3/sqlite_utils.py
--rw-r--r--   0 klemen     (501) staff       (20)    21698 2021-10-10 11:20:52.000000 mysql-to-sqlite3-1.4.8/mysql_to_sqlite3/transporter.py
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 11:34:57.835249 mysql-to-sqlite3-1.4.8/mysql_to_sqlite3.egg-info/
--rw-r--r--   0 klemen     (501) staff       (20)     6650 2021-10-10 11:34:57.000000 mysql-to-sqlite3-1.4.8/mysql_to_sqlite3.egg-info/PKG-INFO
--rw-r--r--   0 klemen     (501) staff       (20)      874 2021-10-10 11:34:57.000000 mysql-to-sqlite3-1.4.8/mysql_to_sqlite3.egg-info/SOURCES.txt
--rw-r--r--   0 klemen     (501) staff       (20)        1 2021-10-10 11:34:57.000000 mysql-to-sqlite3-1.4.8/mysql_to_sqlite3.egg-info/dependency_links.txt
--rw-r--r--   0 klemen     (501) staff       (20)       77 2021-10-10 11:34:57.000000 mysql-to-sqlite3-1.4.8/mysql_to_sqlite3.egg-info/entry_points.txt
--rw-r--r--   0 klemen     (501) staff       (20)        1 2020-07-18 12:41:59.000000 mysql-to-sqlite3-1.4.8/mysql_to_sqlite3.egg-info/not-zip-safe
--rw-r--r--   0 klemen     (501) staff       (20)      347 2021-10-10 11:34:57.000000 mysql-to-sqlite3-1.4.8/mysql_to_sqlite3.egg-info/requires.txt
--rw-r--r--   0 klemen     (501) staff       (20)       17 2021-10-10 11:34:57.000000 mysql-to-sqlite3-1.4.8/mysql_to_sqlite3.egg-info/top_level.txt
--rw-r--r--   0 klemen     (501) staff       (20)      337 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.8/pytest.ini
--rw-r--r--   0 klemen     (501) staff       (20)      736 2021-08-07 16:16:06.000000 mysql-to-sqlite3-1.4.8/requirements_dev.txt
--rw-r--r--   0 klemen     (501) staff       (20)      191 2021-10-10 11:34:57.879473 mysql-to-sqlite3-1.4.8/setup.cfg
--rw-r--r--   0 klemen     (501) staff       (20)     2436 2021-08-07 14:20:50.000000 mysql-to-sqlite3-1.4.8/setup.py
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 11:34:57.845685 mysql-to-sqlite3-1.4.8/tests/
--rw-r--r--   0 klemen     (501) staff       (20)        0 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.8/tests/__init__.py
--rw-r--r--   0 klemen     (501) staff       (20)    12783 2020-08-31 13:37:27.000000 mysql-to-sqlite3-1.4.8/tests/conftest.py
--rw-r--r--   0 klemen     (501) staff       (20)     1321 2020-07-26 12:31:00.000000 mysql-to-sqlite3-1.4.8/tests/database.py
--rw-r--r--   0 klemen     (501) staff       (20)     3820 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.8/tests/factories.py
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 11:34:57.859247 mysql-to-sqlite3-1.4.8/tests/func/
--rw-r--r--   0 klemen     (501) staff       (20)        0 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.8/tests/func/__init__.py
--rw-r--r--   0 klemen     (501) staff       (20)    38476 2021-08-07 11:14:10.000000 mysql-to-sqlite3-1.4.8/tests/func/mysql_to_sqlite3_test.py
--rw-r--r--   0 klemen     (501) staff       (20)    12737 2021-08-07 14:23:37.000000 mysql-to-sqlite3-1.4.8/tests/func/test_cli.py
--rw-r--r--   0 klemen     (501) staff       (20)     5877 2021-03-04 20:56:52.000000 mysql-to-sqlite3-1.4.8/tests/models.py
--rw-r--r--   0 klemen     (501) staff       (20)      201 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.8/tests/sixeptions.py
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 11:34:57.862022 mysql-to-sqlite3-1.4.8/tests/unit/
--rw-r--r--   0 klemen     (501) staff       (20)        0 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.8/tests/unit/__init__.py
--rw-r--r--   0 klemen     (501) staff       (20)    20853 2021-10-10 11:20:52.000000 mysql-to-sqlite3-1.4.8/tests/unit/mysql_to_sqlite3_test.py
+drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 12:25:33.642385 mysql-to-sqlite3-1.4.9/
+-rw-r--r--   0 klemen     (501) staff       (20)     5513 2021-09-19 12:14:51.000000 mysql-to-sqlite3-1.4.9/CODE-OF-CONDUCT.md
+-rw-r--r--   0 klemen     (501) staff       (20)     1069 2021-02-13 10:59:16.000000 mysql-to-sqlite3-1.4.9/LICENSE
+-rw-r--r--   0 klemen     (501) staff       (20)      166 2020-07-19 22:16:56.000000 mysql-to-sqlite3-1.4.9/MANIFEST.in
+-rw-r--r--   0 klemen     (501) staff       (20)     6136 2021-10-10 12:25:33.643053 mysql-to-sqlite3-1.4.9/PKG-INFO
+-rw-r--r--   0 klemen     (501) staff       (20)     4735 2021-10-10 11:20:53.000000 mysql-to-sqlite3-1.4.9/README.md
+drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 12:25:33.595304 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/
+-rw-r--r--   0 klemen     (501) staff       (20)       95 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/__init__.py
+-rw-r--r--   0 klemen     (501) staff       (20)      363 2021-10-10 12:24:54.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/__version__.py
+-rw-r--r--   0 klemen     (501) staff       (20)     4740 2021-10-10 11:20:53.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/cli.py
+-rw-r--r--   0 klemen     (501) staff       (20)     2598 2021-08-07 15:18:45.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/click_utils.py
+-rw-r--r--   0 klemen     (501) staff       (20)     3451 2020-11-05 17:57:09.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/debug_info.py
+-rw-r--r--   0 klemen     (501) staff       (20)      175 2020-08-31 13:42:08.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/sixeptions.py
+-rw-r--r--   0 klemen     (501) staff       (20)     1183 2021-08-01 13:08:36.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/sqlite_utils.py
+-rw-r--r--   0 klemen     (501) staff       (20)    21698 2021-10-10 11:20:52.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/transporter.py
+drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 12:25:33.611977 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3.egg-info/
+-rw-r--r--   0 klemen     (501) staff       (20)     6136 2021-10-10 12:25:33.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3.egg-info/PKG-INFO
+-rw-r--r--   0 klemen     (501) staff       (20)      874 2021-10-10 12:25:33.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3.egg-info/SOURCES.txt
+-rw-r--r--   0 klemen     (501) staff       (20)        1 2021-10-10 12:25:33.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3.egg-info/dependency_links.txt
+-rw-r--r--   0 klemen     (501) staff       (20)       77 2021-10-10 12:25:33.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3.egg-info/entry_points.txt
+-rw-r--r--   0 klemen     (501) staff       (20)        1 2020-07-18 12:41:59.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3.egg-info/not-zip-safe
+-rw-r--r--   0 klemen     (501) staff       (20)      347 2021-10-10 12:25:33.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3.egg-info/requires.txt
+-rw-r--r--   0 klemen     (501) staff       (20)       17 2021-10-10 12:25:33.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3.egg-info/top_level.txt
+-rw-r--r--   0 klemen     (501) staff       (20)      337 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.9/pytest.ini
+-rw-r--r--   0 klemen     (501) staff       (20)      736 2021-08-07 16:16:06.000000 mysql-to-sqlite3-1.4.9/requirements_dev.txt
+-rw-r--r--   0 klemen     (501) staff       (20)      191 2021-10-10 12:25:33.648235 mysql-to-sqlite3-1.4.9/setup.cfg
+-rw-r--r--   0 klemen     (501) staff       (20)     2486 2021-10-10 11:59:45.000000 mysql-to-sqlite3-1.4.9/setup.py
+drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 12:25:33.628152 mysql-to-sqlite3-1.4.9/tests/
+-rw-r--r--   0 klemen     (501) staff       (20)        0 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.9/tests/__init__.py
+-rw-r--r--   0 klemen     (501) staff       (20)    12783 2020-08-31 13:37:27.000000 mysql-to-sqlite3-1.4.9/tests/conftest.py
+-rw-r--r--   0 klemen     (501) staff       (20)     1321 2020-07-26 12:31:00.000000 mysql-to-sqlite3-1.4.9/tests/database.py
+-rw-r--r--   0 klemen     (501) staff       (20)     3820 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.9/tests/factories.py
+drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 12:25:33.633165 mysql-to-sqlite3-1.4.9/tests/func/
+-rw-r--r--   0 klemen     (501) staff       (20)        0 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.9/tests/func/__init__.py
+-rw-r--r--   0 klemen     (501) staff       (20)    38476 2021-08-07 11:14:10.000000 mysql-to-sqlite3-1.4.9/tests/func/mysql_to_sqlite3_test.py
+-rw-r--r--   0 klemen     (501) staff       (20)    12737 2021-08-07 14:23:37.000000 mysql-to-sqlite3-1.4.9/tests/func/test_cli.py
+-rw-r--r--   0 klemen     (501) staff       (20)     5877 2021-03-04 20:56:52.000000 mysql-to-sqlite3-1.4.9/tests/models.py
+-rw-r--r--   0 klemen     (501) staff       (20)      201 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.9/tests/sixeptions.py
+drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 12:25:33.639234 mysql-to-sqlite3-1.4.9/tests/unit/
+-rw-r--r--   0 klemen     (501) staff       (20)        0 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.9/tests/unit/__init__.py
+-rw-r--r--   0 klemen     (501) staff       (20)    20853 2021-10-10 11:20:52.000000 mysql-to-sqlite3-1.4.9/tests/unit/mysql_to_sqlite3_test.py
```

### Comparing `mysql-to-sqlite3-1.4.8/CODE-OF-CONDUCT.md` & `mysql-to-sqlite3-1.4.9/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mysql-to-sqlite3-1.4.8/LICENSE` & `mysql-to-sqlite3-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql-to-sqlite3-1.4.8/PKG-INFO` & `mysql-to-sqlite3-1.4.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,16 @@
 Metadata-Version: 2.1
 Name: mysql-to-sqlite3
-Version: 1.4.8
+Version: 1.4.9
 Summary: A simple Python tool to transfer data from MySQL to SQLite 3
 Home-page: https://github.com/techouse/mysql-to-sqlite3
 Author: Klemen Tusar
 Author-email: techouse@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/techouse/mysql-to-sqlite3
-Description: [![PyPI](https://img.shields.io/pypi/v/mysql-to-sqlite3)](https://pypi.org/project/mysql-to-sqlite3/)
-        [![Downloads](https://pepy.tech/badge/mysql-to-sqlite3)](https://pepy.tech/project/mysql-to-sqlite3)
-        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mysql-to-sqlite3)](https://pypi.org/project/mysql-to-sqlite3/)
-        [![MySQL Support](https://img.shields.io/static/v1?label=MySQL&message=5.5+|+5.6+|+5.7+|+8.0&color=2b5d80)](https://img.shields.io/static/v1?label=MySQL&message=5.6+|+5.7+|+8.0&color=2b5d80)
-        [![MariaDB Support](https://img.shields.io/static/v1?label=MariaDB&message=5.5+|+10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5+|+10.6&color=C0765A)](https://img.shields.io/static/v1?label=MariaDB&message=10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5&color=C0765A)
-        [![GitHub license](https://img.shields.io/github/license/techouse/mysql-to-sqlite3)](https://github.com/techouse/mysql-to-sqlite3/blob/master/LICENSE)
-        [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE-OF-CONDUCT.md)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
-        [![Codacy Badge](https://api.codacy.com/project/badge/Grade/64aae8e9599746d58d277852b35cc2bd)](https://www.codacy.com/manual/techouse/mysql-to-sqlite3?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=techouse/mysql-to-sqlite3&amp;utm_campaign=Badge_Grade)
-        [![Build Status](https://github.com/techouse/mysql-to-sqlite3/workflows/Test/badge.svg)](https://github.com/techouse/mysql-to-sqlite3/actions?query=workflow%3ATest)
-        [![codecov](https://codecov.io/gh/techouse/mysql-to-sqlite3/branch/master/graph/badge.svg)](https://codecov.io/gh/techouse/mysql-to-sqlite3)
-        [![GitHub stars](https://img.shields.io/github/stars/techouse/mysql-to-sqlite3.svg?style=social&label=Star&maxAge=2592000)](https://github.com/techouse/mysql-to-sqlite3/stargazers)
-        
-        
-        # MySQL to SQLite3
-        
-        #### A simple Python tool to transfer data from MySQL to SQLite 3.
-        
-        This is the long overdue complimentary tool to my [SQLite3 to MySQL](https://github.com/techouse/sqlite3-to-mysql). It 
-        transfers all data from a MySQL database to a SQLite3 database.
-        
-        ### How to run
-        
-        ```bash
-        pip install mysql-to-sqlite3
-        mysql2sqlite --help
-        ```
-        
-        ### Usage
-        ```
-        Usage: mysql2sqlite [OPTIONS]
-        
-          Transfer MySQL to SQLite using the provided CLI options.
-        
-        Options:
-          -f, --sqlite-file PATH          SQLite3 database file  [required]
-          -d, --mysql-database TEXT       MySQL database name  [required]
-          -u, --mysql-user TEXT           MySQL user  [required]
-          -p, --prompt-mysql-password     Prompt for MySQL password
-          --mysql-password TEXT           MySQL password
-          -t, --mysql-tables TUPLE        Transfer only these specific tables (space
-                                          separated table names). Implies --without-
-                                          foreign-keys which inhibits the transfer of
-                                          foreign keys.
-          -L, --limit-rows INTEGER        Transfer only a limited number of rows from
-                                          each table.
-          -C, --collation [BINARY|NOCASE|RTRIM]
-                                          Create datatypes of TEXT affinity using a
-                                          specified collation sequence.  [default:
-                                          BINARY]
-          -K, --prefix-indices            Prefix indices with their corresponding
-                                          tables. This ensures that their names remain
-                                          unique across the SQLite database.
-          -X, --without-foreign-keys      Do not transfer foreign keys.
-          -h, --mysql-host TEXT           MySQL host. Defaults to localhost.
-          -P, --mysql-port INTEGER        MySQL port. Defaults to 3306.
-          -S, --skip-ssl                  Disable MySQL connection encryption.
-          -c, --chunk INTEGER             Chunk reading/writing SQL records
-          -l, --log-file PATH             Log file
-          --json-as-text                  Transfer JSON columns as TEXT.
-          -V, --vacuum                    Use the VACUUM command to rebuild the SQLite
-                                          database file, repacking it into a minimal
-                                          amount of disk space
-          --use-buffered-cursors          Use MySQLCursorBuffered for reading the
-                                          MySQL database. This can be useful in
-                                          situations where multiple queries, with
-                                          small result sets, need to be combined or
-                                          computed with each other.
-          -q, --quiet                     Quiet. Display only errors.
-          --version                       Show the version and exit.
-          --help                          Show this message and exit.
-        ```
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
@@ -93,11 +20,88 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Database
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI](https://img.shields.io/pypi/v/mysql-to-sqlite3)](https://pypi.org/project/mysql-to-sqlite3/)
+[![Downloads](https://pepy.tech/badge/mysql-to-sqlite3)](https://pepy.tech/project/mysql-to-sqlite3)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mysql-to-sqlite3)](https://pypi.org/project/mysql-to-sqlite3/)
+[![MySQL Support](https://img.shields.io/static/v1?label=MySQL&message=5.5+|+5.6+|+5.7+|+8.0&color=2b5d80)](https://img.shields.io/static/v1?label=MySQL&message=5.6+|+5.7+|+8.0&color=2b5d80)
+[![MariaDB Support](https://img.shields.io/static/v1?label=MariaDB&message=5.5+|+10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5+|+10.6&color=C0765A)](https://img.shields.io/static/v1?label=MariaDB&message=10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5&color=C0765A)
+[![GitHub license](https://img.shields.io/github/license/techouse/mysql-to-sqlite3)](https://github.com/techouse/mysql-to-sqlite3/blob/master/LICENSE)
+[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE-OF-CONDUCT.md)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+[![Codacy Badge](https://api.codacy.com/project/badge/Grade/64aae8e9599746d58d277852b35cc2bd)](https://www.codacy.com/manual/techouse/mysql-to-sqlite3?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=techouse/mysql-to-sqlite3&amp;utm_campaign=Badge_Grade)
+[![Build Status](https://github.com/techouse/mysql-to-sqlite3/workflows/Test/badge.svg)](https://github.com/techouse/mysql-to-sqlite3/actions?query=workflow%3ATest)
+[![codecov](https://codecov.io/gh/techouse/mysql-to-sqlite3/branch/master/graph/badge.svg)](https://codecov.io/gh/techouse/mysql-to-sqlite3)
+[![GitHub stars](https://img.shields.io/github/stars/techouse/mysql-to-sqlite3.svg?style=social&label=Star&maxAge=2592000)](https://github.com/techouse/mysql-to-sqlite3/stargazers)
+
+
+# MySQL to SQLite3
+
+#### A simple Python tool to transfer data from MySQL to SQLite 3.
+
+This is the long overdue complimentary tool to my [SQLite3 to MySQL](https://github.com/techouse/sqlite3-to-mysql). It 
+transfers all data from a MySQL database to a SQLite3 database.
+
+### How to run
+
+```bash
+pip install mysql-to-sqlite3
+mysql2sqlite --help
+```
+
+### Usage
+```
+Usage: mysql2sqlite [OPTIONS]
+
+  Transfer MySQL to SQLite using the provided CLI options.
+
+Options:
+  -f, --sqlite-file PATH          SQLite3 database file  [required]
+  -d, --mysql-database TEXT       MySQL database name  [required]
+  -u, --mysql-user TEXT           MySQL user  [required]
+  -p, --prompt-mysql-password     Prompt for MySQL password
+  --mysql-password TEXT           MySQL password
+  -t, --mysql-tables TUPLE        Transfer only these specific tables (space
+                                  separated table names). Implies --without-
+                                  foreign-keys which inhibits the transfer of
+                                  foreign keys.
+  -L, --limit-rows INTEGER        Transfer only a limited number of rows from
+                                  each table.
+  -C, --collation [BINARY|NOCASE|RTRIM]
+                                  Create datatypes of TEXT affinity using a
+                                  specified collation sequence.  [default:
+                                  BINARY]
+  -K, --prefix-indices            Prefix indices with their corresponding
+                                  tables. This ensures that their names remain
+                                  unique across the SQLite database.
+  -X, --without-foreign-keys      Do not transfer foreign keys.
+  -h, --mysql-host TEXT           MySQL host. Defaults to localhost.
+  -P, --mysql-port INTEGER        MySQL port. Defaults to 3306.
+  -S, --skip-ssl                  Disable MySQL connection encryption.
+  -c, --chunk INTEGER             Chunk reading/writing SQL records
+  -l, --log-file PATH             Log file
+  --json-as-text                  Transfer JSON columns as TEXT.
+  -V, --vacuum                    Use the VACUUM command to rebuild the SQLite
+                                  database file, repacking it into a minimal
+                                  amount of disk space
+  --use-buffered-cursors          Use MySQLCursorBuffered for reading the
+                                  MySQL database. This can be useful in
+                                  situations where multiple queries, with
+                                  small result sets, need to be combined or
+                                  computed with each other.
+  -q, --quiet                     Quiet. Display only errors.
+  --version                       Show the version and exit.
+  --help                          Show this message and exit.
+```
+
+
```

### Comparing `mysql-to-sqlite3-1.4.8/README.md` & `mysql-to-sqlite3-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `mysql-to-sqlite3-1.4.8/mysql_to_sqlite3/cli.py` & `mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/cli.py`

 * *Files identical despite different names*

### Comparing `mysql-to-sqlite3-1.4.8/mysql_to_sqlite3/click_utils.py` & `mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/click_utils.py`

 * *Files identical despite different names*

### Comparing `mysql-to-sqlite3-1.4.8/mysql_to_sqlite3/debug_info.py` & `mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/debug_info.py`

 * *Files identical despite different names*

### Comparing `mysql-to-sqlite3-1.4.8/mysql_to_sqlite3/sqlite_utils.py` & `mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `mysql-to-sqlite3-1.4.8/mysql_to_sqlite3/transporter.py` & `mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/transporter.py`

 * *Files identical despite different names*

### Comparing `mysql-to-sqlite3-1.4.8/mysql_to_sqlite3.egg-info/PKG-INFO` & `mysql-to-sqlite3-1.4.9/mysql_to_sqlite3.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,16 @@
 Metadata-Version: 2.1
 Name: mysql-to-sqlite3
-Version: 1.4.8
+Version: 1.4.9
 Summary: A simple Python tool to transfer data from MySQL to SQLite 3
 Home-page: https://github.com/techouse/mysql-to-sqlite3
 Author: Klemen Tusar
 Author-email: techouse@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/techouse/mysql-to-sqlite3
-Description: [![PyPI](https://img.shields.io/pypi/v/mysql-to-sqlite3)](https://pypi.org/project/mysql-to-sqlite3/)
-        [![Downloads](https://pepy.tech/badge/mysql-to-sqlite3)](https://pepy.tech/project/mysql-to-sqlite3)
-        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mysql-to-sqlite3)](https://pypi.org/project/mysql-to-sqlite3/)
-        [![MySQL Support](https://img.shields.io/static/v1?label=MySQL&message=5.5+|+5.6+|+5.7+|+8.0&color=2b5d80)](https://img.shields.io/static/v1?label=MySQL&message=5.6+|+5.7+|+8.0&color=2b5d80)
-        [![MariaDB Support](https://img.shields.io/static/v1?label=MariaDB&message=5.5+|+10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5+|+10.6&color=C0765A)](https://img.shields.io/static/v1?label=MariaDB&message=10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5&color=C0765A)
-        [![GitHub license](https://img.shields.io/github/license/techouse/mysql-to-sqlite3)](https://github.com/techouse/mysql-to-sqlite3/blob/master/LICENSE)
-        [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE-OF-CONDUCT.md)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
-        [![Codacy Badge](https://api.codacy.com/project/badge/Grade/64aae8e9599746d58d277852b35cc2bd)](https://www.codacy.com/manual/techouse/mysql-to-sqlite3?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=techouse/mysql-to-sqlite3&amp;utm_campaign=Badge_Grade)
-        [![Build Status](https://github.com/techouse/mysql-to-sqlite3/workflows/Test/badge.svg)](https://github.com/techouse/mysql-to-sqlite3/actions?query=workflow%3ATest)
-        [![codecov](https://codecov.io/gh/techouse/mysql-to-sqlite3/branch/master/graph/badge.svg)](https://codecov.io/gh/techouse/mysql-to-sqlite3)
-        [![GitHub stars](https://img.shields.io/github/stars/techouse/mysql-to-sqlite3.svg?style=social&label=Star&maxAge=2592000)](https://github.com/techouse/mysql-to-sqlite3/stargazers)
-        
-        
-        # MySQL to SQLite3
-        
-        #### A simple Python tool to transfer data from MySQL to SQLite 3.
-        
-        This is the long overdue complimentary tool to my [SQLite3 to MySQL](https://github.com/techouse/sqlite3-to-mysql). It 
-        transfers all data from a MySQL database to a SQLite3 database.
-        
-        ### How to run
-        
-        ```bash
-        pip install mysql-to-sqlite3
-        mysql2sqlite --help
-        ```
-        
-        ### Usage
-        ```
-        Usage: mysql2sqlite [OPTIONS]
-        
-          Transfer MySQL to SQLite using the provided CLI options.
-        
-        Options:
-          -f, --sqlite-file PATH          SQLite3 database file  [required]
-          -d, --mysql-database TEXT       MySQL database name  [required]
-          -u, --mysql-user TEXT           MySQL user  [required]
-          -p, --prompt-mysql-password     Prompt for MySQL password
-          --mysql-password TEXT           MySQL password
-          -t, --mysql-tables TUPLE        Transfer only these specific tables (space
-                                          separated table names). Implies --without-
-                                          foreign-keys which inhibits the transfer of
-                                          foreign keys.
-          -L, --limit-rows INTEGER        Transfer only a limited number of rows from
-                                          each table.
-          -C, --collation [BINARY|NOCASE|RTRIM]
-                                          Create datatypes of TEXT affinity using a
-                                          specified collation sequence.  [default:
-                                          BINARY]
-          -K, --prefix-indices            Prefix indices with their corresponding
-                                          tables. This ensures that their names remain
-                                          unique across the SQLite database.
-          -X, --without-foreign-keys      Do not transfer foreign keys.
-          -h, --mysql-host TEXT           MySQL host. Defaults to localhost.
-          -P, --mysql-port INTEGER        MySQL port. Defaults to 3306.
-          -S, --skip-ssl                  Disable MySQL connection encryption.
-          -c, --chunk INTEGER             Chunk reading/writing SQL records
-          -l, --log-file PATH             Log file
-          --json-as-text                  Transfer JSON columns as TEXT.
-          -V, --vacuum                    Use the VACUUM command to rebuild the SQLite
-                                          database file, repacking it into a minimal
-                                          amount of disk space
-          --use-buffered-cursors          Use MySQLCursorBuffered for reading the
-                                          MySQL database. This can be useful in
-                                          situations where multiple queries, with
-                                          small result sets, need to be combined or
-                                          computed with each other.
-          -q, --quiet                     Quiet. Display only errors.
-          --version                       Show the version and exit.
-          --help                          Show this message and exit.
-        ```
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
@@ -93,11 +20,88 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Database
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI](https://img.shields.io/pypi/v/mysql-to-sqlite3)](https://pypi.org/project/mysql-to-sqlite3/)
+[![Downloads](https://pepy.tech/badge/mysql-to-sqlite3)](https://pepy.tech/project/mysql-to-sqlite3)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mysql-to-sqlite3)](https://pypi.org/project/mysql-to-sqlite3/)
+[![MySQL Support](https://img.shields.io/static/v1?label=MySQL&message=5.5+|+5.6+|+5.7+|+8.0&color=2b5d80)](https://img.shields.io/static/v1?label=MySQL&message=5.6+|+5.7+|+8.0&color=2b5d80)
+[![MariaDB Support](https://img.shields.io/static/v1?label=MariaDB&message=5.5+|+10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5+|+10.6&color=C0765A)](https://img.shields.io/static/v1?label=MariaDB&message=10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5&color=C0765A)
+[![GitHub license](https://img.shields.io/github/license/techouse/mysql-to-sqlite3)](https://github.com/techouse/mysql-to-sqlite3/blob/master/LICENSE)
+[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE-OF-CONDUCT.md)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+[![Codacy Badge](https://api.codacy.com/project/badge/Grade/64aae8e9599746d58d277852b35cc2bd)](https://www.codacy.com/manual/techouse/mysql-to-sqlite3?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=techouse/mysql-to-sqlite3&amp;utm_campaign=Badge_Grade)
+[![Build Status](https://github.com/techouse/mysql-to-sqlite3/workflows/Test/badge.svg)](https://github.com/techouse/mysql-to-sqlite3/actions?query=workflow%3ATest)
+[![codecov](https://codecov.io/gh/techouse/mysql-to-sqlite3/branch/master/graph/badge.svg)](https://codecov.io/gh/techouse/mysql-to-sqlite3)
+[![GitHub stars](https://img.shields.io/github/stars/techouse/mysql-to-sqlite3.svg?style=social&label=Star&maxAge=2592000)](https://github.com/techouse/mysql-to-sqlite3/stargazers)
+
+
+# MySQL to SQLite3
+
+#### A simple Python tool to transfer data from MySQL to SQLite 3.
+
+This is the long overdue complimentary tool to my [SQLite3 to MySQL](https://github.com/techouse/sqlite3-to-mysql). It 
+transfers all data from a MySQL database to a SQLite3 database.
+
+### How to run
+
+```bash
+pip install mysql-to-sqlite3
+mysql2sqlite --help
+```
+
+### Usage
+```
+Usage: mysql2sqlite [OPTIONS]
+
+  Transfer MySQL to SQLite using the provided CLI options.
+
+Options:
+  -f, --sqlite-file PATH          SQLite3 database file  [required]
+  -d, --mysql-database TEXT       MySQL database name  [required]
+  -u, --mysql-user TEXT           MySQL user  [required]
+  -p, --prompt-mysql-password     Prompt for MySQL password
+  --mysql-password TEXT           MySQL password
+  -t, --mysql-tables TUPLE        Transfer only these specific tables (space
+                                  separated table names). Implies --without-
+                                  foreign-keys which inhibits the transfer of
+                                  foreign keys.
+  -L, --limit-rows INTEGER        Transfer only a limited number of rows from
+                                  each table.
+  -C, --collation [BINARY|NOCASE|RTRIM]
+                                  Create datatypes of TEXT affinity using a
+                                  specified collation sequence.  [default:
+                                  BINARY]
+  -K, --prefix-indices            Prefix indices with their corresponding
+                                  tables. This ensures that their names remain
+                                  unique across the SQLite database.
+  -X, --without-foreign-keys      Do not transfer foreign keys.
+  -h, --mysql-host TEXT           MySQL host. Defaults to localhost.
+  -P, --mysql-port INTEGER        MySQL port. Defaults to 3306.
+  -S, --skip-ssl                  Disable MySQL connection encryption.
+  -c, --chunk INTEGER             Chunk reading/writing SQL records
+  -l, --log-file PATH             Log file
+  --json-as-text                  Transfer JSON columns as TEXT.
+  -V, --vacuum                    Use the VACUUM command to rebuild the SQLite
+                                  database file, repacking it into a minimal
+                                  amount of disk space
+  --use-buffered-cursors          Use MySQLCursorBuffered for reading the
+                                  MySQL database. This can be useful in
+                                  situations where multiple queries, with
+                                  small result sets, need to be combined or
+                                  computed with each other.
+  -q, --quiet                     Quiet. Display only errors.
+  --version                       Show the version and exit.
+  --help                          Show this message and exit.
+```
+
+
```

### Comparing `mysql-to-sqlite3-1.4.8/mysql_to_sqlite3.egg-info/SOURCES.txt` & `mysql-to-sqlite3-1.4.9/mysql_to_sqlite3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mysql-to-sqlite3-1.4.8/requirements_dev.txt` & `mysql-to-sqlite3-1.4.9/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `mysql-to-sqlite3-1.4.8/setup.py` & `mysql-to-sqlite3-1.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Database",
     ],
     project_urls={"Source": about["__url__"]},
     entry_points="""
         [console_scripts]
         mysql2sqlite=mysql_to_sqlite3.cli:cli
```

### Comparing `mysql-to-sqlite3-1.4.8/tests/conftest.py` & `mysql-to-sqlite3-1.4.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mysql-to-sqlite3-1.4.8/tests/database.py` & `mysql-to-sqlite3-1.4.9/tests/database.py`

 * *Files identical despite different names*

### Comparing `mysql-to-sqlite3-1.4.8/tests/factories.py` & `mysql-to-sqlite3-1.4.9/tests/factories.py`

 * *Files identical despite different names*

### Comparing `mysql-to-sqlite3-1.4.8/tests/func/mysql_to_sqlite3_test.py` & `mysql-to-sqlite3-1.4.9/tests/func/mysql_to_sqlite3_test.py`

 * *Files identical despite different names*

### Comparing `mysql-to-sqlite3-1.4.8/tests/func/test_cli.py` & `mysql-to-sqlite3-1.4.9/tests/func/test_cli.py`

 * *Files identical despite different names*

### Comparing `mysql-to-sqlite3-1.4.8/tests/models.py` & `mysql-to-sqlite3-1.4.9/tests/models.py`

 * *Files identical despite different names*

### Comparing `mysql-to-sqlite3-1.4.8/tests/unit/mysql_to_sqlite3_test.py` & `mysql-to-sqlite3-1.4.9/tests/unit/mysql_to_sqlite3_test.py`

 * *Files identical despite different names*

