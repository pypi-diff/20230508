# Comparing `tmp/octo_api_client-1.1.3.tar.gz` & `tmp/octo_api_client-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octo_api_client-1.1.3.tar", max compression
+gzip compressed data, was "octo_api_client-1.1.4.tar", max compression
```

## Comparing `octo_api_client-1.1.3.tar` & `octo_api_client-1.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      690 2023-04-20 13:13:48.852958 octo_api_client-1.1.3/README.md
--rw-r--r--   0        0        0      111 2023-04-20 13:13:48.852958 octo_api_client-1.1.3/octo_client/__init__.py
--rw-r--r--   0        0        0    19611 2023-04-20 13:13:48.852958 octo_api_client-1.1.3/octo_client/client.py
--rw-r--r--   0        0        0     2391 2023-04-20 13:13:48.852958 octo_api_client-1.1.3/octo_client/const.py
--rw-r--r--   0        0        0      426 2023-04-20 13:13:48.852958 octo_api_client-1.1.3/octo_client/exceptions.py
--rw-r--r--   0        0        0    11968 2023-04-20 13:13:48.852958 octo_api_client-1.1.3/octo_client/models.py
--rw-r--r--   0        0        0     1110 2023-04-20 13:13:48.852958 octo_api_client-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1406 1970-01-01 00:00:00.000000 octo_api_client-1.1.3/setup.py
--rw-r--r--   0        0        0     1376 1970-01-01 00:00:00.000000 octo_api_client-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      690 2023-05-08 08:57:27.524437 octo_api_client-1.1.4/README.md
+-rw-r--r--   0        0        0      111 2023-05-08 08:57:27.524437 octo_api_client-1.1.4/octo_client/__init__.py
+-rw-r--r--   0        0        0    20193 2023-05-08 08:57:27.524437 octo_api_client-1.1.4/octo_client/client.py
+-rw-r--r--   0        0        0     2391 2023-05-08 08:57:27.524437 octo_api_client-1.1.4/octo_client/const.py
+-rw-r--r--   0        0        0      426 2023-05-08 08:57:27.524437 octo_api_client-1.1.4/octo_client/exceptions.py
+-rw-r--r--   0        0        0    11968 2023-05-08 08:57:27.524437 octo_api_client-1.1.4/octo_client/models.py
+-rw-r--r--   0        0        0     1110 2023-05-08 08:57:27.524437 octo_api_client-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1406 1970-01-01 00:00:00.000000 octo_api_client-1.1.4/setup.py
+-rw-r--r--   0        0        0     1376 1970-01-01 00:00:00.000000 octo_api_client-1.1.4/PKG-INFO
```

### Comparing `octo_api_client-1.1.3/README.md` & `octo_api_client-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `octo_api_client-1.1.3/octo_client/client.py` & `octo_api_client-1.1.4/octo_client/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         """
         self.url = url.rstrip("/")
         self.token = token
         self.logger = custom_logger or logger
         self.supplier_url_map: Dict[str, str] = {}
         self.requests_loglevel = requests_loglevel
         self.log_responses = False
+        self.log_requests = False
         self.log_size_limit = log_size_limit
         self.language = language
         self.strict = strict
 
     @staticmethod
     def _raise_for_status(status_code: int, response_text: str) -> None:
         CODE_EXCEPTION_MAP = {
@@ -96,30 +97,37 @@
         json=None,
         params=None,
         headers=None,
     ):
         if headers is None:
             headers = {}
 
-        if supplier_id:
-            full_url: str = self._build_endpoint_url_for_request(str(supplier_id), path)
-        else:
-            full_url = f"{self.url}/{path}"
+        if params is None:
+            params = {}
+
+        full_url: str = (
+            self._build_endpoint_url_for_request(str(supplier_id), path)
+            if supplier_id
+            else f"{self.url}/{path}"
+        )
+
+        request_log_data: dict = {"json": json, "params": params}
 
         self.logger.log(
             self.requests_loglevel,
             "Sending request to %s (%s)",
             full_url,
             http_method.__name__.upper(),
+            extra={"request": self._filter_request_log_data(len(str(request_log_data)), request_log_data)},
         )
         base_headers = self._get_headers()
         headers = {**base_headers, **headers}
         response = http_method(
             full_url,
-            params=params or {},
+            params=params,
             json=json,
             headers=headers,
         )
         self._raise_for_status(response.status_code, response.text)
         try:
             response_json = response.json()
         except Exception as exc:
@@ -134,16 +142,25 @@
             "Got response from %s (%s)",
             full_url,
             http_method.__name__.upper(),
             extra={"response": self._filter_log_data(len(response.text), response_json)},
         )
         return response_json
 
+    def _filter_request_log_data(
+            self, data_length: int, content: Union[str, dict]
+    ) -> Optional[Union[str, dict]]:
+        if self.log_requests:
+            if self.log_size_limit and data_length > self.log_size_limit:
+                return "TRUNCATED"
+            return content
+        return None
+
     def _filter_log_data(
-        self, response_length: int, response_content: Union[str, dict]
+            self, response_length: int, response_content: Union[str, dict]
     ) -> Optional[Union[str, dict]]:
         if self.log_responses:
             if self.log_size_limit and response_length > self.log_size_limit:
                 return "TRUNCATED"
             return response_content
         return None
```

### Comparing `octo_api_client-1.1.3/octo_client/const.py` & `octo_api_client-1.1.4/octo_client/const.py`

 * *Files identical despite different names*

### Comparing `octo_api_client-1.1.3/octo_client/models.py` & `octo_api_client-1.1.4/octo_client/models.py`

 * *Files identical despite different names*

### Comparing `octo_api_client-1.1.3/pyproject.toml` & `octo_api_client-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "octo-api-client"
-version = "1.1.3"
+version = "1.1.4"
 description = "HTTP client for OCTo (Open Connection for Tourism) APIs."
 authors = ["Tiqets <connections@tiqets.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "octo_client"}]
 
 [tool.poetry.dependencies]
```

### Comparing `octo_api_client-1.1.3/setup.py` & `octo_api_client-1.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.20.0,<3', 'tonalite>=1.7.1,<2']
 
 setup_kwargs = {
     'name': 'octo-api-client',
-    'version': '1.1.3',
+    'version': '1.1.4',
     'description': 'HTTP client for OCTo (Open Connection for Tourism) APIs.',
     'long_description': "# OCTO API client\n\nPython HTTP client for OCTO (Open Connection for Tourism) APIs.\n\nMore info at [octospec.com](https://octospec.com/)\n\nAPI Specification: https://docs.octo.travel/docs/octo/r6gduoa5ah5ne-octo-api\n\n## Installation\n\n    pip install octo-api-client\n\n## Requirements\n\n* Python v3.7+\n\n## Development\n\n### Getting started\n\n    $ pip install poetry\n    $ poetry install\n\n### Running tests and linters\n\nTo run linters:\n\n    $ poetry run ruff octo_client\n    $ poetry run mypy octo_client\n\nTo run tests:\n\n    $ poetry run pytest\n\n\n## Usage\n\n```\nfrom octo_client import OctoClient\n\nclient = OctoClient('https://octo-api.mysupplier.com', 'MY-SECRET_TOKEN')\nclient.get_suppliers()\n```\n",
     'author': 'Tiqets',
     'author_email': 'connections@tiqets.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `octo_api_client-1.1.3/PKG-INFO` & `octo_api_client-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octo-api-client
-Version: 1.1.3
+Version: 1.1.4
 Summary: HTTP client for OCTo (Open Connection for Tourism) APIs.
 License: MIT
 Author: Tiqets
 Author-email: connections@tiqets.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

