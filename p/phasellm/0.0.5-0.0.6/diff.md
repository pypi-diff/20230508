# Comparing `tmp/phasellm-0.0.5.tar.gz` & `tmp/phasellm-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phasellm-0.0.5.tar", last modified: Mon May  1 21:37:59 2023, max compression
+gzip compressed data, was "phasellm-0.0.6.tar", last modified: Mon May  8 17:55:53 2023, max compression
```

## Comparing `phasellm-0.0.5.tar` & `phasellm-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-01 21:37:59.684568 phasellm-0.0.5/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1083 2023-05-01 21:37:50.000000 phasellm-0.0.5/LICENSE
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      739 2023-05-01 21:37:59.684568 phasellm-0.0.5/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4976 2023-05-01 21:37:50.000000 phasellm-0.0.5/README.md
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-01 21:37:59.684568 phasellm-0.0.5/phasellm/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      653 2023-05-01 21:37:50.000000 phasellm-0.0.5/phasellm/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     5152 2023-05-01 21:37:50.000000 phasellm-0.0.5/phasellm/agents.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3499 2023-05-01 21:37:50.000000 phasellm-0.0.5/phasellm/eval.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2013 2023-05-01 21:37:50.000000 phasellm-0.0.5/phasellm/exceptions.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    13653 2023-05-01 21:37:50.000000 phasellm-0.0.5/phasellm/llms.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-01 21:37:59.684568 phasellm-0.0.5/phasellm.egg-info/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      739 2023-05-01 21:37:59.000000 phasellm-0.0.5/phasellm.egg-info/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      282 2023-05-01 21:37:59.000000 phasellm-0.0.5/phasellm.egg-info/SOURCES.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-05-01 21:37:59.000000 phasellm-0.0.5/phasellm.egg-info/dependency_links.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      126 2023-05-01 21:37:59.000000 phasellm-0.0.5/phasellm.egg-info/requires.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        9 2023-05-01 21:37:59.000000 phasellm-0.0.5/phasellm.egg-info/top_level.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       38 2023-05-01 21:37:59.684568 phasellm-0.0.5/setup.cfg
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1167 2023-05-01 21:37:50.000000 phasellm-0.0.5/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 17:55:53.150623 phasellm-0.0.6/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-05-08 17:39:29.000000 phasellm-0.0.6/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-05-08 17:55:53.150623 phasellm-0.0.6/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4976 2023-05-08 17:39:29.000000 phasellm-0.0.6/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 17:55:53.150623 phasellm-0.0.6/phasellm/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      653 2023-05-08 17:39:29.000000 phasellm-0.0.6/phasellm/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5152 2023-05-08 17:39:29.000000 phasellm-0.0.6/phasellm/agents.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4802 2023-05-08 17:39:29.000000 phasellm-0.0.6/phasellm/eval.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3015 2023-05-08 17:39:29.000000 phasellm-0.0.6/phasellm/exceptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16699 2023-05-08 17:39:29.000000 phasellm-0.0.6/phasellm/llms.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 17:55:53.150623 phasellm-0.0.6/phasellm.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-05-08 17:55:53.000000 phasellm-0.0.6/phasellm.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      282 2023-05-08 17:55:53.000000 phasellm-0.0.6/phasellm.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-08 17:55:53.000000 phasellm-0.0.6/phasellm.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      126 2023-05-08 17:55:53.000000 phasellm-0.0.6/phasellm.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-08 17:55:53.000000 phasellm-0.0.6/phasellm.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-08 17:55:53.150623 phasellm-0.0.6/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1167 2023-05-08 17:39:29.000000 phasellm-0.0.6/setup.py
```

### Comparing `phasellm-0.0.5/LICENSE` & `phasellm-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.5/PKG-INFO` & `phasellm-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasellm
-Version: 0.0.5
+Version: 0.0.6
 Summary: Wrappers for common large langugae models (LLMs) with support for evaluation.
 Home-page: UNKNOWN
 Author: Wojciech Gryc
 Author-email: hello@phaseai.com
 License: MIT
 Keywords: llm,nlp,evaluation,ai
 Platform: UNKNOWN
```

### Comparing `phasellm-0.0.5/README.md` & `phasellm-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.5/phasellm/__init__.py` & `phasellm-0.0.6/phasellm/__init__.py`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.5/phasellm/agents.py` & `phasellm-0.0.6/phasellm/agents.py`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.5/phasellm/eval.py` & `phasellm-0.0.6/phasellm/eval.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """
 Support for LLM evaluation.
 """
 
