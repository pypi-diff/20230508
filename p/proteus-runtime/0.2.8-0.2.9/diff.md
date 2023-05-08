# Comparing `tmp/proteus_runtime-0.2.8.tar.gz` & `tmp/proteus_runtime-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteus_runtime-0.2.8.tar", max compression
+gzip compressed data, was "proteus_runtime-0.2.9.tar", max compression
```

## Comparing `proteus_runtime-0.2.8.tar` & `proteus_runtime-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2023-01-17 16:59:14.573635 proteus_runtime-0.2.8/LICENSE
--rw-r--r--   0        0        0     2643 2023-01-17 16:59:14.573635 proteus_runtime-0.2.8/proteus/__init__.py
--rw-r--r--   0        0        0     6699 2023-01-17 16:59:14.573635 proteus_runtime-0.2.8/proteus/api.py
--rw-r--r--   0        0        0        0 2023-01-17 16:59:14.573635 proteus_runtime-0.2.8/proteus/calculator/__init__.py
--rw-r--r--   0        0        0      258 2023-01-17 16:59:14.573635 proteus_runtime-0.2.8/proteus/calculator/calculator.py
--rw-r--r--   0        0        0      475 2023-01-17 16:59:14.573635 proteus_runtime-0.2.8/proteus/calculator/grammar.py
--rw-r--r--   0        0        0     2150 2023-01-17 16:59:14.573635 proteus_runtime-0.2.8/proteus/calculator/operations.py
--rw-r--r--   0        0        0      371 2023-01-17 16:59:14.573635 proteus_runtime-0.2.8/proteus/calculator/parser.py
--rw-r--r--   0        0        0      507 2023-01-17 16:59:14.573635 proteus_runtime-0.2.8/proteus/config.py
--rw-r--r--   0        0        0     1109 2023-01-17 16:59:14.573635 proteus_runtime-0.2.8/proteus/logger.py
--rw-r--r--   0        0        0     6618 2023-01-17 16:59:14.573635 proteus_runtime-0.2.8/proteus/oidc.py
--rw-r--r--   0        0        0     2595 2023-01-17 16:59:14.573635 proteus_runtime-0.2.8/proteus/reporting.py
--rw-r--r--   0        0        0     1432 2023-01-17 16:59:14.573635 proteus_runtime-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      825 1970-01-01 00:00:00.000000 proteus_runtime-0.2.8/setup.py
--rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 proteus_runtime-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/LICENSE
+-rw-r--r--   0        0        0     2851 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/__init__.py
+-rw-r--r--   0        0        0     7519 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/api.py
+-rw-r--r--   0        0        0        0 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/calculator/__init__.py
+-rw-r--r--   0        0        0      258 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/calculator/calculator.py
+-rw-r--r--   0        0        0      518 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/calculator/grammar.py
+-rw-r--r--   0        0        0     2150 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/calculator/operations.py
+-rw-r--r--   0        0        0      371 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/calculator/parser.py
+-rw-r--r--   0        0        0      507 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/config.py
+-rw-r--r--   0        0        0     1109 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/logger.py
+-rw-r--r--   0        0        0     6652 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/oidc.py
+-rw-r--r--   0        0        0     2595 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/reporting.py
+-rw-r--r--   0        0        0     1462 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      825 1970-01-01 00:00:00.000000 proteus_runtime-0.2.9/setup.py
+-rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 proteus_runtime-0.2.9/PKG-INFO
```

### Comparing `proteus_runtime-0.2.8/LICENSE` & `proteus_runtime-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `proteus_runtime-0.2.8/proteus/__init__.py` & `proteus_runtime-0.2.9/proteus/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,19 @@
             @wraps(fn)
             def wrapped(*args, **kwargs):
                 failures = 0
                 while True:
                     try:
                         res = fn(*args, **kwargs)
                         if failures > 0:
-                            logger.warning(f"The process tried: {failures} times")
+                            logger.warning(
+                                f'Call to function "{fn.__name__}" was successful '
+                                f"after {failures} failed "
+                                f"attemp{'' if failures == 1 else 's' }"
+                            )
                         return res
                     except BaseException:
                         failures += 1
                         if failures < times:
                             time.sleep(delay_in_secs)
                         else:
                             raise
```

### Comparing `proteus_runtime-0.2.8/proteus/api.py` & `proteus_runtime-0.2.9/proteus/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import json
 import os
+import uuid
 from copy import deepcopy, copy
 from urllib.parse import urlencode, quote_plus
 
 import requests
-from azure.storage.blob import BlobClient
-from proteus.config import Config
+from azure.storage.blob import BlobClient, BlobBlock
 from requests import Response, HTTPError, JSONDecodeError
 
