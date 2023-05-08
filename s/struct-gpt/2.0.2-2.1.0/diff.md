# Comparing `tmp/struct_gpt-2.0.2.tar.gz` & `tmp/struct_gpt-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct_gpt-2.0.2.tar", last modified: Sun May  7 21:26:48 2023, max compression
+gzip compressed data, was "struct_gpt-2.1.0.tar", last modified: Mon May  8 20:07:33 2023, max compression
```

## Comparing `struct_gpt-2.0.2.tar` & `struct_gpt-2.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1076 2023-05-07 21:26:06.746005 struct_gpt-2.0.2/LICENSE
--rw-r--r--   0        0        0     3749 2023-05-07 21:26:06.746005 struct_gpt-2.0.2/README.md
--rw-r--r--   0        0        0      587 2023-05-07 21:26:48.290264 struct_gpt-2.0.2/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-07 21:26:06.750005 struct_gpt-2.0.2/struct_gpt/__init__.py
--rw-r--r--   0        0        0     3844 2023-05-07 21:26:06.750005 struct_gpt-2.0.2/struct_gpt/models.py
--rw-r--r--   0        0        0     4222 2023-05-07 21:26:06.750005 struct_gpt-2.0.2/tests/test_models.py
--rw-r--r--   0        0        0     5370 1970-01-01 00:00:00.000000 struct_gpt-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-08 20:06:52.571758 struct_gpt-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3786 2023-05-08 20:06:52.571758 struct_gpt-2.1.0/README.md
+-rw-r--r--   0        0        0      587 2023-05-08 20:07:33.344537 struct_gpt-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-08 20:06:52.571758 struct_gpt-2.1.0/struct_gpt/__init__.py
+-rw-r--r--   0        0        0     4797 2023-05-08 20:06:52.571758 struct_gpt-2.1.0/struct_gpt/models.py
+-rw-r--r--   0        0        0     5771 2023-05-08 20:06:52.571758 struct_gpt-2.1.0/tests/test_models.py
+-rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 struct_gpt-2.1.0/PKG-INFO
```

### Comparing `struct_gpt-2.0.2/LICENSE` & `struct_gpt-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.0.2/README.md` & `struct_gpt-2.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 print(
     SentimentAnalysis.from_openai(
         text="As president, I loved the beautiful scenery, but the long hike was exhausting."
     ).json(indent=2)
 )
 ```
 <details>
-<summary>outputs</summary>
+<summary><b>See Output</b></summary>
 
 ```json
 {
   "words_to_sentiment": {
     "As": {
       "sentiment": "0"
     },
@@ -129,15 +129,19 @@
 }
 ```
 
 </details>
 
 ## Improving reliability with examples
 
-`create` can accept a list of examples to guide the model and improve its accuracy. Each example is a dictionary containing an `input` and `output` key. The `input` is the user message and the `output` is the expected assistant message, which should be a valid instance of the schema serialized as a string.
+`create` can accept a list of examples to guide the model and improve its accuracy. 
+
+Each example is a dictionary containing an `input` and `output` key. 
+
+The `input` is an example input and the `output` is its expected output, which should be an instance of the model or its json string representation.
 
 In this example, we are providing the model with examples of positive and negative sentiments:
 
 ```python
 from struct_gpt import OpenAiBase
 from pydantic import Field
 
@@ -150,20 +154,21 @@
     """
 
     sentiment: str = Field(description="Either -1, 0, or 1.")
 
 
 examples = [
     {
-        "input": "this library is neat!",
-        "output": SentimentSchema(sentiment="1").json(),
+        "input": "don't touch that",
+        "output": '{"sentiment": "-1"}',
     },
     {
-        "input": "don't touch that",
-        "output": SentimentSchema(sentiment="-1").json(),
+        "input": "this library is neat!",
+        # the output can be an instance of the model
+        "output": SentimentSchema(sentiment="1"),
     },
 ]
 
 print(SentimentSchema.from_openai(content="I love pizza!", examples=examples).json())
 ```
 outputs:
 ```json
```

### Comparing `struct_gpt-2.0.2/pyproject.toml` & `struct_gpt-2.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 dev = [
     "pytest>=7.3.1",
     "coverage>=7.2.5",
 ]
 
 [project]
 name = "struct-gpt"
-version = "2.0.2"
+version = "2.1.0"
 description = "structured llm outputs"
 authors = [
     { name = "Stephan Fitzpatrick", email = "knowsuchagency@gmail.com" },
 ]
 dependencies = [
     "openai>=0.27.6",
     "pydantic>=1.10.7",
```

### Comparing `struct_gpt-2.0.2/struct_gpt/models.py` & `struct_gpt-2.1.0/struct_gpt/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import io
 import json
 import logging
+from pprint import pprint
 from typing import TypeVar, TypedDict
 
 import openai
 from pydantic import BaseModel, ValidationError
 from ruamel.yaml import YAML
 
 Model = TypeVar("Model", bound=BaseModel)
@@ -12,15 +13,15 @@
 yaml = YAML(typ="safe")
 
 logger = logging.getLogger(__name__)
 
 
 class Example(TypedDict):
     input: str
-    output: str
+    output: str | Model
 
 
 class OpenAiMixin:
     @classmethod
     def from_openai(
         cls: Model,
         temperature=0,
@@ -57,26 +58,46 @@
         # Convert the JSON schema to YAML since it takes up fewer tokens
         with io.StringIO() as fp:
             json_schema = json.loads(cls.schema_json())
             yaml.dump(json_schema, fp)
             yaml_json_schema = fp.getvalue()
 
         # Set up the system message to guide the assistant
+        directions = [
+            f"Please respond ONLY with valid json that conforms to this json_schema:",
+            yaml_json_schema,
+            "Don't include additional text other than the object. It gets deserialized with pydantic_model.parse_raw",
+        ]
+
         system_message = {
             "role": "system",
-            "content": f"Please respond ONLY with valid json that conforms to this json_schema: {yaml_json_schema}. Don't include additional text other than the object as it will be deserialized with pydantic_model.parse_raw",
+            "content": "\n".join(directions),
         }
 
         messages = [system_message]
 
         # Add examples to the messages if provided
         if examples:
             for example in examples:
-                messages.append({"role": "user", "content": example["input"]})
-                messages.append({"role": "assistant", "content": example["output"]})
+                input_ = example["input"]
+                output = example["output"]
+
+                if isinstance(output, str):
+                    try:
+                        output = cls.parse_raw(output).json()
+                    except ValidationError as e:
+                        class_name = cls.__name__
+                        raise e from ValueError(
+                            f"output ({output}) should be a json representation of {class_name} or an instance of it"
+                        )
+                else:
+                    output = output.json()
+
+                messages.append({"role": "user", "content": input_})
+                messages.append({"role": "assistant", "content": output})
 
         prompt = doc.format(**kwargs)
 
         messages.append(
             {
                 "role": "user",
                 "content": prompt,
@@ -93,18 +114,25 @@
                     messages=messages,
                     temperature=temperature,
                     model=model,
                 )["choices"][0]["message"]["content"]
                 obj = json.loads(content)
             except Exception as e:
                 last_exception = e
-                error_msg = f"json.loads error: {e}"
+                error_msg = f"{e.__class__.__name__}: {e}"
                 logger.error(error_msg)
                 messages.append(
-                    {"role": "user", "content": f"{e.__class__.__name__}: {e}"}
+                    {
+                        "role": "user",
+                        "content": (
+                            error_msg
+                            + "\n"
+                            + "note: please don't apologize. simply return the correct json object"
+                        ),
+                    }
                 )
                 attempt += 1
                 continue
 
             try:
                 return cls.parse_obj(obj)
             except ValidationError as e:
@@ -113,12 +141,13 @@
                 logger.error(error_msg)
                 messages.append(
                     {"role": "user", "content": f"{e.__class__.__name__}: {e}"}
                 )
                 attempt += 1
 
         if last_exception:
+            pprint(messages)
             raise last_exception
 
 
 class OpenAiBase(BaseModel, OpenAiMixin):
     ...
```

### Comparing `struct_gpt-2.0.2/tests/test_models.py` & `struct_gpt-2.1.0/tests/test_models.py`

 * *Files 19% similar despite different names*

```diff
@@ -35,31 +35,31 @@
     Also determine the overall sentiment of the text and who the narrator is.
     """
 
     words_to_sentiment: Mapping[str, SentimentSchema]
     overall_sentiment: SentimentSchema
     narrator: str
 
-def test_SentimentSchema_create():
+def test_SentimentSchema_from_openai():
     sentiment = SentimentSchema.from_openai(content="I love pizza!", examples=EXAMPLES)
     assert sentiment.sentiment == "1"
 
-def test_SentimentAnalysis_create():
+def test_SentimentAnalysis_from_openai():
     sentiment_analysis = SentimentAnalysis.from_openai(
         text="As president, I loved the beautiful scenery, but the long hike was exhausting.",
-        examples=EXAMPLES
     )
     assert sentiment_analysis.narrator.lower() == "president"
     assert sentiment_analysis.overall_sentiment.sentiment in ["-1", "0", "1"]
     assert all(word in sentiment_analysis.words_to_sentiment for word in ["As", "president,", "I", "loved", "the", "beautiful", "scenery,", "but", "long", "hike", "was", "exhausting."])
+    assert all(sentiment.sentiment in ["-1", "0", "1"] for sentiment in sentiment_analysis.words_to_sentiment.values())
 
 
-def test_create_with_no_examples_or_kwargs():
+def test_from_openai_with_no_examples_or_kwargs():
     with pytest.raises(AssertionError):
-        # call create without providing examples or kwargs
+        # call from_openai without providing examples or kwargs
         SentimentSchema.from_openai()
 
 def test_no_docstring_raises_exception():
     with pytest.raises(AssertionError) as e:
         OpenAiBase.from_openai(content="I love pizza!", examples=EXAMPLES)
         assert "please add a docstring" in str(e)
 
@@ -86,45 +86,76 @@
 
     mock_chat_completion.side_effect = OpenAiError("API request failed")
 
     # Act and Assert: Ensure that the OpenAI error is propagated
     with pytest.raises(OpenAiError):
         SentimentSchema.from_openai(content="I love pizza!", examples=EXAMPLES)
 
-def test_create_with_invalid_temperature_raises_exception():
+def test_from_openai_with_invalid_temperature_raises_exception():
     with pytest.raises(AssertionError):
         # temperature should be between 0 and 1
         SentimentSchema.from_openai(content="I love pizza!", examples=EXAMPLES, temperature=-1)
 
 
-def test_create_with_invalid_retries_raises_exception():
+def test_from_openai_with_invalid_retries_raises_exception():
     with pytest.raises(AssertionError):
         # retries should be a non-negative integer
         SentimentSchema.from_openai(content="I love pizza!", examples=EXAMPLES, retries=-1)
 
-def test_create_with_invalid_json():
+def test_from_openai_with_invalid_json():
     class DummyModel(BaseModel, OpenAiMixin):
         """
         Example model for testing
 
         {content}
         """
         field1: str
         field2: int
 
     # Mock the OpenAI API to return a JSON that doesn't match the model
-    with mock.patch('openai.ChatCompletion.create') as mock_create:
-        mock_create.return_value = {
+    with mock.patch('openai.ChatCompletion.create') as mock_from_openai:
+        mock_from_openai.return_value = {
             "choices": [
                 {
                     "message": {
                         "content": json.dumps({
                             "field1": "valid string",  # this is valid
                             "field2": "invalid string",  # this should be an int
                         })
                     }
                 }
             ]
         }
 
         with pytest.raises(ValidationError):
             DummyModel.from_openai(content="")
+
+class TestExamplesHandling:
+
+    class TestSchema(OpenAiBase):
+        """what is this person's first name? {full_name}"""
+        first_name: str
+
+    example_input = "Sam Stevens"
+
+    def test_valid_stringified_json(self):
+        examples = [{"input": self.example_input, "output": '{"first_name": "Sam"}'}]
+        instance = self.TestSchema.from_openai(full_name="Alex Boss", examples=examples)
+        assert instance.first_name == "Alex"
+
+    def test_non_apology(self):
+        """
+        Test that the model doesn't prefix failed attempts to return json with some version of 'I apologize...'
+        """
+        examples = [{"input": self.example_input, "output": '{"first_name": "Sam"}'}]
+        self.TestSchema.from_openai(full_name=self.example_input, examples=examples)
+
+    def test_valid_instance(self):
+        examples = [{"input": self.example_input, "output": self.TestSchema(first_name="Sam")}]
+        instance = self.TestSchema.from_openai(full_name="Alex Boss", examples=examples)
+        assert instance.first_name == "Alex"
+
+    def test_invalid_stringified_json(self):
+        examples = [{"input": self.example_input, "output": 'not valid json'}]
+        with pytest.raises(ValueError) as e:
+            self.TestSchema.from_openai(examples=examples)
+            assert "output (not valid json) should be a json representation of TestSchema or an instance of it" in str(e.value)
```

### Comparing `struct_gpt-2.0.2/PKG-INFO` & `struct_gpt-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-gpt
-Version: 2.0.2
+Version: 2.1.0
 Summary: structured llm outputs
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Stephan Fitzpatrick
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -109,15 +109,15 @@
 print(
     SentimentAnalysis.from_openai(
         text="As president, I loved the beautiful scenery, but the long hike was exhausting."
     ).json(indent=2)
 )
 ```
 <details>
-<summary>outputs</summary>
+<summary><b>See Output</b></summary>
 
 ```json
 {
   "words_to_sentiment": {
     "As": {
       "sentiment": "0"
     },
@@ -162,15 +162,19 @@
 }
 ```
 
 </details>
 
 ## Improving reliability with examples
 
-`create` can accept a list of examples to guide the model and improve its accuracy. Each example is a dictionary containing an `input` and `output` key. The `input` is the user message and the `output` is the expected assistant message, which should be a valid instance of the schema serialized as a string.
+`create` can accept a list of examples to guide the model and improve its accuracy. 
+
+Each example is a dictionary containing an `input` and `output` key. 
+
+The `input` is an example input and the `output` is its expected output, which should be an instance of the model or its json string representation.
 
 In this example, we are providing the model with examples of positive and negative sentiments:
 
 ```python
 from struct_gpt import OpenAiBase
 from pydantic import Field
 
@@ -183,20 +187,21 @@
     """
 
     sentiment: str = Field(description="Either -1, 0, or 1.")
 
 
 examples = [
     {
-        "input": "this library is neat!",
-        "output": SentimentSchema(sentiment="1").json(),
+        "input": "don't touch that",
+        "output": '{"sentiment": "-1"}',
     },
     {
-        "input": "don't touch that",
-        "output": SentimentSchema(sentiment="-1").json(),
+        "input": "this library is neat!",
+        # the output can be an instance of the model
+        "output": SentimentSchema(sentiment="1"),
     },
 ]
 
 print(SentimentSchema.from_openai(content="I love pizza!", examples=examples).json())
 ```
 outputs:
 ```json
```