-#TODO I don't like the way I'm structuring this stuff right now. I should actually run some experiments first.
-
 from .llms import OpenAIGPTWrapper
 
 import random
 
 class BinaryPreference():
     """
     Tracks a prompt, prompt variables, responses, and the calculated preference.
@@ -31,21 +29,51 @@
 
     def get_preference(self):
         """
         Get the preference of the class.
         """
         return self.preference 
 
+class EvaluationStream():
+    """
+    Tracks human evaluation on the command line and records results.
+    """
+
+    def __init__(self, objective, prompt, models):
+        """
+        Initializes the stream.
+
+        objective: what you are trying to do.
+        prompt: the prompt you are using. Could be a summary thereof, too. We do not actively use this prompt in generating data for evaluation.
+        models: an array of two models. These can be referenced later if need be, but are not necessary for running the evaluation workflow.
+        """
+        self.models = models
+        self.objective = objective
+        self.prompt = prompt
+        self.objective = objective 
+        self.evaluator = HumanEvaluatorCommandLine()
+        self.prefs = [0]*len(models) # This will be a simple counter for now.
+
+    def __repr__(self):
+        return f"<EvaluationStream>"
+    
+    def evaluate(self, response1, response2):
+        """
+        Shows both sets of options for review and tracks the result.
+        """
+        pref = self.evaluator.choose(self.objective, self.prompt, response1, response2)
+        self.prefs[pref - 1] += 1
+
 class HumanEvaluatorCommandLine():
     """
     Presents an objective, prompt, and two potential responses and has a human choose between the two.
     """
 
     def __repr__(self):
-        return "<HumanEvaluatorComamndLine>"
+        return "<HumanEvaluatorCommandLine>"
     
     def choose(self, objective, prompt, response1, response2):
 
         response_map = {"A": 1, "B": 2}
         response_a = response1
         response_b = response2
         if random.random() <= 0.5:
@@ -73,51 +101,61 @@
         user_input = input()
         if user_input not in ["A", "B"]:
             print("Please put in 'A' or 'B' to tell us which is the better response.")
             user_input = input()
 
         return response_map[user_input]        
 
-# TODO Randomize the ordering so we avoid any bias from GPT-3.5.
-class GPT35Evaluator():
+class GPTEvaluator():
     """
-    Passes two model outputs to GPT-3.5 and has it decide which is the better output.
+    Passes two model outputs to GPT-3.5 or GPT-4 and has it decide which is the better output.
     """
 
-    def __init__(self, apikey):
-        self.model = OpenAIGPTWrapper(apikey)
+    def __init__(self, apikey, model="gpt-3.5-turbo"):
+        self.model = OpenAIGPTWrapper(apikey, model=model)
 
     def __repr__(self):
         return f"GPT35Evaluator()"
     
     def choose(self, objective, prompt, response1, response2):
         """
-        Presents the objective of a modeling task, a prompt, and then two responses. GPT-3.5 chooses the preference.
+        Presents the objective of a modeling task, a prompt, and then two responses. GPT-3.5/GPT-4 chooses the preference.
         """
+
+        response_map = {"A": 1, "B": 2}
+        response_a = response1
+        response_b = response2
+        if random.random() <= 0.5:
+            response_map = {"A": 2, "B": 1}
+            response_a = response2 
+            response_b = response1
+
         prompt = f"""We would like your feedback on a large language model we are building. Specifically, we would like you to compare two different LLM responses and let us know which one is better.
 
 Our objective for the LLM is:
 {objective}
 
 The prompt we are using for the LLM is:
 {prompt}
 
 Here are the two pieces of generated text.
 
-1: `{response1}`
+A: `{response_a}`
 
-2: `{response2}`
+B: `{response_b}`
 
-Please simply respond '1' or '2' as to which of the texts above address our earlier objective more effectively. Do not add any additional explanations, thoughts, punctuation, or anything; simply write '1' or '2'."""
+Please simply respond 'A' or 'B' as to which of the texts above address our earlier objective more effectively. Do not add any additional explanations, thoughts, punctuation, or anything; simply write 'A' or 'B'."""
 
         messages = [
-            {"role":"system", "content":"You are an AI assistant helping with promp engineering and model evaluation."},
+            {"role":"system", "content":"You are an AI assistant helping with prompt engineering and model evaluation."},
             {"role":"user", "content":prompt},
         ]
 
         response = self.model.complete_chat(messages, ['\n'])
 
-        # ChatGPT has a preferences for adding "." to the end of the reply.
+        # ChatGPT has a knack for adding "." to the end of the reply.
         if len(response) == 2:
             response = response[0]
 
-        return response
+        choice = response_map[response]
+
+        return choice
```

### Comparing `phasellm-0.0.5/phasellm/llms.py` & `phasellm-0.0.6/phasellm/llms.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,18 +54,59 @@
 
     def text_completion(self, prompt, stop_sequences=[]):
         """
         Standardizes text completion for large language models.
         """
         pass
 
