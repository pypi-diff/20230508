# Comparing `tmp/anthropic-0.2.7.tar.gz` & `tmp/anthropic-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anthropic-0.2.7.tar", last modified: Sat Apr 15 03:43:38 2023, max compression
+gzip compressed data, was "anthropic-0.2.8.tar", last modified: Mon May  8 20:08:00 2023, max compression
```

## Comparing `anthropic-0.2.7.tar` & `anthropic-0.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:43:38.597907 anthropic-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-15 03:43:29.000000 anthropic-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-15 03:43:38.593907 anthropic-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-15 03:43:29.000000 anthropic-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:43:38.593907 anthropic-0.2.7/anthropic/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-15 03:43:29.000000 anthropic-0.2.7/anthropic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-04-15 03:43:29.000000 anthropic-0.2.7/anthropic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-15 03:43:29.000000 anthropic-0.2.7/anthropic/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-15 03:43:29.000000 anthropic-0.2.7/anthropic/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:43:38.593907 anthropic-0.2.7/anthropic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-15 03:43:38.000000 anthropic-0.2.7/anthropic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-15 03:43:38.000000 anthropic-0.2.7/anthropic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 03:43:38.000000 anthropic-0.2.7/anthropic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-15 03:43:38.000000 anthropic-0.2.7/anthropic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 03:43:38.000000 anthropic-0.2.7/anthropic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-15 03:43:29.000000 anthropic-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 03:43:38.597907 anthropic-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:43:38.593907 anthropic-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-15 03:43:29.000000 anthropic-0.2.7/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:08:00.603917 anthropic-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-08 20:07:49.000000 anthropic-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-08 20:08:00.603917 anthropic-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-08 20:07:49.000000 anthropic-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:08:00.603917 anthropic-0.2.8/anthropic/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-08 20:07:49.000000 anthropic-0.2.8/anthropic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-05-08 20:07:49.000000 anthropic-0.2.8/anthropic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-08 20:07:49.000000 anthropic-0.2.8/anthropic/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-08 20:07:49.000000 anthropic-0.2.8/anthropic/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:08:00.603917 anthropic-0.2.8/anthropic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-08 20:08:00.000000 anthropic-0.2.8/anthropic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-08 20:08:00.000000 anthropic-0.2.8/anthropic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:08:00.000000 anthropic-0.2.8/anthropic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-08 20:08:00.000000 anthropic-0.2.8/anthropic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 20:08:00.000000 anthropic-0.2.8/anthropic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-08 20:07:49.000000 anthropic-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:08:00.603917 anthropic-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:08:00.603917 anthropic-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-08 20:07:49.000000 anthropic-0.2.8/tests/test_api.py
```

### Comparing `anthropic-0.2.7/LICENSE` & `anthropic-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `anthropic-0.2.7/PKG-INFO` & `anthropic-0.2.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anthropic
-Version: 0.2.7
+Version: 0.2.8
 Summary: Library for accessing the anthropic API
 Author: Anthropic
 License: MIT
 Project-URL: homepage, https://github.com/anthropics/anthropic-sdk-python
 Project-URL: repository, https://github.com/anthropics/anthropic-sdk-python.git
 Keywords: anthropic,anthropicai
 Classifier: Programming Language :: Python :: 3
@@ -19,14 +19,26 @@
 
 This python repo provides access to Anthropic's safety-first language model APIs.
 
 For more information on our APIs, please check out [Anthropic's documentation](https://console.anthropic.com/docs).
 
 ## How to use
 
+Install the package with:
+```
+pip install anthropic
+```
+Then write code with:
+```
+import anthropic
+client = anthropic.Client(api_key=<insert token here>)
+client.XXX # look to examples/ directory for code demonstrations
+```
+
+## How to develop and run the examples in this repo
 ```
 pip install .
 export ANTHROPIC_API_KEY=<insert token here>
 python examples/basic_sync.py
 python examples/basic_stream.py
 python examples/count_tokens.py
 ```
```

### Comparing `anthropic-0.2.7/anthropic/api.py` & `anthropic-0.2.8/anthropic/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import logging
 import requests
 import requests.adapters
 import urllib.parse
 import json
 
 from . import constants
-from . import tokenizer
 
 
 class ApiException(Exception):
     pass
 
 
 class Request(NamedTuple):
@@ -266,22 +265,7 @@
         )
     if constants.AI_PROMPT not in prompt:
         raise ApiException(
             f"Prompt must contain anthropic.AI_PROMPT ({repr(constants.AI_PROMPT)})"
         )
     if prompt.endswith(" "):
         raise ApiException(f"Prompt must not end with a space character")
