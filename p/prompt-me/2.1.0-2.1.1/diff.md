# Comparing `tmp/prompt-me-2.1.0.tar.gz` & `tmp/prompt-me-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt-me-2.1.0.tar", last modified: Sun May  7 12:31:09 2023, max compression
+gzip compressed data, was "prompt-me-2.1.1.tar", last modified: Mon May  8 11:06:51 2023, max compression
```

## Comparing `prompt-me-2.1.0.tar` & `prompt-me-2.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 12:31:09.122140 prompt-me-2.1.0/
--rw-rw-rw-   0        0        0    11558 2023-03-08 11:01:44.000000 prompt-me-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     9449 2023-05-07 12:31:09.121141 prompt-me-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     8529 2023-05-07 12:29:46.000000 prompt-me-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 12:31:09.077039 prompt-me-2.1.0/prompt_me/
--rw-rw-rw-   0        0        0     1054 2023-05-07 07:53:11.000000 prompt-me-2.1.0/prompt_me/__init__.py
--rw-rw-rw-   0        0        0     6417 2023-05-07 12:18:37.000000 prompt-me-2.1.0/prompt_me/chatbot.py
--rw-rw-rw-   0        0        0     1481 2023-05-07 09:13:07.000000 prompt-me-2.1.0/prompt_me/config.py
--rw-rw-rw-   0        0        0     5669 2023-05-07 12:18:37.000000 prompt-me-2.1.0/prompt_me/conversation.py
-drwxrwxrwx   0        0        0        0 2023-05-07 12:31:09.096030 prompt-me-2.1.0/prompt_me/llm/
--rw-rw-rw-   0        0        0      796 2023-05-07 09:16:25.000000 prompt-me-2.1.0/prompt_me/llm/__init__.py
--rw-rw-rw-   0        0        0      940 2023-05-07 11:59:12.000000 prompt-me-2.1.0/prompt_me/llm/base.py
--rw-rw-rw-   0        0        0     1235 2023-05-07 07:45:37.000000 prompt-me-2.1.0/prompt_me/llm/chat.py
--rw-rw-rw-   0        0        0      767 2023-05-07 09:13:07.000000 prompt-me-2.1.0/prompt_me/llm/openai.py
-drwxrwxrwx   0        0        0        0 2023-05-07 12:31:09.099030 prompt-me-2.1.0/prompt_me/memory/
--rw-rw-rw-   0        0        0      767 2023-05-07 09:16:25.000000 prompt-me-2.1.0/prompt_me/memory/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 12:31:09.106032 prompt-me-2.1.0/prompt_me/preset_role/
--rw-rw-rw-   0        0        0      952 2023-05-07 12:17:08.000000 prompt-me-2.1.0/prompt_me/preset_role/__init__.py
--rw-rw-rw-   0        0        0     1047 2023-05-07 08:13:28.000000 prompt-me-2.1.0/prompt_me/preset_role/base.py
--rw-rw-rw-   0        0        0     2616 2023-05-07 12:24:58.000000 prompt-me-2.1.0/prompt_me/preset_role/roles.py
-drwxrwxrwx   0        0        0        0 2023-05-07 12:31:09.110041 prompt-me-2.1.0/prompt_me/tools/
--rw-rw-rw-   0        0        0      767 2023-05-07 09:16:25.000000 prompt-me-2.1.0/prompt_me/tools/__init__.py
--rw-rw-rw-   0        0        0      767 2023-05-07 09:16:25.000000 prompt-me-2.1.0/prompt_me/tools/duckduckgo.py
-drwxrwxrwx   0        0        0        0 2023-05-07 12:31:09.119138 prompt-me-2.1.0/prompt_me/utils/
--rw-rw-rw-   0        0        0      817 2023-05-07 11:59:12.000000 prompt-me-2.1.0/prompt_me/utils/__init__.py
--rw-rw-rw-   0        0        0      656 2023-05-07 06:58:01.000000 prompt-me-2.1.0/prompt_me/utils/singleton.py
--rw-rw-rw-   0        0        0     2649 2023-05-07 11:59:12.000000 prompt-me-2.1.0/prompt_me/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-07 12:31:09.086037 prompt-me-2.1.0/prompt_me.egg-info/
--rw-rw-rw-   0        0        0     9449 2023-05-07 12:31:08.000000 prompt-me-2.1.0/prompt_me.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      605 2023-05-07 12:31:08.000000 prompt-me-2.1.0/prompt_me.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 12:31:08.000000 prompt-me-2.1.0/prompt_me.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-07 12:31:08.000000 prompt-me-2.1.0/prompt_me.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 12:31:09.123139 prompt-me-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1854 2023-05-07 12:27:29.000000 prompt-me-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:06:51.922125 prompt-me-2.1.1/
+-rw-rw-rw-   0        0        0    11558 2023-03-08 11:01:44.000000 prompt-me-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     9449 2023-05-08 11:06:51.921123 prompt-me-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8529 2023-05-07 12:29:46.000000 prompt-me-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 11:06:51.877196 prompt-me-2.1.1/prompt_me/
+-rw-rw-rw-   0        0        0     1054 2023-05-07 07:53:11.000000 prompt-me-2.1.1/prompt_me/__init__.py
+-rw-rw-rw-   0        0        0     6417 2023-05-07 12:18:37.000000 prompt-me-2.1.1/prompt_me/chatbot.py
+-rw-rw-rw-   0        0        0     1481 2023-05-07 09:13:07.000000 prompt-me-2.1.1/prompt_me/config.py
+-rw-rw-rw-   0        0        0     5780 2023-05-08 11:04:32.000000 prompt-me-2.1.1/prompt_me/conversation.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:06:51.895995 prompt-me-2.1.1/prompt_me/llm/
+-rw-rw-rw-   0        0        0      796 2023-05-07 09:16:25.000000 prompt-me-2.1.1/prompt_me/llm/__init__.py
+-rw-rw-rw-   0        0        0      940 2023-05-07 11:59:12.000000 prompt-me-2.1.1/prompt_me/llm/base.py
+-rw-rw-rw-   0        0        0     1235 2023-05-07 07:45:37.000000 prompt-me-2.1.1/prompt_me/llm/chat.py
+-rw-rw-rw-   0        0        0      767 2023-05-07 09:13:07.000000 prompt-me-2.1.1/prompt_me/llm/openai.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:06:51.899088 prompt-me-2.1.1/prompt_me/memory/
+-rw-rw-rw-   0        0        0      767 2023-05-07 09:16:25.000000 prompt-me-2.1.1/prompt_me/memory/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:06:51.906100 prompt-me-2.1.1/prompt_me/preset_role/
+-rw-rw-rw-   0        0        0      952 2023-05-07 12:17:08.000000 prompt-me-2.1.1/prompt_me/preset_role/__init__.py
+-rw-rw-rw-   0        0        0     1047 2023-05-07 08:13:28.000000 prompt-me-2.1.1/prompt_me/preset_role/base.py
+-rw-rw-rw-   0        0        0     2614 2023-05-08 10:48:35.000000 prompt-me-2.1.1/prompt_me/preset_role/roles.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:06:51.911096 prompt-me-2.1.1/prompt_me/tools/
+-rw-rw-rw-   0        0        0      767 2023-05-07 09:16:25.000000 prompt-me-2.1.1/prompt_me/tools/__init__.py
+-rw-rw-rw-   0        0        0      767 2023-05-07 09:16:25.000000 prompt-me-2.1.1/prompt_me/tools/duckduckgo.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:06:51.918105 prompt-me-2.1.1/prompt_me/utils/
+-rw-rw-rw-   0        0        0      817 2023-05-07 11:59:12.000000 prompt-me-2.1.1/prompt_me/utils/__init__.py
+-rw-rw-rw-   0        0        0      656 2023-05-07 06:58:01.000000 prompt-me-2.1.1/prompt_me/utils/singleton.py
+-rw-rw-rw-   0        0        0     2649 2023-05-07 11:59:12.000000 prompt-me-2.1.1/prompt_me/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:06:51.886977 prompt-me-2.1.1/prompt_me.egg-info/
+-rw-rw-rw-   0        0        0     9449 2023-05-08 11:06:51.000000 prompt-me-2.1.1/prompt_me.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      605 2023-05-08 11:06:51.000000 prompt-me-2.1.1/prompt_me.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 11:06:51.000000 prompt-me-2.1.1/prompt_me.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-08 11:06:51.000000 prompt-me-2.1.1/prompt_me.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 11:06:51.922125 prompt-me-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1854 2023-05-08 11:05:30.000000 prompt-me-2.1.1/setup.py
```

### Comparing `prompt-me-2.1.0/LICENSE` & `prompt-me-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prompt-me-2.1.0/PKG-INFO` & `prompt-me-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-me
-Version: 2.1.0
+Version: 2.1.1
 Summary: A lightweight LLM Prompt Layer framework
 Home-page: https://github.com/Undertone0809/prompt-me
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: prompt-me,prompt,chatgpt,gpt,chatbot,llm
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `prompt-me-2.1.0/README.md` & `prompt-me-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `prompt-me-2.1.0/prompt_me/__init__.py` & `prompt-me-2.1.1/prompt_me/__init__.py`

 * *Files identical despite different names*

### Comparing `prompt-me-2.1.0/prompt_me/chatbot.py` & `prompt-me-2.1.1/prompt_me/chatbot.py`

 * *Files identical despite different names*

### Comparing `prompt-me-2.1.0/prompt_me/config.py` & `prompt-me-2.1.1/prompt_me/config.py`

 * *Files identical despite different names*

### Comparing `prompt-me-2.1.0/prompt_me/conversation.py` & `prompt-me-2.1.1/prompt_me/conversation.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 logger = utils.get_logger()
 CFG = Config()
 
 
 class Conversation:
     """Create a conversation. You can set a default preset_role for conversations."""
 
