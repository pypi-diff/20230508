# Comparing `tmp/test_jfq_project-0.1.3.tar.gz` & `tmp/test_jfq_project-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_jfq_project-0.1.3.tar", max compression
+gzip compressed data, was "test_jfq_project-0.1.8.tar", max compression
```

## Comparing `test_jfq_project-0.1.3.tar` & `test_jfq_project-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2861 2023-05-05 17:57:59.418778 test_jfq_project-0.1.3/README.md
--rw-r--r--   0        0        0     2187 2023-05-05 17:57:59.422778 test_jfq_project-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       50 2023-05-05 17:57:59.422778 test_jfq_project-0.1.3/src/my_project/__init__.py
--rw-r--r--   0        0        0       50 2023-05-05 17:57:59.422778 test_jfq_project-0.1.3/src/my_project/main.py
--rw-r--r--   0        0        0        0 2023-05-05 17:57:59.422778 test_jfq_project-0.1.3/src/my_project/py.typed
--rw-r--r--   0        0        0     4102 1970-01-01 00:00:00.000000 test_jfq_project-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2861 2023-05-08 11:39:28.943526 test_jfq_project-0.1.8/README.md
+-rw-r--r--   0        0        0     2187 2023-05-08 11:39:28.947526 test_jfq_project-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-05-08 11:39:28.947526 test_jfq_project-0.1.8/src/my_project/__init__.py
+-rw-r--r--   0        0        0       50 2023-05-08 11:39:28.947526 test_jfq_project-0.1.8/src/my_project/main.py
+-rw-r--r--   0        0        0        0 2023-05-08 11:39:28.947526 test_jfq_project-0.1.8/src/my_project/py.typed
+-rw-r--r--   0        0        0     4102 1970-01-01 00:00:00.000000 test_jfq_project-0.1.8/PKG-INFO
```

### Comparing `test_jfq_project-0.1.3/README.md` & `test_jfq_project-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `test_jfq_project-0.1.3/pyproject.toml` & `test_jfq_project-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "test_jfq_project"
-version = "0.1.3"
+version = "0.1.8"
 description = "Short Description"
 authors = [
     "JFQ <quinonesjuanfacundo@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `test_jfq_project-0.1.3/PKG-INFO` & `test_jfq_project-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-jfq-project
-Version: 0.1.3
+Version: 0.1.8
 Summary: Short Description
 Home-page: https://jfquinones.github.io/my_project
 License: MIT
 Author: JFQ
 Author-email: quinonesjuanfacundo@gmail.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: Development Status :: 4 - Beta
```

