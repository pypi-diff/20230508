# Comparing `tmp/checkbox-api-0.1.8.tar.gz` & `tmp/checkbox-api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkbox-api-0.1.8.tar", last modified: Tue Oct  6 20:06:48 2020, max compression
+gzip compressed data, was "checkbox-api-0.1.9.tar", last modified: Sun Oct 11 13:51:56 2020, max compression
```

## Comparing `checkbox-api-0.1.8.tar` & `checkbox-api-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0        0 2020-08-01 18:06:28.337628 checkbox-api-0.1.8/checkbox_api/__init__.py
--rw-r--r--   0        0        0        0 2020-08-01 18:22:04.598851 checkbox-api-0.1.8/checkbox_api/client/__init__.py
--rw-r--r--   0        0        0      114 2020-08-01 18:23:37.529677 checkbox-api-0.1.8/checkbox_api/client/async.py
--rw-r--r--   0        0        0     1992 2020-10-03 17:11:47.400879 checkbox-api-0.1.8/checkbox_api/client/base.py
--rw-r--r--   0        0        0    10014 2020-10-03 17:11:47.404213 checkbox-api-0.1.8/checkbox_api/client/sync.py
--rw-r--r--   0        0        0      143 2020-08-01 20:38:05.917228 checkbox-api-0.1.8/checkbox_api/consts.py
--rw-r--r--   0        0        0     1089 2020-10-03 17:11:47.387546 checkbox-api-0.1.8/checkbox_api/exceptions.py
--rw-r--r--   0        0        0        0 2020-08-01 18:29:33.142765 checkbox-api-0.1.8/checkbox_api/methods/__init__.py
--rw-r--r--   0        0        0     1928 2020-10-03 17:11:47.394212 checkbox-api-0.1.8/checkbox_api/methods/base.py
--rw-r--r--   0        0        0      753 2020-10-03 17:11:47.397546 checkbox-api-0.1.8/checkbox_api/methods/cash_register.py
--rw-r--r--   0        0        0     3395 2020-10-06 20:01:45.076151 checkbox-api-0.1.8/checkbox_api/methods/cashier.py
--rw-r--r--   0        0        0     3349 2020-10-06 19:42:20.193906 checkbox-api-0.1.8/checkbox_api/methods/receipts.py
--rw-r--r--   0        0        0     1419 2020-10-03 17:11:47.394212 checkbox-api-0.1.8/checkbox_api/methods/reports.py
--rw-r--r--   0        0        0     1625 2020-10-03 17:11:47.390879 checkbox-api-0.1.8/checkbox_api/methods/shifts.py
--rw-r--r--   0        0        0       52 2020-08-01 18:08:38.158692 checkbox-api-0.1.8/checkbox_api/session.py
--rw-r--r--   0        0        0        0 2020-08-01 18:21:58.912134 checkbox-api-0.1.8/checkbox_api/storage/__init__.py
--rw-r--r--   0        0        0      782 2020-10-03 17:11:47.390879 checkbox-api-0.1.8/checkbox_api/storage/simple.py
--rw-r--r--   0        0        0      792 2020-10-06 20:06:44.821812 checkbox-api-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      766 2020-10-06 20:06:48.066004 checkbox-api-0.1.8/setup.py
--rw-r--r--   0        0        0      464 2020-10-06 20:06:48.066269 checkbox-api-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-08-01 18:06:28.337628 checkbox-api-0.1.9/checkbox_api/__init__.py
+-rw-r--r--   0        0        0        0 2020-08-01 18:22:04.598851 checkbox-api-0.1.9/checkbox_api/client/__init__.py
+-rw-r--r--   0        0        0      114 2020-08-01 18:23:37.529677 checkbox-api-0.1.9/checkbox_api/client/async.py
+-rw-r--r--   0        0        0     1992 2020-10-11 13:51:27.570834 checkbox-api-0.1.9/checkbox_api/client/base.py
+-rw-r--r--   0        0        0    10870 2020-10-11 13:51:27.574167 checkbox-api-0.1.9/checkbox_api/client/sync.py
+-rw-r--r--   0        0        0      143 2020-08-01 20:38:05.917228 checkbox-api-0.1.9/checkbox_api/consts.py
+-rw-r--r--   0        0        0     1089 2020-10-11 13:51:27.554167 checkbox-api-0.1.9/checkbox_api/exceptions.py
+-rw-r--r--   0        0        0        0 2020-08-01 18:29:33.142765 checkbox-api-0.1.9/checkbox_api/methods/__init__.py
+-rw-r--r--   0        0        0     1928 2020-10-11 13:51:27.560834 checkbox-api-0.1.9/checkbox_api/methods/base.py
+-rw-r--r--   0        0        0     2045 2020-10-11 13:51:27.567501 checkbox-api-0.1.9/checkbox_api/methods/cash_register.py
+-rw-r--r--   0        0        0     2168 2020-10-11 13:51:27.564167 checkbox-api-0.1.9/checkbox_api/methods/cashier.py
+-rw-r--r--   0        0        0     3349 2020-10-11 13:51:27.567501 checkbox-api-0.1.9/checkbox_api/methods/receipts.py
+-rw-r--r--   0        0        0     1419 2020-10-11 13:51:27.564167 checkbox-api-0.1.9/checkbox_api/methods/reports.py
+-rw-r--r--   0        0        0     1625 2020-10-11 13:51:27.560834 checkbox-api-0.1.9/checkbox_api/methods/shifts.py
+-rw-r--r--   0        0        0      859 2020-10-11 13:51:27.564167 checkbox-api-0.1.9/checkbox_api/methods/transactions.py
+-rw-r--r--   0        0        0       52 2020-08-01 18:08:38.158692 checkbox-api-0.1.9/checkbox_api/session.py
+-rw-r--r--   0        0        0        0 2020-08-01 18:21:58.912134 checkbox-api-0.1.9/checkbox_api/storage/__init__.py
+-rw-r--r--   0        0        0      782 2020-10-11 13:51:27.557500 checkbox-api-0.1.9/checkbox_api/storage/simple.py
+-rw-r--r--   0        0        0      792 2020-10-11 13:51:31.314187 checkbox-api-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      766 2020-10-11 13:51:56.567227 checkbox-api-0.1.9/setup.py
+-rw-r--r--   0        0        0      464 2020-10-11 13:51:56.567497 checkbox-api-0.1.9/PKG-INFO
```

### Comparing `checkbox-api-0.1.8/checkbox_api/client/base.py` & `checkbox-api-0.1.9/checkbox_api/client/base.py`

 * *Files identical despite different names*

### Comparing `checkbox-api-0.1.8/checkbox_api/client/sync.py` & `checkbox-api-0.1.9/checkbox_api/client/sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from httpcore import NetworkError
 from httpx import Client, HTTPError, Timeout
 
 from checkbox_api.client.base import BaseCheckBoxClient
 from checkbox_api.consts import DEFAULT_REQUESTS_RELAX
 from checkbox_api.exceptions import CheckBoxError, CheckBoxNetworkError, StatusException
