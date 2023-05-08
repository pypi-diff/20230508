# Comparing `tmp/autoxx-0.0.8.tar.gz` & `tmp/autoxx-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.8.tar", max compression
+gzip compressed data, was "autoxx-0.0.9.tar", max compression
```

## Comparing `autoxx-0.0.8.tar` & `autoxx-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.8/README.md
--rw-r--r--   0        0        0      310 2023-05-06 05:23:14.108735 autoxx-0.0.8/autoxx/agent/base.py
--rw-r--r--   0        0        0      973 2023-05-06 13:18:45.575572 autoxx-0.0.8/autoxx/agent/researcher.py
--rw-r--r--   0        0        0     4125 2023-05-07 04:54:29.318874 autoxx-0.0.8/autoxx/agi.py
--rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.8/autoxx/js/overlay.js
--rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.8/autoxx/requirements.txt
--rw-r--r--   0        0        0     4808 2023-05-07 05:09:39.925805 autoxx-0.0.8/autoxx/search/simple_search.py
--rw-r--r--   0        0        0     4995 2023-05-07 02:59:38.452753 autoxx-0.0.8/autoxx/task_manager.py
--rw-r--r--   0        0        0      633 2023-05-07 05:09:36.133882 autoxx-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 autoxx-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.9/README.md
+-rw-r--r--   0        0        0      310 2023-05-06 05:23:14.108735 autoxx-0.0.9/autoxx/agent/base.py
+-rw-r--r--   0        0        0      970 2023-05-08 02:54:46.023981 autoxx-0.0.9/autoxx/agent/researcher.py
+-rw-r--r--   0        0        0     4125 2023-05-07 04:54:29.318874 autoxx-0.0.9/autoxx/agi.py
+-rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.9/autoxx/js/overlay.js
+-rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.9/autoxx/requirements.txt
+-rw-r--r--   0        0        0     5177 2023-05-08 04:26:50.166173 autoxx-0.0.9/autoxx/search/simple_search.py
+-rw-r--r--   0        0        0     4995 2023-05-07 02:59:38.452753 autoxx-0.0.9/autoxx/task_manager.py
+-rw-r--r--   0        0        0      802 2023-05-08 04:37:21.143113 autoxx-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1131 1970-01-01 00:00:00.000000 autoxx-0.0.9/PKG-INFO
```

### Comparing `autoxx-0.0.8/autoxx/agent/researcher.py` & `autoxx-0.0.9/autoxx/agent/researcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from autogpt.config import Config
 
 CFG = Config()
 
 class ResearchAgent(BaseAgent):  
   
     def execute(self, objective:str, task: str) -> str:  
-        return simple_search(task, 1)
+        return simple_search(task)
   
     def post_process(self, objective:str, task_results:List[Dict]) -> str:  
         task_context = [f"Task({task['task_description']}): {task['data']}" for task in task_results]
         nl = '\n'
         prompt = (
             "You are an task processing AI."
             f"Given the context {nl.join(task_context) } and objective: {objective}. "
```

### Comparing `autoxx-0.0.8/autoxx/agi.py` & `autoxx-0.0.9/autoxx/agi.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.8/autoxx/js/overlay.js` & `autoxx-0.0.9/autoxx/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.8/autoxx/search/simple_search.py` & `autoxx-0.0.9/autoxx/search/simple_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,16 @@
 
     Returns:
         Dict[str, str]: The message to send to the chat completion
     """
     return {
         "role": "user",
         "content": f'"""{chunk}""" Using the above text, answer the following'
-        f' question: "{question}"',
+        f' question: "{question}" -- if the question cannot be answered using the text,'
+        " summarize the text.",
     }
 
 def scroll_to_percentage(driver: WebDriver, ratio: float) -> None:
     """Scroll to a percentage of the page
 
     Args:
         driver (WebDriver): The webdriver to use
@@ -135,18 +136,26 @@
     return summary
 
 def simple_search(question:str, search_num:Optional[int]=2) -> str:
     search_result = google_search(query=question, num_results=search_num)
     search_search_json = json.loads(search_result)
     summaries = []
 
-    for i in range(len(search_search_json)):
-        summary = browse_website(url=search_search_json[i]['href'], question=question)
+    if isinstance(search_search_json, list):
+        for res in search_search_json:
+            summary = browse_website(url=res['href'], question=question)
+            summaries.extend(summary)
+            print(f"\n{res['title']} x {res['href']} summary: {summary}\n")
+    else:
+        summary = browse_website(url=search_search_json['href'], question=question)
         summaries.extend(summary)
-        print(f"\n{search_search_json[i]['title']} x {search_search_json[i]['href']} summary: {summary}\n")
+        print(f"\n{search_search_json['title']} x {search_search_json['href']} summary: {summary}\n")
+
+    if len(summaries) == 1:
+        return summaries[0]
 
     if len(summaries) == 1:
         return summaries[0]
 
     combined_summary = "\n".join(summaries)
     messages = [create_message(combined_summary, question)]
```

### Comparing `autoxx-0.0.8/autoxx/task_manager.py` & `autoxx-0.0.9/autoxx/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.8/pyproject.toml` & `autoxx-0.0.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.8"
+version = "0.0.9"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -20,11 +20,13 @@
 tiktoken = "0.3.3"
 playsound = "1.2.2"
 gTTS = "2.3.1"
 orjson = "3.8.10"
 duckduckgo-search = "^2.9.3"
 spacy = ">=3.0.0,<4.0.0"
 
+[tool.poetry.dependencies.en-core-web-sm]
+url = "https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.5.0/en_core_web_sm-3.5.0-py3-none-any.whl"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `autoxx-0.0.8/PKG-INFO` & `autoxx-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.8
+Version: 0.0.9
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: agpt (==0.2.2)
 Requires-Dist: auto_gpt_plugin_template (==0.0.3)
 Requires-Dist: bs4 (==0.0.1)
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: duckduckgo-search (>=2.9.3,<3.0.0)
+Requires-Dist: en-core-web-sm @ https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.5.0/en_core_web_sm-3.5.0-py3-none-any.whl
 Requires-Dist: gTTS (==2.3.1)
 Requires-Dist: openai (==0.27.6)
 Requires-Dist: orjson (==3.8.10)
 Requires-Dist: pinecone-client (==2.2.1)
 Requires-Dist: playsound (==1.2.2)
 Requires-Dist: python-dotenv (==1.0.0)
 Requires-Dist: selenium (==4.9.0)
```