-    _validate_prompt_length(params)
-
-
-def _validate_prompt_length(params: dict) -> None:
-    prompt: str = params["prompt"]
-    try:
-        prompt_tokens = tokenizer.count_tokens(prompt)
-        max_tokens_to_sample: int = params["max_tokens_to_sample"]
-        token_limit = 9 * 1024
-        if prompt_tokens + max_tokens_to_sample > token_limit:
-            raise ApiException(
-                f"Prompt tokens ({prompt_tokens}) + max-sampled tokens ({max_tokens_to_sample}) exceeds max ({token_limit})",
-            )
-    except tokenizer.TokenizerException as e:
-        logging.warning(f"Cannot guarantee proper prompt lengths, because failed to use tokenizer: {e}")
```

### Comparing `anthropic-0.2.7/anthropic/tokenizer.py` & `anthropic-0.2.8/anthropic/tokenizer.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.2.7/anthropic.egg-info/PKG-INFO` & `anthropic-0.2.8/anthropic.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anthropic
-Version: 0.2.7
+Version: 0.2.8
 Summary: Library for accessing the anthropic API
 Author: Anthropic
 License: MIT
 Project-URL: homepage, https://github.com/anthropics/anthropic-sdk-python
 Project-URL: repository, https://github.com/anthropics/anthropic-sdk-python.git
 Keywords: anthropic,anthropicai
 Classifier: Programming Language :: Python :: 3
@@ -19,14 +19,26 @@
 
 This python repo provides access to Anthropic's safety-first language model APIs.
 
 For more information on our APIs, please check out [Anthropic's documentation](https://console.anthropic.com/docs).
 
 ## How to use
 
+Install the package with:
+```
+pip install anthropic
+```
+Then write code with:
+```
+import anthropic
+client = anthropic.Client(api_key=<insert token here>)
+client.XXX # look to examples/ directory for code demonstrations
+```
+
+## How to develop and run the examples in this repo
 ```
 pip install .
 export ANTHROPIC_API_KEY=<insert token here>
 python examples/basic_sync.py
 python examples/basic_stream.py
 python examples/count_tokens.py
 ```
```

### Comparing `anthropic-0.2.7/pyproject.toml` & `anthropic-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
   "setuptools >= 61.0.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "anthropic"
-version = "0.2.7"
+version = "0.2.8"
 description = "Library for accessing the anthropic API"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["anthropic", "anthropicai"]
 license = {text = "MIT"}
 authors = [
     {name = "Anthropic"}
```

### Comparing `anthropic-0.2.7/tests/test_api.py` & `anthropic-0.2.8/tests/test_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,14 @@
 import pytest
 import anthropic
-from anthropic import api, ApiException, tokenizer
-import os
+from anthropic import api, ApiException
 
 def test_prompt_validator():
     # No exceptions expected
     api._validate_request({"max_tokens_to_sample": 1, "prompt": f"{anthropic.HUMAN_PROMPT} Hello{anthropic.AI_PROMPT}"})
     api._validate_request({"max_tokens_to_sample": 1, "prompt": f"{anthropic.HUMAN_PROMPT} Hello{anthropic.AI_PROMPT} First answer{anthropic.HUMAN_PROMPT} Try again{anthropic.AI_PROMPT}"})
     with pytest.raises(ApiException):
         api._validate_request({"max_tokens_to_sample": 1, "prompt": f"{anthropic.HUMAN_PROMPT} Hello"})
     with pytest.raises(ApiException):
         api._validate_request({"max_tokens_to_sample": 1, "prompt": f"{anthropic.AI_PROMPT} "})
     with pytest.raises(ApiException):
         api._validate_request({"max_tokens_to_sample": 1, "prompt": f"Human: Hello{anthropic.AI_PROMPT}"})
-
-def test_sample_length():
-    # No exceptions expected
-    good_request = {"max_tokens_to_sample": 1, "prompt": f"{anthropic.HUMAN_PROMPT} Hello{anthropic.AI_PROMPT}"}
-    api._validate_request(good_request)
-    bad_request = good_request.copy()
-    bad_request["max_tokens_to_sample"] = 10000
-    with pytest.raises(ApiException):
-        api._validate_request(bad_request)
-
-    bad_request = good_request.copy()
-    bad_request["prompt"] = bad_request["prompt"] * 2000
-    with pytest.raises(ApiException):
-        api._validate_request(bad_request)
-
-def test_prompt_validator_fail(monkeypatch):
-    # Ensure we don't have any tokenizer loaded or saved
-    monkeypatch.setattr(tokenizer, "CLAUDE_TOKENIZER_REMOTE_FILE", tokenizer.CLAUDE_TOKENIZER_REMOTE_FILE + '-but-nonexistent')
-    tokenizer.claude_tokenizer = None
-    os.remove(tokenizer._get_tokenizer_filename())
-    # Now verify a good request fails open
-    api._validate_prompt_length({"max_tokens_to_sample": 1, "prompt": f"{anthropic.HUMAN_PROMPT} Hello{anthropic.AI_PROMPT}"})
-    # And now verify a bad request fails open too
-    api._validate_prompt_length({"max_tokens_to_sample": 100000, "prompt": f"{anthropic.HUMAN_PROMPT} Hello{anthropic.AI_PROMPT}"})
-
```