-from checkbox_api.methods import cash_register, cashier, receipts, shifts
+from checkbox_api.methods import cash_register, cashier, receipts, shifts, transactions
 from checkbox_api.methods.base import AbstractMethod, BaseMethod
 from checkbox_api.storage.simple import SessionStorage
 
 logger = logging.getLogger(__name__)
 
 
 class CheckBoxClient(BaseCheckBoxClient):
@@ -260,11 +260,34 @@
                 f"{initial_transaction['status']!r}: {initial_transaction['response_status']!r} "
                 f"{initial_transaction['response_error_message']!r}"
             )
         return shift
 
     def get_offline_codes(self, count: int = 2000):
         logger.info("Ask offline codes (count=%d)", count)
-        self(cashier.AskOfflineCodes(count=count, sync=True))
+        self(cash_register.AskOfflineCodes(count=count, sync=True))
         logger.info("Load offline codes...")
-        codes = self(cashier.GetOfflineCodes(count=count))
+        codes = self(cash_register.GetOfflineCodes(count=count))
         return [item["fiscal_code"] for item in codes]
+
+    def wait_transaction(
+        self,
+        transaction_id: str,
+        relax: int = DEFAULT_REQUESTS_RELAX,
+        timeout: Optional[int] = None,
+        storage: Optional[SessionStorage] = None,
+    ):
+        transaction = self._wait_status(
+            transactions.GetTransaction(transaction_id=transaction_id),
+            relax=relax,
+            timeout=timeout,
+            storage=storage,
+            field="status",
+            expected_value={"DONE", "ERROR"},
+        )
+        if transaction["status"] == "ERROR":
+            raise StatusException(
+                f"Transaction status moved to {transaction['status']!r} "
+                f"and tax status {transaction['response_status']!r} "
+                f"with message {transaction['response_error_message']!r}"
+            )
+        return transaction
```

### Comparing `checkbox-api-0.1.8/checkbox_api/exceptions.py` & `checkbox-api-0.1.9/checkbox_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `checkbox-api-0.1.8/checkbox_api/methods/base.py` & `checkbox-api-0.1.9/checkbox_api/methods/base.py`

 * *Files identical despite different names*

### Comparing `checkbox-api-0.1.8/checkbox_api/methods/receipts.py` & `checkbox-api-0.1.9/checkbox_api/methods/receipts.py`

 * *Files identical despite different names*

### Comparing `checkbox-api-0.1.8/checkbox_api/methods/reports.py` & `checkbox-api-0.1.9/checkbox_api/methods/reports.py`

 * *Files identical despite different names*

### Comparing `checkbox-api-0.1.8/checkbox_api/methods/shifts.py` & `checkbox-api-0.1.9/checkbox_api/methods/shifts.py`

 * *Files identical despite different names*

### Comparing `checkbox-api-0.1.8/checkbox_api/storage/simple.py` & `checkbox-api-0.1.9/checkbox_api/storage/simple.py`

 * *Files identical despite different names*

### Comparing `checkbox-api-0.1.8/pyproject.toml` & `checkbox-api-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkbox-api"
-version = "0.1.8"
+version = "0.1.9"
 description = "checkbox.in.ua Transactional Processing API Client"
 authors = ["Oleksandr Onufriichuk <oleksandr.onufriichuk@itvaan.com.ua>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = "^0.13.3"
```

### Comparing `checkbox-api-0.1.8/setup.py` & `checkbox-api-0.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['PyJWT>=1.7.1,<2.0.0', 'httpx>=0.13.3,<0.14.0']
 
 setup_kwargs = {
     'name': 'checkbox-api',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'checkbox.in.ua Transactional Processing API Client',
     'long_description': None,
     'author': 'Oleksandr Onufriichuk',
     'author_email': 'oleksandr.onufriichuk@itvaan.com.ua',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

