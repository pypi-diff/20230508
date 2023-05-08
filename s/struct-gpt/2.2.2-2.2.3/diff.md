# Comparing `tmp/struct_gpt-2.2.2.tar.gz` & `tmp/struct_gpt-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct_gpt-2.2.2.tar", last modified: Mon May  8 20:46:55 2023, max compression
+gzip compressed data, was "struct_gpt-2.2.3.tar", last modified: Mon May  8 20:51:05 2023, max compression
```

## Comparing `struct_gpt-2.2.2.tar` & `struct_gpt-2.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1076 2023-05-08 20:46:16.710748 struct_gpt-2.2.2/LICENSE
--rw-r--r--   0        0        0     3843 2023-05-08 20:46:16.710748 struct_gpt-2.2.2/README.md
--rw-r--r--   0        0        0      587 2023-05-08 20:46:55.634556 struct_gpt-2.2.2/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-08 20:46:16.710748 struct_gpt-2.2.2/struct_gpt/__init__.py
--rw-r--r--   0        0        0     4909 2023-05-08 20:46:16.710748 struct_gpt-2.2.2/struct_gpt/models.py
--rw-r--r--   0        0        0     6096 2023-05-08 20:46:16.710748 struct_gpt-2.2.2/tests/test_models.py
--rw-r--r--   0        0        0     5464 1970-01-01 00:00:00.000000 struct_gpt-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-08 20:50:17.866519 struct_gpt-2.2.3/LICENSE
+-rw-r--r--   0        0        0     3721 2023-05-08 20:50:17.866519 struct_gpt-2.2.3/README.md
+-rw-r--r--   0        0        0      587 2023-05-08 20:51:05.350761 struct_gpt-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-08 20:50:17.870519 struct_gpt-2.2.3/struct_gpt/__init__.py
+-rw-r--r--   0        0        0     4909 2023-05-08 20:50:17.870519 struct_gpt-2.2.3/struct_gpt/models.py
+-rw-r--r--   0        0        0     6096 2023-05-08 20:50:17.870519 struct_gpt-2.2.3/tests/test_models.py
+-rw-r--r--   0        0        0     5342 1970-01-01 00:00:00.000000 struct_gpt-2.2.3/PKG-INFO
```

### Comparing `struct_gpt-2.2.2/LICENSE` & `struct_gpt-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.2.2/README.md` & `struct_gpt-2.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,14 @@
 # struct-gpt
 
