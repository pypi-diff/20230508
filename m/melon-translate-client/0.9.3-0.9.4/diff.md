# Comparing `tmp/melon_translate_client-0.9.3.tar.gz` & `tmp/melon_translate_client-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melon_translate_client-0.9.3.tar", max compression
+gzip compressed data, was "melon_translate_client-0.9.4.tar", max compression
```

## Comparing `melon_translate_client-0.9.3.tar` & `melon_translate_client-0.9.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       50 2023-02-15 15:01:16.708397 melon_translate_client-0.9.3/melon_translate_client/__init__.py
--rw-r--r--   0        0        0    16716 2023-02-15 15:01:16.708397 melon_translate_client-0.9.3/melon_translate_client/_client.py
--rw-r--r--   0        0        0      289 2023-02-15 15:01:16.708397 melon_translate_client-0.9.3/melon_translate_client/common/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-15 15:01:16.708397 melon_translate_client-0.9.3/melon_translate_client/tests/__init__.py
--rw-r--r--   0        0        0    13618 2023-02-15 15:01:16.708397 melon_translate_client-0.9.3/melon_translate_client/tests/test_client.py
--rw-r--r--   0        0        0      318 2023-02-15 15:01:16.708397 melon_translate_client-0.9.3/melon_translate_client/utils/logging.py
--rw-r--r--   0        0        0      457 2023-02-15 15:01:16.708397 melon_translate_client-0.9.3/pyproject.toml
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 melon_translate_client-0.9.3/setup.py
--rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 melon_translate_client-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-03-08 16:57:37.778343 melon_translate_client-0.9.4/melon_translate_client/__init__.py
+-rw-r--r--   0        0        0    16716 2023-03-08 16:57:37.778343 melon_translate_client-0.9.4/melon_translate_client/_client.py
+-rw-r--r--   0        0        0      289 2023-03-08 16:57:37.778343 melon_translate_client-0.9.4/melon_translate_client/common/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-08 16:57:37.778343 melon_translate_client-0.9.4/melon_translate_client/tests/__init__.py
+-rw-r--r--   0        0        0    13618 2023-03-08 16:57:37.779343 melon_translate_client-0.9.4/melon_translate_client/tests/test_client.py
+-rw-r--r--   0        0        0      318 2023-03-08 16:57:37.779343 melon_translate_client-0.9.4/melon_translate_client/utils/logging.py
+-rw-r--r--   0        0        0      457 2023-03-08 16:57:37.779343 melon_translate_client-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 melon_translate_client-0.9.4/setup.py
+-rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 melon_translate_client-0.9.4/PKG-INFO
```

### Comparing `melon_translate_client-0.9.3/melon_translate_client/_client.py` & `melon_translate_client-0.9.4/melon_translate_client/_client.py`

 * *Files identical despite different names*

### Comparing `melon_translate_client-0.9.3/melon_translate_client/tests/test_client.py` & `melon_translate_client-0.9.4/melon_translate_client/tests/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         port = self.live_server_url.split(":")[2]
         client = Client(config("TRANSLATE_ADDRESS", default="http://localhost"), port)
         language = "de"
 
         responses = client._get_all_pages(
             language, page_size=4, page=1, chain_together=False
         )
-        assert len(responses) == 2, "Should return 2 pages of results."
+        assert len(responses) == 3, "Should return 3 pages of results."
 
         first_page_response, second_page_response, *_ = responses
         assert first_page_response["count"] == second_page_response["count"]
         assert len(first_page_response["results"]) == 4
         assert len(second_page_response["results"]) == 4
 
     def test_redis_caching_for_filter_method(self):
```

### Comparing `melon_translate_client-0.9.3/setup.py` & `melon_translate_client-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 {'': ['*']}
 
 install_requires = \
 ['python-decouple>=3.6,<4.0', 'redis>=4.3.0,<5.0.0', 'requests>=2.27.0']
 
 setup_kwargs = {
     'name': 'melon-translate-client',
-    'version': '0.9.3',
+    'version': '0.9.4',
     'description': 'Client package for melon-translate.',
     'long_description': 'None',
     'author': 'sam',
     'author_email': 'contact@justsam.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `melon_translate_client-0.9.3/PKG-INFO` & `melon_translate_client-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melon-translate-client
-Version: 0.9.3
+Version: 0.9.4
 Summary: Client package for melon-translate.
 Author: sam
 Author-email: contact@justsam.io
 Requires-Python: >=3.6
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