+from proteus.config import Config
+
 
 class API:
+
+    CONTENT_CHUNK_SIZE = 10 * 1024 * 1024
+
     def __init__(self, auth, config: Config, logger):
         self.auth = auth
         self.config = deepcopy(config or Config())
         self.host = config.api_host
         self.logger = logger
 
     def get(self, url, headers=None, stream=False, **query_args):
@@ -86,22 +91,45 @@
         file_info = original_response.json()["file"]
         assert file_info["ready"] is False
         assert "presigned_url" in file_info, "The file upload is not ready, but no presigned URL was attached"
         assert len(files) == 1
 
         file = next(iter(files.values()))[1]
 
-        # If the file is an stream, ensure it has been rewound
+        # If the file is a stream, ensure it has been rewound
         if hasattr(file, "seek"):
             file.seek(0)
             assert file.tell() == 0
         else:
             assert isinstance(file, (bytes, str))
 
-        BlobClient.from_blob_url(file_info["presigned_url"]["url"]).upload_blob(file, overwrite=True)
+        client = BlobClient.from_blob_url(file_info["presigned_url"]["url"])
+
+        block_list = []
+        block_ids = set()
+        pos = 0
+        while True:
+            if hasattr(file, "read"):
+                chunk = file.read(self.CONTENT_CHUNK_SIZE)
+            else:
+                chunk = file[pos : pos + self.CONTENT_CHUNK_SIZE]
+                pos += self.CONTENT_CHUNK_SIZE
+            if len(chunk) > 0:
+                block_id = str(uuid.uuid4())
+                while block_id in block_ids:
+                    block_id = str(uuid.uuid4())
+
+                client.stage_block(block_id=block_id, data=chunk)
+                block_list.append(BlobBlock(block_id=block_id))
+                block_ids.add(block_id)
+
+            if len(chunk) < self.CONTENT_CHUNK_SIZE:
+                break
+
+        client.commit_block_list(block_list)
 
         response = self.put(
             f'/api/v1/buckets/{file_info["presigned_url"]["bucket_uuid"]}/files/{file_info["uuid"]}',
             {"file": {"ready": True}},
         )
 
         try:
```

### Comparing `proteus_runtime-0.2.8/proteus/calculator/operations.py` & `proteus_runtime-0.2.9/proteus/calculator/operations.py`

 * *Files identical despite different names*

### Comparing `proteus_runtime-0.2.8/proteus/logger.py` & `proteus_runtime-0.2.9/proteus/logger.py`

 * *Files identical despite different names*

### Comparing `proteus_runtime-0.2.8/proteus/oidc.py` & `proteus_runtime-0.2.9/proteus/oidc.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
             refresh["client_secret"] = self.client_secret
         try:
             response = self.send_refresh_request(refresh)
             credentials = response.json()
             assert credentials.get("access_token") is not None
             self._update_credentials(**credentials)
         except Exception:
-            self.proteus.logger.error("Failed.")
+            self.proteus.logger.error("Failed to refresh token, re-loging againg")
             return self.do_login()
         finally:
             self._access_token_locked.release()
         if self._when_refresh_callback is not None:
             self._when_refresh_callback()
 
     def stop(self):
```

### Comparing `proteus_runtime-0.2.8/proteus/reporting.py` & `proteus_runtime-0.2.9/proteus/reporting.py`

 * *Files identical despite different names*

### Comparing `proteus_runtime-0.2.8/pyproject.toml` & `proteus_runtime-0.2.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proteus-runtime"
-version = "0.2.8"
+version = "0.2.9"
 description = ""
 authors = []
 packages = [
     { include = "proteus" },
 ]
 
 [tool.poetry.dependencies]
@@ -36,14 +36,15 @@
     test = ['flake8', 'black_check', 'pytest']
     format = ["black_format"]
 
     [tool.poe.tasks.flake8]
         cmd="""
             flake8 proteus
                 --max-line-length=120
+                --ignore=E203
         """
         help="Check code style using flake8"
     [tool.poe.tasks.black_check]
         cmd="""
             black proteus --check --diff
                 --line-length=120
         """
```

### Comparing `proteus_runtime-0.2.8/setup.py` & `proteus_runtime-0.2.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'parglare>=0.16.0,<0.17.0',
  'python-json-logger>=2.0.4,<3.0.0',
  'requests>=2.28.1,<3.0.0',
  'setuptools>=65.0.0,<66.0.0']
 
 setup_kwargs = {
     'name': 'proteus-runtime',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': '',
     'long_description': 'None',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `proteus_runtime-0.2.8/PKG-INFO` & `proteus_runtime-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteus-runtime
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