-
 [![codecov](https://codecov.io/gh/knowsuchagency/struct-gpt/branch/main/graph/badge.svg?token=TMUQNTCTDI)](https://codecov.io/gh/knowsuchagency/struct-gpt)
 ![PyPI](https://img.shields.io/pypi/v/struct-gpt)
 
-## Features
-
-* Easy creation of custom models using the OpenAI API
-* Integration with Pydantic for model validation and serialization
-* Flexible configuration with retries and temperature settings
-
-## Usage
-
-`pip install struct-gpt`
-
----
 
-Template variables in the class' docstring are replaced with the keyword arguments passed to `from_openai`.
+Get structured output from LLM's.
 
 ```python
 from struct_gpt import OpenAiBase
 from pydantic import Field
 
 
 class SentimentSchema(OpenAiBase):
@@ -41,17 +29,30 @@
 outputs:
 ```json
 {
   "sentiment": "1"
 }
 ```
 
-Classes can reference one another. 
+## Features
 
-You can also use the `OpenAiMixin` to add functionality to existing Pydantic classes.
+* Easy creation of custom models using the OpenAI API
+* Integration with Pydantic for model validation and serialization
+* Flexible configuration with retries and temperature settings
+
+## Installation
+
+`pip install struct-gpt`
+
+
+## Usage
+
+* Template variables in the class' docstring are replaced with the keyword arguments passed to `from_openai`
+* Classes can reference one another
+* You can use the `OpenAiMixin` to add functionality to existing Pydantic classes
 
 ```python
 from struct_gpt import OpenAiBase, OpenAiMixin
 from pydantic import Field, BaseModel
 from typing import Mapping
 
 
@@ -131,23 +132,21 @@
   },
   "narrator": "president"
 }
 ```
 
 </details>
 
-## Improving reliability with examples
+### Improving reliability with examples
 
 `create` can accept a list of examples to guide the model and improve its accuracy. 
 
 Each example is a dictionary containing an `input` and `output` key. 
 
-The `input` is an example input and the `output` is its expected output, which should be an instance of the model, a dictionary, or its json string representation,.
-
-In this example, we are providing the model with examples of positive and negative sentiments:
+`output` should be an instance of the model, a dictionary, or its json string representation,.
 
 ```python
 from struct_gpt import OpenAiBase
 from pydantic import Field
 
 
 class SentimentSchema(OpenAiBase):
```

### Comparing `struct_gpt-2.2.2/pyproject.toml` & `struct_gpt-2.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 dev = [
     "pytest>=7.3.1",
     "coverage>=7.2.5",
 ]
 
 [project]
 name = "struct-gpt"
-version = "2.2.2"
+version = "2.2.3"
 description = "structured llm outputs"
 authors = [
     { name = "Stephan Fitzpatrick", email = "knowsuchagency@gmail.com" },
 ]
 dependencies = [
     "openai>=0.27.6",
     "pydantic>=1.10.7",
```

### Comparing `struct_gpt-2.2.2/struct_gpt/models.py` & `struct_gpt-2.2.3/struct_gpt/models.py`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.2.2/tests/test_models.py` & `struct_gpt-2.2.3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.2.2/PKG-INFO` & `struct_gpt-2.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-gpt
-Version: 2.2.2
+Version: 2.2.3
 Summary: structured llm outputs
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Stephan Fitzpatrick
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,31 +29,19 @@
 Requires-Dist: openai>=0.27.6
 Requires-Dist: pydantic>=1.10.7
 Requires-Dist: ruamel-yaml>=0.17.24
 Description-Content-Type: text/markdown
 
 # struct-gpt
 
-
 [![codecov](https://codecov.io/gh/knowsuchagency/struct-gpt/branch/main/graph/badge.svg?token=TMUQNTCTDI)](https://codecov.io/gh/knowsuchagency/struct-gpt)
 ![PyPI](https://img.shields.io/pypi/v/struct-gpt)
 
-## Features
-
-* Easy creation of custom models using the OpenAI API
-* Integration with Pydantic for model validation and serialization
-* Flexible configuration with retries and temperature settings
-
-## Usage
-
-`pip install struct-gpt`
-
----
 
-Template variables in the class' docstring are replaced with the keyword arguments passed to `from_openai`.
+Get structured output from LLM's.
 
 ```python
 from struct_gpt import OpenAiBase
 from pydantic import Field
 
 
 class SentimentSchema(OpenAiBase):
@@ -74,17 +62,30 @@
 outputs:
 ```json
 {
   "sentiment": "1"
 }
 ```
 
-Classes can reference one another. 
+## Features
 
-You can also use the `OpenAiMixin` to add functionality to existing Pydantic classes.
+* Easy creation of custom models using the OpenAI API
+* Integration with Pydantic for model validation and serialization
+* Flexible configuration with retries and temperature settings
+
+## Installation
+
+`pip install struct-gpt`
+
+
+## Usage
+
+* Template variables in the class' docstring are replaced with the keyword arguments passed to `from_openai`
+* Classes can reference one another
+* You can use the `OpenAiMixin` to add functionality to existing Pydantic classes
 
 ```python
 from struct_gpt import OpenAiBase, OpenAiMixin
 from pydantic import Field, BaseModel
 from typing import Mapping
 
 
@@ -164,23 +165,21 @@
   },
   "narrator": "president"
 }
 ```
 
 </details>
 
-## Improving reliability with examples
+### Improving reliability with examples
 
 `create` can accept a list of examples to guide the model and improve its accuracy. 
 
 Each example is a dictionary containing an `input` and `output` key. 
 
-The `input` is an example input and the `output` is its expected output, which should be an instance of the model, a dictionary, or its json string representation,.
-
-In this example, we are providing the model with examples of positive and negative sentiments:
+`output` should be an instance of the model, a dictionary, or its json string representation,.
 
 ```python
 from struct_gpt import OpenAiBase
 from pydantic import Field
 
 
 class SentimentSchema(OpenAiBase):
```

