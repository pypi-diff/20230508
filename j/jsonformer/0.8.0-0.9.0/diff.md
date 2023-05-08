# Comparing `tmp/jsonformer-0.8.0.tar.gz` & `tmp/jsonformer-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonformer-0.8.0.tar", max compression
+gzip compressed data, was "jsonformer-0.9.0.tar", max compression
```

## Comparing `jsonformer-0.8.0.tar` & `jsonformer-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2850 2023-05-04 16:48:52.075323 jsonformer-0.8.0/README.md
--rw-r--r--   0        0        0       85 2023-05-01 21:32:30.326739 jsonformer-0.8.0/jsonformer/__init__.py
--rw-r--r--   0        0        0     1081 2023-05-04 16:25:05.263995 jsonformer-0.8.0/jsonformer/example.py
--rw-r--r--   0        0        0      995 2023-05-01 17:24:41.244984 jsonformer-0.8.0/jsonformer/format.py
--rw-r--r--   0        0        0     1984 2023-05-01 17:24:41.245061 jsonformer-0.8.0/jsonformer/logits_processors.py
--rw-r--r--   0        0        0     7197 2023-05-04 16:25:05.264416 jsonformer-0.8.0/jsonformer/main.py
--rw-r--r--   0        0        0      476 2023-05-04 16:48:52.075655 jsonformer-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3507 1970-01-01 00:00:00.000000 jsonformer-0.8.0/setup.py
--rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 jsonformer-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2835 2023-05-04 18:05:57.828543 jsonformer-0.9.0/README.md
+-rw-r--r--   0        0        0       85 2023-05-01 21:32:30.326739 jsonformer-0.9.0/jsonformer/__init__.py
+-rw-r--r--   0        0        0     1046 2023-05-04 18:05:57.838879 jsonformer-0.9.0/jsonformer/example.py
+-rw-r--r--   0        0        0      995 2023-05-01 17:24:41.244984 jsonformer-0.9.0/jsonformer/format.py
+-rw-r--r--   0        0        0     1956 2023-05-04 18:05:57.839047 jsonformer-0.9.0/jsonformer/logits_processors.py
+-rw-r--r--   0        0        0     7379 2023-05-04 18:08:31.435417 jsonformer-0.9.0/jsonformer/main.py
+-rw-r--r--   0        0        0      476 2023-05-04 18:06:00.649512 jsonformer-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3492 1970-01-01 00:00:00.000000 jsonformer-0.9.0/setup.py
+-rw-r--r--   0        0        0     3306 1970-01-01 00:00:00.000000 jsonformer-0.9.0/PKG-INFO
```

### Comparing `jsonformer-0.8.0/README.md` & `jsonformer-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             "type": "array",
             "items": {"type": "string"}
         }
     }
 }
 
 prompt = "Generate a person's information based on the following schema:"
-jsonformer = Jsonformer(model, tokenizer, json_schema, prompt, device="cuda")
+jsonformer = Jsonformer(model, tokenizer, json_schema, prompt)
 generated_data = jsonformer()
 
 print(generated_data)
 ```
 
 ## Features
```

