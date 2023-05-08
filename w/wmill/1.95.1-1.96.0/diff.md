# Comparing `tmp/wmill-1.95.1.tar.gz` & `tmp/wmill-1.96.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wmill-1.95.1.tar", max compression
+gzip compressed data, was "wmill-1.96.0.tar", max compression
```

## Comparing `wmill-1.95.1.tar` & `wmill-1.96.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      796 2023-05-06 10:10:54.105391 wmill-1.95.1/README.md
--rw-r--r--   0        0        0      952 2023-05-06 10:10:54.105391 wmill-1.95.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-06 10:10:54.105391 wmill-1.95.1/wmill/__init__.py
--rw-r--r--   0        0        0    10540 2023-05-06 10:10:54.105391 wmill-1.95.1/wmill/client.py
--rw-r--r--   0        0        0       26 2023-05-06 10:10:54.105391 wmill-1.95.1/wmill/py.typed
--rw-r--r--   0        0        0     1508 1970-01-01 00:00:00.000000 wmill-1.95.1/setup.py
--rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 wmill-1.95.1/PKG-INFO
+-rw-r--r--   0        0        0      796 2023-05-08 17:44:59.113147 wmill-1.96.0/README.md
+-rw-r--r--   0        0        0      952 2023-05-08 17:44:59.113147 wmill-1.96.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-08 17:44:59.113147 wmill-1.96.0/wmill/__init__.py
+-rw-r--r--   0        0        0    10540 2023-05-08 17:44:59.113147 wmill-1.96.0/wmill/client.py
+-rw-r--r--   0        0        0       26 2023-05-08 17:44:59.113147 wmill-1.96.0/wmill/py.typed
+-rw-r--r--   0        0        0     1508 1970-01-01 00:00:00.000000 wmill-1.96.0/setup.py
+-rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 wmill-1.96.0/PKG-INFO
```

### Comparing `wmill-1.95.1/README.md` & `wmill-1.96.0/README.md`

 * *Files identical despite different names*

### Comparing `wmill-1.95.1/pyproject.toml` & `wmill-1.96.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wmill"
-version = "1.95.1"
+version = "1.96.0"
 description = "A client library for accessing Windmill server wrapping the Windmill client API"
 license = "Apache-2.0"
 homepage = "https://windmill.dev"
 documentation = "https://docs.windmill.dev"
 
 authors = ["Ruben Fiszel <ruben@windmill.dev>"]
 
@@ -12,15 +12,15 @@
 packages = [
     {include = "wmill"},
 ]
 include = ["wmill/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-windmill-api = "^1.95.1"
+windmill-api = "^1.96.0"
 
 [build-system]
 requires = ["poetry>=1.0.2", "poetry-dynamic-versioning"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry-dynamic-versioning]
 enable = true
```

### Comparing `wmill-1.95.1/wmill/client.py` & `wmill-1.96.0/wmill/client.py`

 * *Files identical despite different names*

### Comparing `wmill-1.95.1/setup.py` & `wmill-1.96.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['wmill']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['windmill-api>=1.95.1,<2.0.0']
+['windmill-api>=1.96.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'wmill',
-    'version': '1.95.1',
+    'version': '1.96.0',
     'description': 'A client library for accessing Windmill server wrapping the Windmill client API',
     'long_description': '# wmill\n\nThe core client for the [Windmill](https://windmill.dev) platform.\n\nIt is a convenient wrapper around the exhaustive, automatically generated from\nOpenApi but less user-friendly\n[windmill-api](https://pypi.org/project/windmill-api/).\n\n## Quickstart\n\n```python\nimport wmill\n\n\ndef main():\n    #os.environ.set("WM_TOKEN", "<mytoken>") OPTIONAL to set token used by the wmill client\n    version = wmill.get_version()\n    resource = wmill.get_resource("u/user/resource_path")\n\n    # run synchronously, will return the result\n    res = wmill.run_script_sync(hash="000000000000002a", args={})\n    print(res)\n\n    for _ in range(3):\n        # run asynchrnously, will return immediately. Can be scheduled\n        wmill.run_script_async(hash="000000000000002a", args={}, scheduled_in_secs=10)\n```\n',
     'author': 'Ruben Fiszel',
     'author_email': 'ruben@windmill.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://windmill.dev',
```

### Comparing `wmill-1.95.1/PKG-INFO` & `wmill-1.96.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: wmill
-Version: 1.95.1
+Version: 1.96.0
 Summary: A client library for accessing Windmill server wrapping the Windmill client API
 Home-page: https://windmill.dev
 License: Apache-2.0
 Author: Ruben Fiszel
 Author-email: ruben@windmill.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: windmill-api (>=1.95.1,<2.0.0)
+Requires-Dist: windmill-api (>=1.96.0,<2.0.0)
 Project-URL: Documentation, https://docs.windmill.dev
 Description-Content-Type: text/markdown
 
 # wmill
 
 The core client for the [Windmill](https://windmill.dev) platform.
```

