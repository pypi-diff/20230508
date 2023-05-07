# Comparing `tmp/fastapi_jwt_login-0.1.0.tar.gz` & `tmp/fastapi_jwt_login-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_jwt_login-0.1.0.tar", max compression
+gzip compressed data, was "fastapi_jwt_login-0.1.1.tar", max compression
```

## Comparing `fastapi_jwt_login-0.1.0.tar` & `fastapi_jwt_login-0.1.1.tar`

### file list

```diff
@@ -1,3 +1,4 @@
--rw-r--r--   0        0        0      872 2023-05-04 20:22:31.698341 fastapi_jwt_login-0.1.0/fastapi_jwt_login/__init__.py
--rw-r--r--   0        0        0      441 2023-05-04 14:49:09.371026 fastapi_jwt_login-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 fastapi_jwt_login-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35129 2023-05-07 22:58:20.152245 fastapi_jwt_login-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1081 2023-05-07 22:55:47.148868 fastapi_jwt_login-0.1.1/fastapi_jwt_login/__init__.py
+-rw-r--r--   0        0        0      441 2023-05-07 23:06:21.047944 fastapi_jwt_login-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 fastapi_jwt_login-0.1.1/PKG-INFO
```

### Comparing `fastapi_jwt_login-0.1.0/fastapi_jwt_login/__init__.py` & `fastapi_jwt_login-0.1.1/fastapi_jwt_login/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import typing as t
 from random import choice
 from starlette.middleware.base import BaseHTTPMiddleware
 from fastapi import FastAPI, Response
 from fastapi import Request
 from starlette.types import ASGIApp, Receive, Scope, Send
 from jose import jwt
+from datetime import timedelta
 
 class JWTLogin:
     def __init__(self, secret_key: str, cookie_name: str = 'x-jwt-login-token', algorithm: str = 'HS256'):
         self.cookie_name = cookie_name
         self.secret = secret_key
         self.algorithm = algorithm
         
     def set_token_header(self, response: Response, data: dict[str, t.Any]):
-        encoded_token = jwt.encode(data, self.secret, self.algorithm)
-        response.set_cookie(self.cookie_name, encoded_token)
+        if data is not None:
+            encoded_token = jwt.encode(data, self.secret, self.algorithm)
+            response.set_cookie(self.cookie_name, encoded_token, httponly=True, expires=timedelta(days=90))
+        else:
+            response.set_cookie(self.cookie_name, '', expires=timedelta(seconds=1))
         
     def get_jwt_in_cookies(self, request: Request):
         cookie = request.cookies.get(self.cookie_name)
         return jwt.decode(cookie, self.secret, self.algorithm)
```

### Comparing `fastapi_jwt_login-0.1.0/PKG-INFO` & `fastapi_jwt_login-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-jwt-login
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Michael Piccirillo
 Author-email: 70709374+Khrysys@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

