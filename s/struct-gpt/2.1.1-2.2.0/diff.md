# Comparing `tmp/struct_gpt-2.1.1.tar.gz` & `tmp/struct_gpt-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct_gpt-2.1.1.tar", last modified: Mon May  8 20:15:19 2023, max compression
+gzip compressed data, was "struct_gpt-2.2.0.tar", last modified: Mon May  8 20:33:42 2023, max compression
```

## Comparing `struct_gpt-2.1.1.tar` & `struct_gpt-2.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1076 2023-05-08 20:14:38.735384 struct_gpt-2.1.1/LICENSE
--rw-r--r--   0        0        0     3721 2023-05-08 20:14:38.735384 struct_gpt-2.1.1/README.md
--rw-r--r--   0        0        0      587 2023-05-08 20:15:19.681957 struct_gpt-2.1.1/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-08 20:14:38.735384 struct_gpt-2.1.1/struct_gpt/__init__.py
--rw-r--r--   0        0        0     4797 2023-05-08 20:14:38.735384 struct_gpt-2.1.1/struct_gpt/models.py
--rw-r--r--   0        0        0     5846 2023-05-08 20:14:38.735384 struct_gpt-2.1.1/tests/test_models.py
--rw-r--r--   0        0        0     5342 1970-01-01 00:00:00.000000 struct_gpt-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-08 20:33:00.571404 struct_gpt-2.2.0/LICENSE
+-rw-r--r--   0        0        0     3773 2023-05-08 20:33:00.571404 struct_gpt-2.2.0/README.md
+-rw-r--r--   0        0        0      587 2023-05-08 20:33:42.567635 struct_gpt-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-08 20:33:00.571404 struct_gpt-2.2.0/struct_gpt/__init__.py
+-rw-r--r--   0        0        0     4909 2023-05-08 20:33:00.571404 struct_gpt-2.2.0/struct_gpt/models.py
+-rw-r--r--   0        0        0     6096 2023-05-08 20:33:00.571404 struct_gpt-2.2.0/tests/test_models.py
+-rw-r--r--   0        0        0     5394 1970-01-01 00:00:00.000000 struct_gpt-2.2.0/PKG-INFO
```

### Comparing `struct_gpt-2.1.1/LICENSE` & `struct_gpt-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.1.1/README.md` & `struct_gpt-2.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
 ## Improving reliability with examples
 
 `create` can accept a list of examples to guide the model and improve its accuracy. 
 
 Each example is a dictionary containing an `input` and `output` key. 
 
-The `input` is an example input and the `output` is its expected output, which should be an instance of the model or its json string representation.
+The `input` is an example input and the `output` is its expected output, which should be an instance of the model, a dictionary, or its json string representation,.
 
 In this example, we are providing the model with examples of positive and negative sentiments:
 
 ```python
 from struct_gpt import OpenAiBase
 from pydantic import Field
 
@@ -155,20 +155,23 @@
     """
 
     sentiment: str = Field(description="Either -1, 0, or 1.")
 
 
 examples = [
     {
+        "input": "I love the beach!",
+        "output": {"sentiment": "1"},
+    },
+    {
         "input": "don't touch that",
         "output": '{"sentiment": "-1"}',
     },
     {
         "input": "this library is neat!",
-        # the output can be an instance of the model
         "output": SentimentSchema(sentiment="1"),
     },
 ]
 
 print(SentimentSchema.from_openai(content="I love pizza!", examples=examples).json())
 ```
 outputs:
```

### Comparing `struct_gpt-2.1.1/pyproject.toml` & `struct_gpt-2.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 dev = [
     "pytest>=7.3.1",
     "coverage>=7.2.5",
 ]
 
 [project]
 name = "struct-gpt"
-version = "2.1.1"
+version = "2.2.0"
 description = "structured llm outputs"
 authors = [
     { name = "Stephan Fitzpatrick", email = "knowsuchagency@gmail.com" },
 ]
 dependencies = [
     "openai>=0.27.6",
     "pydantic>=1.10.7",
```

### Comparing `struct_gpt-2.1.1/struct_gpt/models.py` & `struct_gpt-2.2.0/struct_gpt/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 yaml = YAML(typ="safe")
 
 logger = logging.getLogger(__name__)
 
 
 class Example(TypedDict):
     input: str
-    output: str | Model
+    output: str | dict | Model
 
 
 class OpenAiMixin:
     @classmethod
     def from_openai(
         cls: Model,
         temperature=0,
@@ -85,14 +85,16 @@
                     try:
                         output = cls.parse_raw(output).json()
                     except ValidationError as e:
                         class_name = cls.__name__
                         raise e from ValueError(
                             f"output ({output}) should be a json representation of {class_name} or an instance of it"
                         )
+                elif isinstance(output, dict):
+                    output = cls.parse_obj(output).json()
                 else:
                     output = output.json()
 
                 messages.append({"role": "user", "content": input_})
                 messages.append({"role": "assistant", "content": output})
 
         prompt = doc.format(**kwargs)
```

### Comparing `struct_gpt-2.1.1/tests/test_models.py` & `struct_gpt-2.2.0/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,19 @@
     example_input = "Sam Stevens"
 
     def test_valid_stringified_json(self):
         examples = [{"input": self.example_input, "output": '{"first_name": "Sam"}'}]
         instance = self.TestSchema.from_openai(full_name="Alex Boss", examples=examples)
         assert instance.first_name == "Alex"
 
+    def test_valid_dict(self):
+        examples = [{"input": self.example_input, "output": {"first_name": "Sam"}}]
+        instance = self.TestSchema.from_openai(full_name="Alex Boss", examples=examples)
+        assert instance.first_name == "Alex"
+
     def test_non_apology(self):
         """
         Test that the model doesn't prefix failed attempts to return json with some version of 'I apologize...'
         """
         examples = [{"input": self.example_input, "output": '{"first_name": "Sam"}'}]
         self.TestSchema.from_openai(full_name=self.example_input, examples=examples)
```

### Comparing `struct_gpt-2.1.1/PKG-INFO` & `struct_gpt-2.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-gpt
-Version: 2.1.1
+Version: 2.2.0
 Summary: structured llm outputs
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Stephan Fitzpatrick
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -167,15 +167,15 @@
 
 ## Improving reliability with examples
 
 `create` can accept a list of examples to guide the model and improve its accuracy. 
 
 Each example is a dictionary containing an `input` and `output` key. 
 
-The `input` is an example input and the `output` is its expected output, which should be an instance of the model or its json string representation.
+The `input` is an example input and the `output` is its expected output, which should be an instance of the model, a dictionary, or its json string representation,.
 
 In this example, we are providing the model with examples of positive and negative sentiments:
 
 ```python
 from struct_gpt import OpenAiBase
 from pydantic import Field
 
@@ -188,20 +188,23 @@
     """
 
     sentiment: str = Field(description="Either -1, 0, or 1.")
 
 
 examples = [
     {
+        "input": "I love the beach!",
+        "output": {"sentiment": "1"},
+    },
+    {
         "input": "don't touch that",
         "output": '{"sentiment": "-1"}',
     },
     {
         "input": "this library is neat!",
-        # the output can be an instance of the model
         "output": SentimentSchema(sentiment="1"),
     },
 ]
 
 print(SentimentSchema.from_openai(content="I love pizza!", examples=examples).json())
 ```
 outputs:
```

