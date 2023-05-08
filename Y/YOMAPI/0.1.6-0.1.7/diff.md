# Comparing `tmp/YOMAPI-0.1.6.tar.gz` & `tmp/YOMAPI-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/YOMAPI-0.1.6.tar", last modified: Fri Apr 28 12:39:49 2023, max compression
+gzip compressed data, was "dist/YOMAPI-0.1.7.tar", last modified: Mon May  8 18:36:50 2023, max compression
```

## Comparing `YOMAPI-0.1.6.tar` & `YOMAPI-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-28 12:39:49.000000 YOMAPI-0.1.6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-28 12:39:49.000000 YOMAPI-0.1.6/YOMAPI/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    39250 2023-04-28 12:39:39.000000 YOMAPI-0.1.6/YOMAPI/YOMAPI.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)       68 2023-04-28 12:39:39.000000 YOMAPI-0.1.6/YOMAPI/__init__.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)       39 2023-04-28 12:39:39.000000 YOMAPI-0.1.6/setup.cfg
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      922 2023-04-28 12:39:39.000000 YOMAPI-0.1.6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2023-04-28 12:39:49.000000 YOMAPI-0.1.6/PKG-INFO
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-08 18:36:50.000000 YOMAPI-0.1.7/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-08 18:36:50.000000 YOMAPI-0.1.7/YOMAPI/
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    39853 2023-05-08 18:36:41.000000 YOMAPI-0.1.7/YOMAPI/YOMAPI.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)       68 2023-05-08 18:36:41.000000 YOMAPI-0.1.7/YOMAPI/__init__.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)       39 2023-05-08 18:36:41.000000 YOMAPI-0.1.7/setup.cfg
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      922 2023-05-08 18:36:41.000000 YOMAPI-0.1.7/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2023-05-08 18:36:50.000000 YOMAPI-0.1.7/PKG-INFO
```

### Comparing `YOMAPI-0.1.6/YOMAPI/YOMAPI.py` & `YOMAPI-0.1.7/YOMAPI/YOMAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -816,14 +816,31 @@
         session = self.__build_session(token)
         try:
             response = session.delete(path)
             return response
         except Exception as error:
             raise ApiResponseError(path, str(error))
         
+    """
+    Commerce Payment Header Endpoints
+    """
+    def update_bulk_commerce_payment_header(self, batch, fields_not_to_be_updated, token):
+        path = self.url_v3 + '/api/v3/admin/payments/commerce-payment-header/bulk'
+        session = self.__build_session(token)
+        try:
+            body = {
+                'data': batch,
+                'fieldsNotToBeUpdated': fields_not_to_be_updated
+            }
+
+            response = session.put(path, json.dumps(body))
+            return response
+        except Exception as error:
+            raise ApiResponseError(path, str(error))
+        
 
     """
     Shopping Lists Endpoints
     """
     def update_bulk_shopping_lists(self, batch, token):
         path = f'{self.url}/api/v2/shopping-lists/bulk'
         session = self.__build_session(token)
```

### Comparing `YOMAPI-0.1.6/setup.py` & `YOMAPI-0.1.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from distutils.core import setup
 setup(
   name = 'YOMAPI',
   packages = ['YOMAPI'],
-  version = '0.1.6',
+  version = '0.1.7',
   license='MIT',
   description = 'A PACKAGE TO USE THE SAME YOM API INTERFACE FROM YOM INTEGRATIONS',
   author = 'Camilo Jiménez',
   author_email = 'camilo@youorder.me',
   url = 'https://github.com/user/reponame',
   # download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz', 
   keywords = ['YOM-INTEGRATIONS'],   # Keywords that define your package best
```

### Comparing `YOMAPI-0.1.6/PKG-INFO` & `YOMAPI-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: YOMAPI
-Version: 0.1.6
+Version: 0.1.7
 Summary: A PACKAGE TO USE THE SAME YOM API INTERFACE FROM YOM INTEGRATIONS
 Home-page: https://github.com/user/reponame
 Author: Camilo Jiménez
 Author-email: camilo@youorder.me
 License: MIT
 Description: UNKNOWN
 Keywords: YOM-INTEGRATIONS
```

