# Comparing `tmp/getsmarter-api-clients-0.5.1.tar.gz` & `tmp/getsmarter-api-clients-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getsmarter-api-clients-0.5.1.tar", last modified: Fri May  5 19:28:55 2023, max compression
+gzip compressed data, was "getsmarter-api-clients-0.5.2.tar", last modified: Mon May  8 13:46:16 2023, max compression
```

## Comparing `getsmarter-api-clients-0.5.1.tar` & `getsmarter-api-clients-0.5.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 19:28:55.508992 getsmarter-api-clients-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-05-05 19:28:51.000000 getsmarter-api-clients-0.5.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-05 19:28:51.000000 getsmarter-api-clients-0.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-05 19:28:51.000000 getsmarter-api-clients-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6126 2023-05-05 19:28:55.508992 getsmarter-api-clients-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4599 2023-05-05 19:28:51.000000 getsmarter-api-clients-0.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 19:28:55.508992 getsmarter-api-clients-0.5.1/getsmarter_api_clients/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-05 19:28:51.000000 getsmarter-api-clients-0.5.1/getsmarter_api_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9540 2023-05-05 19:28:51.000000 getsmarter-api-clients-0.5.1/getsmarter_api_clients/geag.py
--rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-05-05 19:28:51.000000 getsmarter-api-clients-0.5.1/getsmarter_api_clients/oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 19:28:55.508992 getsmarter-api-clients-0.5.1/getsmarter_api_clients.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6126 2023-05-05 19:28:55.000000 getsmarter-api-clients-0.5.1/getsmarter_api_clients.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-05-05 19:28:55.000000 getsmarter-api-clients-0.5.1/getsmarter_api_clients.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 19:28:55.000000 getsmarter-api-clients-0.5.1/getsmarter_api_clients.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 19:28:55.000000 getsmarter-api-clients-0.5.1/getsmarter_api_clients.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-05 19:28:55.000000 getsmarter-api-clients-0.5.1/getsmarter_api_clients.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-05 19:28:55.000000 getsmarter-api-clients-0.5.1/getsmarter_api_clients.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 19:28:55.508992 getsmarter-api-clients-0.5.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-05-05 19:28:51.000000 getsmarter-api-clients-0.5.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-05 19:28:51.000000 getsmarter-api-clients-0.5.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-05 19:28:55.508992 getsmarter-api-clients-0.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     4952 2023-05-05 19:28:51.000000 getsmarter-api-clients-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:46:16.110408 getsmarter-api-clients-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      953 2023-05-08 13:46:11.000000 getsmarter-api-clients-0.5.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-08 13:46:11.000000 getsmarter-api-clients-0.5.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-08 13:46:11.000000 getsmarter-api-clients-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6177 2023-05-08 13:46:16.110408 getsmarter-api-clients-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4599 2023-05-08 13:46:11.000000 getsmarter-api-clients-0.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:46:16.110408 getsmarter-api-clients-0.5.2/getsmarter_api_clients/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-08 13:46:11.000000 getsmarter-api-clients-0.5.2/getsmarter_api_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9583 2023-05-08 13:46:11.000000 getsmarter-api-clients-0.5.2/getsmarter_api_clients/geag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-05-08 13:46:11.000000 getsmarter-api-clients-0.5.2/getsmarter_api_clients/oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:46:16.110408 getsmarter-api-clients-0.5.2/getsmarter_api_clients.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6177 2023-05-08 13:46:16.000000 getsmarter-api-clients-0.5.2/getsmarter_api_clients.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-05-08 13:46:16.000000 getsmarter-api-clients-0.5.2/getsmarter_api_clients.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 13:46:16.000000 getsmarter-api-clients-0.5.2/getsmarter_api_clients.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 13:46:16.000000 getsmarter-api-clients-0.5.2/getsmarter_api_clients.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-08 13:46:16.000000 getsmarter-api-clients-0.5.2/getsmarter_api_clients.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-08 13:46:16.000000 getsmarter-api-clients-0.5.2/getsmarter_api_clients.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 13:46:16.110408 getsmarter-api-clients-0.5.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-05-08 13:46:11.000000 getsmarter-api-clients-0.5.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-08 13:46:11.000000 getsmarter-api-clients-0.5.2/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-08 13:46:16.110408 getsmarter-api-clients-0.5.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4952 2023-05-08 13:46:11.000000 getsmarter-api-clients-0.5.2/setup.py
```

### Comparing `getsmarter-api-clients-0.5.1/CHANGELOG.rst` & `getsmarter-api-clients-0.5.2/CHANGELOG.rst`

 * *Files 19% similar despite different names*

```diff
@@ -12,19 +12,22 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
 *
 
