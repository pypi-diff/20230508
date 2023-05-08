# Comparing `tmp/tastytrade_sdk-0.0.2a0.dev69.tar.gz` & `tmp/tastytrade-sdk-0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade_sdk-0.0.2a0.dev69.tar", max compression
+gzip compressed data, was "tastytrade-sdk-0.0.dev1.tar", last modified: Sun May  7 01:57:12 2023, max compression
```

## Comparing `tastytrade_sdk-0.0.2a0.dev69.tar` & `tastytrade-sdk-0.0.dev1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       85 2023-05-08 02:59:09.641551 tastytrade_sdk-0.0.2a0.dev69/README.md
--rw-r--r--   0        0        0      593 2023-05-08 02:59:38.094043 tastytrade_sdk-0.0.2a0.dev69/pyproject.toml
--rw-r--r--   0        0        0       75 2023-05-08 02:59:09.645552 tastytrade_sdk-0.0.2a0.dev69/src/tastytrade_sdk/__init__.py
--rw-r--r--   0        0        0     1309 2023-05-08 02:59:09.645552 tastytrade_sdk-0.0.2a0.dev69/src/tastytrade_sdk/api.py
--rw-r--r--   0        0        0       90 2023-05-08 02:59:09.645552 tastytrade_sdk-0.0.2a0.dev69/src/tastytrade_sdk/instruments/__init__.py
--rw-r--r--   0        0        0     1787 2023-05-08 02:59:09.645552 tastytrade_sdk-0.0.2a0.dev69/src/tastytrade_sdk/instruments/instruments.py
--rw-r--r--   0        0        0      323 2023-05-08 02:59:09.645552 tastytrade_sdk-0.0.2a0.dev69/src/tastytrade_sdk/instruments/models.py
--rw-r--r--   0        0        0      100 2023-05-08 02:59:09.645552 tastytrade_sdk-0.0.2a0.dev69/src/tastytrade_sdk/market_metrics/__init__.py
--rw-r--r--   0        0        0     1155 2023-05-08 02:59:09.645552 tastytrade_sdk-0.0.2a0.dev69/src/tastytrade_sdk/market_metrics/market_metrics.py
--rw-r--r--   0        0        0      272 2023-05-08 02:59:09.645552 tastytrade_sdk-0.0.2a0.dev69/src/tastytrade_sdk/market_metrics/models.py
--rw-r--r--   0        0        0      757 2023-05-08 02:59:09.645552 tastytrade_sdk-0.0.2a0.dev69/src/tastytrade_sdk/tastytrade.py
--rw-r--r--   0        0        0       86 2023-05-08 02:59:09.645552 tastytrade_sdk-0.0.2a0.dev69/src/tastytrade_sdk/watchlists/__init__.py
--rw-r--r--   0        0        0      461 2023-05-08 02:59:09.645552 tastytrade_sdk-0.0.2a0.dev69/src/tastytrade_sdk/watchlists/watchlists.py
--rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 tastytrade_sdk-0.0.2a0.dev69/PKG-INFO
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2023-05-07 01:57:12.388528 tastytrade-sdk-0.0.dev1/
+-rw-r--r--   0 aaron      (501) staff       (20)      447 2023-05-07 01:57:12.388366 tastytrade-sdk-0.0.dev1/PKG-INFO
+-rw-r--r--   0 aaron      (501) staff       (20)        0 2023-05-06 05:56:32.000000 tastytrade-sdk-0.0.dev1/README.md
+-rw-r--r--   0 aaron      (501) staff       (20)      470 2023-05-07 01:57:00.000000 tastytrade-sdk-0.0.dev1/pyproject.toml
+-rw-r--r--   0 aaron      (501) staff       (20)       38 2023-05-07 01:57:12.388566 tastytrade-sdk-0.0.dev1/setup.cfg
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2023-05-07 01:57:12.387338 tastytrade-sdk-0.0.dev1/tastytrade_sdk/
+-rw-r--r--   0 aaron      (501) staff       (20)      430 2023-05-06 22:20:51.000000 tastytrade-sdk-0.0.dev1/tastytrade_sdk/__init__.py
+-rw-r--r--   0 aaron      (501) staff       (20)     1097 2023-05-06 16:42:26.000000 tastytrade-sdk-0.0.dev1/tastytrade_sdk/api.py
+-rw-r--r--   0 aaron      (501) staff       (20)      393 2023-05-06 16:49:48.000000 tastytrade-sdk-0.0.dev1/tastytrade_sdk/watchlists.py
+drwxr-xr-x   0 aaron      (501) staff       (20)        0 2023-05-07 01:57:12.388187 tastytrade-sdk-0.0.dev1/tastytrade_sdk.egg-info/
+-rw-r--r--   0 aaron      (501) staff       (20)      447 2023-05-07 01:57:12.000000 tastytrade-sdk-0.0.dev1/tastytrade_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 aaron      (501) staff       (20)      254 2023-05-07 01:57:12.000000 tastytrade-sdk-0.0.dev1/tastytrade_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 aaron      (501) staff       (20)        1 2023-05-07 01:57:12.000000 tastytrade-sdk-0.0.dev1/tastytrade_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 aaron      (501) staff       (20)       15 2023-05-07 01:57:12.000000 tastytrade-sdk-0.0.dev1/tastytrade_sdk.egg-info/top_level.txt
```

### Comparing `tastytrade_sdk-0.0.2a0.dev69/src/tastytrade_sdk/api.py` & `tastytrade-sdk-0.0.dev1/tastytrade_sdk/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,33 @@
 import json
-from typing import Optional, Tuple, List, Any
+from types import MappingProxyType
+from typing import Optional, Any, Dict
 
 import requests
-from injector import singleton
 
 
-@singleton
 class Api:
     __base_url = 'https://api.tastyworks.com'
     __token: Optional[str] = None
 
     def login(self, login: str, password: str) -> None:
         self.__token = requests.post(f'{self.__base_url}/sessions', data={
             'login': login,
             'password': password
         }).json()['data']['session-token']
 
-    def get(self, path: str, params: List[Tuple[str, Any]] = tuple()) -> Optional[dict]:
+    def get(self, path: str, params: Optional[Dict[str, Any]] = MappingProxyType({})) -> Optional[dict]:
         response = requests.get(
-            self.__url(path, params),
-            headers=self.__headers()
+            f'{self.__base_url}{path}',
+            params=params,
+            headers={'Authorization': self.__token, 'content-type': 'application/json'}
         )
         if response.status_code == 404:
             return None
         return response.json()
 
     def put(self, path: str, payload: dict) -> dict:
         return requests.put(
             f'{self.__base_url}{path}',
             data=json.dumps(payload),
-            headers=self.__headers()
+            headers={'Authorization': self.__token, 'content-type': 'application/json'}
         ).json()
-
-    def __url(self, path: str, params: List[Tuple[str, Any]] = tuple()) -> str:
-        url = f'{self.__base_url}{path}'
-        if params:
-            url += '?' + '&'.join(f'{p[0]}={p[1]}' for p in params)
-        return url
-
-    def __headers(self) -> dict:
-        return {'Authorization': self.__token, 'content-type': 'application/json'}
```

