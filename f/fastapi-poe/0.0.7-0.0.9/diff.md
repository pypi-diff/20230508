# Comparing `tmp/fastapi_poe-0.0.7.tar.gz` & `tmp/fastapi_poe-0.0.9.tar.gz`

## Comparing `fastapi_poe-0.0.7.tar` & `fastapi_poe-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fastapi_poe-0.0.7/src/fastapi_poe/__init__.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 fastapi_poe-0.0.7/src/fastapi_poe/__main__.py
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 fastapi_poe-0.0.7/src/fastapi_poe/base.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 fastapi_poe-0.0.7/src/fastapi_poe/types.py
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 fastapi_poe-0.0.7/src/fastapi_poe/samples/catbot.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastapi_poe-0.0.7/src/fastapi_poe/samples/echo.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fastapi_poe-0.0.7/.gitignore
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 fastapi_poe-0.0.7/README.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 fastapi_poe-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 fastapi_poe-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fastapi_poe-0.0.9/src/fastapi_poe/__init__.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 fastapi_poe-0.0.9/src/fastapi_poe/__main__.py
+-rw-r--r--   0        0        0     7962 2020-02-02 00:00:00.000000 fastapi_poe-0.0.9/src/fastapi_poe/base.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 fastapi_poe-0.0.9/src/fastapi_poe/types.py
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 fastapi_poe-0.0.9/src/fastapi_poe/samples/catbot.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastapi_poe-0.0.9/src/fastapi_poe/samples/echo.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fastapi_poe-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 fastapi_poe-0.0.9/README.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 fastapi_poe-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 fastapi_poe-0.0.9/PKG-INFO
```

### Comparing `fastapi_poe-0.0.7/src/fastapi_poe/base.py` & `fastapi_poe-0.0.9/src/fastapi_poe/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,16 +154,20 @@
         return JSONResponse({})
 
     async def handle_settings(self, settings_request: SettingsRequest) -> JSONResponse:
         settings = await self.get_settings(settings_request)
         return JSONResponse(settings.dict())
 
     async def handle_query(self, query: QueryRequest) -> AsyncIterable[ServerSentEvent]:
-        async for event in self.get_response(query):
-            yield event
+        try:
+            async for event in self.get_response(query):
+                yield event
+        except Exception as e:
+            logger.exception("Error responding to query")
+            yield self.error_event(repr(e), allow_retry=False)
         yield self.done_event()
 
 
 def run(handler: PoeHandler, api_key: str = "") -> None:
     """
     Run a Poe bot server using FastAPI.
 
@@ -180,15 +184,15 @@
 
     global logger
     logger = logging.getLogger("uvicorn.default")
     app = FastAPI()
     app.add_exception_handler(RequestValidationError, exception_handler)
 
     global auth_key
-    auth_key = api_key if api_key else os.environ.get("POE_API_KEY", None)
+    auth_key = api_key if api_key else os.environ.get("POE_API_KEY")
 
     @app.get("/")
     async def index() -> Response:
         url = "https://poe.com/create_bot?api=1"
         return HTMLResponse(
             "<html><body><h1>FastAPI Poe bot server</h1><p>Congratulations! Your server"
             " is running. To connect it to Poe, create a bot at <a"
```

### Comparing `fastapi_poe-0.0.7/src/fastapi_poe/types.py` & `fastapi_poe-0.0.9/src/fastapi_poe/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     type: FeedbackType
     reason: Optional[str]
 
 
 class ProtocolMessage(BaseModel):
     """A message as used in the Poe protocol."""
 
-    role: Literal["system", "user", "bot", "assistant"]
+    role: Literal["system", "user", "bot"]
     content: str
     content_type: ContentType
     timestamp: int
     message_id: str
     message_type: Optional[str]
     feedback: List[MessageFeedback]
```

### Comparing `fastapi_poe-0.0.7/src/fastapi_poe/samples/catbot.py` & `fastapi_poe-0.0.9/src/fastapi_poe/samples/catbot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 
-Demo bot: Altai the cat.
+Demo bot: catbot.
 
 """
 from __future__ import annotations
 
 import asyncio
 import json
 from typing import AsyncIterable
@@ -76,15 +76,15 @@
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
             yield ServerSentEvent(event="purr", data=json.dumps({"text": "purr"}))
         elif "toy" in last_message:
             for _ in range(1010):
                 yield self.text_event("hit ")
         elif "bed" in last_message:
             yield self.text_event("z" * 10_010)
```

### Comparing `fastapi_poe-0.0.7/src/fastapi_poe/samples/echo.py` & `fastapi_poe-0.0.9/src/fastapi_poe/samples/echo.py`

 * *Files identical despite different names*

### Comparing `fastapi_poe-0.0.7/README.md` & `fastapi_poe-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_poe-0.0.7/pyproject.toml` & `fastapi_poe-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastapi_poe"
-version = "0.0.7"
+version = "0.0.9"
 authors = [
   { name="Lida Li", email="lli@quora.com" },
 ]
 description = "A demonstration of the Poe protocol using FastAPI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `fastapi_poe-0.0.7/PKG-INFO` & `fastapi_poe-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_poe
-Version: 0.0.7
+Version: 0.0.9
 Summary: A demonstration of the Poe protocol using FastAPI
 Project-URL: Homepage, https://github.com/quora/poe-protocol
 Author-email: Lida Li <lli@quora.com>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

