# Comparing `tmp/simple_ai_server-0.2.0.tar.gz` & `tmp/simple_ai_server-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_ai_server-0.2.0.tar", max compression
+gzip compressed data, was "simple_ai_server-0.2.1.tar", max compression
```

## Comparing `simple_ai_server-0.2.0.tar` & `simple_ai_server-0.2.1.tar`

### file list

```diff
@@ -1,44 +1,46 @@
--rw-r--r--   0        0        0     1092 2023-04-12 14:38:29.075976 simple_ai_server-0.2.0/LICENSE
--rw-r--r--   0        0        0     5572 2023-04-12 15:29:07.213015 simple_ai_server-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5386 2023-04-12 14:38:29.076977 simple_ai_server-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-03-18 16:45:18.115514 simple_ai_server-0.2.0/src/simple_ai/__init__.py
--rw-r--r--   0        0        0     1072 2023-04-05 13:55:01.576228 simple_ai_server-0.2.0/src/simple_ai/__main__.py
--rw-r--r--   0        0        0     3286 2023-03-31 16:24:31.515208 simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/__pycache__/client.cpython-311.pyc
--rw-r--r--   0        0        0     2027 2023-03-31 15:37:59.978527 simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/__pycache__/llm_chat_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     3570 2023-03-31 16:24:31.521708 simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/__pycache__/llm_chat_pb2_grpc.cpython-311.pyc
--rw-r--r--   0        0        0     1219 2023-03-31 15:37:59.985026 simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/__pycache__/model.cpython-311.pyc
--rw-r--r--   0        0        0     3138 2023-04-12 14:38:29.078476 simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/client.py
--rw-r--r--   0        0        0     2432 2023-04-12 14:38:29.078476 simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/llm_chat_pb2.py
--rw-r--r--   0        0        0     2402 2023-04-05 13:55:01.577727 simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/llm_chat_pb2.pyi
--rw-r--r--   0        0        0     4016 2023-04-12 14:38:29.078976 simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/llm_chat_pb2_grpc.py
--rw-r--r--   0        0        0      435 2023-04-12 14:38:29.079476 simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/model.py
--rw-r--r--   0        0        0     2883 2023-04-12 14:38:29.079975 simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/server.py
--rw-r--r--   0        0        0     2387 2023-03-31 16:24:31.475207 simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/__pycache__/client.cpython-311.pyc
--rw-r--r--   0        0        0     1958 2023-03-31 16:24:31.498707 simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/__pycache__/llm_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     4830 2023-03-31 16:24:31.513707 simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/__pycache__/llm_pb2_grpc.cpython-311.pyc
--rw-r--r--   0        0        0     2969 2023-04-12 14:38:29.080975 simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/client.py
--rw-r--r--   0        0        0     2186 2023-04-05 13:55:01.579226 simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/llm_pb2.py
--rw-r--r--   0        0        0     2246 2023-04-05 13:55:01.579727 simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/llm_pb2.pyi
--rw-r--r--   0        0        0     3956 2023-04-05 13:55:01.580227 simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/llm_pb2_grpc.py
--rw-r--r--   0        0        0     1326 2023-04-12 14:38:29.081475 simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/model.py
--rw-r--r--   0        0        0     2564 2023-04-12 14:38:29.081975 simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/server.py
--rw-r--r--   0        0        0     1788 2023-03-31 16:24:31.524207 simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/__pycache__/client.cpython-311.pyc
--rw-r--r--   0        0        0     1880 2023-03-31 16:24:31.525208 simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/__pycache__/llm_embed_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     3594 2023-03-31 16:24:31.526707 simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/__pycache__/llm_embed_pb2_grpc.cpython-311.pyc
--rw-r--r--   0        0        0      813 2023-04-05 13:55:01.581227 simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/client.py
--rw-r--r--   0        0        0     1808 2023-04-05 13:55:01.581727 simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/llm_embed_pb2.py
--rw-r--r--   0        0        0     1175 2023-04-05 13:55:01.581727 simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/llm_embed_pb2.pyi
--rw-r--r--   0        0        0     2483 2023-04-05 13:55:01.582227 simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/llm_embed_pb2_grpc.py
--rw-r--r--   0        0        0      266 2023-04-05 13:55:01.582727 simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/model.py
--rw-r--r--   0        0        0     1577 2023-04-05 13:55:01.583227 simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/server.py
--rw-r--r--   0        0        0     1005 2023-04-12 14:38:29.082476 simple_ai_server-0.2.0/src/simple_ai/api/grpc/protos/llm_chat.proto
--rw-r--r--   0        0        0      955 2023-04-05 13:55:01.584227 simple_ai_server-0.2.0/src/simple_ai/api/grpc/protos/llm_complete.proto
--rw-r--r--   0        0        0      599 2023-04-05 13:55:01.584227 simple_ai_server-0.2.0/src/simple_ai/api/grpc/protos/llm_embed.proto
--rw-r--r--   0        0        0     1233 2023-04-12 14:38:29.082975 simple_ai_server-0.2.0/src/simple_ai/api_models.py
--rw-r--r--   0        0        0     2345 2023-04-12 15:10:37.779433 simple_ai_server-0.2.0/src/simple_ai/dummy.py
--rw-r--r--   0        0        0     5743 2023-04-12 14:38:29.083476 simple_ai_server-0.2.0/src/simple_ai/models.py
--rw-r--r--   0        0        0      226 2023-03-17 17:21:47.275098 simple_ai_server-0.2.0/src/simple_ai/models.toml
--rw-r--r--   0        0        0      214 2023-04-05 13:55:01.586227 simple_ai_server-0.2.0/src/simple_ai/models.toml.template
--rw-r--r--   0        0        0     6049 2023-04-12 14:38:29.083975 simple_ai_server-0.2.0/src/simple_ai/server.py
--rw-r--r--   0        0        0     3677 2023-04-12 15:10:37.779934 simple_ai_server-0.2.0/src/simple_ai/utils.py
--rw-r--r--   0        0        0     5818 1970-01-01 00:00:00.000000 simple_ai_server-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-12 14:38:29.075976 simple_ai_server-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5572 2023-05-08 11:35:05.011016 simple_ai_server-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7064 2023-05-08 11:27:06.205433 simple_ai_server-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-03-18 16:45:18.115514 simple_ai_server-0.2.1/src/simple_ai/__init__.py
+-rw-r--r--   0        0        0     1072 2023-04-05 13:55:01.576228 simple_ai_server-0.2.1/src/simple_ai/__main__.py
+-rw-r--r--   0        0        0     5301 2023-04-12 18:02:19.982416 simple_ai_server-0.2.1/src/simple_ai/api/grpc/chat/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0        0        0     2138 2023-04-12 18:02:19.368416 simple_ai_server-0.2.1/src/simple_ai/api/grpc/chat/__pycache__/llm_chat_pb2.cpython-311.pyc
+-rw-r--r--   0        0        0     4745 2023-04-12 18:02:20.045416 simple_ai_server-0.2.1/src/simple_ai/api/grpc/chat/__pycache__/llm_chat_pb2_grpc.cpython-311.pyc
+-rw-r--r--   0        0        0     1469 2023-04-12 18:31:07.688955 simple_ai_server-0.2.1/src/simple_ai/api/grpc/chat/__pycache__/model.cpython-311.pyc
+-rw-r--r--   0        0        0     4926 2023-04-12 18:31:07.686953 simple_ai_server-0.2.1/src/simple_ai/api/grpc/chat/__pycache__/server.cpython-311.pyc
+-rw-r--r--   0        0        0     3138 2023-04-26 18:45:51.117116 simple_ai_server-0.2.1/src/simple_ai/api/grpc/chat/client.py
+-rw-r--r--   0        0        0     2432 2023-04-12 14:38:29.078476 simple_ai_server-0.2.1/src/simple_ai/api/grpc/chat/llm_chat_pb2.py
+-rw-r--r--   0        0        0     2402 2023-04-05 13:55:01.577727 simple_ai_server-0.2.1/src/simple_ai/api/grpc/chat/llm_chat_pb2.pyi
+-rw-r--r--   0        0        0     4016 2023-04-12 14:38:29.078976 simple_ai_server-0.2.1/src/simple_ai/api/grpc/chat/llm_chat_pb2_grpc.py
+-rw-r--r--   0        0        0      435 2023-04-26 18:45:51.117614 simple_ai_server-0.2.1/src/simple_ai/api/grpc/chat/model.py
+-rw-r--r--   0        0        0     2883 2023-04-12 14:38:29.079975 simple_ai_server-0.2.1/src/simple_ai/api/grpc/chat/server.py
+-rw-r--r--   0        0        0     4131 2023-04-12 18:02:20.052416 simple_ai_server-0.2.1/src/simple_ai/api/grpc/completion/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0        0        0     1951 2023-04-12 18:02:20.060416 simple_ai_server-0.2.1/src/simple_ai/api/grpc/completion/__pycache__/llm_pb2.cpython-311.pyc
+-rw-r--r--   0        0        0     4770 2023-04-12 18:02:20.067416 simple_ai_server-0.2.1/src/simple_ai/api/grpc/completion/__pycache__/llm_pb2_grpc.cpython-311.pyc
+-rw-r--r--   0        0        0     2969 2023-04-12 14:38:29.080975 simple_ai_server-0.2.1/src/simple_ai/api/grpc/completion/client.py
+-rw-r--r--   0        0        0     2186 2023-04-05 13:55:01.579226 simple_ai_server-0.2.1/src/simple_ai/api/grpc/completion/llm_pb2.py
+-rw-r--r--   0        0        0     2246 2023-04-05 13:55:01.579727 simple_ai_server-0.2.1/src/simple_ai/api/grpc/completion/llm_pb2.pyi
+-rw-r--r--   0        0        0     3956 2023-04-05 13:55:01.580227 simple_ai_server-0.2.1/src/simple_ai/api/grpc/completion/llm_pb2_grpc.py
+-rw-r--r--   0        0        0     1326 2023-04-26 18:45:51.118115 simple_ai_server-0.2.1/src/simple_ai/api/grpc/completion/model.py
+-rw-r--r--   0        0        0     2564 2023-04-12 14:38:29.081975 simple_ai_server-0.2.1/src/simple_ai/api/grpc/completion/server.py
+-rw-r--r--   0        0        0     1781 2023-04-12 18:02:20.072915 simple_ai_server-0.2.1/src/simple_ai/api/grpc/embedding/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0        0        0     1878 2023-04-12 18:02:20.074917 simple_ai_server-0.2.1/src/simple_ai/api/grpc/embedding/__pycache__/llm_embed_pb2.cpython-311.pyc
+-rw-r--r--   0        0        0     3544 2023-04-12 18:02:20.080916 simple_ai_server-0.2.1/src/simple_ai/api/grpc/embedding/__pycache__/llm_embed_pb2_grpc.cpython-311.pyc
+-rw-r--r--   0        0        0      813 2023-04-05 13:55:01.581227 simple_ai_server-0.2.1/src/simple_ai/api/grpc/embedding/client.py
+-rw-r--r--   0        0        0     1808 2023-04-05 13:55:01.581727 simple_ai_server-0.2.1/src/simple_ai/api/grpc/embedding/llm_embed_pb2.py
+-rw-r--r--   0        0        0     1175 2023-04-05 13:55:01.581727 simple_ai_server-0.2.1/src/simple_ai/api/grpc/embedding/llm_embed_pb2.pyi
+-rw-r--r--   0        0        0     2483 2023-04-05 13:55:01.582227 simple_ai_server-0.2.1/src/simple_ai/api/grpc/embedding/llm_embed_pb2_grpc.py
+-rw-r--r--   0        0        0      266 2023-04-26 18:45:51.118615 simple_ai_server-0.2.1/src/simple_ai/api/grpc/embedding/model.py
+-rw-r--r--   0        0        0     1577 2023-04-05 13:55:01.583227 simple_ai_server-0.2.1/src/simple_ai/api/grpc/embedding/server.py
+-rw-r--r--   0        0        0      510 2023-04-12 17:43:20.233161 simple_ai_server-0.2.1/src/simple_ai/api/grpc/protos/images.proto
+-rw-r--r--   0        0        0     1005 2023-04-12 14:38:29.082476 simple_ai_server-0.2.1/src/simple_ai/api/grpc/protos/llm_chat.proto
+-rw-r--r--   0        0        0      955 2023-04-05 13:55:01.584227 simple_ai_server-0.2.1/src/simple_ai/api/grpc/protos/llm_complete.proto
+-rw-r--r--   0        0        0      599 2023-04-05 13:55:01.584227 simple_ai_server-0.2.1/src/simple_ai/api/grpc/protos/llm_embed.proto
+-rw-r--r--   0        0        0     1968 2023-04-30 14:22:44.494160 simple_ai_server-0.2.1/src/simple_ai/api_models.py
+-rw-r--r--   0        0        0     2345 2023-04-12 15:10:37.779433 simple_ai_server-0.2.1/src/simple_ai/dummy.py
+-rw-r--r--   0        0        0     6061 2023-05-08 11:27:06.206432 simple_ai_server-0.2.1/src/simple_ai/models.py
+-rw-r--r--   0        0        0      226 2023-03-17 17:21:47.275098 simple_ai_server-0.2.1/src/simple_ai/models.toml
+-rw-r--r--   0        0        0      214 2023-04-05 13:55:01.586227 simple_ai_server-0.2.1/src/simple_ai/models.toml.template
+-rw-r--r--   0        0        0     6284 2023-05-08 11:27:06.207432 simple_ai_server-0.2.1/src/simple_ai/server.py
+-rw-r--r--   0        0        0     3917 2023-05-08 11:27:06.208432 simple_ai_server-0.2.1/src/simple_ai/utils.py
+-rw-r--r--   0        0        0     7439 1970-01-01 00:00:00.000000 simple_ai_server-0.2.1/PKG-INFO
```

### Comparing `simple_ai_server-0.2.0/LICENSE` & `simple_ai_server-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/pyproject.toml` & `simple_ai_server-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simple_ai_server"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Louis Hénault"]
 readme = "README.md"
 packages = [{include = "simple_ai", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `simple_ai_server-0.2.0/README.md` & `simple_ai_server-0.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -140,14 +140,71 @@
 openai.api_base = "http://127.0.0.1:8080"
 
 # Do your usual things, for instance a completion query:
 print(openai.Model.list())
 completion = openai.Completion.create(model="llama-7B", prompt="Hello everyone this is")
 ```
 
+## Common issues and solutions
+
+### Adding a CORS middleware
+
+If you encounter CORS issues, it is suggested to not use the `simple_ai serve` command, but to rather use your own script to add your CORS configuration, using the [FastAPI CORS middleware](https://fastapi.tiangolo.com/tutorial/cors/).
+
+For instance you can create `my_server.py` with:
+
+```python
+from simple_ai.server import app
+from fastapi.middleware.cors import CORSMiddleware
+
+def add_cors(app):
+    origins = [
+        "http://localhost",
+        "http://localhost:8080"
+    ]
+    app.add_middleware(
+        CORSMiddleware,
+        allow_origins=origins,
+        allow_credentials=True,
+        allow_methods=["*"],
+        allow_headers=["*"],
+    )
+    return app
+
+def serve_app(host="127.0.0.1", port=8080, **kwargs):
+    app = add_cors(app)
+    uvicorn.run(app=app, host=host, port=port)
+    
+if __name__ == "__main__":
+    serve_app(host="127.0.0.1", port=8080)
+    
+```
+
+And run it as `python3 my_server.py` instead.
+
+### I needd `/v1` prefix in the endpoints
+
+Some projects have decided to include the `/v1` prefix as part of the endpoints, while OpenAI client includes it in its `api_base` parameter. If you need to have it as part of the endpoints for your project, you can use a custom script instead of `simple_ai serve`:
+
+```python
+import uvicorn
+from simple_ai.server import app as v1_app
+from fastapi import APIRouter, FastAPI
+
+sai_app = FastAPI()
+sai_app.mount("/v1", v1_app)
+
+def serve_app(app=sai_app, host="0.0.0.0", port=8080):
+    uvicorn.run(app=app, host=host, port=port)
+    
+if __name__ == "__main__":
+    serve_app()
+    
+```
+
 ## Contribute
 
 This is very much work in progress and far from being perfect, so let me know if you want to help. PR, issues, documentation, cool logo, all the usual candidates are welcome.
 
 ### Development Environment
 
 In order for the following steps to work it is required to have make and poetry installed on your system.
```

### Comparing `simple_ai_server-0.2.0/src/simple_ai/__main__.py` & `simple_ai_server-0.2.1/src/simple_ai/__main__.py`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/__pycache__/llm_chat_pb2.cpython-311.pyc` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/chat/__pycache__/llm_chat_pb2.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x60fc2664 (Fri Mar 31 15:29:36 2023 UTC)
-files sz: 2065
+moddate:  0x65c23664 (Wed Apr 12 14:38:29 2023 UTC)
+files sz: 2432
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x970064005a00640164026c016d025a030100640164036c046d055a0601
@@ -51,130 +51,133 @@
      8          42 LOAD_CONST               1 (0)
                 44 LOAD_CONST               5 (('symbol_database',))
                 46 IMPORT_NAME              4 (google.protobuf)
                 48 IMPORT_FROM              9 (symbol_database)
                 50 STORE_NAME              10 (_symbol_database)
                 52 POP_TOP
    
-    11          54 PUSH_NULL
+    12          54 PUSH_NULL
                 56 LOAD_NAME               10 (_symbol_database)
                 58 LOAD_ATTR               11 (Default)
                 68 PRECALL                  0
                 72 CALL                     0
                 82 STORE_NAME              12 (_sym_db)
    
-    16          84 PUSH_NULL
+    15          84 PUSH_NULL
                 86 LOAD_NAME                8 (_descriptor_pool)
                 88 LOAD_ATTR               11 (Default)
                 98 PRECALL                  0
                102 CALL                     0
                112 LOAD_METHOD             13 (AddSerializedFile)
-               134 LOAD_CONST               6 (b'\n\x0ellm_chat.proto\x12\x11languagemodelchat"\xe3\x01\n\x0cChatLogInput\x12)\n\x08messages\x18\x01 \x03(\x0b2\x17.languagemodelchat.Chat\x12\x12\n\nmax_tokens\x18\x02 \x01(\x05\x12\x13\n\x0btemperature\x18\x03 \x01(\x02\x12\r\n\x05top_p\x18\x04 \x01(\x02\x12\t\n\x01n\x18\x05 \x01(\x05\x12\x0e\n\x06stream\x18\x06 \x01(\x08\x12\x0c\n\x04stop\x18\x07 \x01(\t\x12\x18\n\x10presence_penalty\x18\x08 \x01(\x02\x12\x19\n\x11frequence_penalty\x18\t \x01(\x02\x12\x12\n\nlogit_bias\x18\n \x01(\t":\n\rChatLogOutput\x12)\n\x08messages\x18\x01 \x03(\x0b2\x17.languagemodelchat.Chat"%\n\x04Chat\x12\x0c\n\x04role\x18\x01 \x01(\t\x12\x0f\n\x07content\x18\x02 \x01(\t2\\\n\rLanguageModel\x12K\n\x04Chat\x12\x1f.languagemodelchat.ChatLogInput\x1a .languagemodelchat.ChatLogOutput"\x00B3\n\x15io.grpc.examples.chatB\x11LanguageModelChatP\x01\xa2\x02\x04chatb\x06proto3')
-               136 PRECALL                  1
+   
+    16         134 LOAD_CONST               6 (b'\n\x0ellm_chat.proto\x12\x11languagemodelchat"\xe3\x01\n\x0cChatLogInput\x12)\n\x08messages\x18\x01 \x03(\x0b2\x17.languagemodelchat.Chat\x12\x12\n\nmax_tokens\x18\x02 \x01(\x05\x12\x13\n\x0btemperature\x18\x03 \x01(\x02\x12\r\n\x05top_p\x18\x04 \x01(\x02\x12\t\n\x01n\x18\x05 \x01(\x05\x12\x0e\n\x06stream\x18\x06 \x01(\x08\x12\x0c\n\x04stop\x18\x07 \x01(\t\x12\x18\n\x10presence_penalty\x18\x08 \x01(\x02\x12\x19\n\x11frequence_penalty\x18\t \x01(\x02\x12\x12\n\nlogit_bias\x18\n \x01(\t":\n\rChatLogOutput\x12)\n\x08messages\x18\x01 \x03(\x0b2\x17.languagemodelchat.Chat"D\n\x04Chat\x12\x11\n\x04role\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x14\n\x07content\x18\x02 \x01(\tH\x01\x88\x01\x01B\x07\n\x05_roleB\n\n\x08_content2\xad\x01\n\rLanguageModel\x12K\n\x04Chat\x12\x1f.languagemodelchat.ChatLogInput\x1a .languagemodelchat.ChatLogOutput"\x00\x12O\n\x06Stream\x12\x1f.languagemodelchat.ChatLogInput\x1a .languagemodelchat.ChatLogOutput"\x000\x01B3\n\x15io.grpc.examples.chatB\x11LanguageModelChatP\x01\xa2\x02\x04chatb\x06proto3')
+   
+    15         136 PRECALL                  1
                140 CALL                     1
                150 STORE_NAME              14 (DESCRIPTOR)
    
-    18         152 PUSH_NULL
+    30         152 PUSH_NULL
                154 LOAD_NAME                3 (_builder)
                156 LOAD_ATTR               15 (BuildMessageAndEnumDescriptors)
                166 LOAD_NAME               14 (DESCRIPTOR)
                168 PUSH_NULL
                170 LOAD_NAME               16 (globals)
                172 PRECALL                  0
                176 CALL                     0
                186 PRECALL                  2
                190 CALL                     2
                200 POP_TOP
    
-    19         202 PUSH_NULL
+    31         202 PUSH_NULL
                204 LOAD_NAME                3 (_builder)
                206 LOAD_ATTR               17 (BuildTopDescriptorsAndMessages)
                216 LOAD_NAME               14 (DESCRIPTOR)
                218 LOAD_CONST               7 ('llm_chat_pb2')
                220 PUSH_NULL
                222 LOAD_NAME               16 (globals)
                224 PRECALL                  0
                228 CALL                     0
                238 PRECALL                  3
                242 CALL                     3
                252 POP_TOP
    
-    20         254 LOAD_NAME                6 (_descriptor)
+    32         254 LOAD_NAME                6 (_descriptor)
                256 LOAD_ATTR               18 (_USE_C_DESCRIPTORS)
                266 LOAD_CONST               8 (False)
                268 COMPARE_OP               2 (==)
                274 POP_JUMP_FORWARD_IF_FALSE    72 (to 420)
    
-    22         276 LOAD_CONST               9 (None)
+    33         276 LOAD_CONST               9 (None)
                278 LOAD_NAME               14 (DESCRIPTOR)
                280 STORE_ATTR              19 (_options)
    
-    23         290 LOAD_CONST              10 (b'\n\x15io.grpc.examples.chatB\x11LanguageModelChatP\x01\xa2\x02\x04chat')
-               292 LOAD_NAME               14 (DESCRIPTOR)
+    35         290 LOAD_CONST              10 (b'\n\x15io.grpc.examples.chatB\x11LanguageModelChatP\x01\xa2\x02\x04chat')
+   
+    34         292 LOAD_NAME               14 (DESCRIPTOR)
                294 STORE_ATTR              20 (_serialized_options)
    
-    24         304 LOAD_CONST              11 (38)
+    37         304 LOAD_CONST              11 (38)
                306 LOAD_NAME               21 (_CHATLOGINPUT)
                308 STORE_ATTR              22 (_serialized_start)
    
-    25         318 LOAD_CONST              12 (265)
+    38         318 LOAD_CONST              12 (265)
                320 LOAD_NAME               21 (_CHATLOGINPUT)
                322 STORE_ATTR              23 (_serialized_end)
    
-    26         332 LOAD_CONST              13 (267)
+    39         332 LOAD_CONST              13 (267)
                334 LOAD_NAME               24 (_CHATLOGOUTPUT)
                336 STORE_ATTR              22 (_serialized_start)
    
-    27         346 LOAD_CONST              14 (325)
+    40         346 LOAD_CONST              14 (325)
                348 LOAD_NAME               24 (_CHATLOGOUTPUT)
                350 STORE_ATTR              23 (_serialized_end)
    
-    28         360 LOAD_CONST              15 (327)
+    41         360 LOAD_CONST              15 (327)
                362 LOAD_NAME               25 (_CHAT)
                364 STORE_ATTR              22 (_serialized_start)
    
-    29         374 LOAD_CONST              16 (364)
+    42         374 LOAD_CONST              16 (395)
                376 LOAD_NAME               25 (_CHAT)
                378 STORE_ATTR              23 (_serialized_end)
    
-    30         388 LOAD_CONST              17 (366)
+    43         388 LOAD_CONST              17 (398)
                390 LOAD_NAME               26 (_LANGUAGEMODEL)
                392 STORE_ATTR              22 (_serialized_start)
    
-    31         402 LOAD_CONST              18 (458)
+    44         402 LOAD_CONST              18 (571)
                404 LOAD_NAME               26 (_LANGUAGEMODEL)
                406 STORE_ATTR              23 (_serialized_end)
                416 LOAD_CONST               9 (None)
                418 RETURN_VALUE
    
-    20     >>  420 LOAD_CONST               9 (None)
+    32     >>  420 LOAD_CONST               9 (None)
                422 RETURN_VALUE
    consts
       'Generated protocol buffer code.'
       0
       ('builder',)
       ('descriptor',)
       ('descriptor_pool',)
       ('symbol_database',)
-      b'\n\x0ellm_chat.proto\x12\x11languagemodelchat"\xe3\x01\n\x0cChatLogInput\x12)\n\x08messages\x18\x01 \x03(\x0b2\x17.languagemodelchat.Chat\x12\x12\n\nmax_tokens\x18\x02 \x01(\x05\x12\x13\n\x0btemperature\x18\x03 \x01(\x02\x12\r\n\x05top_p\x18\x04 \x01(\x02\x12\t\n\x01n\x18\x05 \x01(\x05\x12\x0e\n\x06stream\x18\x06 \x01(\x08\x12\x0c\n\x04stop\x18\x07 \x01(\t\x12\x18\n\x10presence_penalty\x18\x08 \x01(\x02\x12\x19\n\x11frequence_penalty\x18\t \x01(\x02\x12\x12\n\nlogit_bias\x18\n \x01(\t":\n\rChatLogOutput\x12)\n\x08messages\x18\x01 \x03(\x0b2\x17.languagemodelchat.Chat"%\n\x04Chat\x12\x0c\n\x04role\x18\x01 \x01(\t\x12\x0f\n\x07content\x18\x02 \x01(\t2\\\n\rLanguageModel\x12K\n\x04Chat\x12\x1f.languagemodelchat.ChatLogInput\x1a .languagemodelchat.ChatLogOutput"\x00B3\n\x15io.grpc.examples.chatB\x11LanguageModelChatP\x01\xa2\x02\x04chatb\x06proto3'
+      b'\n\x0ellm_chat.proto\x12\x11languagemodelchat"\xe3\x01\n\x0cChatLogInput\x12)\n\x08messages\x18\x01 \x03(\x0b2\x17.languagemodelchat.Chat\x12\x12\n\nmax_tokens\x18\x02 \x01(\x05\x12\x13\n\x0btemperature\x18\x03 \x01(\x02\x12\r\n\x05top_p\x18\x04 \x01(\x02\x12\t\n\x01n\x18\x05 \x01(\x05\x12\x0e\n\x06stream\x18\x06 \x01(\x08\x12\x0c\n\x04stop\x18\x07 \x01(\t\x12\x18\n\x10presence_penalty\x18\x08 \x01(\x02\x12\x19\n\x11frequence_penalty\x18\t \x01(\x02\x12\x12\n\nlogit_bias\x18\n \x01(\t":\n\rChatLogOutput\x12)\n\x08messages\x18\x01 \x03(\x0b2\x17.languagemodelchat.Chat"D\n\x04Chat\x12\x11\n\x04role\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x14\n\x07content\x18\x02 \x01(\tH\x01\x88\x01\x01B\x07\n\x05_roleB\n\n\x08_content2\xad\x01\n\rLanguageModel\x12K\n\x04Chat\x12\x1f.languagemodelchat.ChatLogInput\x1a .languagemodelchat.ChatLogOutput"\x00\x12O\n\x06Stream\x12\x1f.languagemodelchat.ChatLogInput\x1a .languagemodelchat.ChatLogOutput"\x000\x01B3\n\x15io.grpc.examples.chatB\x11LanguageModelChatP\x01\xa2\x02\x04chatb\x06proto3'
       'llm_chat_pb2'
       False
       None
       b'\n\x15io.grpc.examples.chatB\x11LanguageModelChatP\x01\xa2\x02\x04chat'
       38
       265
       267
       325
       327
-      364
-      366
-      458
+      395
+      398
+      571
    names      ('__doc__', 'google.protobuf.internal', 'builder', '_builder', 'google.protobuf', 'descriptor', '_descriptor', 'descriptor_pool', '_descriptor_pool', 'symbol_database', '_symbol_database', 'Default', '_sym_db', 'AddSerializedFile', 'DESCRIPTOR', 'BuildMessageAndEnumDescriptors', 'globals', 'BuildTopDescriptorsAndMessages', '_USE_C_DESCRIPTORS', '_options', '_serialized_options', '_CHATLOGINPUT', '_serialized_start', '_serialized_end', '_CHATLOGOUTPUT', '_CHAT', '_LANGUAGEMODEL')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\chat\\llm_chat_pb2.py'
+   filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\chat\\llm_chat_pb2.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020404010c010c010c010c031e0544023201340116020e010e010e
-      010e010e010e010e010e010e0112f5
+      0x00ff020404010c010c010c010c041e03320102ff100f3201340116010e
+      0202ff0c030e010e010e010e010e010e010e0112f4
```

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/__pycache__/llm_chat_pb2_grpc.cpython-311.pyc` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/embedding/__pycache__/llm_embed_pb2_grpc.cpython-311.pyc`

 * *Files 19% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xe1002764 (Fri Mar 31 15:48:49 2023 UTC)
-files sz: 2348
+moddate:  0xb57d2d64 (Wed Apr  5 13:55:01 2023 UTC)
+files sz: 2483
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x970064005a00640164026c015a01640364046c026d035a040100020047
@@ -19,84 +19,84 @@
    
      3           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (None)
                 10 IMPORT_NAME              1 (grpc)
                 12 STORE_NAME               1 (grpc)
    
      5          14 LOAD_CONST               3 (1)
-                16 LOAD_CONST               4 (('llm_chat_pb2',))
+                16 LOAD_CONST               4 (('llm_embed_pb2',))
                 18 IMPORT_NAME              2
-                20 IMPORT_FROM              3 (llm_chat_pb2)
-                22 STORE_NAME               4 (llm__chat__pb2)
+                20 IMPORT_FROM              3 (llm_embed_pb2)
+                22 STORE_NAME               4 (llm__embed__pb2)
                 24 POP_TOP
    
-     7          26 PUSH_NULL
+     8          26 PUSH_NULL
                 28 LOAD_BUILD_CLASS
-                30 LOAD_CONST               5 (<code object LanguageModelStub, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\python\chat\llm_chat_pb2_grpc.py", line 7>)
+                30 LOAD_CONST               5 (<code object LanguageModelStub, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\embedding\llm_embed_pb2_grpc.py", line 8>)
                 32 MAKE_FUNCTION            0
                 34 LOAD_CONST               6 ('LanguageModelStub')
                 36 LOAD_NAME                5 (object)
                 38 PRECALL                  3
                 42 CALL                     3
                 52 STORE_NAME               6 (LanguageModelStub)
    
     24          54 PUSH_NULL
                 56 LOAD_BUILD_CLASS
-                58 LOAD_CONST               7 (<code object LanguageModelServicer, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\python\chat\llm_chat_pb2_grpc.py", line 24>)
+                58 LOAD_CONST               7 (<code object LanguageModelServicer, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\embedding\llm_embed_pb2_grpc.py", line 24>)
                 60 MAKE_FUNCTION            0
                 62 LOAD_CONST               8 ('LanguageModelServicer')
                 64 LOAD_NAME                5 (object)
                 66 PRECALL                  3
                 70 CALL                     3
                 80 STORE_NAME               7 (LanguageModelServicer)
    
-    36          82 LOAD_CONST               9 (<code object add_LanguageModelServicer_to_server, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\python\chat\llm_chat_pb2_grpc.py", line 36>)
+    34          82 LOAD_CONST               9 (<code object add_LanguageModelServicer_to_server, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\embedding\llm_embed_pb2_grpc.py", line 34>)
                 84 MAKE_FUNCTION            0
                 86 STORE_NAME               8 (add_LanguageModelServicer_to_server)
    
-    50          88 PUSH_NULL
+    49          88 PUSH_NULL
                 90 LOAD_BUILD_CLASS
-                92 LOAD_CONST              10 (<code object LanguageModel, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\python\chat\llm_chat_pb2_grpc.py", line 50>)
+                92 LOAD_CONST              10 (<code object LanguageModel, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\embedding\llm_embed_pb2_grpc.py", line 49>)
                 94 MAKE_FUNCTION            0
                 96 LOAD_CONST              11 ('LanguageModel')
                 98 LOAD_NAME                5 (object)
                100 PRECALL                  3
                104 CALL                     3
                114 STORE_NAME               9 (LanguageModel)
                116 LOAD_CONST               2 (None)
                118 RETURN_VALUE
    consts
       'Client and server classes corresponding to protobuf-defined services.'
       0
       None
       1
-      ('llm_chat_pb2',)
+      ('llm_embed_pb2',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a03640284005a0464035300
-           7           0 RESUME                   0
+           8           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('LanguageModelStub')
                        8 STORE_NAME               2 (__qualname__)
          
-           8          10 LOAD_CONST               1 ('Interface exported by the server.\n    ')
+           9          10 LOAD_CONST               1 ('Interface exported by the server.')
                       12 STORE_NAME               3 (__doc__)
          
-          11          14 LOAD_CONST               2 (<code object __init__, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\python\chat\llm_chat_pb2_grpc.py", line 11>)
+          11          14 LOAD_CONST               2 (<code object __init__, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\embedding\llm_embed_pb2_grpc.py", line 11>)
                       16 MAKE_FUNCTION            0
                       18 STORE_NAME               4 (__init__)
                       20 LOAD_CONST               3 (None)
                       22 RETURN_VALUE
          consts
             'LanguageModelStub'
-            'Interface exported by the server.\n    '
+            'Interface exported by the server.'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x97007c01a0000000000000000000000000000000000000000000640174
@@ -105,131 +105,131 @@
                   000000ac02a6030000ab0300000000000000007c005f0600000000000000
                   0064035300
                 11           0 RESUME                   0
                
                 17           2 LOAD_FAST                1 (channel)
                              4 LOAD_METHOD              0 (unary_unary)
                
-                18          26 LOAD_CONST               1 ('/languagemodelchat.LanguageModel/Chat')
+                18          26 LOAD_CONST               1 ('/languagemodelembeddings.LanguageModel/Embed')
                
-                19          28 LOAD_GLOBAL              2 (llm__chat__pb2)
-                            40 LOAD_ATTR                2 (ChatLogInput)
+                19          28 LOAD_GLOBAL              2 (llm__embed__pb2)
+                            40 LOAD_ATTR                2 (Sentences)
                             50 LOAD_ATTR                3 (SerializeToString)
                
-                20          60 LOAD_GLOBAL              2 (llm__chat__pb2)
-                            72 LOAD_ATTR                4 (ChatLogOutput)
+                20          60 LOAD_GLOBAL              2 (llm__embed__pb2)
+                            72 LOAD_ATTR                4 (ListOfEmbeddings)
                             82 LOAD_ATTR                5 (FromString)
                
                 17          92 KW_NAMES                 2
                             94 PRECALL                  3
                             98 CALL                     3
                            108 LOAD_FAST                0 (self)
-                           110 STORE_ATTR               6 (Chat)
+                           110 STORE_ATTR               6 (Embed)
                            120 LOAD_CONST               3 (None)
                            122 RETURN_VALUE
                consts
                   'Constructor.\n\n        Args:\n            channel: A grpc.Channel.\n        '
-                  '/languagemodelchat.LanguageModel/Chat'
+                  '/languagemodelembeddings.LanguageModel/Embed'
                   ('request_serializer', 'response_deserializer')
                   None
-               names      ('unary_unary', 'llm__chat__pb2', 'ChatLogInput', 'SerializeToString', 'ChatLogOutput', 'FromString', 'Chat')
+               names      ('unary_unary', 'llm__embed__pb2', 'Sentences', 'SerializeToString', 'ListOfEmbeddings', 'FromString', 'Embed')
                varnames   ('self', 'channel')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\chat\\llm_chat_pb2_grpc.py'
+               filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\embedding\\llm_embed_pb2_grpc.py'
                name       '__init__'
                firstlineno 11
                lnotab 0x020618010201200120fd
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\chat\\llm_chat_pb2_grpc.py'
+         filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\embedding\\llm_embed_pb2_grpc.py'
          name       'LanguageModelStub'
-         firstlineno 7
-         lnotab 0x0a010403
+         firstlineno 8
+         lnotab 0x0a010402
       'LanguageModelStub'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a03640284005a0464035300
           24           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('LanguageModelServicer')
                        8 STORE_NAME               2 (__qualname__)
          
-          25          10 LOAD_CONST               1 ('Interface exported by the server.\n    ')
+          25          10 LOAD_CONST               1 ('Interface exported by the server.')
                       12 STORE_NAME               3 (__doc__)
          
-          28          14 LOAD_CONST               2 (<code object Chat, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\python\chat\llm_chat_pb2_grpc.py", line 28>)
+          27          14 LOAD_CONST               2 (<code object Embed, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\embedding\llm_embed_pb2_grpc.py", line 27>)
                       16 MAKE_FUNCTION            0
-                      18 STORE_NAME               4 (Chat)
+                      18 STORE_NAME               4 (Embed)
                       20 LOAD_CONST               3 (None)
                       22 RETURN_VALUE
          consts
             'LanguageModelServicer'
-            'Interface exported by the server.\n    '
+            'Interface exported by the server.'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c02a0000000000000000000000000000000000000000000740200
                   0000000000000000006a0200000000000000006a030000000000000000a6
                   010000ab01000000000000000001007c02a0040000000000000000000000
                   0000000000000000006401a6010000ab0100000000000000000100740b00
                   0000000000000000006401a6010000ab0100000000000000008201
-                28           0 RESUME                   0
+                27           0 RESUME                   0
                
-                31           2 LOAD_FAST                2 (context)
+                29           2 LOAD_FAST                2 (context)
                              4 LOAD_METHOD              0 (set_code)
                             26 LOAD_GLOBAL              2 (grpc)
                             38 LOAD_ATTR                2 (StatusCode)
                             48 LOAD_ATTR                3 (UNIMPLEMENTED)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 POP_TOP
                
-                32          74 LOAD_FAST                2 (context)
+                30          74 LOAD_FAST                2 (context)
                             76 LOAD_METHOD              4 (set_details)
                             98 LOAD_CONST               1 ('Method not implemented!')
                            100 PRECALL                  1
                            104 CALL                     1
                            114 POP_TOP
                
-                33         116 LOAD_GLOBAL             11 (NULL + NotImplementedError)
+                31         116 LOAD_GLOBAL             11 (NULL + NotImplementedError)
                            128 LOAD_CONST               1 ('Method not implemented!')
                            130 PRECALL                  1
                            134 CALL                     1
                            144 RAISE_VARARGS            1
                consts
-                  'Simple RPC\n        '
+                  'Simple RPC'
                   'Method not implemented!'
                names      ('set_code', 'grpc', 'StatusCode', 'UNIMPLEMENTED', 'set_details', 'NotImplementedError')
                varnames   ('self', 'request', 'context')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\chat\\llm_chat_pb2_grpc.py'
-               name       'Chat'
-               firstlineno 28
-               lnotab 0x020348012a01
+               filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\embedding\\llm_embed_pb2_grpc.py'
+               name       'Embed'
+               firstlineno 27
+               lnotab 0x020248012a01
             None
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'Chat')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'Embed')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\chat\\llm_chat_pb2_grpc.py'
+         filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\embedding\\llm_embed_pb2_grpc.py'
          name       'LanguageModelServicer'
          firstlineno 24
-         lnotab 0x0a010403
+         lnotab 0x0a010402
       'LanguageModelServicer'
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
@@ -237,184 +237,195 @@
             0200000000000000007406000000000000000000006a0400000000000000
             006a0500000000000000007406000000000000000000006a060000000000
             0000006a070000000000000000ac02a6030000ab03000000000000000069
             017d027401000000000000000000006a08000000000000000064037c02a6
             020000ab0200000000000000007d037c01a0090000000000000000000000
             0000000000000000007c036601a6010000ab010000000000000000010064
             005300
-          36           0 RESUME                   0
+          34           0 RESUME                   0
          
-          38           2 LOAD_CONST               1 ('Chat')
+          36           2 LOAD_CONST               1 ('Embed')
                        4 LOAD_GLOBAL              1 (NULL + grpc)
                       16 LOAD_ATTR                1 (unary_unary_rpc_method_handler)
          
-          39          26 LOAD_FAST                0 (servicer)
-                      28 LOAD_ATTR                2 (Chat)
+          37          26 LOAD_FAST                0 (servicer)
+                      28 LOAD_ATTR                2 (Embed)
          
-          40          38 LOAD_GLOBAL              6 (llm__chat__pb2)
-                      50 LOAD_ATTR                4 (ChatLogInput)
+          38          38 LOAD_GLOBAL              6 (llm__embed__pb2)
+                      50 LOAD_ATTR                4 (Sentences)
                       60 LOAD_ATTR                5 (FromString)
          
-          41          70 LOAD_GLOBAL              6 (llm__chat__pb2)
-                      82 LOAD_ATTR                6 (ChatLogOutput)
+          39          70 LOAD_GLOBAL              6 (llm__embed__pb2)
+                      82 LOAD_ATTR                6 (ListOfEmbeddings)
                       92 LOAD_ATTR                7 (SerializeToString)
          
-          38         102 KW_NAMES                 2
+          36         102 KW_NAMES                 2
                      104 PRECALL                  3
                      108 CALL                     3
          
-          37         118 BUILD_MAP                1
+          35         118 BUILD_MAP                1
                      120 STORE_FAST               2 (rpc_method_handlers)
          
-          44         122 LOAD_GLOBAL              1 (NULL + grpc)
+          42         122 LOAD_GLOBAL              1 (NULL + grpc)
                      134 LOAD_ATTR                8 (method_handlers_generic_handler)
          
-          45         144 LOAD_CONST               3 ('languagemodelchat.LanguageModel')
+          43         144 LOAD_CONST               3 ('languagemodelembeddings.LanguageModel')
                      146 LOAD_FAST                2 (rpc_method_handlers)
          
-          44         148 PRECALL                  2
+          42         148 PRECALL                  2
                      152 CALL                     2
                      162 STORE_FAST               3 (generic_handler)
          
-          46         164 LOAD_FAST                1 (server)
+          45         164 LOAD_FAST                1 (server)
                      166 LOAD_METHOD              9 (add_generic_rpc_handlers)
                      188 LOAD_FAST                3 (generic_handler)
                      190 BUILD_TUPLE              1
                      192 PRECALL                  1
                      196 CALL                     1
                      206 POP_TOP
                      208 LOAD_CONST               0 (None)
                      210 RETURN_VALUE
          consts
             None
-            'Chat'
+            'Embed'
             ('request_deserializer', 'response_serializer')
-            'languagemodelchat.LanguageModel'
-         names      ('grpc', 'unary_unary_rpc_method_handler', 'Chat', 'llm__chat__pb2', 'ChatLogInput', 'FromString', 'ChatLogOutput', 'SerializeToString', 'method_handlers_generic_handler', 'add_generic_rpc_handlers')
+            'languagemodelembeddings.LanguageModel'
+         names      ('grpc', 'unary_unary_rpc_method_handler', 'Embed', 'llm__embed__pb2', 'Sentences', 'FromString', 'ListOfEmbeddings', 'SerializeToString', 'method_handlers_generic_handler', 'add_generic_rpc_handlers')
          varnames   ('servicer', 'server', 'rpc_method_handlers', 'generic_handler')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\chat\\llm_chat_pb2_grpc.py'
+         filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\embedding\\llm_embed_pb2_grpc.py'
          name       'add_LanguageModelServicer_to_server'
-         firstlineno 36
-         lnotab 0x020218010c01200120fd10ff0407160104ff1002
+         firstlineno 34
+         lnotab 0x020218010c01200120fd10ff0407160104ff1003
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0264015a03650409000900090009000900090009
             000900640664058401a6000000ab0000000000000000005a0564035300
-          50           0 RESUME                   0
+          49           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('LanguageModel')
                        8 STORE_NAME               2 (__qualname__)
          
-          51          10 LOAD_CONST               1 ('Interface exported by the server.\n    ')
+          50          10 LOAD_CONST               1 ('Interface exported by the server.')
                       12 STORE_NAME               3 (__doc__)
          
-          54          14 LOAD_NAME                4 (staticmethod)
+          52          14 LOAD_NAME                4 (staticmethod)
          
-          57          16 NOP
+          56          16 NOP
          
-          58          18 NOP
+          57          18 NOP
          
-          59          20 NOP
+          58          20 NOP
          
-          60          22 NOP
+          59          22 NOP
          
-          61          24 NOP
+          60          24 NOP
          
-          62          26 NOP
+          61          26 NOP
          
-          63          28 NOP
+          62          28 NOP
          
-          64          30 NOP
+          63          30 NOP
          
-          55          32 LOAD_CONST               6 (((), None, None, False, None, None, None, None))
-                      34 LOAD_CONST               5 (<code object Chat, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\python\chat\llm_chat_pb2_grpc.py", line 54>)
+          53          32 LOAD_CONST               6 (((), None, None, False, None, None, None, None))
+                      34 LOAD_CONST               5 (<code object Embed, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\embedding\llm_embed_pb2_grpc.py", line 52>)
                       36 MAKE_FUNCTION            1 (defaults)
          
-          54          38 PRECALL                  0
+          52          38 PRECALL                  0
                       42 CALL                     0
          
-          55          52 STORE_NAME               5 (Chat)
+          53          52 STORE_NAME               5 (Embed)
                       54 LOAD_CONST               3 (None)
                       56 RETURN_VALUE
          consts
             'LanguageModel'
-            'Interface exported by the server.\n    '
+            'Interface exported by the server.'
             ()
             None
             False
             code
                argcount  : 10
                nlocals   : 10
                stacksize : 15
                flags     : 3
                code
                   0x97007400000000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000007c007c01640174060000000000
                   00000000006a0400000000000000006a0500000000000000007406000000
                   000000000000006a0600000000000000006a0700000000000000007c027c
                   037c057c047c067c077c087c09a60d0000ab0d00000000000000005300
-                54           0 RESUME                   0
+                52           0 RESUME                   0
                
                 65           2 LOAD_GLOBAL              0 (grpc)
                             14 LOAD_ATTR                1 (experimental)
                             24 LOAD_METHOD              2 (unary_unary)
-                            46 LOAD_FAST                0 (request)
-                            48 LOAD_FAST                1 (target)
-                            50 LOAD_CONST               1 ('/languagemodelchat.LanguageModel/Chat')
                
-                66          52 LOAD_GLOBAL              6 (llm__chat__pb2)
-                            64 LOAD_ATTR                4 (ChatLogInput)
+                66          46 LOAD_FAST                0 (request)
+               
+                67          48 LOAD_FAST                1 (target)
+               
+                68          50 LOAD_CONST               1 ('/languagemodelembeddings.LanguageModel/Embed')
+               
+                69          52 LOAD_GLOBAL              6 (llm__embed__pb2)
+                            64 LOAD_ATTR                4 (Sentences)
                             74 LOAD_ATTR                5 (SerializeToString)
                
-                67          84 LOAD_GLOBAL              6 (llm__chat__pb2)
-                            96 LOAD_ATTR                6 (ChatLogOutput)
+                70          84 LOAD_GLOBAL              6 (llm__embed__pb2)
+                            96 LOAD_ATTR                6 (ListOfEmbeddings)
                            106 LOAD_ATTR                7 (FromString)
                
-                68         116 LOAD_FAST                2 (options)
-                           118 LOAD_FAST                3 (channel_credentials)
+                71         116 LOAD_FAST                2 (options)
+               
+                72         118 LOAD_FAST                3 (channel_credentials)
+               
+                73         120 LOAD_FAST                5 (insecure)
+               
+                74         122 LOAD_FAST                4 (call_credentials)
+               
+                75         124 LOAD_FAST                6 (compression)
+               
+                76         126 LOAD_FAST                7 (wait_for_ready)
+               
+                77         128 LOAD_FAST                8 (timeout)
                
-                69         120 LOAD_FAST                5 (insecure)
-                           122 LOAD_FAST                4 (call_credentials)
-                           124 LOAD_FAST                6 (compression)
-                           126 LOAD_FAST                7 (wait_for_ready)
-                           128 LOAD_FAST                8 (timeout)
-                           130 LOAD_FAST                9 (metadata)
+                78         130 LOAD_FAST                9 (metadata)
                
                 65         132 PRECALL                 13
                            136 CALL                    13
                            146 RETURN_VALUE
                consts
                   None
-                  '/languagemodelchat.LanguageModel/Chat'
-               names      ('grpc', 'experimental', 'unary_unary', 'llm__chat__pb2', 'ChatLogInput', 'SerializeToString', 'ChatLogOutput', 'FromString')
+                  '/languagemodelembeddings.LanguageModel/Embed'
+               names      ('grpc', 'experimental', 'unary_unary', 'llm__embed__pb2', 'Sentences', 'SerializeToString', 'ListOfEmbeddings', 'FromString')
                varnames   ('request', 'target', 'options', 'channel_credentials', 'call_credentials', 'insecure', 'compression', 'wait_for_ready', 'timeout', 'metadata')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\chat\\llm_chat_pb2_grpc.py'
-               name       'Chat'
-               firstlineno 54
-               lnotab 0x020b32012001200104010cfc
+               filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\embedding\\llm_embed_pb2_grpc.py'
+               name       'Embed'
+               firstlineno 52
+               lnotab
+                  0x020d2c0102010201020120012001020102010201020102010201020102
+                  f3
             ((), None, None, False, None, None, None, None)
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'staticmethod', 'Chat')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'staticmethod', 'Embed')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\chat\\llm_chat_pb2_grpc.py'
+         filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\embedding\\llm_embed_pb2_grpc.py'
          name       'LanguageModel'
-         firstlineno 50
-         lnotab 0x0a0104030203020102010201020102010201020102f706ff0e01
+         firstlineno 49
+         lnotab 0x0a0104020204020102010201020102010201020102f606ff0e01
       'LanguageModel'
-   names      ('__doc__', 'grpc', '', 'llm_chat_pb2', 'llm__chat__pb2', 'object', 'LanguageModelStub', 'LanguageModelServicer', 'add_LanguageModelServicer_to_server', 'LanguageModel')
+   names      ('__doc__', 'grpc', '', 'llm_embed_pb2', 'llm__embed__pb2', 'object', 'LanguageModelStub', 'LanguageModelServicer', 'add_LanguageModelServicer_to_server', 'LanguageModel')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\chat\\llm_chat_pb2_grpc.py'
+   filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\embedding\\llm_embed_pb2_grpc.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0202040108020c021c111c0c060e
+   lnotab 0x00ff0202040108020c031c101c0a060f
```

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/client.py` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/chat/client.py`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/llm_chat_pb2.py` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/chat/llm_chat_pb2.py`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/llm_chat_pb2.pyi` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/chat/llm_chat_pb2.pyi`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/llm_chat_pb2_grpc.py` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/chat/llm_chat_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/server.py` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/chat/server.py`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/__pycache__/llm_pb2.cpython-311.pyc` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/completion/__pycache__/llm_pb2.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xa7021264 (Wed Mar 15 17:38:47 2023 UTC)
-files sz: 2047
+moddate:  0xb57d2d64 (Wed Apr  5 13:55:01 2023 UTC)
+files sz: 2186
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x970064005a00640164026c016d025a030100640164036c046d055a0601
@@ -50,98 +50,100 @@
      8          42 LOAD_CONST               1 (0)
                 44 LOAD_CONST               5 (('symbol_database',))
                 46 IMPORT_NAME              4 (google.protobuf)
                 48 IMPORT_FROM              9 (symbol_database)
                 50 STORE_NAME              10 (_symbol_database)
                 52 POP_TOP
    
-    11          54 PUSH_NULL
+    12          54 PUSH_NULL
                 56 LOAD_NAME               10 (_symbol_database)
                 58 LOAD_ATTR               11 (Default)
                 68 PRECALL                  0
                 72 CALL                     0
                 82 STORE_NAME              12 (_sym_db)
    
-    16          84 PUSH_NULL
+    15          84 PUSH_NULL
                 86 LOAD_NAME                8 (_descriptor_pool)
                 88 LOAD_ATTR               11 (Default)
                 98 PRECALL                  0
                102 CALL                     0
                112 LOAD_METHOD             13 (AddSerializedFile)
-               134 LOAD_CONST               6 (b'\n\tllm.proto\x12\rlanguagemodel"\x84\x02\n\x07Message\x12\x0e\n\x06prompt\x18\x01 \x01(\t\x12\x0e\n\x06suffix\x18\x02 \x01(\t\x12\x12\n\nmax_tokens\x18\x03 \x01(\x05\x12\x13\n\x0btemperature\x18\x04 \x01(\x02\x12\r\n\x05top_p\x18\x05 \x01(\x02\x12\t\n\x01n\x18\x06 \x01(\x05\x12\x0e\n\x06stream\x18\x07 \x01(\x08\x12\x10\n\x08logprobs\x18\x08 \x01(\x05\x12\x0c\n\x04echo\x18\t \x01(\x08\x12\x0c\n\x04stop\x18\n \x01(\t\x12\x18\n\x10presence_penalty\x18\x0b \x01(\x02\x12\x19\n\x11frequence_penalty\x18\x0c \x01(\x02\x12\x0f\n\x07best_of\x18\r \x01(\x05\x12\x12\n\nlogit_bias\x18\x0e \x01(\t"\x1c\n\x0bCompletions\x12\r\n\x05reply\x18\x01 \x01(\t2\x9b\x01\n\rLanguageModel\x12@\n\x08Complete\x12\x16.languagemodel.Message\x1a\x1a.languagemodel.Completions"\x00\x12H\n\x0eStreamComplete\x12\x16.languagemodel.Message\x1a\x1a.languagemodel.Completions"\x000\x01B+\n\x13io.grpc.examples.lmB\rLanguageModelP\x01\xa2\x02\x02LMb\x06proto3')
-               136 PRECALL                  1
+   
+    16         134 LOAD_CONST               6 (b'\n\tllm.proto\x12\rlanguagemodel"\x84\x02\n\x07Message\x12\x0e\n\x06prompt\x18\x01 \x01(\t\x12\x0e\n\x06suffix\x18\x02 \x01(\t\x12\x12\n\nmax_tokens\x18\x03 \x01(\x05\x12\x13\n\x0btemperature\x18\x04 \x01(\x02\x12\r\n\x05top_p\x18\x05 \x01(\x02\x12\t\n\x01n\x18\x06 \x01(\x05\x12\x0e\n\x06stream\x18\x07 \x01(\x08\x12\x10\n\x08logprobs\x18\x08 \x01(\x05\x12\x0c\n\x04echo\x18\t \x01(\x08\x12\x0c\n\x04stop\x18\n \x01(\t\x12\x18\n\x10presence_penalty\x18\x0b \x01(\x02\x12\x19\n\x11frequence_penalty\x18\x0c \x01(\x02\x12\x0f\n\x07best_of\x18\r \x01(\x05\x12\x12\n\nlogit_bias\x18\x0e \x01(\t"\x1c\n\x0bCompletions\x12\r\n\x05reply\x18\x01 \x01(\t2\x9b\x01\n\rLanguageModel\x12@\n\x08Complete\x12\x16.languagemodel.Message\x1a\x1a.languagemodel.Completions"\x00\x12H\n\x0eStreamComplete\x12\x16.languagemodel.Message\x1a\x1a.languagemodel.Completions"\x000\x01B+\n\x13io.grpc.examples.lmB\rLanguageModelP\x01\xa2\x02\x02LMb\x06proto3')
+   
+    15         136 PRECALL                  1
                140 CALL                     1
                150 STORE_NAME              14 (DESCRIPTOR)
    
-    18         152 PUSH_NULL
+    28         152 PUSH_NULL
                154 LOAD_NAME                3 (_builder)
                156 LOAD_ATTR               15 (BuildMessageAndEnumDescriptors)
                166 LOAD_NAME               14 (DESCRIPTOR)
                168 PUSH_NULL
                170 LOAD_NAME               16 (globals)
                172 PRECALL                  0
                176 CALL                     0
                186 PRECALL                  2
                190 CALL                     2
                200 POP_TOP
    
-    19         202 PUSH_NULL
+    29         202 PUSH_NULL
                204 LOAD_NAME                3 (_builder)
                206 LOAD_ATTR               17 (BuildTopDescriptorsAndMessages)
                216 LOAD_NAME               14 (DESCRIPTOR)
                218 LOAD_CONST               7 ('llm_pb2')
                220 PUSH_NULL
                222 LOAD_NAME               16 (globals)
                224 PRECALL                  0
                228 CALL                     0
                238 PRECALL                  3
                242 CALL                     3
                252 POP_TOP
    
-    20         254 LOAD_NAME                6 (_descriptor)
+    30         254 LOAD_NAME                6 (_descriptor)
                256 LOAD_ATTR               18 (_USE_C_DESCRIPTORS)
                266 LOAD_CONST               8 (False)
                268 COMPARE_OP               2 (==)
                274 POP_JUMP_FORWARD_IF_FALSE    58 (to 392)
    
-    22         276 LOAD_CONST               9 (None)
+    31         276 LOAD_CONST               9 (None)
                278 LOAD_NAME               14 (DESCRIPTOR)
                280 STORE_ATTR              19 (_options)
    
-    23         290 LOAD_CONST              10 (b'\n\x13io.grpc.examples.lmB\rLanguageModelP\x01\xa2\x02\x02LM')
+    32         290 LOAD_CONST              10 (b'\n\x13io.grpc.examples.lmB\rLanguageModelP\x01\xa2\x02\x02LM')
                292 LOAD_NAME               14 (DESCRIPTOR)
                294 STORE_ATTR              20 (_serialized_options)
    
-    24         304 LOAD_CONST              11 (29)
+    33         304 LOAD_CONST              11 (29)
                306 LOAD_NAME               21 (_MESSAGE)
                308 STORE_ATTR              22 (_serialized_start)
    
-    25         318 LOAD_CONST              12 (289)
+    34         318 LOAD_CONST              12 (289)
                320 LOAD_NAME               21 (_MESSAGE)
                322 STORE_ATTR              23 (_serialized_end)
    
-    26         332 LOAD_CONST              13 (291)
+    35         332 LOAD_CONST              13 (291)
                334 LOAD_NAME               24 (_COMPLETIONS)
                336 STORE_ATTR              22 (_serialized_start)
    
-    27         346 LOAD_CONST              14 (319)
+    36         346 LOAD_CONST              14 (319)
                348 LOAD_NAME               24 (_COMPLETIONS)
                350 STORE_ATTR              23 (_serialized_end)
    
-    28         360 LOAD_CONST              15 (322)
+    37         360 LOAD_CONST              15 (322)
                362 LOAD_NAME               25 (_LANGUAGEMODEL)
                364 STORE_ATTR              22 (_serialized_start)
    
-    29         374 LOAD_CONST              16 (477)
+    38         374 LOAD_CONST              16 (477)
                376 LOAD_NAME               25 (_LANGUAGEMODEL)
                378 STORE_ATTR              23 (_serialized_end)
                388 LOAD_CONST               9 (None)
                390 RETURN_VALUE
    
-    20     >>  392 LOAD_CONST               9 (None)
+    30     >>  392 LOAD_CONST               9 (None)
                394 RETURN_VALUE
    consts
       'Generated protocol buffer code.'
       0
       ('builder',)
       ('descriptor',)
       ('descriptor_pool',)
@@ -157,13 +159,13 @@
       319
       322
       477
    names      ('__doc__', 'google.protobuf.internal', 'builder', '_builder', 'google.protobuf', 'descriptor', '_descriptor', 'descriptor_pool', '_descriptor_pool', 'symbol_database', '_symbol_database', 'Default', '_sym_db', 'AddSerializedFile', 'DESCRIPTOR', 'BuildMessageAndEnumDescriptors', 'globals', 'BuildTopDescriptorsAndMessages', '_USE_C_DESCRIPTORS', '_options', '_serialized_options', '_MESSAGE', '_serialized_start', '_serialized_end', '_COMPLETIONS', '_LANGUAGEMODEL')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\completion\\llm_pb2.py'
+   filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\completion\\llm_pb2.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020404010c010c010c010c031e0544023201340116020e010e010e
-      010e010e010e010e0112f7
+      0x00ff020404010c010c010c010c041e03320102ff100d3201340116010e
+      010e010e010e010e010e010e0112f8
```

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/__pycache__/llm_pb2_grpc.cpython-311.pyc` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/completion/__pycache__/llm_pb2_grpc.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x94ec1564 (Sat Mar 18 16:53:40 2023 UTC)
-files sz: 3773
+moddate:  0xb57d2d64 (Wed Apr  5 13:55:01 2023 UTC)
+files sz: 3956
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x970064005a00640164026c015a01640364046c026d035a040100020047
@@ -27,39 +27,39 @@
                 18 IMPORT_NAME              2
                 20 IMPORT_FROM              3 (llm_pb2)
                 22 STORE_NAME               4 (llm__pb2)
                 24 POP_TOP
    
      8          26 PUSH_NULL
                 28 LOAD_BUILD_CLASS
-                30 LOAD_CONST               5 (<code object LanguageModelStub, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\python\completion\llm_pb2_grpc.py", line 8>)
+                30 LOAD_CONST               5 (<code object LanguageModelStub, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\completion\llm_pb2_grpc.py", line 8>)
                 32 MAKE_FUNCTION            0
                 34 LOAD_CONST               6 ('LanguageModelStub')
                 36 LOAD_NAME                5 (object)
                 38 PRECALL                  3
                 42 CALL                     3
                 52 STORE_NAME               6 (LanguageModelStub)
    
-    30          54 PUSH_NULL
+    29          54 PUSH_NULL
                 56 LOAD_BUILD_CLASS
-                58 LOAD_CONST               7 (<code object LanguageModelServicer, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\python\completion\llm_pb2_grpc.py", line 30>)
+                58 LOAD_CONST               7 (<code object LanguageModelServicer, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\completion\llm_pb2_grpc.py", line 29>)
                 60 MAKE_FUNCTION            0
                 62 LOAD_CONST               8 ('LanguageModelServicer')
                 64 LOAD_NAME                5 (object)
                 66 PRECALL                  3
                 70 CALL                     3
                 80 STORE_NAME               7 (LanguageModelServicer)
    
-    49          82 LOAD_CONST               9 (<code object add_LanguageModelServicer_to_server, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\python\completion\llm_pb2_grpc.py", line 49>)
+    45          82 LOAD_CONST               9 (<code object add_LanguageModelServicer_to_server, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\completion\llm_pb2_grpc.py", line 45>)
                 84 MAKE_FUNCTION            0
                 86 STORE_NAME               8 (add_LanguageModelServicer_to_server)
    
-    68          88 PUSH_NULL
+    65          88 PUSH_NULL
                 90 LOAD_BUILD_CLASS
-                92 LOAD_CONST              10 (<code object LanguageModel, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\python\completion\llm_pb2_grpc.py", line 68>)
+                92 LOAD_CONST              10 (<code object LanguageModel, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\completion\llm_pb2_grpc.py", line 65>)
                 94 MAKE_FUNCTION            0
                 96 LOAD_CONST              11 ('LanguageModel')
                 98 LOAD_NAME                5 (object)
                100 PRECALL                  3
                104 CALL                     3
                114 STORE_NAME               9 (LanguageModel)
                116 LOAD_CONST               2 (None)
@@ -78,25 +78,25 @@
          code 0x970065005a0164005a0264015a03640284005a0464035300
            8           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('LanguageModelStub')
                        8 STORE_NAME               2 (__qualname__)
          
-           9          10 LOAD_CONST               1 ('Interface exported by the server.\n    ')
+           9          10 LOAD_CONST               1 ('Interface exported by the server.')
                       12 STORE_NAME               3 (__doc__)
          
-          12          14 LOAD_CONST               2 (<code object __init__, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\python\completion\llm_pb2_grpc.py", line 12>)
+          11          14 LOAD_CONST               2 (<code object __init__, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\completion\llm_pb2_grpc.py", line 11>)
                       16 MAKE_FUNCTION            0
                       18 STORE_NAME               4 (__init__)
                       20 LOAD_CONST               3 (None)
                       22 RETURN_VALUE
          consts
             'LanguageModelStub'
-            'Interface exported by the server.\n    '
+            'Interface exported by the server.'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x97007c01a0000000000000000000000000000000000000000000640174
@@ -104,49 +104,49 @@
                   007402000000000000000000006a0400000000000000006a050000000000
                   000000ac02a6030000ab0300000000000000007c005f0600000000000000
                   007c01a00700000000000000000000000000000000000000006403740200
                   0000000000000000006a0200000000000000006a03000000000000000074
                   02000000000000000000006a0400000000000000006a0500000000000000
                   00ac02a6030000ab0300000000000000007c005f08000000000000000064
                   045300
-                12           0 RESUME                   0
+                11           0 RESUME                   0
                
-                18           2 LOAD_FAST                1 (channel)
+                17           2 LOAD_FAST                1 (channel)
                              4 LOAD_METHOD              0 (unary_unary)
                
-                19          26 LOAD_CONST               1 ('/languagemodel.LanguageModel/Complete')
+                18          26 LOAD_CONST               1 ('/languagemodel.LanguageModel/Complete')
                
-                20          28 LOAD_GLOBAL              2 (llm__pb2)
+                19          28 LOAD_GLOBAL              2 (llm__pb2)
                             40 LOAD_ATTR                2 (Message)
                             50 LOAD_ATTR                3 (SerializeToString)
                
-                21          60 LOAD_GLOBAL              2 (llm__pb2)
+                20          60 LOAD_GLOBAL              2 (llm__pb2)
                             72 LOAD_ATTR                4 (Completions)
                             82 LOAD_ATTR                5 (FromString)
                
-                18          92 KW_NAMES                 2
+                17          92 KW_NAMES                 2
                             94 PRECALL                  3
                             98 CALL                     3
                            108 LOAD_FAST                0 (self)
                            110 STORE_ATTR               6 (Complete)
                
-                23         120 LOAD_FAST                1 (channel)
+                22         120 LOAD_FAST                1 (channel)
                            122 LOAD_METHOD              7 (unary_stream)
                
-                24         144 LOAD_CONST               3 ('/languagemodel.LanguageModel/StreamComplete')
+                23         144 LOAD_CONST               3 ('/languagemodel.LanguageModel/StreamComplete')
                
-                25         146 LOAD_GLOBAL              2 (llm__pb2)
+                24         146 LOAD_GLOBAL              2 (llm__pb2)
                            158 LOAD_ATTR                2 (Message)
                            168 LOAD_ATTR                3 (SerializeToString)
                
-                26         178 LOAD_GLOBAL              2 (llm__pb2)
+                25         178 LOAD_GLOBAL              2 (llm__pb2)
                            190 LOAD_ATTR                4 (Completions)
                            200 LOAD_ATTR                5 (FromString)
                
-                23         210 KW_NAMES                 2
+                22         210 KW_NAMES                 2
                            212 PRECALL                  3
                            216 CALL                     3
                            226 LOAD_FAST                0 (self)
                            228 STORE_ATTR               8 (StreamComplete)
                            238 LOAD_CONST               4 (None)
                            240 RETURN_VALUE
                consts
@@ -155,156 +155,156 @@
                   ('request_serializer', 'response_deserializer')
                   '/languagemodel.LanguageModel/StreamComplete'
                   None
                names      ('unary_unary', 'llm__pb2', 'Message', 'SerializeToString', 'Completions', 'FromString', 'Complete', 'unary_stream', 'StreamComplete')
                varnames   ('self', 'channel')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\completion\\llm_pb2_grpc.py'
+               filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\completion\\llm_pb2_grpc.py'
                name       '__init__'
-               firstlineno 12
+               firstlineno 11
                lnotab 0x020618010201200120fd1c0518010201200120fd
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\completion\\llm_pb2_grpc.py'
+         filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\completion\\llm_pb2_grpc.py'
          name       'LanguageModelStub'
          firstlineno 8
-         lnotab 0x0a010403
+         lnotab 0x0a010402
       'LanguageModelStub'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a03640284005a04640384005a05640453
             00
-          30           0 RESUME                   0
+          29           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('LanguageModelServicer')
                        8 STORE_NAME               2 (__qualname__)
          
-          31          10 LOAD_CONST               1 ('Interface exported by the server.\n    ')
+          30          10 LOAD_CONST               1 ('Interface exported by the server.')
                       12 STORE_NAME               3 (__doc__)
          
-          34          14 LOAD_CONST               2 (<code object Complete, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\python\completion\llm_pb2_grpc.py", line 34>)
+          32          14 LOAD_CONST               2 (<code object Complete, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\completion\llm_pb2_grpc.py", line 32>)
                       16 MAKE_FUNCTION            0
                       18 STORE_NAME               4 (Complete)
          
-          41          20 LOAD_CONST               3 (<code object StreamComplete, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\python\completion\llm_pb2_grpc.py", line 41>)
+          38          20 LOAD_CONST               3 (<code object StreamComplete, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\completion\llm_pb2_grpc.py", line 38>)
                       22 MAKE_FUNCTION            0
                       24 STORE_NAME               5 (StreamComplete)
                       26 LOAD_CONST               4 (None)
                       28 RETURN_VALUE
          consts
             'LanguageModelServicer'
-            'Interface exported by the server.\n    '
+            'Interface exported by the server.'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c02a0000000000000000000000000000000000000000000740200
                   0000000000000000006a0200000000000000006a030000000000000000a6
                   010000ab01000000000000000001007c02a0040000000000000000000000
                   0000000000000000006401a6010000ab0100000000000000000100740b00
                   0000000000000000006401a6010000ab0100000000000000008201
-                34           0 RESUME                   0
+                32           0 RESUME                   0
                
-                37           2 LOAD_FAST                2 (context)
+                34           2 LOAD_FAST                2 (context)
                              4 LOAD_METHOD              0 (set_code)
                             26 LOAD_GLOBAL              2 (grpc)
                             38 LOAD_ATTR                2 (StatusCode)
                             48 LOAD_ATTR                3 (UNIMPLEMENTED)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 POP_TOP
                
-                38          74 LOAD_FAST                2 (context)
+                35          74 LOAD_FAST                2 (context)
                             76 LOAD_METHOD              4 (set_details)
                             98 LOAD_CONST               1 ('Method not implemented!')
                            100 PRECALL                  1
                            104 CALL                     1
                            114 POP_TOP
                
-                39         116 LOAD_GLOBAL             11 (NULL + NotImplementedError)
+                36         116 LOAD_GLOBAL             11 (NULL + NotImplementedError)
                            128 LOAD_CONST               1 ('Method not implemented!')
                            130 PRECALL                  1
                            134 CALL                     1
                            144 RAISE_VARARGS            1
                consts
-                  'Simple RPC.\n        '
+                  'Simple RPC.'
                   'Method not implemented!'
                names      ('set_code', 'grpc', 'StatusCode', 'UNIMPLEMENTED', 'set_details', 'NotImplementedError')
                varnames   ('self', 'request', 'context')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\completion\\llm_pb2_grpc.py'
+               filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\completion\\llm_pb2_grpc.py'
                name       'Complete'
-               firstlineno 34
-               lnotab 0x020348012a01
+               firstlineno 32
+               lnotab 0x020248012a01
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c02a0000000000000000000000000000000000000000000740200
                   0000000000000000006a0200000000000000006a030000000000000000a6
                   010000ab01000000000000000001007c02a0040000000000000000000000
                   0000000000000000006401a6010000ab0100000000000000000100740b00
                   0000000000000000006401a6010000ab0100000000000000008201
-                41           0 RESUME                   0
+                38           0 RESUME                   0
                
-                44           2 LOAD_FAST                2 (context)
+                40           2 LOAD_FAST                2 (context)
                              4 LOAD_METHOD              0 (set_code)
                             26 LOAD_GLOBAL              2 (grpc)
                             38 LOAD_ATTR                2 (StatusCode)
                             48 LOAD_ATTR                3 (UNIMPLEMENTED)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 POP_TOP
                
-                45          74 LOAD_FAST                2 (context)
+                41          74 LOAD_FAST                2 (context)
                             76 LOAD_METHOD              4 (set_details)
                             98 LOAD_CONST               1 ('Method not implemented!')
                            100 PRECALL                  1
                            104 CALL                     1
                            114 POP_TOP
                
-                46         116 LOAD_GLOBAL             11 (NULL + NotImplementedError)
+                42         116 LOAD_GLOBAL             11 (NULL + NotImplementedError)
                            128 LOAD_CONST               1 ('Method not implemented!')
                            130 PRECALL                  1
                            134 CALL                     1
                            144 RAISE_VARARGS            1
                consts
-                  'Server-to-client streaming RPC.\n        '
+                  'Server-to-client streaming RPC.'
                   'Method not implemented!'
                names      ('set_code', 'grpc', 'StatusCode', 'UNIMPLEMENTED', 'set_details', 'NotImplementedError')
                varnames   ('self', 'request', 'context')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\completion\\llm_pb2_grpc.py'
+               filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\completion\\llm_pb2_grpc.py'
                name       'StreamComplete'
-               firstlineno 41
-               lnotab 0x020348012a01
+               firstlineno 38
+               lnotab 0x020248012a01
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'Complete', 'StreamComplete')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\completion\\llm_pb2_grpc.py'
+         filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\completion\\llm_pb2_grpc.py'
          name       'LanguageModelServicer'
-         firstlineno 30
-         lnotab 0x0a0104030607
+         firstlineno 29
+         lnotab 0x0a0104020606
       'LanguageModelServicer'
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
@@ -315,67 +315,67 @@
             0000000000000000006a0800000000000000007c006a0900000000000000
             007406000000000000000000006a0400000000000000006a050000000000
             0000007406000000000000000000006a0600000000000000006a07000000
             0000000000ac01a6030000ab03000000000000000064029c027d02740100
             0000000000000000006a0a000000000000000064037c02a6020000ab0200
             000000000000007d037c01a00b0000000000000000000000000000000000
             0000007c036601a6010000ab010000000000000000010064005300
-          49           0 RESUME                   0
+          45           0 RESUME                   0
          
-          51           2 LOAD_GLOBAL              1 (NULL + grpc)
+          47           2 LOAD_GLOBAL              1 (NULL + grpc)
                       14 LOAD_ATTR                1 (unary_unary_rpc_method_handler)
          
-          52          24 LOAD_FAST                0 (servicer)
+          48          24 LOAD_FAST                0 (servicer)
                       26 LOAD_ATTR                2 (Complete)
          
-          53          36 LOAD_GLOBAL              6 (llm__pb2)
+          49          36 LOAD_GLOBAL              6 (llm__pb2)
                       48 LOAD_ATTR                4 (Message)
                       58 LOAD_ATTR                5 (FromString)
          
-          54          68 LOAD_GLOBAL              6 (llm__pb2)
+          50          68 LOAD_GLOBAL              6 (llm__pb2)
                       80 LOAD_ATTR                6 (Completions)
                       90 LOAD_ATTR                7 (SerializeToString)
          
-          51         100 KW_NAMES                 1
+          47         100 KW_NAMES                 1
                      102 PRECALL                  3
                      106 CALL                     3
          
-          56         116 LOAD_GLOBAL              1 (NULL + grpc)
+          52         116 LOAD_GLOBAL              1 (NULL + grpc)
                      128 LOAD_ATTR                8 (unary_stream_rpc_method_handler)
          
-          57         138 LOAD_FAST                0 (servicer)
+          53         138 LOAD_FAST                0 (servicer)
                      140 LOAD_ATTR                9 (StreamComplete)
          
-          58         150 LOAD_GLOBAL              6 (llm__pb2)
+          54         150 LOAD_GLOBAL              6 (llm__pb2)
                      162 LOAD_ATTR                4 (Message)
                      172 LOAD_ATTR                5 (FromString)
          
-          59         182 LOAD_GLOBAL              6 (llm__pb2)
+          55         182 LOAD_GLOBAL              6 (llm__pb2)
                      194 LOAD_ATTR                6 (Completions)
                      204 LOAD_ATTR                7 (SerializeToString)
          
-          56         214 KW_NAMES                 1
+          52         214 KW_NAMES                 1
                      216 PRECALL                  3
                      220 CALL                     3
          
-          50         230 LOAD_CONST               2 (('Complete', 'StreamComplete'))
+          46         230 LOAD_CONST               2 (('Complete', 'StreamComplete'))
                      232 BUILD_CONST_KEY_MAP      2
                      234 STORE_FAST               2 (rpc_method_handlers)
          
-          62         236 LOAD_GLOBAL              1 (NULL + grpc)
+          58         236 LOAD_GLOBAL              1 (NULL + grpc)
                      248 LOAD_ATTR               10 (method_handlers_generic_handler)
          
-          63         258 LOAD_CONST               3 ('languagemodel.LanguageModel')
+          59         258 LOAD_CONST               3 ('languagemodel.LanguageModel')
                      260 LOAD_FAST                2 (rpc_method_handlers)
          
-          62         262 PRECALL                  2
+          58         262 PRECALL                  2
                      266 CALL                     2
                      276 STORE_FAST               3 (generic_handler)
          
-          64         278 LOAD_FAST                1 (server)
+          61         278 LOAD_FAST                1 (server)
                      280 LOAD_METHOD             11 (add_generic_rpc_handlers)
                      302 LOAD_FAST                3 (generic_handler)
                      304 BUILD_TUPLE              1
                      306 PRECALL                  1
                      310 CALL                     1
                      320 POP_TOP
                      322 LOAD_CONST               0 (None)
@@ -385,217 +385,239 @@
             ('request_deserializer', 'response_serializer')
             ('Complete', 'StreamComplete')
             'languagemodel.LanguageModel'
          names      ('grpc', 'unary_unary_rpc_method_handler', 'Complete', 'llm__pb2', 'Message', 'FromString', 'Completions', 'SerializeToString', 'unary_stream_rpc_method_handler', 'StreamComplete', 'method_handlers_generic_handler', 'add_generic_rpc_handlers')
          varnames   ('servicer', 'server', 'rpc_method_handlers', 'generic_handler')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\completion\\llm_pb2_grpc.py'
+         filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\completion\\llm_pb2_grpc.py'
          name       'add_LanguageModelServicer_to_server'
-         firstlineno 49
+         firstlineno 45
          lnotab
             0x020216010c01200120fd100516010c01200120fd10fa060c160104ff10
-            02
+            03
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0264015a03650409000900090009000900090009
             000900640764058401a6000000ab0000000000000000005a056504090009
             00090009000900090009000900640764068401a6000000ab000000000000
             0000005a0664035300
-          68           0 RESUME                   0
+          65           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('LanguageModel')
                        8 STORE_NAME               2 (__qualname__)
          
-          69          10 LOAD_CONST               1 ('Interface exported by the server.\n    ')
+          66          10 LOAD_CONST               1 ('Interface exported by the server.')
                       12 STORE_NAME               3 (__doc__)
          
-          72          14 LOAD_NAME                4 (staticmethod)
+          68          14 LOAD_NAME                4 (staticmethod)
          
-          75          16 NOP
+          72          16 NOP
          
-          76          18 NOP
+          73          18 NOP
          
-          77          20 NOP
+          74          20 NOP
          
-          78          22 NOP
+          75          22 NOP
          
-          79          24 NOP
+          76          24 NOP
          
-          80          26 NOP
+          77          26 NOP
          
-          81          28 NOP
+          78          28 NOP
          
-          82          30 NOP
+          79          30 NOP
          
-          73          32 LOAD_CONST               7 (((), None, None, False, None, None, None, None))
-                      34 LOAD_CONST               5 (<code object Complete, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\python\completion\llm_pb2_grpc.py", line 72>)
+          69          32 LOAD_CONST               7 (((), None, None, False, None, None, None, None))
+                      34 LOAD_CONST               5 (<code object Complete, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\completion\llm_pb2_grpc.py", line 68>)
                       36 MAKE_FUNCTION            1 (defaults)
          
-          72          38 PRECALL                  0
+          68          38 PRECALL                  0
                       42 CALL                     0
          
-          73          52 STORE_NAME               5 (Complete)
+          69          52 STORE_NAME               5 (Complete)
          
-          89          54 LOAD_NAME                4 (staticmethod)
+          97          54 LOAD_NAME                4 (staticmethod)
          
-          92          56 NOP
+         101          56 NOP
          
-          93          58 NOP
+         102          58 NOP
          
-          94          60 NOP
+         103          60 NOP
          
-          95          62 NOP
+         104          62 NOP
          
-          96          64 NOP
+         105          64 NOP
          
-          97          66 NOP
+         106          66 NOP
          
-          98          68 NOP
+         107          68 NOP
          
-          99          70 NOP
+         108          70 NOP
          
-          90          72 LOAD_CONST               7 (((), None, None, False, None, None, None, None))
-                      74 LOAD_CONST               6 (<code object StreamComplete, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\python\completion\llm_pb2_grpc.py", line 89>)
+          98          72 LOAD_CONST               7 (((), None, None, False, None, None, None, None))
+                      74 LOAD_CONST               6 (<code object StreamComplete, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\completion\llm_pb2_grpc.py", line 97>)
                       76 MAKE_FUNCTION            1 (defaults)
          
-          89          78 PRECALL                  0
+          97          78 PRECALL                  0
                       82 CALL                     0
          
-          90          92 STORE_NAME               6 (StreamComplete)
+          98          92 STORE_NAME               6 (StreamComplete)
                       94 LOAD_CONST               3 (None)
                       96 RETURN_VALUE
          consts
             'LanguageModel'
-            'Interface exported by the server.\n    '
+            'Interface exported by the server.'
             ()
             None
             False
             code
                argcount  : 10
                nlocals   : 10
                stacksize : 15
                flags     : 3
                code
                   0x97007400000000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000007c007c01640174060000000000
                   00000000006a0400000000000000006a0500000000000000007406000000
                   000000000000006a0600000000000000006a0700000000000000007c027c
                   037c057c047c067c077c087c09a60d0000ab0d00000000000000005300
-                72           0 RESUME                   0
+                68           0 RESUME                   0
                
-                83           2 LOAD_GLOBAL              0 (grpc)
+                81           2 LOAD_GLOBAL              0 (grpc)
                             14 LOAD_ATTR                1 (experimental)
                             24 LOAD_METHOD              2 (unary_unary)
-                            46 LOAD_FAST                0 (request)
-                            48 LOAD_FAST                1 (target)
-                            50 LOAD_CONST               1 ('/languagemodel.LanguageModel/Complete')
                
-                84          52 LOAD_GLOBAL              6 (llm__pb2)
+                82          46 LOAD_FAST                0 (request)
+               
+                83          48 LOAD_FAST                1 (target)
+               
+                84          50 LOAD_CONST               1 ('/languagemodel.LanguageModel/Complete')
+               
+                85          52 LOAD_GLOBAL              6 (llm__pb2)
                             64 LOAD_ATTR                4 (Message)
                             74 LOAD_ATTR                5 (SerializeToString)
                
-                85          84 LOAD_GLOBAL              6 (llm__pb2)
+                86          84 LOAD_GLOBAL              6 (llm__pb2)
                             96 LOAD_ATTR                6 (Completions)
                            106 LOAD_ATTR                7 (FromString)
                
-                86         116 LOAD_FAST                2 (options)
-                           118 LOAD_FAST                3 (channel_credentials)
+                87         116 LOAD_FAST                2 (options)
+               
+                88         118 LOAD_FAST                3 (channel_credentials)
+               
+                89         120 LOAD_FAST                5 (insecure)
+               
+                90         122 LOAD_FAST                4 (call_credentials)
+               
+                91         124 LOAD_FAST                6 (compression)
+               
+                92         126 LOAD_FAST                7 (wait_for_ready)
+               
+                93         128 LOAD_FAST                8 (timeout)
                
-                87         120 LOAD_FAST                5 (insecure)
-                           122 LOAD_FAST                4 (call_credentials)
-                           124 LOAD_FAST                6 (compression)
-                           126 LOAD_FAST                7 (wait_for_ready)
-                           128 LOAD_FAST                8 (timeout)
-                           130 LOAD_FAST                9 (metadata)
+                94         130 LOAD_FAST                9 (metadata)
                
-                83         132 PRECALL                 13
+                81         132 PRECALL                 13
                            136 CALL                    13
                            146 RETURN_VALUE
                consts
                   None
                   '/languagemodel.LanguageModel/Complete'
                names      ('grpc', 'experimental', 'unary_unary', 'llm__pb2', 'Message', 'SerializeToString', 'Completions', 'FromString')
                varnames   ('request', 'target', 'options', 'channel_credentials', 'call_credentials', 'insecure', 'compression', 'wait_for_ready', 'timeout', 'metadata')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\completion\\llm_pb2_grpc.py'
+               filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\completion\\llm_pb2_grpc.py'
                name       'Complete'
-               firstlineno 72
-               lnotab 0x020b32012001200104010cfc
+               firstlineno 68
+               lnotab
+                  0x020d2c0102010201020120012001020102010201020102010201020102
+                  f3
             code
                argcount  : 10
                nlocals   : 10
                stacksize : 15
                flags     : 3
                code
                   0x97007400000000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000007c007c01640174060000000000
                   00000000006a0400000000000000006a0500000000000000007406000000
                   000000000000006a0600000000000000006a0700000000000000007c027c
                   037c057c047c067c077c087c09a60d0000ab0d00000000000000005300
-                89           0 RESUME                   0
+                97           0 RESUME                   0
                
-               100           2 LOAD_GLOBAL              0 (grpc)
+               110           2 LOAD_GLOBAL              0 (grpc)
                             14 LOAD_ATTR                1 (experimental)
                             24 LOAD_METHOD              2 (unary_stream)
-                            46 LOAD_FAST                0 (request)
-                            48 LOAD_FAST                1 (target)
-                            50 LOAD_CONST               1 ('/languagemodel.LanguageModel/StreamComplete')
                
-               101          52 LOAD_GLOBAL              6 (llm__pb2)
+               111          46 LOAD_FAST                0 (request)
+               
+               112          48 LOAD_FAST                1 (target)
+               
+               113          50 LOAD_CONST               1 ('/languagemodel.LanguageModel/StreamComplete')
+               
+               114          52 LOAD_GLOBAL              6 (llm__pb2)
                             64 LOAD_ATTR                4 (Message)
                             74 LOAD_ATTR                5 (SerializeToString)
                
-               102          84 LOAD_GLOBAL              6 (llm__pb2)
+               115          84 LOAD_GLOBAL              6 (llm__pb2)
                             96 LOAD_ATTR                6 (Completions)
                            106 LOAD_ATTR                7 (FromString)
                
-               103         116 LOAD_FAST                2 (options)
-                           118 LOAD_FAST                3 (channel_credentials)
+               116         116 LOAD_FAST                2 (options)
+               
+               117         118 LOAD_FAST                3 (channel_credentials)
+               
+               118         120 LOAD_FAST                5 (insecure)
+               
+               119         122 LOAD_FAST                4 (call_credentials)
+               
+               120         124 LOAD_FAST                6 (compression)
+               
+               121         126 LOAD_FAST                7 (wait_for_ready)
+               
+               122         128 LOAD_FAST                8 (timeout)
                
-               104         120 LOAD_FAST                5 (insecure)
-                           122 LOAD_FAST                4 (call_credentials)
-                           124 LOAD_FAST                6 (compression)
-                           126 LOAD_FAST                7 (wait_for_ready)
-                           128 LOAD_FAST                8 (timeout)
-                           130 LOAD_FAST                9 (metadata)
+               123         130 LOAD_FAST                9 (metadata)
                
-               100         132 PRECALL                 13
+               110         132 PRECALL                 13
                            136 CALL                    13
                            146 RETURN_VALUE
                consts
                   None
                   '/languagemodel.LanguageModel/StreamComplete'
                names      ('grpc', 'experimental', 'unary_stream', 'llm__pb2', 'Message', 'SerializeToString', 'Completions', 'FromString')
                varnames   ('request', 'target', 'options', 'channel_credentials', 'call_credentials', 'insecure', 'compression', 'wait_for_ready', 'timeout', 'metadata')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\completion\\llm_pb2_grpc.py'
+               filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\completion\\llm_pb2_grpc.py'
                name       'StreamComplete'
-               firstlineno 89
-               lnotab 0x020b32012001200104010cfc
+               firstlineno 97
+               lnotab
+                  0x020d2c0102010201020120012001020102010201020102010201020102
+                  f3
             ((), None, None, False, None, None, None, None)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'staticmethod', 'Complete', 'StreamComplete')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\completion\\llm_pb2_grpc.py'
+         filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\completion\\llm_pb2_grpc.py'
          name       'LanguageModel'
-         firstlineno 68
+         firstlineno 65
          lnotab
-            0x0a0104030203020102010201020102010201020102f706ff0e01021002
-            03020102010201020102010201020102f706ff0e01
+            0x0a0104020204020102010201020102010201020102f606ff0e01021c02
+            04020102010201020102010201020102f606ff0e01
       'LanguageModel'
    names      ('__doc__', 'grpc', '', 'llm_pb2', 'llm__pb2', 'object', 'LanguageModelStub', 'LanguageModelServicer', 'add_LanguageModelServicer_to_server', 'LanguageModel')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\completion\\llm_pb2_grpc.py'
+   filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\completion\\llm_pb2_grpc.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0202040108020c031c161c130613
+   lnotab 0x00ff0202040108020c031c151c100614
```

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/client.py` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/completion/client.py`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/llm_pb2.py` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/completion/llm_pb2.py`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/llm_pb2.pyi` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/completion/llm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/llm_pb2_grpc.py` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/completion/llm_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/model.py` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/completion/model.py`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/server.py` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/completion/server.py`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/__pycache__/client.cpython-311.pyc` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/embedding/__pycache__/client.cpython-311.pyc`

 * *Files 18% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x55911c64 (Thu Mar 23 17:50:13 2023 UTC)
-files sz: 810
+moddate:  0xb57d2d64 (Wed Apr  5 13:55:01 2023 UTC)
+files sz: 813
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x970064005a00640164026c016d025a020100640164036c036d045a0401
@@ -52,35 +52,35 @@
     10          62 LOAD_CONST               6 (1)
                 64 LOAD_CONST               8 (('llm_embed_pb2_grpc',))
                 66 IMPORT_NAME              8
                 68 IMPORT_FROM             10 (llm_embed_pb2_grpc)
                 70 STORE_NAME              10 (llm_embed_pb2_grpc)
                 72 POP_TOP
    
-    12          74 LOAD_CONST               9 (<code object get_embeddings, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\python\embedding\client.py", line 12>)
+    13          74 LOAD_CONST               9 (<code object get_embeddings, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\embedding\client.py", line 13>)
                 76 MAKE_FUNCTION            0
                 78 STORE_NAME              11 (get_embeddings)
    
-    21          80 NOP
+    22          80 NOP
    
-    22          82 NOP
+    23          82 NOP
    
-    20          84 LOAD_CONST              15 (('localhost:50051', ''))
+    21          84 LOAD_CONST              15 (('localhost:50051', ''))
                 86 LOAD_CONST              12 ('url')
    
-    21          88 LOAD_NAME               12 (str)
+    22          88 LOAD_NAME               12 (str)
    
-    20          90 LOAD_CONST              13 ('inputs')
+    21          90 LOAD_CONST              13 ('inputs')
    
-    22          92 LOAD_NAME                4 (List)
+    23          92 LOAD_NAME                4 (List)
                 94 LOAD_NAME               12 (str)
                 96 BINARY_SUBSCR
    
-    20         106 BUILD_TUPLE              4
-               108 LOAD_CONST              14 (<code object run, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\python\embedding\client.py", line 20>)
+    21         106 BUILD_TUPLE              4
+               108 LOAD_CONST              14 (<code object run, file "C:\Users\lno\Code\simpleai\src\simple_ai\api\grpc\embedding\client.py", line 21>)
                110 MAKE_FUNCTION            5 (defaults, annotations)
                112 STORE_NAME              13 (run)
                114 LOAD_CONST               4 (None)
                116 RETURN_VALUE
    consts
       'The Python implementation of the gRPC route guide client.'
       0
@@ -99,59 +99,59 @@
          code
             0x97007c00a00000000000000000000000000000000000000000007c01a6
             010000ab0100000000000000007d0267007d037c026a0100000000000000
             0044005d377d047c03a00200000000000000000000000000000000000000
             007407000000000000000000007c04a6010000ab010000000000000000a0
             0400000000000000000000000000000000000000006401a6010000ab0100
             00000000000000a6010000ab01000000000000000001008c387c035300
-          12           0 RESUME                   0
+          13           0 RESUME                   0
          
-          13           2 LOAD_FAST                0 (stub)
+          14           2 LOAD_FAST                0 (stub)
                        4 LOAD_METHOD              0 (Embed)
                       26 LOAD_FAST                1 (sentences)
                       28 PRECALL                  1
                       32 CALL                     1
                       42 STORE_FAST               2 (response)
          
-          14          44 BUILD_LIST               0
+          15          44 BUILD_LIST               0
                       46 STORE_FAST               3 (results)
          
-          15          48 LOAD_FAST                2 (response)
+          16          48 LOAD_FAST                2 (response)
                       50 LOAD_ATTR                1 (embedding)
                       60 GET_ITER
                  >>   62 FOR_ITER                55 (to 174)
                       64 STORE_FAST               4 (message)
          
-          16          66 LOAD_FAST                3 (results)
+          17          66 LOAD_FAST                3 (results)
                       68 LOAD_METHOD              2 (append)
                       90 LOAD_GLOBAL              7 (NULL + MessageToDict)
                      102 LOAD_FAST                4 (message)
                      104 PRECALL                  1
                      108 CALL                     1
                      118 LOAD_METHOD              4 (get)
                      140 LOAD_CONST               1 ('feature')
                      142 PRECALL                  1
                      146 CALL                     1
                      156 PRECALL                  1
                      160 CALL                     1
                      170 POP_TOP
                      172 JUMP_BACKWARD           56 (to 62)
          
-          17     >>  174 LOAD_FAST                3 (results)
+          18     >>  174 LOAD_FAST                3 (results)
                      176 RETURN_VALUE
          consts
             None
             'feature'
          names      ('Embed', 'embedding', 'append', 'MessageToDict', 'get')
          varnames   ('stub', 'sentences', 'response', 'results', 'message')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\embedding\\client.py'
+         filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\embedding\\client.py'
          name       'get_embeddings'
-         firstlineno 12
+         firstlineno 13
          lnotab 0x02012a01040112016c01
       'localhost:50051'
       ''
       'url'
       'inputs'
       code
          argcount  : 2
@@ -162,48 +162,48 @@
             0x97007401000000000000000000006a0100000000000000007c00a60100
             00ab01000000000000000035007d027405000000000000000000006a0300
             000000000000007c02a6010000ab0100000000000000007d037409000000
             000000000000006a0500000000000000007c01ac01a6010000ab01000000
             00000000007d04740d000000000000000000007c037c04a6020000ab0200
             000000000000006302640064006400a6020000ab02000000000000000001
             0053002300310073047702780359007701010059000100010064005300
-          20           0 RESUME                   0
+          21           0 RESUME                   0
          
-          24           2 LOAD_GLOBAL              1 (NULL + grpc)
+          25           2 LOAD_GLOBAL              1 (NULL + grpc)
                       14 LOAD_ATTR                1 (insecure_channel)
                       24 LOAD_FAST                0 (url)
                       26 PRECALL                  1
                       30 CALL                     1
                       40 BEFORE_WITH
                       42 STORE_FAST               2 (channel)
          
-          25          44 LOAD_GLOBAL              5 (NULL + llm_embed_pb2_grpc)
+          26          44 LOAD_GLOBAL              5 (NULL + llm_embed_pb2_grpc)
                       56 LOAD_ATTR                3 (LanguageModelStub)
                       66 LOAD_FAST                2 (channel)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               3 (stub)
          
-          26          84 LOAD_GLOBAL              9 (NULL + llm_embed_pb2)
+          27          84 LOAD_GLOBAL              9 (NULL + llm_embed_pb2)
                       96 LOAD_ATTR                5 (Sentences)
          
-          27         106 LOAD_FAST                1 (inputs)
+          28         106 LOAD_FAST                1 (inputs)
          
-          26         108 KW_NAMES                 1
+          27         108 KW_NAMES                 1
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               4 (sentences)
          
-          29         126 LOAD_GLOBAL             13 (NULL + get_embeddings)
+          30         126 LOAD_GLOBAL             13 (NULL + get_embeddings)
                      138 LOAD_FAST                3 (stub)
                      140 LOAD_FAST                4 (sentences)
                      142 PRECALL                  2
                      146 CALL                     2
          
-          24         156 SWAP                     2
+          25         156 SWAP                     2
                      158 LOAD_CONST               0 (None)
                      160 LOAD_CONST               0 (None)
                      162 LOAD_CONST               0 (None)
                      164 PRECALL                  2
                      168 CALL                     2
                      178 POP_TOP
                      180 RETURN_VALUE
@@ -227,22 +227,22 @@
          consts
             None
             ('inputs',)
          names      ('grpc', 'insecure_channel', 'llm_embed_pb2_grpc', 'LanguageModelStub', 'llm_embed_pb2', 'Sentences', 'get_embeddings')
          varnames   ('url', 'inputs', 'channel', 'stub', 'sentences')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\embedding\\client.py'
+         filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\embedding\\client.py'
          name       'run'
-         firstlineno 20
+         firstlineno 21
          lnotab 0x02042a012801160102ff12031efb
       ('localhost:50051', '')
    names      ('__doc__', '__future__', 'print_function', 'typing', 'List', 'grpc', 'google.protobuf.json_format', 'MessageToDict', '', 'llm_embed_pb2', 'llm_embed_pb2_grpc', 'get_embeddings', 'str', 'run')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\embedding\\client.py'
+   filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\embedding\\client.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020104020c020c0208010c010c010c020609020102fe040102ff02
+      0x00ff020104020c020c0208010c010c010c030609020102fe040102ff02
       020efe
```

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/__pycache__/llm_embed_pb2.cpython-311.pyc` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/embedding/__pycache__/llm_embed_pb2.cpython-311.pyc`

 * *Files 24% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xea591a64 (Wed Mar 22 01:29:14 2023 UTC)
-files sz: 1697
+moddate:  0xb57d2d64 (Wed Apr  5 13:55:01 2023 UTC)
+files sz: 1808
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x970064005a00640164026c016d025a030100640164036c046d055a0601
@@ -51,106 +51,109 @@
      8          42 LOAD_CONST               1 (0)
                 44 LOAD_CONST               5 (('symbol_database',))
                 46 IMPORT_NAME              4 (google.protobuf)
                 48 IMPORT_FROM              9 (symbol_database)
                 50 STORE_NAME              10 (_symbol_database)
                 52 POP_TOP
    
-    11          54 PUSH_NULL
+    12          54 PUSH_NULL
                 56 LOAD_NAME               10 (_symbol_database)
                 58 LOAD_ATTR               11 (Default)
                 68 PRECALL                  0
                 72 CALL                     0
                 82 STORE_NAME              12 (_sym_db)
    
-    16          84 PUSH_NULL
+    15          84 PUSH_NULL
                 86 LOAD_NAME                8 (_descriptor_pool)
                 88 LOAD_ATTR               11 (Default)
                 98 PRECALL                  0
                102 CALL                     0
                112 LOAD_METHOD             13 (AddSerializedFile)
-               134 LOAD_CONST               6 (b'\n\x0fllm_embed.proto\x12\x17languagemodelembeddings"\x1b\n\tSentences\x12\x0e\n\x06inputs\x18\x01 \x03(\t"\x1c\n\tEmbedding\x12\x0f\n\x07feature\x18\x01 \x03(\x02"I\n\x10ListOfEmbeddings\x125\n\tembedding\x18\x01 \x03(\x0b2".languagemodelembeddings.Embedding2i\n\rLanguageModel\x12X\n\x05Embed\x12".languagemodelembeddings.Sentences\x1a).languagemodelembeddings.ListOfEmbeddings"\x00B:\n\x16io.grpc.examples.embedB\x16LanguageModelEmbeddingP\x01\xa2\x02\x05embedb\x06proto3')
-               136 PRECALL                  1
+   
+    16         134 LOAD_CONST               6 (b'\n\x0fllm_embed.proto\x12\x17languagemodelembeddings"\x1b\n\tSentences\x12\x0e\n\x06inputs\x18\x01 \x03(\t"\x1c\n\tEmbedding\x12\x0f\n\x07feature\x18\x01 \x03(\x02"I\n\x10ListOfEmbeddings\x125\n\tembedding\x18\x01 \x03(\x0b2".languagemodelembeddings.Embedding2i\n\rLanguageModel\x12X\n\x05Embed\x12".languagemodelembeddings.Sentences\x1a).languagemodelembeddings.ListOfEmbeddings"\x00B:\n\x16io.grpc.examples.embedB\x16LanguageModelEmbeddingP\x01\xa2\x02\x05embedb\x06proto3')
+   
+    15         136 PRECALL                  1
                140 CALL                     1
                150 STORE_NAME              14 (DESCRIPTOR)
    
-    18         152 PUSH_NULL
+    22         152 PUSH_NULL
                154 LOAD_NAME                3 (_builder)
                156 LOAD_ATTR               15 (BuildMessageAndEnumDescriptors)
                166 LOAD_NAME               14 (DESCRIPTOR)
                168 PUSH_NULL
                170 LOAD_NAME               16 (globals)
                172 PRECALL                  0
                176 CALL                     0
                186 PRECALL                  2
                190 CALL                     2
                200 POP_TOP
    
-    19         202 PUSH_NULL
+    23         202 PUSH_NULL
                204 LOAD_NAME                3 (_builder)
                206 LOAD_ATTR               17 (BuildTopDescriptorsAndMessages)
                216 LOAD_NAME               14 (DESCRIPTOR)
                218 LOAD_CONST               7 ('llm_embed_pb2')
                220 PUSH_NULL
                222 LOAD_NAME               16 (globals)
                224 PRECALL                  0
                228 CALL                     0
                238 PRECALL                  3
                242 CALL                     3
                252 POP_TOP
    
-    20         254 LOAD_NAME                6 (_descriptor)
+    24         254 LOAD_NAME                6 (_descriptor)
                256 LOAD_ATTR               18 (_USE_C_DESCRIPTORS)
                266 LOAD_CONST               8 (False)
                268 COMPARE_OP               2 (==)
                274 POP_JUMP_FORWARD_IF_FALSE    72 (to 420)
    
-    22         276 LOAD_CONST               9 (None)
+    25         276 LOAD_CONST               9 (None)
                278 LOAD_NAME               14 (DESCRIPTOR)
                280 STORE_ATTR              19 (_options)
    
-    23         290 LOAD_CONST              10 (b'\n\x16io.grpc.examples.embedB\x16LanguageModelEmbeddingP\x01\xa2\x02\x05embed')
-               292 LOAD_NAME               14 (DESCRIPTOR)
+    27         290 LOAD_CONST              10 (b'\n\x16io.grpc.examples.embedB\x16LanguageModelEmbeddingP\x01\xa2\x02\x05embed')
+   
+    26         292 LOAD_NAME               14 (DESCRIPTOR)
                294 STORE_ATTR              20 (_serialized_options)
    
-    24         304 LOAD_CONST              11 (44)
+    29         304 LOAD_CONST              11 (44)
                306 LOAD_NAME               21 (_SENTENCES)
                308 STORE_ATTR              22 (_serialized_start)
    
-    25         318 LOAD_CONST              12 (71)
+    30         318 LOAD_CONST              12 (71)
                320 LOAD_NAME               21 (_SENTENCES)
                322 STORE_ATTR              23 (_serialized_end)
    
-    26         332 LOAD_CONST              13 (73)
+    31         332 LOAD_CONST              13 (73)
                334 LOAD_NAME               24 (_EMBEDDING)
                336 STORE_ATTR              22 (_serialized_start)
    
-    27         346 LOAD_CONST              14 (101)
+    32         346 LOAD_CONST              14 (101)
                348 LOAD_NAME               24 (_EMBEDDING)
                350 STORE_ATTR              23 (_serialized_end)
    
-    28         360 LOAD_CONST              15 (103)
+    33         360 LOAD_CONST              15 (103)
                362 LOAD_NAME               25 (_LISTOFEMBEDDINGS)
                364 STORE_ATTR              22 (_serialized_start)
    
-    29         374 LOAD_CONST              16 (176)
+    34         374 LOAD_CONST              16 (176)
                376 LOAD_NAME               25 (_LISTOFEMBEDDINGS)
                378 STORE_ATTR              23 (_serialized_end)
    
-    30         388 LOAD_CONST              17 (178)
+    35         388 LOAD_CONST              17 (178)
                390 LOAD_NAME               26 (_LANGUAGEMODEL)
                392 STORE_ATTR              22 (_serialized_start)
    
-    31         402 LOAD_CONST              18 (283)
+    36         402 LOAD_CONST              18 (283)
                404 LOAD_NAME               26 (_LANGUAGEMODEL)
                406 STORE_ATTR              23 (_serialized_end)
                416 LOAD_CONST               9 (None)
                418 RETURN_VALUE
    
-    20     >>  420 LOAD_CONST               9 (None)
+    24     >>  420 LOAD_CONST               9 (None)
                422 RETURN_VALUE
    consts
       'Generated protocol buffer code.'
       0
       ('builder',)
       ('descriptor',)
       ('descriptor_pool',)
@@ -168,13 +171,13 @@
       176
       178
       283
    names      ('__doc__', 'google.protobuf.internal', 'builder', '_builder', 'google.protobuf', 'descriptor', '_descriptor', 'descriptor_pool', '_descriptor_pool', 'symbol_database', '_symbol_database', 'Default', '_sym_db', 'AddSerializedFile', 'DESCRIPTOR', 'BuildMessageAndEnumDescriptors', 'globals', 'BuildTopDescriptorsAndMessages', '_USE_C_DESCRIPTORS', '_options', '_serialized_options', '_SENTENCES', '_serialized_start', '_serialized_end', '_EMBEDDING', '_LISTOFEMBEDDINGS', '_LANGUAGEMODEL')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\python\\embedding\\llm_embed_pb2.py'
+   filename   'C:\\Users\\lno\\Code\\simpleai\\src\\simple_ai\\api\\grpc\\embedding\\llm_embed_pb2.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020404010c010c010c010c031e0544023201340116020e010e010e
-      010e010e010e010e010e010e0112f5
+      0x00ff020404010c010c010c010c041e03320102ff10073201340116010e
+      0202ff0c030e010e010e010e010e010e010e0112f4
```

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/client.py` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/embedding/client.py`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/llm_embed_pb2.py` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/embedding/llm_embed_pb2.py`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/llm_embed_pb2.pyi` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/embedding/llm_embed_pb2.pyi`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/llm_embed_pb2_grpc.py` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/embedding/llm_embed_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/server.py` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/embedding/server.py`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/protos/llm_chat.proto` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/protos/llm_chat.proto`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/protos/llm_complete.proto` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/protos/llm_complete.proto`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/api/grpc/protos/llm_embed.proto` & `simple_ai_server-0.2.1/src/simple_ai/api/grpc/protos/llm_embed.proto`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/dummy.py` & `simple_ai_server-0.2.1/src/simple_ai/dummy.py`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.2.0/src/simple_ai/models.py` & `simple_ai_server-0.2.1/src/simple_ai/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     import tomllib
 else:
     import tomli as tomllib
 
 from .api.grpc.chat import client as chat_client
 from .api.grpc.completion import client as lm_client
 from .api.grpc.embedding import client as embed_client
+from .api_models import ModelConfig, ModelInterfaceTypes, ModelTaskTypes
 
 path = pathlib.Path(os.environ.get("SIMPLEAI_CONFIG_PATH", "models.toml"))
 with path.open(mode="rb") as fp:
     MODELS_ZOO = tomllib.load(fp)
 
 
 @dataclass(unsafe_hash=True)
@@ -162,37 +163,43 @@
             stop=stop,
             presence_penalty=presence_penalty,
             frequence_penalty=frequence_penalty,
             logit_bias=logit_bias,
         )
 
 
-def select_model_type(model_interface: str = "gRPC", task: str = "complete"):
+def select_model_type(model_interface: str, task: str):
     if model_interface == "gRPC":
         if task == "embed":
             return RpcEmbeddingLanguageModel
         if task == "chat":
             return RpcChatLanguageModel
-        return RpcCompletionLanguageModel
-    return RpcCompletionLanguageModel
+        if task == "complete":
+            return RpcCompletionLanguageModel
+        raise ValueError(f"`task` value must be in {ModelTaskTypes.list()}, got `{task}` instead`.")
+    return ValueError(
+        f"`model_interface` value must be in {ModelInterfaceTypes.list()} `gRPC`, got"
+        f" `{model_interface}` instead."
+    )
 
 
-def get_model(model_id: str, metadata: dict = MODELS_ZOO, task: str = "complete"):
+def get_model(model_id: str, task: ModelTaskTypes, metadata: dict = MODELS_ZOO):
     if model_id in metadata.keys():
-        model_interface = metadata.get(model_id).get("network", dict())
-        model_url = model_interface.get("url", None)
-        model_interface = model_interface.get("type", None)
-        return select_model_type(model_interface, task)(name=model_id, url=model_url)
+        model_config = ModelConfig(**metadata.get(model_id)).network
+        return select_model_type(model_config.type, task)(name=model_id, url=model_config.url)
     else:
-        return None
+        raise ValueError(f"Cannot find model named `{model_id}` in configuration.")
 
 
 def list_models(metadata: dict = MODELS_ZOO) -> list:
     return dict(
-        data=[{"id": key, **meta.get("metadata")} for key, meta in metadata.items()], object="list"
+        data=[
+            {"id": key, **meta.get("metadata"), "object": "model"} for key, meta in metadata.items()
+        ],
+        object="list",
     )
 
 
 def get_model_infos(model_id, metadata: dict = MODELS_ZOO) -> list:
     if model_id in metadata.keys():
         return {"id": model_id, **metadata.get(model_id).get("metadata")}
     return {}
```

### Comparing `simple_ai_server-0.2.0/src/simple_ai/server.py` & `simple_ai_server-0.2.1/src/simple_ai/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,56 +12,57 @@
 from .dummy import dummy_chat, dummy_complete, dummy_edit, dummy_embedding
 from .models import get_model, get_model_infos, list_models
 from .utils import (
     add_instructions,
     format_autocompletion_response,
     format_autocompletion_stream_response,
     format_chat_delta_response,
+    format_chat_delta_response_helper,
     format_chat_response,
     format_edits_response,
     format_embeddings_results,
 )
 
 app = FastAPI(
     title="SimpleAI",
     description="A self-hosted alternative API to the not so Open one",
-    version="0.0.1",
-    terms_of_service="http://example.com/terms/",
+    version="0.2",
+    terms_of_service="https://github.com/lhenault",
     contact={
         "name": "Lhenault",
         "url": "https://github.com/lhenault",
     },
 )
 
 
 # Models
-@app.get("/models/")
+@app.get("/models")
 async def show_models():
     return list_models()
 
 
 @app.get("/models/{model_id}")
 async def show_model(model_id: str):
     return get_model_infos(model_id)
 
 
 # Completions
-@app.post("/completions/")
+@app.post("/completions")
 async def complete(
     body: Annotated[CompletionInput, Body(example=dummy_complete)],
     background_tasks: fastapi.background.BackgroundTasks,
 ):
     assert body.logprobs <= 5
 
     prompt = body.prompt
     if isinstance(prompt, list):
         assert len(body.prompt) == 1, "unsupported, at most 1 prompt allowed"
         prompt = body.prompt[0]
 
-    llm = get_model(model_id=body.model)
+    llm = get_model(model_id=body.model, task="complete")
     if not body.stream:
         predictions = llm.complete(
             prompt=prompt,
             suffix=body.suffix,
             max_tokens=body.max_tokens,
             temperature=body.temperature,
             top_p=body.top_p,
@@ -148,38 +149,40 @@
     background_tasks.add_task(lambda f: f.close(), predictions_stream)
 
     uuid = uuid4().hex
     current_timestamp = int(dt.now().timestamp())
     postprocessed = map(
         partial(format_chat_delta_response, current_timestamp, uuid, body.model), predictions_stream
     )
-
-    with_finaliser = chain(postprocessed, ("data: [DONE]\n",))
+    stop_message = format_chat_delta_response_helper(
+        current_timestamp, uuid, body.model, predictions=("",), finish_reason="stop"
+    )
+    with_finaliser = chain(postprocessed, stop_message, ("data: [DONE]\n",))
     return StreamingResponse(with_finaliser, media_type="text/event-stream")
 
 
 # Edits
-@app.post("/edits/")
+@app.post("/edits")
 async def edit(body: Annotated[InstructionInput, Body(example=dummy_edit)]):
-    llm = get_model(model_id=body.model)
-    input_text = add_instructions(instructions=body.instruction, text=input)
+    llm = get_model(model_id=body.model, task="complete")
+    input_text = add_instructions(instructions=body.instruction, text=body.input)
 
     predictions = llm.complete(
         prompt=input_text,
         temperature=body.temperature,
         top_p=body.top_p,
         n=body.n,
         max_tokens=body.max_tokens,
     )
     output = format_edits_response(model_name=llm.name, predictions=predictions)
     return output
 
 
 # Embeddings
-@app.post("/embeddings/")
+@app.post("/embeddings")
 async def embed(body: Annotated[EmbeddingInput, Body(example=dummy_embedding)]):
     llm = get_model(model_id=body.model, task="embed")
     if isinstance(body.input, str):
         body.input = [body.input]
 
     results = llm.embed(inputs=body.input)
```

### Comparing `simple_ai_server-0.2.0/src/simple_ai/utils.py` & `simple_ai_server-0.2.1/src/simple_ai/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ) -> dict:
     data = {
         "id": response_id,
         "object": "text_completion",
         "created": current_timestamp,
         "model": model_name,
         "choices": [
-            {"text": text, "index": idx, "logprobs": None, "finish_reason": ""}
+            {"text": text, "index": idx, "logprobs": None, "finish_reason": None}
             for idx, text in enumerate(predictions)
         ],
     }
 
     data = f"DATA: {data}\n\n"
 
     return data
@@ -68,61 +68,69 @@
     return {
         "id": response_id,
         "model": model_name,
         "object": "chat.completion",
         "created": current_timestamp,
         "choices": [
             {
-                "role": "assistant",
                 "index": idx,
-                "message": {"role": "assistant", "content": text},
+                "message": message,
                 "finish_reason": "stop",
             }
-            for idx, text in enumerate(predictions)
+            for idx, message in enumerate(predictions)
         ],
         "usage": usage,
     }
 
 
-def format_chat_delta_response(
-    current_timestamp, response_id, model_name: str, predictions
+def format_chat_delta_response_helper(
+    current_timestamp, response_id, model_name: str, predictions, finish_reason=None
 ) -> dict:
     data = {
         "id": response_id,
         "model": model_name,
         "object": "chat.completion.chunk",
         "created": current_timestamp,
         "choices": [
             {
                 "index": idx,
                 "delta": message,
-                "finish_reason": "stop",
+                "finish_reason": finish_reason,
             }
             for idx, message in enumerate(predictions)
         ],
     }
-
     return f"data: {json.dumps(data)}\n\n"
 
 
+def format_chat_delta_response(
+    current_timestamp, response_id, model_name: str, predictions
+) -> dict:
+    data = format_chat_delta_response_helper(
+        current_timestamp, response_id, model_name, predictions, finish_reason=None
+    )
+
+    return data
+
+
 def format_embeddings_results(model_name: str, embeddings: list, usage: dict = dummy_usage) -> dict:
     return {
         "object": "list",
         "data": [
             {"object": "embedding", "embedding": embedding, "index": idx}
             for idx, embedding in enumerate(embeddings)
         ],
         "model": model_name,
         "usage": usage,
     }
 
 
 def add_instructions(instructions: str, text: str) -> str:
     prompt = f"### Instruction:\n{instructions}.\n\n"
-    if input:
+    if text:
         prompt += f"### Input:\n{text}.\n\n"
     prompt += "### Response:"
     return prompt
 
 
 def format_chat_log(chat: list[dict[str, str]] = dict()) -> str:
     raw_chat_text = ""
```

### Comparing `simple_ai_server-0.2.0/PKG-INFO` & `simple_ai_server-0.2.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-ai-server
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Louis Hénault
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -157,14 +157,71 @@
 openai.api_base = "http://127.0.0.1:8080"
 
 # Do your usual things, for instance a completion query:
 print(openai.Model.list())
 completion = openai.Completion.create(model="llama-7B", prompt="Hello everyone this is")
 ```
 
+## Common issues and solutions
+
+### Adding a CORS middleware
+
+If you encounter CORS issues, it is suggested to not use the `simple_ai serve` command, but to rather use your own script to add your CORS configuration, using the [FastAPI CORS middleware](https://fastapi.tiangolo.com/tutorial/cors/).
+
+For instance you can create `my_server.py` with:
+
+```python
+from simple_ai.server import app
+from fastapi.middleware.cors import CORSMiddleware
+
+def add_cors(app):
+    origins = [
+        "http://localhost",
+        "http://localhost:8080"
+    ]
+    app.add_middleware(
+        CORSMiddleware,
+        allow_origins=origins,
+        allow_credentials=True,
+        allow_methods=["*"],
+        allow_headers=["*"],
+    )
+    return app
+
+def serve_app(host="127.0.0.1", port=8080, **kwargs):
+    app = add_cors(app)
+    uvicorn.run(app=app, host=host, port=port)
+    
+if __name__ == "__main__":
+    serve_app(host="127.0.0.1", port=8080)
+    
+```
+
+And run it as `python3 my_server.py` instead.
+
+### I needd `/v1` prefix in the endpoints
+
+Some projects have decided to include the `/v1` prefix as part of the endpoints, while OpenAI client includes it in its `api_base` parameter. If you need to have it as part of the endpoints for your project, you can use a custom script instead of `simple_ai serve`:
+
+```python
+import uvicorn
+from simple_ai.server import app as v1_app
+from fastapi import APIRouter, FastAPI
+
+sai_app = FastAPI()
+sai_app.mount("/v1", v1_app)
+
+def serve_app(app=sai_app, host="0.0.0.0", port=8080):
+    uvicorn.run(app=app, host=host, port=port)
+    
+if __name__ == "__main__":
+    serve_app()
+    
+```
+
 ## Contribute
 
 This is very much work in progress and far from being perfect, so let me know if you want to help. PR, issues, documentation, cool logo, all the usual candidates are welcome.
 
 ### Development Environment
 
 In order for the following steps to work it is required to have make and poetry installed on your system.
```

