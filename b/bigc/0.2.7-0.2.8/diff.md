# Comparing `tmp/bigc-0.2.7.tar.gz` & `tmp/bigc-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigc-0.2.7.tar", max compression
+gzip compressed data, was "bigc-0.2.8.tar", max compression
```

## Comparing `bigc-0.2.7.tar` & `bigc-0.2.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-05-03 17:25:21.521933 bigc-0.2.7/LICENSE.txt
--rw-r--r--   0        0        0     1596 2023-05-03 17:25:21.521933 bigc-0.2.7/README.md
--rw-r--r--   0        0        0       32 2023-05-03 17:25:21.521933 bigc-0.2.7/bigc/__init__.py
--rw-r--r--   0        0        0     1069 2023-05-03 17:25:21.521933 bigc-0.2.7/bigc/api.py
--rw-r--r--   0        0        0     6458 2023-05-03 17:25:21.521933 bigc-0.2.7/bigc/api_client.py
--rw-r--r--   0        0        0       49 2023-05-03 17:25:21.521933 bigc-0.2.7/bigc/data/__init__.py
--rw-r--r--   0        0        0      482 2023-05-03 17:25:21.521933 bigc-0.2.7/bigc/data/order_status.py
--rw-r--r--   0        0        0     1639 2023-05-03 17:25:21.521933 bigc-0.2.7/bigc/exceptions.py
--rw-r--r--   0        0        0      431 2023-05-03 17:25:21.521933 bigc-0.2.7/bigc/resources/__init__.py
--rw-r--r--   0        0        0     1741 2023-05-03 17:25:21.521933 bigc-0.2.7/bigc/resources/carts.py
--rw-r--r--   0        0        0     1180 2023-05-03 17:25:21.521933 bigc-0.2.7/bigc/resources/categories.py
--rw-r--r--   0        0        0     4116 2023-05-03 17:25:21.521933 bigc-0.2.7/bigc/resources/checkouts.py
--rw-r--r--   0        0        0     1178 2023-05-03 17:25:21.521933 bigc-0.2.7/bigc/resources/customer_groups.py
--rw-r--r--   0        0        0     4088 2023-05-03 17:25:21.521933 bigc-0.2.7/bigc/resources/customers.py
--rw-r--r--   0        0        0     4504 2023-05-03 17:25:21.521933 bigc-0.2.7/bigc/resources/orders.py
--rw-r--r--   0        0        0     1414 2023-05-03 17:25:21.521933 bigc-0.2.7/bigc/resources/product_variants.py
--rw-r--r--   0        0        0     2682 2023-05-03 17:25:21.521933 bigc-0.2.7/bigc/resources/products.py
--rw-r--r--   0        0        0     1205 2023-05-03 17:25:21.521933 bigc-0.2.7/bigc/resources/webhooks.py
--rw-r--r--   0        0        0      557 2023-05-03 17:25:21.521933 bigc-0.2.7/bigc/utils.py
--rw-r--r--   0        0        0      770 2023-05-03 17:25:21.521933 bigc-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 bigc-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-08 18:38:58.364096 bigc-0.2.8/LICENSE.txt
+-rw-r--r--   0        0        0     1596 2023-05-08 18:38:58.364096 bigc-0.2.8/README.md
+-rw-r--r--   0        0        0       32 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/__init__.py
+-rw-r--r--   0        0        0     1069 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/api.py
+-rw-r--r--   0        0        0     6458 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/api_client.py
+-rw-r--r--   0        0        0       49 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/data/__init__.py
+-rw-r--r--   0        0        0      482 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/data/order_status.py
+-rw-r--r--   0        0        0     1639 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/exceptions.py
+-rw-r--r--   0        0        0      431 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/resources/__init__.py
+-rw-r--r--   0        0        0     1741 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/resources/carts.py
+-rw-r--r--   0        0        0     1180 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/resources/categories.py
+-rw-r--r--   0        0        0     4116 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/resources/checkouts.py
+-rw-r--r--   0        0        0     1178 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/resources/customer_groups.py
+-rw-r--r--   0        0        0     4346 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/resources/customers.py
+-rw-r--r--   0        0        0     4504 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/resources/orders.py
+-rw-r--r--   0        0        0     1414 2023-05-08 18:38:58.364096 bigc-0.2.8/bigc/resources/product_variants.py
+-rw-r--r--   0        0        0     2682 2023-05-08 18:38:58.368097 bigc-0.2.8/bigc/resources/products.py
+-rw-r--r--   0        0        0     1205 2023-05-08 18:38:58.368097 bigc-0.2.8/bigc/resources/webhooks.py
+-rw-r--r--   0        0        0      557 2023-05-08 18:38:58.368097 bigc-0.2.8/bigc/utils.py
+-rw-r--r--   0        0        0      770 2023-05-08 18:38:58.368097 bigc-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 bigc-0.2.8/PKG-INFO
```

### Comparing `bigc-0.2.7/LICENSE.txt` & `bigc-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bigc-0.2.7/README.md` & `bigc-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `bigc-0.2.7/bigc/api.py` & `bigc-0.2.8/bigc/api.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.7/bigc/api_client.py` & `bigc-0.2.8/bigc/api_client.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.7/bigc/exceptions.py` & `bigc-0.2.8/bigc/exceptions.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.7/bigc/resources/carts.py` & `bigc-0.2.8/bigc/resources/carts.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.7/bigc/resources/categories.py` & `bigc-0.2.8/bigc/resources/categories.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.7/bigc/resources/checkouts.py` & `bigc-0.2.8/bigc/resources/checkouts.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.7/bigc/resources/customer_groups.py` & `bigc-0.2.8/bigc/resources/customer_groups.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.7/bigc/resources/customers.py` & `bigc-0.2.8/bigc/resources/customers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections.abc import Iterator
 from typing import Any, Iterable
 from urllib.parse import urlencode, urlparse, urlunparse
 
 from bigc.api_client import BigCommerceAPIClient
-from bigc.exceptions import ResourceNotFoundError
+from bigc.exceptions import BigCommerceAPIException, ResourceNotFoundError
 
 
 class BigCommerceCustomersAPI:
     def __init__(self, api_client: BigCommerceAPIClient):
         self._api = api_client
 
     def all(self, *, id_in: Iterable[int] = None, include_formfields: bool = False,
@@ -94,16 +94,22 @@
         try:
             return self._api.v3.get(f'/customers/addresses?customer_id:in={customer_id}&id:in={address_id}')[0]
         except IndexError:
             raise ResourceNotFoundError()
 
     def create_address(self, customer_id: int, **kwargs) -> dict:
         """Add an address to the customer's address book"""
-        return self._api.v3.post('/customers/addresses', json=[{'customer_id': customer_id, **kwargs}])
+        try:
+            return self._api.v3.post('/customers/addresses', json=[{'customer_id': customer_id, **kwargs}])[0]
+        except IndexError:
+            raise BigCommerceAPIException('This address already exists')
 
     def update_address(self, address_id: int, **kwargs) -> dict:
         """Update an address by its ID"""
-        return self._api.v3.put('/customers/addresses', json=[{'id': address_id, **kwargs}])
+        try:
+            return self._api.v3.put('/customers/addresses', json=[{'id': address_id, **kwargs}])[0]
+        except IndexError:
+            raise BigCommerceAPIException('This address already exists')
 
-    def delete_address(self, address_id: int) -> dict:
+    def delete_address(self, address_id: int) -> None:
         """Delete an address by its ID"""
-        return self._api.v3.delete(f"/customers/addresses?id:in={address_id}")
+        self._api.v3.delete(f"/customers/addresses?id:in={address_id}")
```

