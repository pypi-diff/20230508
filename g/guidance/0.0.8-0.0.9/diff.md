# Comparing `tmp/guidance-0.0.8.tar.gz` & `tmp/guidance-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guidance-0.0.8.tar", last modified: Fri Dec  9 21:41:36 2022, max compression
+gzip compressed data, was "guidance-0.0.9.tar", last modified: Mon Dec 12 19:58:33 2022, max compression
```

## Comparing `guidance-0.0.8.tar` & `guidance-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxr-x   0 slundberg  (1000) slundberg  (1000)        0 2022-12-09 21:41:36.819430 guidance-0.0.8/
--rw-rw-r--   0 slundberg  (1000) slundberg  (1000)     1071 2022-11-10 18:22:31.000000 guidance-0.0.8/LICENSE
--rw-rw-r--   0 slundberg  (1000) slundberg  (1000)      295 2022-12-09 21:41:36.819430 guidance-0.0.8/PKG-INFO
--rw-rw-r--   0 slundberg  (1000) slundberg  (1000)     2716 2022-11-21 16:40:25.000000 guidance-0.0.8/README.md
-drwxrwxr-x   0 slundberg  (1000) slundberg  (1000)        0 2022-12-09 21:41:36.819430 guidance-0.0.8/guidance/
--rw-rw-r--   0 slundberg  (1000) slundberg  (1000)      138 2022-12-09 21:41:14.000000 guidance-0.0.8/guidance/__init__.py
--rw-rw-r--   0 slundberg  (1000) slundberg  (1000)    17595 2022-12-09 18:16:18.000000 guidance-0.0.8/guidance/_prompt.py
--rw-rw-r--   0 slundberg  (1000) slundberg  (1000)     3941 2022-12-09 21:38:28.000000 guidance-0.0.8/guidance/generators.py
-drwxrwxr-x   0 slundberg  (1000) slundberg  (1000)        0 2022-12-09 21:41:36.819430 guidance-0.0.8/guidance/library/
--rw-rw-r--   0 slundberg  (1000) slundberg  (1000)       25 2022-12-01 04:16:58.000000 guidance-0.0.8/guidance/library/__init__.py
--rw-rw-r--   0 slundberg  (1000) slundberg  (1000)     2319 2022-12-02 02:07:24.000000 guidance-0.0.8/guidance/library/_shell.py
--rw-rw-r--   0 slundberg  (1000) slundberg  (1000)    14116 2022-11-21 15:31:38.000000 guidance-0.0.8/guidance/prompt_old.py
-drwxrwxr-x   0 slundberg  (1000) slundberg  (1000)        0 2022-12-09 21:41:36.819430 guidance-0.0.8/guidance.egg-info/
--rw-rw-r--   0 slundberg  (1000) slundberg  (1000)      295 2022-12-09 21:41:36.000000 guidance-0.0.8/guidance.egg-info/PKG-INFO
--rw-rw-r--   0 slundberg  (1000) slundberg  (1000)      328 2022-12-09 21:41:36.000000 guidance-0.0.8/guidance.egg-info/SOURCES.txt
--rw-rw-r--   0 slundberg  (1000) slundberg  (1000)        1 2022-12-09 21:41:36.000000 guidance-0.0.8/guidance.egg-info/dependency_links.txt
--rw-rw-r--   0 slundberg  (1000) slundberg  (1000)       25 2022-12-09 21:41:36.000000 guidance-0.0.8/guidance.egg-info/requires.txt
--rw-rw-r--   0 slundberg  (1000) slundberg  (1000)        9 2022-12-09 21:41:36.000000 guidance-0.0.8/guidance.egg-info/top_level.txt
--rw-rw-r--   0 slundberg  (1000) slundberg  (1000)       38 2022-12-09 21:41:36.819430 guidance-0.0.8/setup.cfg
--rw-rw-r--   0 slundberg  (1000) slundberg  (1000)      956 2022-11-17 23:23:04.000000 guidance-0.0.8/setup.py
+drwxrwxr-x   0 slundberg  (1000) slundberg  (1000)        0 2022-12-12 19:58:33.060860 guidance-0.0.9/
+-rw-rw-r--   0 slundberg  (1000) slundberg  (1000)     1071 2022-11-10 18:22:31.000000 guidance-0.0.9/LICENSE
+-rw-rw-r--   0 slundberg  (1000) slundberg  (1000)      295 2022-12-12 19:58:33.056860 guidance-0.0.9/PKG-INFO
+-rw-rw-r--   0 slundberg  (1000) slundberg  (1000)     2716 2022-11-21 16:40:25.000000 guidance-0.0.9/README.md
+drwxrwxr-x   0 slundberg  (1000) slundberg  (1000)        0 2022-12-12 19:58:33.056860 guidance-0.0.9/guidance/
+-rw-rw-r--   0 slundberg  (1000) slundberg  (1000)      138 2022-12-12 19:54:56.000000 guidance-0.0.9/guidance/__init__.py
+-rw-rw-r--   0 slundberg  (1000) slundberg  (1000)    17595 2022-12-09 18:16:18.000000 guidance-0.0.9/guidance/_prompt.py
+-rw-rw-r--   0 slundberg  (1000) slundberg  (1000)     4230 2022-12-12 19:56:45.000000 guidance-0.0.9/guidance/generators.py
+drwxrwxr-x   0 slundberg  (1000) slundberg  (1000)        0 2022-12-12 19:58:33.056860 guidance-0.0.9/guidance/library/
+-rw-rw-r--   0 slundberg  (1000) slundberg  (1000)       25 2022-12-01 04:16:58.000000 guidance-0.0.9/guidance/library/__init__.py
+-rw-rw-r--   0 slundberg  (1000) slundberg  (1000)     2319 2022-12-02 02:07:24.000000 guidance-0.0.9/guidance/library/_shell.py
+drwxrwxr-x   0 slundberg  (1000) slundberg  (1000)        0 2022-12-12 19:58:33.056860 guidance-0.0.9/guidance.egg-info/
+-rw-rw-r--   0 slundberg  (1000) slundberg  (1000)      295 2022-12-12 19:58:32.000000 guidance-0.0.9/guidance.egg-info/PKG-INFO
+-rw-rw-r--   0 slundberg  (1000) slundberg  (1000)      305 2022-12-12 19:58:33.000000 guidance-0.0.9/guidance.egg-info/SOURCES.txt
+-rw-rw-r--   0 slundberg  (1000) slundberg  (1000)        1 2022-12-12 19:58:32.000000 guidance-0.0.9/guidance.egg-info/dependency_links.txt
+-rw-rw-r--   0 slundberg  (1000) slundberg  (1000)       25 2022-12-12 19:58:32.000000 guidance-0.0.9/guidance.egg-info/requires.txt
+-rw-rw-r--   0 slundberg  (1000) slundberg  (1000)        9 2022-12-12 19:58:32.000000 guidance-0.0.9/guidance.egg-info/top_level.txt
+-rw-rw-r--   0 slundberg  (1000) slundberg  (1000)       38 2022-12-12 19:58:33.060860 guidance-0.0.9/setup.cfg
+-rw-rw-r--   0 slundberg  (1000) slundberg  (1000)      956 2022-11-17 23:23:04.000000 guidance-0.0.9/setup.py
```

### Comparing `guidance-0.0.8/LICENSE` & `guidance-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `guidance-0.0.8/README.md` & `guidance-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `guidance-0.0.8/guidance/_prompt.py` & `guidance-0.0.9/guidance/_prompt.py`

 * *Files identical despite different names*

### Comparing `guidance-0.0.8/guidance/generators.py` & `guidance-0.0.9/guidance/generators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 import openai
 import pathlib
 import diskcache
 import os
 import time
 import requests
