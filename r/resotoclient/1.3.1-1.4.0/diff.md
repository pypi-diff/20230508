# Comparing `tmp/resotoclient-1.3.1.tar.gz` & `tmp/resotoclient-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoclient-1.3.1.tar", max compression
+gzip compressed data, was "resotoclient-1.4.0.tar", max compression
```

## Comparing `resotoclient-1.3.1.tar` & `resotoclient-1.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-05-02 12:40:14.056864 resotoclient-1.3.1/LICENSE
--rw-r--r--   0        0        0     1243 2023-05-02 12:40:14.056864 resotoclient-1.3.1/README.md
--rw-r--r--   0        0        0     2082 2023-05-02 12:40:14.056864 resotoclient-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    20455 2023-05-02 12:40:14.056864 resotoclient-1.3.1/resotoclient/__init__.py
--rw-r--r--   0        0        0    23018 2023-05-02 12:40:14.056864 resotoclient-1.3.1/resotoclient/async_client.py
--rw-r--r--   0        0        0     6219 2023-05-02 12:40:14.056864 resotoclient-1.3.1/resotoclient/ca.py
--rw-r--r--   0        0        0     2813 2023-05-02 12:40:14.056864 resotoclient-1.3.1/resotoclient/http_client/__init__.py
--rw-r--r--   0        0        0    10672 2023-05-02 12:40:14.056864 resotoclient-1.3.1/resotoclient/http_client/aiohttp_client.py
--rw-r--r--   0        0        0     1282 2023-05-02 12:40:14.056864 resotoclient-1.3.1/resotoclient/http_client/event_loop_thread.py
--rw-r--r--   0        0        0      693 2023-05-02 12:40:14.056864 resotoclient-1.3.1/resotoclient/json_utils.py
--rw-r--r--   0        0        0     3431 2023-05-02 12:40:14.056864 resotoclient-1.3.1/resotoclient/jwt_utils.py
--rw-r--r--   0        0        0     2283 2023-05-02 12:40:14.056864 resotoclient-1.3.1/resotoclient/models.py
--rw-r--r--   0        0        0     2721 1970-01-01 00:00:00.000000 resotoclient-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-08 13:39:50.853873 resotoclient-1.4.0/LICENSE
+-rw-r--r--   0        0        0     1243 2023-05-08 13:39:50.853873 resotoclient-1.4.0/README.md
+-rw-r--r--   0        0        0     2082 2023-05-08 13:39:50.857874 resotoclient-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    20715 2023-05-08 13:39:50.857874 resotoclient-1.4.0/resotoclient/__init__.py
+-rw-r--r--   0        0        0    23316 2023-05-08 13:39:50.857874 resotoclient-1.4.0/resotoclient/async_client.py
+-rw-r--r--   0        0        0     6219 2023-05-08 13:39:50.857874 resotoclient-1.4.0/resotoclient/ca.py
+-rw-r--r--   0        0        0     2813 2023-05-08 13:39:50.857874 resotoclient-1.4.0/resotoclient/http_client/__init__.py
+-rw-r--r--   0        0        0    12959 2023-05-08 13:39:50.857874 resotoclient-1.4.0/resotoclient/http_client/aiohttp_client.py
+-rw-r--r--   0        0        0     1282 2023-05-08 13:39:50.857874 resotoclient-1.4.0/resotoclient/http_client/event_loop_thread.py
+-rw-r--r--   0        0        0      693 2023-05-08 13:39:50.857874 resotoclient-1.4.0/resotoclient/json_utils.py
+-rw-r--r--   0        0        0     3813 2023-05-08 13:39:50.857874 resotoclient-1.4.0/resotoclient/jwt_utils.py
+-rw-r--r--   0        0        0     2283 2023-05-08 13:39:50.857874 resotoclient-1.4.0/resotoclient/models.py
+-rw-r--r--   0        0        0     2721 1970-01-01 00:00:00.000000 resotoclient-1.4.0/PKG-INFO
```

### Comparing `resotoclient-1.3.1/LICENSE` & `resotoclient-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `resotoclient-1.3.1/README.md` & `resotoclient-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `resotoclient-1.3.1/pyproject.toml` & `resotoclient-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "resotoclient"
-version = "1.3.1"
+version = "1.4.0"
 description = "Resoto Python client library"
 authors = ["Some Engineering Inc."]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/someengineering/resotoclient-python"
 repository = "https://github.com/someengineering/resotoclient-python"
 packages = [
```

### Comparing `resotoclient-1.3.1/resotoclient/__init__.py` & `resotoclient-1.4.0/resotoclient/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,22 +111,24 @@
         self,
         url: str,
         *,
         psk: Optional[str] = None,
         additional_headers: Optional[Dict[str, str]] = None,
         custom_ca_cert_path: Optional[str] = None,
         verify: bool = True,
-        renew_before: timedelta = timedelta(days=1),
+        renew_certificate_before: timedelta = timedelta(days=1),
+        renew_auth_token_before: timedelta = timedelta(minutes=5),
     ):
         self.resotocore_url = url
         self.psk = psk
         self.additional_headers = additional_headers
         self.custom_ca_cert_path = custom_ca_cert_path
         self.verify = verify