### Comparing `bigc-0.2.7/bigc/resources/orders.py` & `bigc-0.2.8/bigc/resources/orders.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.7/bigc/resources/product_variants.py` & `bigc-0.2.8/bigc/resources/product_variants.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.7/bigc/resources/products.py` & `bigc-0.2.8/bigc/resources/products.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.7/bigc/resources/webhooks.py` & `bigc-0.2.8/bigc/resources/webhooks.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.7/bigc/utils.py` & `bigc-0.2.8/bigc/utils.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.7/pyproject.toml` & `bigc-0.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bigc"
-version = "0.2.7"
+version = "0.2.8"
 description = "Unofficial client for the BigCommerce API"
 license = "MIT"
 authors = ["Ryan Thomson <ryan@medshift.com>", "Dillon Hartley <dillon@medshift.com>", "Adam Walsh <adam@medshift.com>"]
 readme = "README.md"
 homepage = "https://github.com/MedShift/bigc"
 repository = "https://github.com/MedShift/bigc.git"
 keywords = ["bigcommerce", "api", "client"]
```

### Comparing `bigc-0.2.7/PKG-INFO` & `bigc-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigc
-Version: 0.2.7
+Version: 0.2.8
 Summary: Unofficial client for the BigCommerce API
 Home-page: https://github.com/MedShift/bigc
 License: MIT
 Keywords: bigcommerce,api,client
 Author: Ryan Thomson
 Author-email: ryan@medshift.com
 Requires-Python: >=3.9,<4.0
```

