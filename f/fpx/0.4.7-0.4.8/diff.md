# Comparing `tmp/fpx-0.4.7.tar.gz` & `tmp/fpx-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpx-0.4.7.tar", last modified: Fri Nov 25 19:13:45 2022, max compression
+gzip compressed data, was "fpx-0.4.8.tar", last modified: Mon May  8 06:52:38 2023, max compression
```

## Comparing `fpx-0.4.7.tar` & `fpx-0.4.8.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-11-25 19:13:45.153078 fpx-0.4.7/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       53 2022-08-02 11:55:50.000000 fpx-0.4.7/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6426 2022-11-25 19:13:45.153078 fpx-0.4.7/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5862 2022-09-19 11:20:13.000000 fpx-0.4.7/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-11-25 19:13:45.143078 fpx-0.4.7/fpx/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)       59 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/__main__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2012 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/alembic.ini
--rw-r--r--   0 sergey    (1000) sergey    (1000)      937 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/app.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-11-25 19:13:45.143078 fpx-0.4.7/fpx/cli/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      299 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/cli/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1217 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/cli/client.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      787 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/cli/db.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      161 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/cli/server.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      759 2022-08-07 18:43:59.000000 fpx-0.4.7/fpx/cli/ticket.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1161 2022-11-25 15:12:26.000000 fpx-0.4.7/fpx/config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      464 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/context.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      343 2022-09-12 10:40:24.000000 fpx-0.4.7/fpx/exception.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      997 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/middleware.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-11-25 19:13:45.143078 fpx-0.4.7/fpx/migrations/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/migrations/README
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/migrations/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-11-25 19:13:45.143078 fpx-0.4.7/fpx/migrations/__pycache__/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1610 2022-08-02 11:59:46.000000 fpx-0.4.7/fpx/migrations/__pycache__/env.cpython-38.pyc
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2016 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/migrations/env.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/migrations/script.py.mako
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-11-25 19:13:45.143078 fpx-0.4.7/fpx/migrations/versions/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      512 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/migrations/versions/6a22a6995723_create_clients_table.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-11-25 19:13:45.143078 fpx-0.4.7/fpx/migrations/versions/__pycache__/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      826 2022-08-02 11:59:46.000000 fpx-0.4.7/fpx/migrations/versions/__pycache__/6a22a6995723_create_clients_table.cpython-38.pyc
--rw-r--r--   0 sergey    (1000) sergey    (1000)      862 2022-08-02 11:59:46.000000 fpx-0.4.7/fpx/migrations/versions/__pycache__/ac8a8750d3e2_add_options_column_to_ticket_table.cpython-38.pyc
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1023 2022-08-02 11:59:46.000000 fpx-0.4.7/fpx/migrations/versions/__pycache__/ef515c12c8ff_create_tickets_table.cpython-38.pyc
--rw-r--r--   0 sergey    (1000) sergey    (1000)      514 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/migrations/versions/ac8a8750d3e2_add_options_column_to_ticket_table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      805 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/migrations/versions/ef515c12c8ff_create_tickets_table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1770 2022-08-08 20:16:28.000000 fpx-0.4.7/fpx/model.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5024 2022-11-25 15:12:04.000000 fpx-0.4.7/fpx/pipes.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-11-25 19:13:45.143078 fpx-0.4.7/fpx/route/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      573 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/route/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1744 2022-11-25 15:09:55.000000 fpx-0.4.7/fpx/route/stream.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4384 2022-11-25 15:10:02.000000 fpx-0.4.7/fpx/route/ticket.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2586 2022-09-12 10:40:24.000000 fpx-0.4.7/fpx/schema.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-11-25 19:13:45.153078 fpx-0.4.7/fpx/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1820 2022-08-08 18:07:39.000000 fpx-0.4.7/fpx/tests/conftest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-11-25 19:13:45.153078 fpx-0.4.7/fpx/tests/route/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/tests/route/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1337 2022-11-25 19:12:42.000000 fpx-0.4.7/fpx/tests/route/test_stream.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7235 2022-11-25 19:12:05.000000 fpx-0.4.7/fpx/tests/route/test_ticket.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)       26 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/tests/settings.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      483 2022-08-02 11:55:50.000000 fpx-0.4.7/fpx/tests/test_model.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2441 2022-09-20 13:44:49.000000 fpx-0.4.7/fpx/utils.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-11-25 19:13:45.143078 fpx-0.4.7/fpx.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6426 2022-11-25 19:13:45.000000 fpx-0.4.7/fpx.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1338 2022-11-25 19:13:45.000000 fpx-0.4.7/fpx.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2022-11-25 19:13:45.000000 fpx-0.4.7/fpx.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       36 2022-11-25 19:13:45.000000 fpx-0.4.7/fpx.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      256 2022-11-25 19:13:45.000000 fpx-0.4.7/fpx.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        4 2022-11-25 19:13:45.000000 fpx-0.4.7/fpx.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      860 2022-08-02 11:55:50.000000 fpx-0.4.7/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1071 2022-11-25 19:13:45.153078 fpx-0.4.7/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2022-08-02 11:55:50.000000 fpx-0.4.7/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-08 06:52:38.627540 fpx-0.4.8/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       53 2022-08-02 11:55:50.000000 fpx-0.4.8/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6426 2023-05-08 06:52:38.627540 fpx-0.4.8/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5862 2022-09-19 11:20:13.000000 fpx-0.4.8/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-08 06:52:38.627540 fpx-0.4.8/fpx/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       59 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/__main__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2012 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/alembic.ini
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      937 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/app.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-08 06:52:38.627540 fpx-0.4.8/fpx/cli/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      299 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/cli/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1217 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/cli/client.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      787 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/cli/db.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      161 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/cli/server.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      759 2022-08-07 18:43:59.000000 fpx-0.4.8/fpx/cli/ticket.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1161 2022-11-25 15:12:26.000000 fpx-0.4.8/fpx/config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      464 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/context.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      343 2022-09-12 10:40:24.000000 fpx-0.4.8/fpx/exception.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      997 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/middleware.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-08 06:52:38.627540 fpx-0.4.8/fpx/migrations/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/migrations/README
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/migrations/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-08 06:52:38.627540 fpx-0.4.8/fpx/migrations/__pycache__/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1610 2022-08-02 11:59:46.000000 fpx-0.4.8/fpx/migrations/__pycache__/env.cpython-38.pyc
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2016 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/migrations/env.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/migrations/script.py.mako
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-08 06:52:38.627540 fpx-0.4.8/fpx/migrations/versions/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      512 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/migrations/versions/6a22a6995723_create_clients_table.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-08 06:52:38.627540 fpx-0.4.8/fpx/migrations/versions/__pycache__/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      826 2022-08-02 11:59:46.000000 fpx-0.4.8/fpx/migrations/versions/__pycache__/6a22a6995723_create_clients_table.cpython-38.pyc
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      862 2022-08-02 11:59:46.000000 fpx-0.4.8/fpx/migrations/versions/__pycache__/ac8a8750d3e2_add_options_column_to_ticket_table.cpython-38.pyc
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1023 2022-08-02 11:59:46.000000 fpx-0.4.8/fpx/migrations/versions/__pycache__/ef515c12c8ff_create_tickets_table.cpython-38.pyc
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      514 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/migrations/versions/ac8a8750d3e2_add_options_column_to_ticket_table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      805 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/migrations/versions/ef515c12c8ff_create_tickets_table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1770 2022-08-08 20:16:28.000000 fpx-0.4.8/fpx/model.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5024 2022-11-25 15:12:04.000000 fpx-0.4.8/fpx/pipes.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-08 06:52:38.627540 fpx-0.4.8/fpx/route/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      573 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/route/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1744 2022-11-25 15:09:55.000000 fpx-0.4.8/fpx/route/stream.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4384 2022-12-12 14:41:03.000000 fpx-0.4.8/fpx/route/ticket.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2586 2022-09-12 10:40:24.000000 fpx-0.4.8/fpx/schema.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-08 06:52:38.627540 fpx-0.4.8/fpx/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1844 2023-05-08 06:28:45.000000 fpx-0.4.8/fpx/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-08 06:52:38.627540 fpx-0.4.8/fpx/tests/route/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/tests/route/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1337 2022-11-25 19:12:42.000000 fpx-0.4.8/fpx/tests/route/test_stream.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7235 2022-11-25 19:12:05.000000 fpx-0.4.8/fpx/tests/route/test_ticket.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       26 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/tests/settings.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      483 2022-08-02 11:55:50.000000 fpx-0.4.8/fpx/tests/test_model.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2441 2022-09-20 13:44:49.000000 fpx-0.4.8/fpx/utils.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-08 06:52:38.627540 fpx-0.4.8/fpx.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6426 2023-05-08 06:52:38.000000 fpx-0.4.8/fpx.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1338 2023-05-08 06:52:38.000000 fpx-0.4.8/fpx.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-05-08 06:52:38.000000 fpx-0.4.8/fpx.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       36 2023-05-08 06:52:38.000000 fpx-0.4.8/fpx.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      287 2023-05-08 06:52:38.000000 fpx-0.4.8/fpx.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        4 2023-05-08 06:52:38.000000 fpx-0.4.8/fpx.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      860 2022-08-02 11:55:50.000000 fpx-0.4.8/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1104 2023-05-08 06:52:38.627540 fpx-0.4.8/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2022-08-02 11:55:50.000000 fpx-0.4.8/setup.py
```

### Comparing `fpx-0.4.7/PKG-INFO` & `fpx-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpx
-Version: 0.4.7
+Version: 0.4.8
 Summary: Stream archiver/proxy
 Home-page: https://github.com/DataShades/fpx
 Author: Sergey Motornyuk
 License: AGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `fpx-0.4.7/README.md` & `fpx-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/alembic.ini` & `fpx-0.4.8/fpx/alembic.ini`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/app.py` & `fpx-0.4.8/fpx/app.py`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/cli/client.py` & `fpx-0.4.8/fpx/cli/client.py`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/cli/db.py` & `fpx-0.4.8/fpx/cli/db.py`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/cli/ticket.py` & `fpx-0.4.8/fpx/cli/ticket.py`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/config.py` & `fpx-0.4.8/fpx/config.py`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/middleware.py` & `fpx-0.4.8/fpx/middleware.py`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/migrations/__pycache__/env.cpython-38.pyc` & `fpx-0.4.8/fpx/migrations/__pycache__/env.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/migrations/env.py` & `fpx-0.4.8/fpx/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/migrations/versions/6a22a6995723_create_clients_table.py` & `fpx-0.4.8/fpx/migrations/versions/6a22a6995723_create_clients_table.py`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/migrations/versions/__pycache__/6a22a6995723_create_clients_table.cpython-38.pyc` & `fpx-0.4.8/fpx/migrations/versions/__pycache__/6a22a6995723_create_clients_table.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/migrations/versions/__pycache__/ac8a8750d3e2_add_options_column_to_ticket_table.cpython-38.pyc` & `fpx-0.4.8/fpx/migrations/versions/__pycache__/ac8a8750d3e2_add_options_column_to_ticket_table.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/migrations/versions/__pycache__/ef515c12c8ff_create_tickets_table.cpython-38.pyc` & `fpx-0.4.8/fpx/migrations/versions/__pycache__/ef515c12c8ff_create_tickets_table.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/migrations/versions/ac8a8750d3e2_add_options_column_to_ticket_table.py` & `fpx-0.4.8/fpx/migrations/versions/ac8a8750d3e2_add_options_column_to_ticket_table.py`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/migrations/versions/ef515c12c8ff_create_tickets_table.py` & `fpx-0.4.8/fpx/migrations/versions/ef515c12c8ff_create_tickets_table.py`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/model.py` & `fpx-0.4.8/fpx/model.py`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/pipes.py` & `fpx-0.4.8/fpx/pipes.py`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/route/__init__.py` & `fpx-0.4.8/fpx/route/__init__.py`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/route/stream.py` & `fpx-0.4.8/fpx/route/stream.py`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/route/ticket.py` & `fpx-0.4.8/fpx/route/ticket.py`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/schema.py` & `fpx-0.4.8/fpx/schema.py`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/tests/conftest.py` & `fpx-0.4.8/fpx/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import factory
 import pytest
+from sanic import Sanic
 from aioresponses import aioresponses
 from pytest_factoryboy import register
 
 # from sanic_testing import TestManager
 from sanic_testing.reusable import ReusableClient
 
 from fpx.app import make_app
```

