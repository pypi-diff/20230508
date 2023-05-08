# Comparing `tmp/struct_gpt-2.1.0.tar.gz` & `tmp/struct_gpt-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct_gpt-2.1.0.tar", last modified: Mon May  8 20:07:33 2023, max compression
+gzip compressed data, was "struct_gpt-2.1.1.tar", last modified: Mon May  8 20:15:19 2023, max compression
```

## Comparing `struct_gpt-2.1.0.tar` & `struct_gpt-2.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1076 2023-05-08 20:06:52.571758 struct_gpt-2.1.0/LICENSE
--rw-r--r--   0        0        0     3786 2023-05-08 20:06:52.571758 struct_gpt-2.1.0/README.md
--rw-r--r--   0        0        0      587 2023-05-08 20:07:33.344537 struct_gpt-2.1.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-08 20:06:52.571758 struct_gpt-2.1.0/struct_gpt/__init__.py
--rw-r--r--   0        0        0     4797 2023-05-08 20:06:52.571758 struct_gpt-2.1.0/struct_gpt/models.py
--rw-r--r--   0        0        0     5771 2023-05-08 20:06:52.571758 struct_gpt-2.1.0/tests/test_models.py
--rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 struct_gpt-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-08 20:14:38.735384 struct_gpt-2.1.1/LICENSE
+-rw-r--r--   0        0        0     3721 2023-05-08 20:14:38.735384 struct_gpt-2.1.1/README.md
+-rw-r--r--   0        0        0      587 2023-05-08 20:15:19.681957 struct_gpt-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-08 20:14:38.735384 struct_gpt-2.1.1/struct_gpt/__init__.py
+-rw-r--r--   0        0        0     4797 2023-05-08 20:14:38.735384 struct_gpt-2.1.1/struct_gpt/models.py
+-rw-r--r--   0        0        0     5846 2023-05-08 20:14:38.735384 struct_gpt-2.1.1/tests/test_models.py
+-rw-r--r--   0        0        0     5342 1970-01-01 00:00:00.000000 struct_gpt-2.1.1/PKG-INFO
```

### Comparing `struct_gpt-2.1.0/LICENSE` & `struct_gpt-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.1.0/README.md` & `struct_gpt-2.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,17 @@
 outputs:
 ```json
 {
   "sentiment": "1"
 }
 ```
 
-Your classes can reference one another. You can also use the `OpenAiMixin` to add functionality to your own classes.
+Classes can reference one another. 
+
+You can also use the `OpenAiMixin` to add functionality to existing Pydantic classes.
 
 ```python
 from struct_gpt import OpenAiBase, OpenAiMixin
 from pydantic import Field, BaseModel
 from typing import Mapping
 
 
@@ -56,15 +58,14 @@
 
     {content}
     """
 
     sentiment: str = Field(description="Either -1, 0, or 1.")
 
 
-# you can use the OpenAiMixin to add functionality to your own classes
 class SentimentAnalysis(BaseModel, OpenAiMixin):
     """
     Determine the sentiment of each word in the following: {text}
 
     Also determine the overall sentiment of the text and who the narrator is.
     """
```

### Comparing `struct_gpt-2.1.0/pyproject.toml` & `struct_gpt-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 dev = [
     "pytest>=7.3.1",
     "coverage>=7.2.5",
 ]
 
 [project]
 name = "struct-gpt"
