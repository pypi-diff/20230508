# Comparing `tmp/wmill_pg-1.95.1.tar.gz` & `tmp/wmill_pg-1.96.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wmill_pg-1.95.1.tar", max compression
+gzip compressed data, was "wmill_pg-1.96.0.tar", max compression
```

## Comparing `wmill_pg-1.95.1.tar` & `wmill_pg-1.96.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      326 2023-05-06 10:10:54.105391 wmill_pg-1.95.1/README.md
--rw-r--r--   0        0        0      958 2023-05-06 10:10:54.105391 wmill_pg-1.95.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-06 10:10:54.105391 wmill_pg-1.95.1/wmill_pg/__init__.py
--rw-r--r--   0        0        0     1153 2023-05-06 10:10:54.105391 wmill_pg-1.95.1/wmill_pg/client.py
--rw-r--r--   0        0        0       26 2023-05-06 10:10:54.105391 wmill_pg-1.95.1/wmill_pg/py.typed
--rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 wmill_pg-1.95.1/setup.py
--rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 wmill_pg-1.95.1/PKG-INFO
+-rw-r--r--   0        0        0      326 2023-05-08 17:44:59.113147 wmill_pg-1.96.0/README.md
+-rw-r--r--   0        0        0      958 2023-05-08 17:44:59.113147 wmill_pg-1.96.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-08 17:44:59.113147 wmill_pg-1.96.0/wmill_pg/__init__.py
+-rw-r--r--   0        0        0     1153 2023-05-08 17:44:59.113147 wmill_pg-1.96.0/wmill_pg/client.py
+-rw-r--r--   0        0        0       26 2023-05-08 17:44:59.113147 wmill_pg-1.96.0/wmill_pg/py.typed
+-rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 wmill_pg-1.96.0/setup.py
+-rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 wmill_pg-1.96.0/PKG-INFO
```

### Comparing `wmill_pg-1.95.1/pyproject.toml` & `wmill_pg-1.96.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wmill-pg"
-version = "1.95.1"
+version = "1.96.0"
 description = "An extension client for the wmill client library focused on pg"
 license = "Apache-2.0"
 homepage = "https://windmill.dev"
 documentation = "https://docs.windmill.dev"
 
 authors = ["Ruben Fiszel <ruben@windmill.dev>"]
```

### Comparing `wmill_pg-1.95.1/wmill_pg/client.py` & `wmill_pg-1.96.0/wmill_pg/client.py`

 * *Files identical despite different names*

### Comparing `wmill_pg-1.95.1/setup.py` & `wmill_pg-1.96.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['psycopg2-binary', 'wmill>=1.5.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'wmill-pg',
-    'version': '1.95.1',
+    'version': '1.96.0',
     'description': 'An extension client for the wmill client library focused on pg',
     'long_description': '# wmill\n\nThe postgres extension client for the [Windmill](https://windmill.dev) platform.\n\n[windmill-api](https://pypi.org/project/windmill-api/).\n\n## Quickstart\n\n```python\nimport wmill_pg\n\n\ndef main():\n    my_list = query("UPDATE demo SET value = \'value\' RETURNING key, value")\n    for key, value in my_list:\n        ...\n```\n',
     'author': 'Ruben Fiszel',
     'author_email': 'ruben@windmill.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://windmill.dev',
```

### Comparing `wmill_pg-1.95.1/PKG-INFO` & `wmill_pg-1.96.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmill-pg
-Version: 1.95.1
+Version: 1.96.0
 Summary: An extension client for the wmill client library focused on pg
 Home-page: https://windmill.dev
 License: Apache-2.0
 Author: Ruben Fiszel
 Author-email: ruben@windmill.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