-        self.renew_before = renew_before
+        self.renew_certificate_before = renew_certificate_before
+        self.renew_auth_token_before = renew_auth_token_before
         self.event_loop_thread = EventLoopThread()
         self.event_loop_thread.daemon = True
         atexit.register(self.shutdown)
 
         self.state_lock = threading.Lock()
         self.client_state = ClientState.INITIALIZED
 
@@ -157,15 +159,16 @@
 
             self.async_client = AsyncResotoClient(
                 url=self.resotocore_url,
                 psk=self.psk,
                 additional_headers=self.additional_headers,
                 custom_ca_cert_path=self.custom_ca_cert_path,
                 verify=self.verify,
-                renew_before=self.renew_before,
+                renew_certificate_before=self.renew_certificate_before,
+                renew_auth_token_before=self.renew_auth_token_before,
                 loop=self.event_loop_thread.loop,
             )
 
             self.event_loop_thread.run_coroutine(self.async_client.start())
 
             self.client_state = ClientState.STARTED
```

### Comparing `resotoclient-1.3.1/resotoclient/async_client.py` & `resotoclient-1.4.0/resotoclient/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,43 +49,46 @@
         self,
         url: str,
         *,
         psk: Optional[str] = None,
         additional_headers: Optional[Dict[str, str]] = None,
         custom_ca_cert_path: Optional[str] = None,
         verify: bool = True,
-        renew_before: timedelta = timedelta(days=1),
+        renew_certificate_before: timedelta = timedelta(days=1),
+        renew_auth_token_before: timedelta = timedelta(minutes=5),
         loop: Optional[AbstractEventLoop] = None,
     ):
         """
         Create a new resoto client instance.
         :param url: the url of the resotocore instance.
         :param psk: the optional pre-shared key to use for authentication. The PSK is used to authenticate the client. If you do not have access to the PSK, you can use the auth_header parameter to authenticate with a JWT token.
         :param additional_headers: additional headers to send with each request.
         :param custom_ca_cert_path: path to a custom CA certificate to use for verifying the server certificate.
         :param verify: whether to verify the server certificate.
-        :param renew_before: how long before the certificate expires to renew it.
+        :param renew_certificate_before: how long before the certificate expires to renew it.
+        :param renew_auth_token_before: how long before the auth token expires to renew it.
         :param loop: the event loop to use.
         """
         self.resotocore_url = url
         self.psk = psk
         self.verify = verify
         self.session_id = rnd_str()
         self.holder = CertificatesHolder(
             resotocore_url=url,
             psk=psk,
             custom_ca_cert_path=custom_ca_cert_path,
-            renew_before=renew_before,
+            renew_before=renew_certificate_before,
         )
         self.http_client = AioHttpClient(
             url=url,
             psk=psk,
             session_id=self.session_id,
             get_ssl_context=self.holder.ssl_context if verify else None,
             additional_headers=additional_headers,
+            renew_auth_token_before=renew_auth_token_before,
             loop=loop,
         )
 
     async def __aenter__(self) -> "ResotoClient":
         await self.start()
         return self
 
@@ -94,18 +97,19 @@
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> None:
         await self.shutdown()
 
     async def start(self) -> None:
+        await self.http_client.start()
         await self.holder.start()
 
     async def shutdown(self) -> None:
-        await self.http_client.close()
+        await self.http_client.shutdown()
         self.holder.shutdown()
 
     def _headers(self) -> Dict[str, str]:
         headers = {"Content-type": "application/json", "Accept": "application/json"}
 
         if self.psk:
             encode_jwt_to_headers(headers, {}, self.psk)
```

### Comparing `resotoclient-1.3.1/resotoclient/ca.py` & `resotoclient-1.4.0/resotoclient/ca.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.3.1/resotoclient/http_client/__init__.py` & `resotoclient-1.4.0/resotoclient/http_client/__init__.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.3.1/resotoclient/http_client/aiohttp_client.py` & `resotoclient-1.4.0/resotoclient/http_client/aiohttp_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import asyncio
 import json
 import logging
 from contextlib import asynccontextmanager, suppress
+from datetime import datetime, timedelta, timezone
 
 from aiohttp import WSMsgType
 
 from resotoclient.http_client import AsyncHttpClient
 from resotoclient.http_client import HttpResponse