### Comparing `fpx-0.4.7/fpx/tests/route/test_stream.py` & `fpx-0.4.8/fpx/tests/route/test_stream.py`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/tests/route/test_ticket.py` & `fpx-0.4.8/fpx/tests/route/test_ticket.py`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx/utils.py` & `fpx-0.4.8/fpx/utils.py`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/fpx.egg-info/PKG-INFO` & `fpx-0.4.8/fpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpx
-Version: 0.4.7
+Version: 0.4.8
 Summary: Stream archiver/proxy
 Home-page: https://github.com/DataShades/fpx
 Author: Sergey Motornyuk
 License: AGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `fpx-0.4.7/fpx.egg-info/SOURCES.txt` & `fpx-0.4.8/fpx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/pyproject.toml` & `fpx-0.4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fpx-0.4.7/setup.cfg` & `fpx-0.4.8/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fpx
-version = 0.4.7
+version = 0.4.8
 description = Stream archiver/proxy
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Sergey Motornyuk
 url = https://github.com/DataShades/fpx
 license = AGPL
 classifiers = 
@@ -23,20 +23,21 @@
 	asyncblink==0.3.2
 	sqlalchemy~=1.4.0
 	alembic~=1.4.0
 	aiohttp[speedups]~=3.8.0
 	click
 	webargs-sanic~=2.2.0
 	pyjwt
+	websockets>=10.0, <11.0
 
 [options.extras_require]
 postgresql = 
 	psycopg2
 test = 
-	sanic-testing
+	sanic-testing~=22.6.0
 	pytest
 	pytest-asyncio
 	factory_boy
 	pytest-factoryboy
 	aioresponses
 
 [options.package_data]
```

