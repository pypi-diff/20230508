# Comparing `tmp/async_rotating_proxy-0.0.3.tar.gz` & `tmp/async_rotating_proxy-0.0.4.tar.gz`

## Comparing `async_rotating_proxy-0.0.3.tar` & `async_rotating_proxy-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.3/requirements.txt
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.3/src/async_rotating_proxy/__init__.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.3/src/async_rotating_proxy/browser.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.3/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.3/README.md
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.4/src/async_rotating_proxy/__init__.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.4/src/async_rotating_proxy/browser.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.4/README.md
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 async_rotating_proxy-0.0.4/PKG-INFO
```

### Comparing `async_rotating_proxy-0.0.3/src/async_rotating_proxy/__init__.py` & `async_rotating_proxy-0.0.4/src/async_rotating_proxy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 from fastapi import FastAPI
+from fastapi.requests import Request
 from fastapi.responses import HTMLResponse
 import uvicorn
 
+from fake_headers import Headers
+
 import aiohttp
 from multiprocessing import Process
 
 import urllib.parse
 import random
 import os
 
 
 def app(proxies: list[str],
         proxy_username: str | None = None, 
         proxy_password: str | None = None,
         proxy_scheme: str = "http",
-        headers: dict = {"User-Agent": "Chrome"}):
+        fake_headers: bool = True
+        ):
     """Create a FastAPI instance which routes GET requests through proxies.
 
     Args:
         proxies (list[str]): List of proxies to route traffic through in format ip:port
         username (str | None): Username for authentication if any
         password: (str | None): Password for authenticaiton if any
         schemes: (tuple[str]): URI schemes for proxies (http, https, socks5)
-        headers (dict): HTTP Headers to attach to requests
+        fake_headers (bool): Generate fake headers for requests
 
     Returns:
         FastAPI: The proxy-redirect server
     """
 
     app = FastAPI()
 
     app.pid = os.getpid()
 
     @app.get("/")
-    async def forward_proxy(url: str):
+    async def forward_proxy(request: Request, url: str):
         """Forward a request through a proxy and return the response
 
         Args:
             url (str): URL to get encoded with urllib.parse.quote_plus()
 
         Returns:
             HTMLResponse: The requested page obtained through proxy
@@ -52,14 +56,16 @@
         if proxy_username and proxy_password:
             proxy = f"{proxy_scheme}://{proxy_username}:{proxy_password}@{proxy}"
         else:
             proxy = f"{proxy_scheme}://{proxy}"
 
         # Get the page and return HTML response
         async with aiohttp.ClientSession() as session:
+            headers = Headers(headers=True).generate() if fake_headers else {}
+
             async with session.get(url, proxy=proxy, headers=headers) as response:
                 html = await response.content.read()
                 return HTMLResponse(html.decode())
 
     return app
 
 
@@ -74,30 +80,33 @@
 
     Constructor Args:
         proxies (list[str]): List of proxies to rotate through in ip:port form
         proxy_username (str | None): Username for proxy authentication if applicable
         proxy_password (str | None): Password for proxy authentication if applicable
         port (int): The port on localhost where the proxy API is running
         proxy_scheme (http): The scheme of the proxy server
+        fake_headers (bool): Set fake headers on each request
     """
     api_pid: int
 
     def __init__(
             self,
             proxies: list[str], 
             proxy_username: str | None = None,
             proxy_password: str | None = None,
             port: int = 8000,
-            proxy_scheme: str = "http"
+            proxy_scheme: str = "http",
+            fake_headers: bool = True
         ):
         self.proxies = proxies
         self.proxy_username = proxy_username
         self.proxy_password = proxy_password
         self.port = port
         self.proxy_scheme = proxy_scheme
+        self.fake_headers = fake_headers
 
 
     def __enter__(self):
         self._process = Process(target=self._start_server)
         self._process.start()
         return self
         
@@ -107,15 +116,16 @@
 
 
     def _start_server(self):
         """Start a FastAPI daemon for routing requests through proxies."""
         api = app(self.proxies, 
                   proxy_username=self.proxy_username,
                   proxy_password=self.proxy_password,
-                  proxy_scheme=self.proxy_scheme)
+                  proxy_scheme=self.proxy_scheme,
+                  fake_headers=self.fake_headers)
 
         uvicorn.run(api, port=self.port)
 
 
     def format_url(self, url: str):
         """Format the URL to route through the ProxyAPI server.
```

### Comparing `async_rotating_proxy-0.0.3/src/async_rotating_proxy/browser.py` & `async_rotating_proxy-0.0.4/src/async_rotating_proxy/browser.py`

 * *Files identical despite different names*

### Comparing `async_rotating_proxy-0.0.3/LICENSE.txt` & `async_rotating_proxy-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `async_rotating_proxy-0.0.3/README.md` & `async_rotating_proxy-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `async_rotating_proxy-0.0.3/pyproject.toml` & `async_rotating_proxy-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "async_rotating_proxy"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="Greg Bizup", email="g.bizup@gmail.com" }
 ]
 description = "Run an API on your local machine that reroutes traffic through rotating proxies. Useful for pyppeteer proxy rotation."
 readme = "README.md"
 requires-python = ">3.10"
 classifiers = [
```

### Comparing `async_rotating_proxy-0.0.3/PKG-INFO` & `async_rotating_proxy-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_rotating_proxy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Run an API on your local machine that reroutes traffic through rotating proxies. Useful for pyppeteer proxy rotation.
 Project-URL: Homepage, https://github.com/gbiz123/async-rotating-proxy
 Author-email: Greg Bizup <g.bizup@gmail.com>
 License-File: LICENSE.txt
 Keywords: fastapi,proxy,pyppeteer,rotating proxy,scraping
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