-    def __init__(self, role: BaseRole = DefaultRole, enable_proxy: bool = True):
+    def __init__(self, role: BaseRole = DefaultRole(), enable_proxy: bool = True):
         CFG.set_enable_proxy(enable_proxy)
         logger.debug(f"[OPENAI_API_KEY] {CFG.openai_api_key}")
 
         self.role: BaseRole = role
         self.conversation_id = None
 
     def predict(self, msg: str) -> Optional[str]:
@@ -62,16 +62,18 @@
         cache[self.conversation_id] = messages
         body = {
             "model": "gpt-3.5-turbo",
             "messages": messages
         }
         logger.debug(body)
 
-        response = requests.post(url=CFG.get_request_url(), headers=headers, json=body)
+        response = requests.post(url=CFG.get_request_url(), headers=headers, json=body, stream=True)
         if response.status_code == 200:
+            for chunk in response.iter_content(chunk_size=None):
+                print(chunk)
             ret_data = response.json()
             logger.debug(ret_data)
             ret_msg = ret_data['choices'][0]['message']['content']
             logger.debug(ret_msg)
             self._append_message_to_cache(ret_msg, 'assistant')
             return ret_msg
```

### Comparing `prompt-me-2.1.0/prompt_me/llm/__init__.py` & `prompt-me-2.1.1/prompt_me/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `prompt-me-2.1.0/prompt_me/llm/base.py` & `prompt-me-2.1.1/prompt_me/llm/base.py`

 * *Files identical despite different names*