+[0.5.2]
+~~~~~~~
+* Include payload in error message
+
 [0.5.1]
 ~~~~~~~
 * Catch a `requests.HTTPError`, not an `urllib.error.HTTPError`.
 
-
 [0.5.0] - 2023-04-12
 ~~~~~~~~~~~~~~~~~~~~
 
 * Added new field for data_share_consent in enterprise_allocations
 
 [0.4.0] - 2022-09-12
 ~~~~~~~~~~~~~~~~~~~~
```

### Comparing `getsmarter-api-clients-0.5.1/LICENSE.txt` & `getsmarter-api-clients-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `getsmarter-api-clients-0.5.1/PKG-INFO` & `getsmarter-api-clients-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getsmarter-api-clients
-Version: 0.5.1
+Version: 0.5.2
 Summary: Clients to interact with GetSmarter APIs.
 Home-page: https://github.com/edx/getsmarter-api-clients
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -169,19 +169,22 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
 *
 
+[0.5.2]
+~~~~~~~
+* Include payload in error message
+
 [0.5.1]
 ~~~~~~~
 * Catch a `requests.HTTPError`, not an `urllib.error.HTTPError`.
 
-
 [0.5.0] - 2023-04-12
 ~~~~~~~~~~~~~~~~~~~~
 
 * Added new field for data_share_consent in enterprise_allocations
 
 [0.4.0] - 2022-09-12
 ~~~~~~~~~~~~~~~~~~~~
```

### Comparing `getsmarter-api-clients-0.5.1/README.rst` & `getsmarter-api-clients-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `getsmarter-api-clients-0.5.1/getsmarter_api_clients/geag.py` & `getsmarter-api-clients-0.5.2/getsmarter_api_clients/geag.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,11 +254,12 @@
 
         response = self.post(url, json=payload)
         try:
             response.raise_for_status()
         except HTTPError:
             message = (
               f'Enterprise allocation failed to be created for order {payment_reference} '
-              f'with reasons: {response.text}'
+              f'with reasons: {response.text}, '
+              f'with payload: {payload}'
             )
             logger.error(message)
             raise
```

### Comparing `getsmarter-api-clients-0.5.1/getsmarter_api_clients/oauth.py` & `getsmarter-api-clients-0.5.2/getsmarter_api_clients/oauth.py`

 * *Files identical despite different names*

### Comparing `getsmarter-api-clients-0.5.1/getsmarter_api_clients.egg-info/PKG-INFO` & `getsmarter-api-clients-0.5.2/getsmarter_api_clients.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getsmarter-api-clients
-Version: 0.5.1
+Version: 0.5.2
 Summary: Clients to interact with GetSmarter APIs.
 Home-page: https://github.com/edx/getsmarter-api-clients
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -169,19 +169,22 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
 *
 
+[0.5.2]
+~~~~~~~
+* Include payload in error message
+
 [0.5.1]
 ~~~~~~~
 * Catch a `requests.HTTPError`, not an `urllib.error.HTTPError`.
 
-
 [0.5.0] - 2023-04-12
 ~~~~~~~~~~~~~~~~~~~~
 
 * Added new field for data_share_consent in enterprise_allocations
 
 [0.4.0] - 2022-09-12
 ~~~~~~~~~~~~~~~~~~~~
```

### Comparing `getsmarter-api-clients-0.5.1/requirements/constraints.txt` & `getsmarter-api-clients-0.5.2/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `getsmarter-api-clients-0.5.1/setup.py` & `getsmarter-api-clients-0.5.2/setup.py`

 * *Files identical despite different names*