+import warnings
 
 curr_dir = pathlib.Path(__file__).parent.resolve()
 _file_cache = diskcache.Cache(f"{curr_dir}/../lm.diskcache")
 
-OPENAI_API_KEY = os.environ.get("OPENAI_API_KEY", None)
-
-if OPENAI_API_KEY is None:
-    try:
-        with open(os.path.expanduser('~/.openai_api_key'), 'r') as file:
-            openai.api_key = file.read().replace('\n', '')
-    except:
-        raise Exception("Warning: No OpenAI api key found, you need to set the OPENAI_API_KEY environment variable or put your key in the file ~/.openai_api_key")
-
-try:
-    with open(os.path.expanduser('~/.openai_lm_model_name'), 'r') as file:
-        gpt_model = file.read().replace('\n', '')
-except:
-    raise Exception("Warning: No OpenAI model name found, you need to put your OpenAI model name in the file ~/.openai_lm_model_name")
-
 class OpenAI():
     def __init__(self, model=None, caching=True, max_retries=2, token=None, endpoint=None):
 
-        # default to environment variable values
+        # fill in default model value
+        if model is None:
+            model = os.environ.get("OPENAI_MODEL", None)
         if model is None:
-            model = os.environ.get("OPENAI_MODEL", gpt_model)
+            try:
+                with open(os.path.expanduser('~/.openai_model'), 'r') as file:
+                    model = file.read().replace('\n', '')
+            except:
+                pass
+        
+        # fill in default API key value
+        if token is None:
+            token = os.environ.get("OPENAI_API_KEY", openai.api_key)
         if token is None:
