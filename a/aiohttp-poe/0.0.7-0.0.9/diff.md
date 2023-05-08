# Comparing `tmp/aiohttp_poe-0.0.7.tar.gz` & `tmp/aiohttp_poe-0.0.9.tar.gz`

## Comparing `aiohttp_poe-0.0.7.tar` & `aiohttp_poe-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.7/src/aiohttp_poe/__init__.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.7/src/aiohttp_poe/__main__.py
--rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.7/src/aiohttp_poe/base.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.7/src/aiohttp_poe/types.py
--rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.7/src/aiohttp_poe/samples/catbot.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.7/src/aiohttp_poe/samples/echo.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.7/.gitignore
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.7/README.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.9/src/aiohttp_poe/__init__.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.9/src/aiohttp_poe/__main__.py
+-rw-r--r--   0        0        0     6022 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.9/src/aiohttp_poe/base.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.9/src/aiohttp_poe/types.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.9/src/aiohttp_poe/samples/catbot.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.9/src/aiohttp_poe/samples/echo.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.9/README.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.9/PKG-INFO
```

### Comparing `aiohttp_poe-0.0.7/src/aiohttp_poe/base.py` & `aiohttp_poe-0.0.9/src/aiohttp_poe/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,13 +160,13 @@
     handler: Callable[[web.Request], Awaitable[web.Response]], api_key: str = ""
 ) -> None:
     parser = argparse.ArgumentParser("aiohttp sample Poe bot server")
     parser.add_argument("-p", "--port", type=int, default=8080)
     args = parser.parse_args()
 
     global auth_key
-    auth_key = api_key if api_key else os.environ.get("POE_API_KEY", None)
+    auth_key = api_key if api_key else os.environ.get("POE_API_KEY")
 
     app = web.Application(middlewares=[auth_middleware])
     app.add_routes([web.get("/", index)])
     app.add_routes([web.post("/", handler)])
     web.run_app(app, port=args.port)
```

### Comparing `aiohttp_poe-0.0.7/src/aiohttp_poe/types.py` & `aiohttp_poe-0.0.9/src/aiohttp_poe/types.py`

 * *Files identical despite different names*

### Comparing `aiohttp_poe-0.0.7/src/aiohttp_poe/samples/catbot.py` & `aiohttp_poe-0.0.9/src/aiohttp_poe/samples/catbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 
-Demo bot: Altai the cat.
+Demo bot: catbot.
 
 """
 from __future__ import annotations
 
 import asyncio
 from typing import AsyncIterator
 
@@ -78,15 +78,15 @@
                 "Cube snacks are even less tasty.", allow_retry=False
             )
         elif "count" in last_message:
             for i in range(1, 11):
                 yield self.replace_response_event(str(i))
                 if "quickly" not in last_message:
                     await asyncio.sleep(1)
-        # These messages make Altai do something that's not allowed by the protocol
+        # These messages make the cat do something that's not allowed by the protocol
         elif "scratch" in last_message:
             yield ("purr", {"text": "purr"})  # type: ignore
         elif "toy" in last_message:
             for _ in range(1010):
                 yield self.text_event("hit ")
         elif "bed" in last_message:
             yield self.text_event("z" * 10_010)
```

### Comparing `aiohttp_poe-0.0.7/src/aiohttp_poe/samples/echo.py` & `aiohttp_poe-0.0.9/src/aiohttp_poe/samples/echo.py`

 * *Files identical despite different names*

### Comparing `aiohttp_poe-0.0.7/README.md` & `aiohttp_poe-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `aiohttp_poe-0.0.7/pyproject.toml` & `aiohttp_poe-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aiohttp_poe"
-version = "0.0.7"
+version = "0.0.9"
 authors = [
   { name="Jelle Zijlstra", email="jelle@quora.com" },
 ]
 description = "A demonstration of the Poe protocol using aiohttp"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `aiohttp_poe-0.0.7/PKG-INFO` & `aiohttp_poe-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp_poe
-Version: 0.0.7
+Version: 0.0.9
 Summary: A demonstration of the Poe protocol using aiohttp
 Project-URL: Homepage, https://github.com/quora/poe-protocol
 Author-email: Jelle Zijlstra <jelle@quora.com>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