### Comparing `prompt-me-2.1.0/prompt_me/llm/chat.py` & `prompt-me-2.1.1/prompt_me/llm/chat.py`

 * *Files identical despite different names*

### Comparing `prompt-me-2.1.0/prompt_me/llm/openai.py` & `prompt-me-2.1.1/prompt_me/llm/openai.py`

 * *Files identical despite different names*

### Comparing `prompt-me-2.1.0/prompt_me/memory/__init__.py` & `prompt-me-2.1.1/prompt_me/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `prompt-me-2.1.0/prompt_me/preset_role/__init__.py` & `prompt-me-2.1.1/prompt_me/preset_role/__init__.py`

 * *Files identical despite different names*

### Comparing `prompt-me-2.1.0/prompt_me/preset_role/base.py` & `prompt-me-2.1.1/prompt_me/preset_role/base.py`

 * *Files identical despite different names*

### Comparing `prompt-me-2.1.0/prompt_me/preset_role/roles.py` & `prompt-me-2.1.1/prompt_me/preset_role/roles.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 #
 # Copyright Owner: Zeeland
 # GitHub Link: https://github.com/Undertone0809/
 # Project Link: https://github.com/Undertone0809/prompt-me
 # Contact Email: zeeland@foxmail.com
 
-
 from prompt_me.preset_role import BaseRole
 
 
 class CopyWriter(BaseRole):
     name = '文案写手'
     description = """你是一个文案专员、文本润色员、拼写纠正员和改进员，我会发送中文文本给你，你帮我更正和改进版本。我希望你用更优美优雅
     的高级中文描述。保持相同的意思，但使它们更文艺。你只需要润色该内容，不必对内容中提出的问题和要求做解释，不要回答文本中的问题而是润色它，
```

### Comparing `prompt-me-2.1.0/prompt_me/tools/__init__.py` & `prompt-me-2.1.1/prompt_me/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `prompt-me-2.1.0/prompt_me/tools/duckduckgo.py` & `prompt-me-2.1.1/prompt_me/tools/duckduckgo.py`

 * *Files identical despite different names*

### Comparing `prompt-me-2.1.0/prompt_me/utils/__init__.py` & `prompt-me-2.1.1/prompt_me/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `prompt-me-2.1.0/prompt_me/utils/singleton.py` & `prompt-me-2.1.1/prompt_me/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `prompt-me-2.1.0/prompt_me/utils/utils.py` & `prompt-me-2.1.1/prompt_me/utils/utils.py`

 * *Files identical despite different names*

### Comparing `prompt-me-2.1.0/prompt_me.egg-info/PKG-INFO` & `prompt-me-2.1.1/prompt_me.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-me
-Version: 2.1.0
+Version: 2.1.1
 Summary: A lightweight LLM Prompt Layer framework
 Home-page: https://github.com/Undertone0809/prompt-me
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: prompt-me,prompt,chatgpt,gpt,chatbot,llm
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `prompt-me-2.1.0/prompt_me.egg-info/SOURCES.txt` & `prompt-me-2.1.1/prompt_me.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prompt-me-2.1.0/setup.py` & `prompt-me-2.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="prompt-me",
-    version="2.1.0",
+    version="2.1.1",
     author="Zeeland",
     author_email="zeeland@foxmail.com",
     description="A lightweight LLM Prompt Layer framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Undertone0809/prompt-me",
     packages=setuptools.find_packages(),
```