-            token = os.environ.get("OPENAI_API_KEY", None)
+            try:
+                with open(os.path.expanduser('~/.openai_api_key'), 'r') as file:
+                    token = file.read().replace('\n', '')
+            except:
+                pass
+        
+        # fill in default endpoint value
         if endpoint is None:
             endpoint = os.environ.get("OPENAI_ENDPOINT", None)
         
         self.model = model
         self.caching = caching
         self.max_retries = max_retries
         self.token = token
@@ -42,14 +44,17 @@
 
         if self.endpoint is None:
             self.caller = self._library_call
         else:
             self.caller = self._rest_call
     
     def __call__(self, prompt, stop=None, temperature=0.0, n=1, max_tokens=1000, logprobs=None, top_p=1.0):
+        """ Generate a completion of the given prompt.
+        """
+
         key = "_---_".join([str(v) for v in (self.model, prompt, stop, temperature, n, max_tokens, logprobs)])
         if key not in _file_cache or not self.caching:
 
             fail_count = 0
             while True:
                 try_again = False
                 try:
@@ -69,17 +74,28 @@
                 if fail_count > self.max_retries:
                     raise Exception(f"Too many (more than {self.max_retries}) OpenAI API RateLimitError's in a row!")
 
             _file_cache[key] = out
         return _file_cache[key]
 
     def _library_call(self, **kwargs):
-        return openai.Completion.create(**kwargs)
+        """ Call the OpenAI API using the python package.
+
+        Note that is uses the local auth token, and does not rely on the openai one.
+        """
+        prev_key = openai.api_key
+        openai.api_key = self.token
+        out = openai.Completion.create(**kwargs)
+        openai.api_key = prev_key
+        return out
 
     def _rest_call(self, **kwargs):
+        """ Call the OpenAI API using the REST API.
+        """
+
         # Define the request headers
         headers = {
             'Content-Type': 'application/json',
             'Authorization': f'Bearer {self.token}'
         }
 
         # Define the request data
```

### Comparing `guidance-0.0.8/guidance/library/_shell.py` & `guidance-0.0.9/guidance/library/_shell.py`

 * *Files identical despite different names*

### Comparing `guidance-0.0.8/setup.py` & `guidance-0.0.9/setup.py`

 * *Files identical despite different names*