-version = "2.1.0"
+version = "2.1.1"
 description = "structured llm outputs"
 authors = [
     { name = "Stephan Fitzpatrick", email = "knowsuchagency@gmail.com" },
 ]
 dependencies = [
     "openai>=0.27.6",
     "pydantic>=1.10.7",
```

### Comparing `struct_gpt-2.1.0/struct_gpt/models.py` & `struct_gpt-2.1.1/struct_gpt/models.py`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.1.0/tests/test_models.py` & `struct_gpt-2.1.1/tests/test_models.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,140 +3,159 @@
 from unittest import mock
 
 import pytest
 from pydantic import Field, BaseModel, ValidationError
 
 from struct_gpt.models import OpenAiBase, OpenAiMixin
 
-# Test data
-EXAMPLES = [
-    {
-        "input": "this library is neat!",
-        "output": '{"sentiment": "1"}',
-    },
-    {
-        "input": "don't touch that",
-        "output": '{"sentiment": "-1"}',
-    },
-]
 
 class SentimentSchema(OpenAiBase):
     """
     Determine the sentiment of the given text:
 
     {content}
     """
 
     sentiment: str = Field(description="Either -1, 0, or 1.")
 
+
 class SentimentAnalysis(BaseModel, OpenAiMixin):
     """
     Determine the sentiment of each word in the following: {text}
 
     Also determine the overall sentiment of the text and who the narrator is.
     """
 
     words_to_sentiment: Mapping[str, SentimentSchema]
     overall_sentiment: SentimentSchema
     narrator: str
 
+
 def test_SentimentSchema_from_openai():
-    sentiment = SentimentSchema.from_openai(content="I love pizza!", examples=EXAMPLES)
+    examples = [
+        {
+            "input": "this library is neat!",
+            "output": '{"sentiment": "1"}',
+        },
+        {
+            "input": "don't touch that",
+            "output": '{"sentiment": "-1"}',
+        },
+    ]
+    sentiment = SentimentSchema.from_openai(content="I love pizza!", examples=examples)
     assert sentiment.sentiment == "1"
 
+
 def test_SentimentAnalysis_from_openai():
+    text = (
+        "As president, I loved the beautiful scenery, but the long hike was exhausting."
+    )
     sentiment_analysis = SentimentAnalysis.from_openai(
-        text="As president, I loved the beautiful scenery, but the long hike was exhausting.",
+        text=text,
     )
     assert sentiment_analysis.narrator.lower() == "president"
     assert sentiment_analysis.overall_sentiment.sentiment in ["-1", "0", "1"]
-    assert all(word in sentiment_analysis.words_to_sentiment for word in ["As", "president,", "I", "loved", "the", "beautiful", "scenery,", "but", "long", "hike", "was", "exhausting."])
-    assert all(sentiment.sentiment in ["-1", "0", "1"] for sentiment in sentiment_analysis.words_to_sentiment.values())
+    assert all(word in sentiment_analysis.words_to_sentiment for word in text.split())
+    assert all(
+        sentiment.sentiment in ["-1", "0", "1"]
+        for sentiment in sentiment_analysis.words_to_sentiment.values()
+    )
 
 
 def test_from_openai_with_no_examples_or_kwargs():
     with pytest.raises(AssertionError):
         # call from_openai without providing examples or kwargs
         SentimentSchema.from_openai()
 
+
 def test_no_docstring_raises_exception():
     with pytest.raises(AssertionError) as e:
-        OpenAiBase.from_openai(content="I love pizza!", examples=EXAMPLES)
+        OpenAiBase.from_openai(content="I love pizza!")
         assert "please add a docstring" in str(e)
 
+
 def test_incorrect_example_format_raises_exception():
     incorrect_examples = [
         {
             "input": "this library is neat!",
             # missing output key
         },
         {
             # missing input key
             "output": '{"sentiment": "1"}',
         },
     ]
 
     with pytest.raises(KeyError):
-        SentimentSchema.from_openai(content="I love pizza!", examples=incorrect_examples)
+        SentimentSchema.from_openai(
+            content="I love pizza!", examples=incorrect_examples
+        )
+
 
 @mock.patch("openai.ChatCompletion.create")
 def test_openai_api_failure_raises_exception(mock_chat_completion):
     # Arrange: Mock the OpenAI API to simulate a failure
     class OpenAiError(Exception):
         pass
 
     mock_chat_completion.side_effect = OpenAiError("API request failed")
 
     # Act and Assert: Ensure that the OpenAI error is propagated
     with pytest.raises(OpenAiError):
-        SentimentSchema.from_openai(content="I love pizza!", examples=EXAMPLES)
+        SentimentSchema.from_openai(content="I love pizza!")
+
 
 def test_from_openai_with_invalid_temperature_raises_exception():
     with pytest.raises(AssertionError):
         # temperature should be between 0 and 1
-        SentimentSchema.from_openai(content="I love pizza!", examples=EXAMPLES, temperature=-1)
+        SentimentSchema.from_openai(content="I love pizza!", temperature=-1)
 
 
 def test_from_openai_with_invalid_retries_raises_exception():
     with pytest.raises(AssertionError):
         # retries should be a non-negative integer
-        SentimentSchema.from_openai(content="I love pizza!", examples=EXAMPLES, retries=-1)
+        SentimentSchema.from_openai(content="I love pizza!", retries=-1)
+
 
 def test_from_openai_with_invalid_json():
     class DummyModel(BaseModel, OpenAiMixin):
         """
         Example model for testing
 
         {content}
         """
+
         field1: str
         field2: int
 
     # Mock the OpenAI API to return a JSON that doesn't match the model
-    with mock.patch('openai.ChatCompletion.create') as mock_from_openai:
+    with mock.patch("openai.ChatCompletion.create") as mock_from_openai:
         mock_from_openai.return_value = {
             "choices": [
                 {
                     "message": {
-                        "content": json.dumps({
-                            "field1": "valid string",  # this is valid
-                            "field2": "invalid string",  # this should be an int
-                        })
+                        "content": json.dumps(
+                            {
+                                "field1": "valid string",  # this is valid
+                                "field2": "invalid string",  # this should be an int
+                            }
+                        )
                     }
                 }
             ]
         }
 
         with pytest.raises(ValidationError):
             DummyModel.from_openai(content="")
 
-class TestExamplesHandling:
 
+class TestExamplesHandling:
     class TestSchema(OpenAiBase):
         """what is this person's first name? {full_name}"""
+
         first_name: str
 
     example_input = "Sam Stevens"
 
     def test_valid_stringified_json(self):
         examples = [{"input": self.example_input, "output": '{"first_name": "Sam"}'}]
         instance = self.TestSchema.from_openai(full_name="Alex Boss", examples=examples)
@@ -146,16 +165,21 @@
         """
         Test that the model doesn't prefix failed attempts to return json with some version of 'I apologize...'
         """
         examples = [{"input": self.example_input, "output": '{"first_name": "Sam"}'}]
         self.TestSchema.from_openai(full_name=self.example_input, examples=examples)
 
     def test_valid_instance(self):
-        examples = [{"input": self.example_input, "output": self.TestSchema(first_name="Sam")}]
+        examples = [
+            {"input": self.example_input, "output": self.TestSchema(first_name="Sam")}
+        ]
         instance = self.TestSchema.from_openai(full_name="Alex Boss", examples=examples)
         assert instance.first_name == "Alex"
 
     def test_invalid_stringified_json(self):
-        examples = [{"input": self.example_input, "output": 'not valid json'}]
+        examples = [{"input": self.example_input, "output": "not valid json"}]
         with pytest.raises(ValueError) as e:
             self.TestSchema.from_openai(examples=examples)
-            assert "output (not valid json) should be a json representation of TestSchema or an instance of it" in str(e.value)
+            assert (
+                "output (not valid json) should be a json representation of TestSchema or an instance of it"
+                in str(e.value)
+            )
```

### Comparing `struct_gpt-2.1.0/PKG-INFO` & `struct_gpt-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-gpt
-Version: 2.1.0
+Version: 2.1.1
 Summary: structured llm outputs
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Stephan Fitzpatrick
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -71,15 +71,17 @@
 outputs:
 ```json
 {
   "sentiment": "1"
 }
 ```
 
-Your classes can reference one another. You can also use the `OpenAiMixin` to add functionality to your own classes.
+Classes can reference one another. 
+
+You can also use the `OpenAiMixin` to add functionality to existing Pydantic classes.
 
 ```python
 from struct_gpt import OpenAiBase, OpenAiMixin
 from pydantic import Field, BaseModel
 from typing import Mapping
 
 
@@ -89,15 +91,14 @@
 
     {content}
     """
 
     sentiment: str = Field(description="Either -1, 0, or 1.")
 
 
-# you can use the OpenAiMixin to add functionality to your own classes
 class SentimentAnalysis(BaseModel, OpenAiMixin):
     """
     Determine the sentiment of each word in the following: {text}
 
     Also determine the overall sentiment of the text and who the narrator is.
     """
```