-from typing import Dict, Optional, Callable, Union, AsyncIterator, Awaitable
+from typing import Dict, Optional, Callable, Union, AsyncIterator, Awaitable, Any
 from resotoclient.models import JsValue, JsObject
-from resotoclient.jwt_utils import encode_jwt_to_headers
+from resotoclient.jwt_utils import encode_jwt_to_headers, jwt_expiration
 import aiohttp
 import ssl
 from yarl import URL
 from asyncio import AbstractEventLoop, Queue
 from multidict import CIMultiDict
 
 log = logging.getLogger(__name__)
@@ -28,23 +29,58 @@
     def __init__(
         self,
         url: str,
         *,
         psk: Optional[str],
         additional_headers: Optional[Dict[str, str]] = None,
         session_id: str,
+        renew_auth_token_before: timedelta,
         get_ssl_context: Optional[Callable[[], Awaitable[ssl.SSLContext]]] = None,
         loop: Optional[AbstractEventLoop] = None,
     ):
         self.session = aiohttp.ClientSession(loop=loop)
         self.url = url
         self.psk = psk
         self.get_ssl_context = get_ssl_context
         self.session_id = session_id
+        self.renew_auth_token_before = renew_auth_token_before
         self.additional_headers = additional_headers or {}
+        self.renew_auth_task: Optional[asyncio.Task[Any]] = None
+
+    async def start(self) -> None:
+        if "Authorization" in self.additional_headers:
+            self.renew_auth_task = asyncio.create_task(self.__schedule_renew_auth_token())
+
+    async def shutdown(self) -> None:
+        await self.close()
+        if self.renew_auth_task is not None:
+            self.renew_auth_task.cancel()
+            with suppress(asyncio.CancelledError):
+                await self.renew_auth_task
+
+    async def __schedule_renew_auth_token(self) -> None:
+        while True:
+            # get the expiration time of the current token, fallback to now
+            exp = jwt_expiration(self.additional_headers.get("Authorization", "")) or datetime.now(timezone.utc)
+            # next run is shortly before expiration, but at least 10 seconds away
+            next_run_in = max((exp - self.renew_auth_token_before) - datetime.now(timezone.utc), timedelta(seconds=10))
+            log.debug(f"Renew auth token in {next_run_in}. Going to sleep.")
+            # wait until the token should be renewed
+            await asyncio.sleep(next_run_in.total_seconds())
+            # renew the token
+            try:
+                response = await self.get("/authorization/renew")
+                if response.status_code == 200 and "Authorization" in response.headers:
+                    log.debug("Successfully renewed auth token. Replace Authorization header.")
+                    self.additional_headers["Authorization"] = response.headers["Authorization"]
+                else:
+                    # will be retried in 10 seconds. By default, we start 5 minutes before expiration - 12 attempts.
+                    log.error(f"Failed to renew auth token: {response.status_code} {await response.text()}")
+            except Exception as e:
+                log.error(f"Failed to renew auth token: {e}")
 
     async def _ssl_context(self) -> Union[ssl.SSLContext, bool]:
         if self.get_ssl_context:
             return await self.get_ssl_context()
         else:
             return False
 
@@ -96,15 +132,17 @@
         query_params = self._default_query_params()
         query_params.update(params or {})
         url = URL(self.url).with_path(path).with_query(query_params)
         request_headers = self._default_headers()
         if stream:
             request_headers.update({"Accept": "application/x-ndjson"})
         request_headers.update(headers or {})
