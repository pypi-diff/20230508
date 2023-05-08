# Comparing `tmp/autoxx-0.0.10.tar.gz` & `tmp/autoxx-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.10.tar", max compression
+gzip compressed data, was "autoxx-0.0.11.tar", max compression
```

## Comparing `autoxx-0.0.10.tar` & `autoxx-0.0.11.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.10/README.md
--rw-r--r--   0        0        0      310 2023-05-06 05:23:14.108735 autoxx-0.0.10/autoxx/agent/base.py
--rw-r--r--   0        0        0      970 2023-05-08 02:54:46.023981 autoxx-0.0.10/autoxx/agent/researcher.py
--rw-r--r--   0        0        0     4125 2023-05-07 04:54:29.318874 autoxx-0.0.10/autoxx/agi.py
--rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.10/autoxx/js/overlay.js
--rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.10/autoxx/requirements.txt
--rw-r--r--   0        0        0     5177 2023-05-08 04:26:50.166173 autoxx-0.0.10/autoxx/search/simple_search.py
--rw-r--r--   0        0        0     4995 2023-05-07 02:59:38.452753 autoxx-0.0.10/autoxx/task_manager.py
--rw-r--r--   0        0        0      633 2023-05-08 04:44:58.143037 autoxx-0.0.10/pyproject.toml
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 autoxx-0.0.10/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.11/README.md
+-rw-r--r--   0        0        0      310 2023-05-06 05:23:14.108735 autoxx-0.0.11/autoxx/agent/base.py
+-rw-r--r--   0        0        0      970 2023-05-08 02:54:46.023981 autoxx-0.0.11/autoxx/agent/researcher.py
+-rw-r--r--   0        0        0     4126 2023-05-08 07:15:16.426595 autoxx-0.0.11/autoxx/agi.py
+-rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.11/autoxx/js/overlay.js
+-rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.11/autoxx/requirements.txt
+-rw-r--r--   0        0        0     5307 2023-05-08 08:04:26.191393 autoxx-0.0.11/autoxx/search/simple_search.py
+-rw-r--r--   0        0        0     4995 2023-05-07 02:59:38.452753 autoxx-0.0.11/autoxx/task_manager.py
+-rw-r--r--   0        0        0      633 2023-05-08 08:07:15.998759 autoxx-0.0.11/pyproject.toml
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 autoxx-0.0.11/PKG-INFO
```

### Comparing `autoxx-0.0.10/autoxx/agent/researcher.py` & `autoxx-0.0.11/autoxx/agent/researcher.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.10/autoxx/agi.py` & `autoxx-0.0.11/autoxx/agi.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     return {
         "role": "user",
         "content": prompt,
     }
 
 def task_creation_agent(objective: str, task: Dict, task_list: List[str], allowed_new_task: Optional[int] = 1):
     prompt = (
-        f"You are an task creation AI that uses the result of an execution agent to create new tasks with the following objective: {objective}, "
+        f"You are an task creation AI that uses the result of an execution agent to create new tasks with the following objective: {objective}.\n"
         f"The last completed task has the result: {task['data']}. "
         f"This result was based on this task description: {task['task_description']}. "
         f"These are incomplete tasks: {', '.join(task_list)}. "
         f"Based on the result, create new tasks to be completed by the AI system that do not overlap with incomplete tasks. Up to {allowed_new_task} new tasks can be created.\n"
         "You should only respond in JSON format as described below \n"
         f"Response Format: \n{response_format} \nEnsure the response can be parsed by Python json.loads"
     )
```

### Comparing `autoxx-0.0.10/autoxx/js/overlay.js` & `autoxx-0.0.11/autoxx/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.10/autoxx/search/simple_search.py` & `autoxx-0.0.11/autoxx/search/simple_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,21 +138,23 @@
 def simple_search(question:str, search_num:Optional[int]=2) -> str:
     search_result = google_search(query=question, num_results=search_num)
     search_search_json = json.loads(search_result)
     summaries = []
 
     if isinstance(search_search_json, list):
         for res in search_search_json:
+            print(f"{res['title']} x {res['href']}\n")
             summary = browse_website(url=res['href'], question=question)
             summaries.extend(summary)
-            print(f"\n{res['title']} x {res['href']} summary: {summary}\n")
+            print(f"{res['title']} x {res['href']} summary: {summary}\n")
     else:
+        print(f"{search_search_json['title']} x {search_search_json['href']}")
         summary = browse_website(url=search_search_json['href'], question=question)
         summaries.extend(summary)
-        print(f"\n{search_search_json['title']} x {search_search_json['href']} summary: {summary}\n")
+        print(f"{search_search_json['title']} x {search_search_json['href']} summary: {summary}\n")
 
     if len(summaries) == 1:
         return summaries[0]
 
     if len(summaries) == 1:
         return summaries[0]
```

### Comparing `autoxx-0.0.10/autoxx/task_manager.py` & `autoxx-0.0.11/autoxx/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.10/pyproject.toml` & `autoxx-0.0.11/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.10"
+version = "0.0.11"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `autoxx-0.0.10/PKG-INFO` & `autoxx-0.0.11/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.10
+Version: 0.0.11
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