+class ChatPrompt():
+    """
+    This is used to generate messages for a ChatBot. Like the Prompt class, it enables you to to have variables that get replaced. This can be done for roles and messages.
+    """
+
+    def __init__(self, messages=[]):
+
+        self.messages = messages 
+
+    def __repr__(self):
+        return "ChatPrompt()"
+    
+    def chat_repr(self):
+        return _clean_messages_to_prompt(self.messages)
+    
+    def fill(self, **kwargs):
+        filled_messages = []
+        for i in range(0, len(self.messages)):
+            pattern = r'\{\s*[a-zA-Z0-9_]+\s*\}'
+
+            role = self.messages[i]["role"]
+            content = self.messages[i]["content"]
+
+            role_matches = re.findall(pattern, role)
+            new_role = role 
+            for m in role_matches:
+                keyword = m.replace("{", "").replace("}", "").strip()
+                if keyword in kwargs:
+                    new_role = new_role.replace(m, kwargs[keyword])
+
+            content_matches = re.findall(pattern, content)
+            new_content = content 
+            for m in content_matches:
+                keyword = m.replace("{", "").replace("}", "").strip()
+                if keyword in kwargs:
+                    new_content = new_content.replace(m, kwargs[keyword])
+
+            filled_messages.append({"role":new_role, "content":new_content})
+
+        return filled_messages
+
 class Prompt():
     """
     Prompts are used to generate text completions. Prompts can be simple Strings. They can also include variables surrounded by curly braces. For example:
-    Hello {name}!
+    > Hello {name}!
     In this case, 'name' can be filled using the fill_prompts() function. This makes it easier to loop through prompts that follow a specific pattern or structure.
     """
 
     def __init__(self, prompt):
         self.prompt = prompt
 
     def __repr__(self):
@@ -73,32 +114,74 @@
 
     def get_prompt(self):
         """
         Return the raw prompt command (i.e., does not fill in variables.)
         """
         return self.prompt
     
-    def fill_prompts(self, **kwargs):
+    def fill(self, **kwargs):
         """
         Return a prompt with variables filled in.
         """
         pattern = r'\{\s*[a-zA-Z0-9_]+\s*\}'
         matches = re.findall(pattern, self.prompt)
         new_prompt = self.prompt
         for m in matches:
             keyword = m.replace("{", "").replace("}", "").strip()
             if keyword in kwargs:
                 new_prompt = new_prompt.replace(m, kwargs[keyword])
         return new_prompt
 
+class HuggingFaceInferenceWrapper():
+    """
+    Wrapper for Hugging Face's Inference API. Requires access to Hugging Face's inference API.
+    """
+    def __init__(self, apikey, model_url="https://api-inference.huggingface.co/models/bigscience/bloom"):
+        self.apikey = apikey
+        self.model_url = model_url
+
+    def __repr__(self):
+        return f"HuggingFaceInferenceWrapper()"
+
+
+    def complete_chat(self, messages, append_role=None):
+        """
+        Mimicks a chat scenario via a list of {"role": <str>, "content":<str>} objects.
+        """
+
+        prompt_preamble = "You are a friendly chat assistant. You are speaking to the 'user' below and will respond at the end, where it says 'assistant'.\n"
+        prompt_text = prompt_preamble + _clean_messages_to_prompt(messages)
+        if append_role is not None and len(append_role) > 0:
+            prompt_text += f"\n{append_role}:"
+
+        headers = {"Authorization": f"Bearer {self.apikey}"}
+
+        response = requests.post(self.model_url, headers=headers, json={"inputs": prompt_text}).json()
+        new_text = response[0]['generated_text']
+
+        # We only return the first line of text.
+        newline_location = new_text.find("\n") 
+        if newline_location > 0:
+            new_text = new_text[:newline_location]
+        return new_text
+
+    def text_completion(self, prompt):
+        """
+        Completes text.
+        """
+        headers = {"Authorization": f"Bearer {self.apikey}"}
+        response = requests.post(self.model_url, headers=headers, json={"inputs": prompt}).json()
+        all_text = response[0]['generated_text']
+        return all_text
+
 class BloomWrapper():
     """
     Wrapper for Hugging Face's BLOOM model. Requires access to Hugging Face's inference API.
     """
-    def __init__(self, apikey):
+    def __init__(self, apikey, model ):
         self.apikey = apikey
 
     def __repr__(self):
         return f"BloomWrapper()"
 
     def complete_chat(self, messages, append_role=None):
         """
```

### Comparing `phasellm-0.0.5/phasellm.egg-info/PKG-INFO` & `phasellm-0.0.6/phasellm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasellm
-Version: 0.0.5
+Version: 0.0.6
 Summary: Wrappers for common large langugae models (LLMs) with support for evaluation.
 Home-page: UNKNOWN
 Author: Wojciech Gryc
 Author-email: hello@phaseai.com
 License: MIT
 Keywords: llm,nlp,evaluation,ai
 Platform: UNKNOWN
```

### Comparing `phasellm-0.0.5/setup.py` & `phasellm-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 
 DESCRIPTION = "Wrappers for common large langugae models (LLMs) with support for evaluation."
 
 LONG_DESCRIPTION = "PhaseLLM provides wrappers for common large language models and use cases. This makes it easy to swap models in and out as needed. We also provide support for evaluation of models so you can choose which models are better to use."
 
 setup(
     name="phasellm",
```