-        resp = await self.session.get(url, ssl=await self._ssl_context(), headers=request_headers)
+        resp = await self.session.get(
+            url, ssl=await self._ssl_context(), headers=request_headers, allow_redirects=False
+        )
 
         return HttpResponse(
             status_code=resp.status,
             headers=resp.headers,
             text=resp.text,
             json=resp.json,
             payload_bytes=resp.read,
@@ -146,14 +184,15 @@
         request_headers.update(headers or {})
         resp = await self.session.post(
             url,
             ssl=await self._ssl_context(),
             headers=request_headers,
             json=json,
             data=data,
+            allow_redirects=False,
         )
 
         return HttpResponse(
             status_code=resp.status,
             headers=resp.headers,
             text=resp.text,
             json=resp.json,
@@ -174,15 +213,17 @@
 
         """
 
         query_params = self._default_query_params()
         query_params.update(params or {})
         url = URL(self.url).with_path(path).with_query(query_params)
         request_headers = self._default_headers()
-        resp = await self.session.put(url, ssl=await self._ssl_context(), headers=request_headers, json=json)
+        resp = await self.session.put(
+            url, ssl=await self._ssl_context(), headers=request_headers, json=json, allow_redirects=False
+        )
 
         return HttpResponse(
             status_code=resp.status,
             headers=resp.headers,
             text=resp.text,
             json=resp.json,
             payload_bytes=resp.read,
@@ -200,15 +241,17 @@
 
         """
 
         url = URL(self.url).with_path(path)
 
         request_headers = self._default_headers()
 
-        resp = await self.session.patch(url, ssl=await self._ssl_context(), headers=request_headers, json=json)
+        resp = await self.session.patch(
+            url, ssl=await self._ssl_context(), headers=request_headers, json=json, allow_redirects=False
+        )
 
         return HttpResponse(
             status_code=resp.status,
             headers=resp.headers,
             text=resp.text,
             json=resp.json,
             payload_bytes=resp.read,
@@ -226,15 +269,17 @@
 
         """
 
         query_params = self._default_query_params()
         query_params.update(params or {})
         url = URL(self.url).with_path(path).with_query(query_params)
         request_headers = self._default_headers()
-        resp = await self.session.delete(url, ssl=await self._ssl_context(), headers=request_headers)
+        resp = await self.session.delete(
+            url, ssl=await self._ssl_context(), headers=request_headers, allow_redirects=False
+        )
 
         return HttpResponse(
             status_code=resp.status,
             headers=resp.headers,
             text=resp.text,
             json=resp.json,
             payload_bytes=resp.read,
```

### Comparing `resotoclient-1.3.1/resotoclient/http_client/event_loop_thread.py` & `resotoclient-1.4.0/resotoclient/http_client/event_loop_thread.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.3.1/resotoclient/json_utils.py` & `resotoclient-1.4.0/resotoclient/json_utils.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.3.1/resotoclient/jwt_utils.py` & `resotoclient-1.4.0/resotoclient/jwt_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from contextlib import suppress
+from datetime import datetime, timezone
 from typing import Dict, Any, Optional, Tuple
 import os
 import jwt
 import base64
 import hashlib
 import time
 
@@ -44,23 +46,28 @@
     scheme: str = "Bearer",
     headers: Optional[Dict[str, str]] = None,
     expire_in: int = 300,
 ) -> Dict[str, str]:
     """Takes a payload and psk turns them into a JWT and adds that to a http headers
     dictionary. Also returns that dict.
     """
-    http_headers.update(
-        {"Authorization": f"{scheme} {encode_jwt(payload, psk, headers, expire_in)}"}
-    )
+    http_headers.update({"Authorization": f"{scheme} {encode_jwt(payload, psk, headers, expire_in)}"})
     return http_headers
 
 
-def decode_jwt(
-    encoded_jwt: str, psk: str, options: Optional[Dict[str, Any]] = None
-) -> Dict[str, Any]:
+def jwt_expiration(auth_header: str) -> Optional[datetime]:
+    with suppress(Exception):
+        encoded_jwt = auth_header.split(" ")[1]
+        data = jwt.decode(encoded_jwt, options={"verify_signature": False})  # type: ignore
+        if exp := data.get("exp"):
+            return datetime.fromtimestamp(exp, timezone.utc)
+    return None
+
+
+def decode_jwt(encoded_jwt: str, psk: str, options: Optional[Dict[str, Any]] = None) -> Dict[str, Any]:
     """Decode a JWT using a key derived from a pre-shared-key and a salt stored
     in the JWT headers.
     """
     salt_encoded: bytes = jwt.get_unverified_header(encoded_jwt).get("salt")  # type: ignore
     salt = base64.standard_b64decode(salt_encoded)
     key, _ = key_from_psk(psk, salt)
     return jwt.decode(encoded_jwt, key, algorithms=["HS256"], options=options or {})  # type: ignore
@@ -71,17 +78,15 @@
     psk: str,
     scheme: str = "Bearer",
     options: Optional[Dict[str, Any]] = None,
 ) -> Optional[Dict[str, str]]:
     """Retrieves the Authorization header from a http headers dictionary and
     passes it to `decode_jwt_from_header_value()` to return the decoded payload.
     """
-    authorization_header = {
-        str(k).capitalize(): v for k, v in http_headers.items()
-    }.get("Authorization")
+    authorization_header = {str(k).capitalize(): v for k, v in http_headers.items()}.get("Authorization")
     if authorization_header is None:
         return None
     return decode_jwt_from_header_value(authorization_header, psk, scheme, options)
 
 
 def decode_jwt_from_header_value(
     authorization_header: str,
```

### Comparing `resotoclient-1.3.1/resotoclient/models.py` & `resotoclient-1.4.0/resotoclient/models.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.3.1/PKG-INFO` & `resotoclient-1.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoclient
-Version: 1.3.1
+Version: 1.4.0
 Summary: Resoto Python client library
 Home-page: https://github.com/someengineering/resotoclient-python
 License: Apache-2.0
 Author: Some Engineering Inc.
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