### Comparing `jsonformer-0.8.0/jsonformer/example.py` & `jsonformer-0.9.0/jsonformer/example.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,16 +34,14 @@
 
 
 builder = Jsonformer(
     model=model,
     tokenizer=tokenizer,
     json_schema=weather_schema,
     prompt="generate the weather",
-    debug=True,
-    device="cuda",
 )
 
 print("Generating...")
 output = builder()
 
 highlight_values(
     output,
```

### Comparing `jsonformer-0.8.0/jsonformer/format.py` & `jsonformer-0.9.0/jsonformer/format.py`

 * *Files identical despite different names*

### Comparing `jsonformer-0.8.0/jsonformer/logits_processors.py` & `jsonformer-0.9.0/jsonformer/logits_processors.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,67 @@
+from typing import List
 from transformers import PreTrainedTokenizer, LogitsWarper, StoppingCriteria
 import torch
 
 
 class NumberStoppingCriteria(StoppingCriteria):
-    def __init__(self, tokenizer: PreTrainedTokenizer, precision: int = 2):
+    def __init__(
+        self,
+        tokenizer: PreTrainedTokenizer,
+        prompt_length: int,
+        precision: int = 3,
+    ):
         self.tokenizer = tokenizer
         self.precision = precision
+        self.prompt_length = prompt_length
 
     def __call__(
         self,
         input_ids: torch.LongTensor,
         scores: torch.FloatTensor,
     ) -> bool:
-        decoded = self.tokenizer.decode(input_ids[0], skip_special_tokens=True)
+        decoded = self.tokenizer.decode(
+            input_ids[0][self.prompt_length :], skip_special_tokens=True
+        )
+
         if decoded.count(".") > 1:
             return True
 
         if (
             decoded.count(".") == 1
             and len(decoded.strip().split(".")[1]) > self.precision
         ):
             return True
 
+        if (
+            len(decoded) > 1
+            and any(c.isdigit() for c in decoded)
+            and decoded[-1] in [" ", "\n"]
+        ):
+            return True
+
         return False
 
 
 class OutputNumbersTokens(LogitsWarper):
     def __init__(self, tokenizer: PreTrainedTokenizer, prompt: str):
-        self.whitelist_tokens = [
-            # tokenizer.eos_token_id
-        ]
+        self.whitelist_tokens = []
         self.tokenized_prompt = tokenizer(prompt, return_tensors="pt")
+        self.tokenizer = tokenizer
 
-        for token_str, token_id in tokenizer.get_vocab().items():
-            if (
-                (
-                    token_str.startswith("Ġ")
-                    and (
-                        all(c.isdigit() or c == "." for c in token_str[1:])
-                        and token_str.count(".") <= 1
-                    )
-                )
-                or (
-                    all(c.isdigit() or c == "." for c in token_str)
-                    and token_str.count(".") <= 1
-                )
-                or (
-                    token_str[-1] == " "
-                    and all(c.isdigit() or c == "." for c in token_str[:-1])
-                )
+        for _, token_id in tokenizer.get_vocab().items():
+            token_str = tokenizer.decode(token_id)
+            token_str = token_str.strip()
+
+            if token_str == "" or (
+                all(c.isdigit() or c == "." for c in token_str)
+                and token_str.count(".") <= 1
             ):
                 self.whitelist_tokens.append(token_id)
 
     def __call__(self, input_ids, scores):
         input_ids = input_ids[:, len(self.tokenized_prompt["input_ids"][0]) :]
+
         scores[
             :, [i for i in range(len(scores[0])) if i not in self.whitelist_tokens]
         ] = -float("inf")
         return scores
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jsonformer-0.8.0/jsonformer/main.py` & `jsonformer-0.9.0/jsonformer/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,64 +13,68 @@
     def __init__(
         self,
         model: PreTrainedModel,
         tokenizer: PreTrainedTokenizer,
         json_schema: Dict[str, Any],
         prompt: str,
         *,
-        device: str,
         debug: bool = False,
         max_array_length: int = 10,
         max_number_tokens: int = 6,
         temperature: float = 1.0,
         max_string_token_length: int = 10,
     ):
         self.model = model
         self.tokenizer = tokenizer
         self.json_schema = json_schema
         self.prompt = prompt
 
         self.number_logit_processor = OutputNumbersTokens(self.tokenizer, self.prompt)
-        self.number_stop_criteria = NumberStoppingCriteria(self.tokenizer, 3)
 
         self.generation_marker = "|GENERATION|"
         self.debug_on = debug
         self.max_array_length = max_array_length
 
         self.max_number_tokens = max_number_tokens
         self.temperature = temperature
         self.max_string_token_length = max_string_token_length
-        self.device = device
 
     def debug(self, *args, **kwargs):
         if self.debug_on:
             print(*args, **kwargs)
 
-    def generate_number(self) -> float:
+    def generate_number(self, temperature: Union[float, None] = None, iterations=0):
         prompt = self.get_prompt()
         self.debug("[generate_number] prompt", prompt)
+        input_tokens = self.tokenizer.encode(prompt, return_tensors="pt").to(
+            self.model.device
+        )
         response = self.model.generate(
-            self.tokenizer.encode(prompt, return_tensors="pt").to(self.model.device),
+            input_tokens,
             max_new_tokens=self.max_number_tokens,
             num_return_sequences=1,
             logits_processor=[self.number_logit_processor],
-            stopping_criteria=[self.number_stop_criteria],
-            temperature=self.temperature,
+            stopping_criteria=[
+                NumberStoppingCriteria(self.tokenizer, len(input_tokens[0]))
+            ],
+            temperature=temperature or self.temperature,
             pad_token_id=self.tokenizer.eos_token_id,
         )
         response = self.tokenizer.decode(response[0], skip_special_tokens=True)
         self.debug("[generate_number] response", response)
         response = response[len(prompt) :]
         response = response.strip().rstrip(".")
 
         try:
             return float(response)
         except ValueError:
-            print("ValueError")
-            return
+            if iterations > 3:
+                raise ValueError("Failed to generate a valid number")
+
+            return self.generate_number(temperature=self.temperature * 1.3)
 
     def generate_boolean(self) -> bool:
         prompt = self.get_prompt()
         self.debug("[generate_boolean] prompt", prompt)
 
         input_tensor = self.tokenizer.encode(prompt, return_tensors="pt")
         output = self.model.forward(input_tensor.to(self.model.device))
```

### Comparing `jsonformer-0.8.0/setup.py` & `jsonformer-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['termcolor>=2.3.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'jsonformer',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': '',
-    'long_description': '# Jsonformer: A Bulletproof Way to Generate Structured JSON from Language Models.\n\n### Problem: Getting models to output structured JSON is hard\n\n### Solution: Only generate the content tokens and fill in the fixed tokens\n\n[![colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/1rgs/jsonformer/blob/main/Jsonformer_example.ipynb)\n\n![cover](img/cover4.png)\n\nGenerating structured JSON from language models is a challenging task. The\ngenerated JSON must be syntactically correct, and it must conform to a schema\nthat specifies the structure of the JSON.\n\nCurrent approaches to this problem are brittle and error-prone. They rely on prompt engineering, fine-tuning, and post-processing, but they still fail to generate syntactically correct JSON in many cases.\n\nJsonformer is a new approach to this problem. In structured data, many tokens are fixed and predictable. Jsonformer is a wrapper around HuggingFace models that fills in the fixed tokens during the generation process, and only delegates the generation of content tokens to the language model. This makes it more efficient and bulletproof than existing approaches.\n\nThis currently supports a subset of JSON Schema. Below is a list of the supported schema types:\n\n- number\n- boolean\n- string\n- array\n- object\n\n## Example\n\n```python\nfrom jsonformer import Jsonformer\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\n\nmodel = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-12b")\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\njson_schema = {\n    "type": "object",\n    "properties": {\n        "name": {"type": "string"},\n        "age": {"type": "number"},\n        "is_student": {"type": "boolean"},\n        "courses": {\n            "type": "array",\n            "items": {"type": "string"}\n        }\n    }\n}\n\nprompt = "Generate a person\'s information based on the following schema:"\njsonformer = Jsonformer(model, tokenizer, json_schema, prompt, device="cuda")\ngenerated_data = jsonformer()\n\nprint(generated_data)\n```\n\n## Features\n\n- Bulletproof JSON generation: Jsonformer ensures that the generated JSON is always syntactically correct and conforms to the specified schema.\n- Efficiency: By generating only the content tokens and filling in the fixed tokens, Jsonformer is more efficient than generating a full JSON string and parsing it.\n- Flexible and extendable: Jsonformer is built on top of the HuggingFace transformers library, making it compatible with any model that supports the HuggingFace interface.\n\n## Installation\n\n```bash\npip install jsonformer\n```\n\n## License\n\nJsonformer is released under the MIT License. You are free to use, modify, and distribute this software for any purpose, commercial or non-commercial, as long as the original copyright and license notice are included.\n',
+    'long_description': '# Jsonformer: A Bulletproof Way to Generate Structured JSON from Language Models.\n\n### Problem: Getting models to output structured JSON is hard\n\n### Solution: Only generate the content tokens and fill in the fixed tokens\n\n[![colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/1rgs/jsonformer/blob/main/Jsonformer_example.ipynb)\n\n![cover](img/cover4.png)\n\nGenerating structured JSON from language models is a challenging task. The\ngenerated JSON must be syntactically correct, and it must conform to a schema\nthat specifies the structure of the JSON.\n\nCurrent approaches to this problem are brittle and error-prone. They rely on prompt engineering, fine-tuning, and post-processing, but they still fail to generate syntactically correct JSON in many cases.\n\nJsonformer is a new approach to this problem. In structured data, many tokens are fixed and predictable. Jsonformer is a wrapper around HuggingFace models that fills in the fixed tokens during the generation process, and only delegates the generation of content tokens to the language model. This makes it more efficient and bulletproof than existing approaches.\n\nThis currently supports a subset of JSON Schema. Below is a list of the supported schema types:\n\n- number\n- boolean\n- string\n- array\n- object\n\n## Example\n\n```python\nfrom jsonformer import Jsonformer\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\n\nmodel = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-12b")\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\njson_schema = {\n    "type": "object",\n    "properties": {\n        "name": {"type": "string"},\n        "age": {"type": "number"},\n        "is_student": {"type": "boolean"},\n        "courses": {\n            "type": "array",\n            "items": {"type": "string"}\n        }\n    }\n}\n\nprompt = "Generate a person\'s information based on the following schema:"\njsonformer = Jsonformer(model, tokenizer, json_schema, prompt)\ngenerated_data = jsonformer()\n\nprint(generated_data)\n```\n\n## Features\n\n- Bulletproof JSON generation: Jsonformer ensures that the generated JSON is always syntactically correct and conforms to the specified schema.\n- Efficiency: By generating only the content tokens and filling in the fixed tokens, Jsonformer is more efficient than generating a full JSON string and parsing it.\n- Flexible and extendable: Jsonformer is built on top of the HuggingFace transformers library, making it compatible with any model that supports the HuggingFace interface.\n\n## Installation\n\n```bash\npip install jsonformer\n```\n\n## License\n\nJsonformer is released under the MIT License. You are free to use, modify, and distribute this software for any purpose, commercial or non-commercial, as long as the original copyright and license notice are included.\n',
     'author': '1rgs',
     'author_email': 'rgsduke@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `jsonformer-0.8.0/PKG-INFO` & `jsonformer-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonformer
-Version: 0.8.0
+Version: 0.9.0
 Summary: 
 Author: 1rgs
 Author-email: rgsduke@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -58,15 +58,15 @@
             "type": "array",
             "items": {"type": "string"}
         }
     }
 }
 
 prompt = "Generate a person's information based on the following schema:"
-jsonformer = Jsonformer(model, tokenizer, json_schema, prompt, device="cuda")
+jsonformer = Jsonformer(model, tokenizer, json_schema, prompt)
 generated_data = jsonformer()
 
 print(generated_data)
 ```
 
 ## Features
```

