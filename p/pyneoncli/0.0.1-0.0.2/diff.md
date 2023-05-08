# Comparing `tmp/pyneoncli-0.0.1.tar.gz` & `tmp/pyneoncli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneoncli-0.0.1.tar", max compression
+gzip compressed data, was "pyneoncli-0.0.2.tar", max compression
```

## Comparing `pyneoncli-0.0.1.tar` & `pyneoncli-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-05-08 12:47:09.933275 pyneoncli-0.0.1/LICENSE
--rw-r--r--   0        0        0       11 2023-05-08 12:47:09.933361 pyneoncli-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-08 12:47:09.933740 pyneoncli-0.0.1/pyneoncli/__init__.py
--rw-r--r--   0        0        0      487 2023-05-08 15:07:42.127080 pyneoncli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 pyneoncli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-08 12:47:09.933275 pyneoncli-0.0.2/LICENSE
+-rw-r--r--   0        0        0      299 2023-05-08 18:06:57.594209 pyneoncli-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 12:47:09.933740 pyneoncli-0.0.2/pyneoncli/__init__.py
+-rw-r--r--   0        0        0     2082 2023-05-08 18:32:25.736376 pyneoncli-0.0.2/pyneoncli/cli_main.py
+-rw-r--r--   0        0        0      565 2023-05-08 18:32:33.727989 pyneoncli-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 pyneoncli-0.0.2/PKG-INFO
```

### Comparing `pyneoncli-0.0.1/LICENSE` & `pyneoncli-0.0.2/LICENSE`

 * *Files identical despite different names*

