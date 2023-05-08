# Comparing `tmp/gpt-review-0.8.0rc517.post1.tar.gz` & `tmp/gpt-review-0.8.0rc518.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.8.0rc517.post1.tar", last modified: Mon May  8 21:46:06 2023, max compression
+gzip compressed data, was "gpt-review-0.8.0rc518.post1.tar", last modified: Mon May  8 21:49:37 2023, max compression
```

## Comparing `gpt-review-0.8.0rc517.post1.tar` & `gpt-review-0.8.0rc518.post1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      336 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     2153 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4172 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1761 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1808 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/.pypirc
--rw-r--r--   0        0        0     1125 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/LICENSE
--rw-r--r--   0        0        0     3251 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/README.md
--rw-r--r--   0        0        0     3561 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/action.yml
--rw-r--r--   0        0        0      218 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/config.summary.template.yml
--rw-r--r--   0        0        0     8346 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/pyproject.toml
--rw-r--r--   0        0        0        1 2023-05-08 21:46:05.747187 gpt-review-0.8.0rc517.post1/src/gpt/__init__.py
--rw-r--r--   0        0        0      171 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/src/gpt/__main__.py
--rw-r--r--   0        0        0      366 2023-05-08 21:46:05.747187 gpt-review-0.8.0rc517.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0      171 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/src/gpt_review/__main__.py
--rw-r--r--   0        0        0    10048 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-08 21:45:58.027246 gpt-review-0.8.0rc517.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     2772 2023-05-08 21:45:58.031246 gpt-review-0.8.0rc517.post1/src/gpt_review/_git.py
--rw-r--r--   0        0        0     5738 2023-05-08 21:45:58.031246 gpt-review-0.8.0rc517.post1/src/gpt_review/_github.py
--rw-r--r--   0        0        0     1441 2023-05-08 21:45:58.031246 gpt-review-0.8.0rc517.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0     3221 2023-05-08 21:45:58.031246 gpt-review-0.8.0rc517.post1/src/gpt_review/_llama_index.py
--rw-r--r--   0        0        0      788 2023-05-08 21:45:58.031246 gpt-review-0.8.0rc517.post1/src/gpt_review/_repository.py
--rw-r--r--   0        0        0     9707 2023-05-08 21:45:58.031246 gpt-review-0.8.0rc517.post1/src/gpt_review/_review.py
--rw-r--r--   0        0        0      464 2023-05-08 21:45:58.031246 gpt-review-0.8.0rc517.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0      568 2023-05-08 21:45:58.031246 gpt-review-0.8.0rc517.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0      218 2023-05-08 21:45:58.031246 gpt-review-0.8.0rc517.post1/tests/config.summary.test.yml
--rw-r--r--   0        0        0     3124 2023-05-08 21:45:58.031246 gpt-review-0.8.0rc517.post1/tests/conftest.py
--rw-r--r--   0        0        0      639 2023-05-08 21:45:58.031246 gpt-review-0.8.0rc517.post1/tests/mock.diff
--rw-r--r--   0        0        0      462 2023-05-08 21:45:58.031246 gpt-review-0.8.0rc517.post1/tests/test_git.py
--rw-r--r--   0        0        0     1363 2023-05-08 21:45:58.031246 gpt-review-0.8.0rc517.post1/tests/test_github.py
--rw-r--r--   0        0        0     6815 2023-05-08 21:45:58.031246 gpt-review-0.8.0rc517.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0      590 2023-05-08 21:45:58.031246 gpt-review-0.8.0rc517.post1/tests/test_llama_index.py
--rw-r--r--   0        0        0     1015 2023-05-08 21:45:58.031246 gpt-review-0.8.0rc517.post1/tests/test_report.py
--rw-r--r--   0        0        0      420 2023-05-08 21:45:58.031246 gpt-review-0.8.0rc517.post1/tests/test_review.py
--rw-r--r--   0        0        0     5425 1970-01-01 00:00:00.000000 gpt-review-0.8.0rc517.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-08 21:49:30.686168 gpt-review-0.8.0rc518.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-08 21:49:30.686168 gpt-review-0.8.0rc518.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-08 21:49:30.686168 gpt-review-0.8.0rc518.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-08 21:49:30.686168 gpt-review-0.8.0rc518.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-08 21:49:30.686168 gpt-review-0.8.0rc518.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-08 21:49:30.686168 gpt-review-0.8.0rc518.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-08 21:49:30.686168 gpt-review-0.8.0rc518.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     2153 2023-05-08 21:49:30.686168 gpt-review-0.8.0rc518.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4172 2023-05-08 21:49:30.686168 gpt-review-0.8.0rc518.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-08 21:49:30.686168 gpt-review-0.8.0rc518.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1761 2023-05-08 21:49:30.686168 gpt-review-0.8.0rc518.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1808 2023-05-08 21:49:30.686168 gpt-review-0.8.0rc518.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-08 21:49:30.686168 gpt-review-0.8.0rc518.post1/.pypirc
+-rw-r--r--   0        0        0     1125 2023-05-08 21:49:30.686168 gpt-review-0.8.0rc518.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-08 21:49:30.686168 gpt-review-0.8.0rc518.post1/LICENSE
+-rw-r--r--   0        0        0     3251 2023-05-08 21:49:30.686168 gpt-review-0.8.0rc518.post1/README.md
+-rw-r--r--   0        0        0     3561 2023-05-08 21:49:30.686168 gpt-review-0.8.0rc518.post1/action.yml
+-rw-r--r--   0        0        0      218 2023-05-08 21:49:30.686168 gpt-review-0.8.0rc518.post1/config.summary.template.yml
+-rw-r--r--   0        0        0     8346 2023-05-08 21:49:30.686168 gpt-review-0.8.0rc518.post1/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-05-08 21:49:36.714258 gpt-review-0.8.0rc518.post1/src/gpt/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-08 21:49:30.686168 gpt-review-0.8.0rc518.post1/src/gpt/__main__.py
+-rw-r--r--   0        0        0      366 2023-05-08 21:49:36.714258 gpt-review-0.8.0rc518.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-08 21:49:30.690168 gpt-review-0.8.0rc518.post1/src/gpt_review/__main__.py
+-rw-r--r--   0        0        0    10080 2023-05-08 21:49:30.690168 gpt-review-0.8.0rc518.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-08 21:49:30.690168 gpt-review-0.8.0rc518.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     2772 2023-05-08 21:49:30.690168 gpt-review-0.8.0rc518.post1/src/gpt_review/_git.py
+-rw-r--r--   0        0        0     5738 2023-05-08 21:49:30.690168 gpt-review-0.8.0rc518.post1/src/gpt_review/_github.py
+-rw-r--r--   0        0        0     1441 2023-05-08 21:49:30.690168 gpt-review-0.8.0rc518.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0     3266 2023-05-08 21:49:30.690168 gpt-review-0.8.0rc518.post1/src/gpt_review/_llama_index.py
+-rw-r--r--   0        0        0      788 2023-05-08 21:49:30.690168 gpt-review-0.8.0rc518.post1/src/gpt_review/_repository.py
+-rw-r--r--   0        0        0     9707 2023-05-08 21:49:30.690168 gpt-review-0.8.0rc518.post1/src/gpt_review/_review.py
+-rw-r--r--   0        0        0      523 2023-05-08 21:49:30.690168 gpt-review-0.8.0rc518.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0      568 2023-05-08 21:49:30.690168 gpt-review-0.8.0rc518.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0      218 2023-05-08 21:49:30.690168 gpt-review-0.8.0rc518.post1/tests/config.summary.test.yml
+-rw-r--r--   0        0        0     3124 2023-05-08 21:49:30.690168 gpt-review-0.8.0rc518.post1/tests/conftest.py
+-rw-r--r--   0        0        0      639 2023-05-08 21:49:30.690168 gpt-review-0.8.0rc518.post1/tests/mock.diff
+-rw-r--r--   0        0        0      462 2023-05-08 21:49:30.690168 gpt-review-0.8.0rc518.post1/tests/test_git.py
+-rw-r--r--   0        0        0     1363 2023-05-08 21:49:30.690168 gpt-review-0.8.0rc518.post1/tests/test_github.py
+-rw-r--r--   0        0        0     6815 2023-05-08 21:49:30.690168 gpt-review-0.8.0rc518.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0      590 2023-05-08 21:49:30.690168 gpt-review-0.8.0rc518.post1/tests/test_llama_index.py
+-rw-r--r--   0        0        0     1015 2023-05-08 21:49:30.690168 gpt-review-0.8.0rc518.post1/tests/test_report.py
+-rw-r--r--   0        0        0      420 2023-05-08 21:49:30.690168 gpt-review-0.8.0rc518.post1/tests/test_review.py
+-rw-r--r--   0        0        0     5425 1970-01-01 00:00:00.000000 gpt-review-0.8.0rc518.post1/PKG-INFO
```

### Comparing `gpt-review-0.8.0rc517.post1/.devcontainer/devcontainer.json` & `gpt-review-0.8.0rc518.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.8.0rc518.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/.github/dependabot.yml` & `gpt-review-0.8.0rc518.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/.github/pull_request_template.md` & `gpt-review-0.8.0rc518.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/.github/workflows/codeql.yml` & `gpt-review-0.8.0rc518.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/.github/workflows/dependency-review.yml` & `gpt-review-0.8.0rc518.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt-review-0.8.0rc518.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/.github/workflows/python.yml` & `gpt-review-0.8.0rc518.post1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/.github/workflows/test-action.yml` & `gpt-review-0.8.0rc518.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/.gitignore` & `gpt-review-0.8.0rc518.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/.vscode/settings.json` & `gpt-review-0.8.0rc518.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/LICENSE` & `gpt-review-0.8.0rc518.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/README.md` & `gpt-review-0.8.0rc518.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/action.yml` & `gpt-review-0.8.0rc518.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/pyproject.toml` & `gpt-review-0.8.0rc518.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/src/gpt_review/_ask.py` & `gpt-review-0.8.0rc518.post1/src/gpt_review/_ask.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,16 +160,16 @@
             temperature=temperature,
             top_p=top_p,
             frequency_penalty=frequency_penalty,
             presence_penalty=presence_penalty,
         )
         return completion.choices[0].message.content  # type: ignore
     except RateLimitError as error:
-        if retry < 5:
-            logging.warning("Call to GPT failed due to rate limit, retry attempt: %s", retry)
+        if retry < C.MAX_RETRIES:
+            logging.warning("Call to GPT failed due to rate limit, retry attempt %s of %s", retry, C.MAX_RETRIES)
             time.sleep(retry * 10)
             return _call_gpt(prompt, temperature, max_tokens, top_p, frequency_penalty, presence_penalty, retry + 1)
         raise RateLimitError("Retry limit exceeded") from error
 
 
 def _get_engine(prompt: str, max_tokens: int, fast: bool = False, large: bool = False) -> str:
     """
```

### Comparing `gpt-review-0.8.0rc517.post1/src/gpt_review/_git.py` & `gpt-review-0.8.0rc518.post1/src/gpt_review/_git.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/src/gpt_review/_github.py` & `gpt-review-0.8.0rc518.post1/src/gpt_review/_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.8.0rc518.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/src/gpt_review/_llama_index.py` & `gpt-review-0.8.0rc518.post1/src/gpt_review/_llama_index.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 from langchain.chat_models import AzureChatOpenAI
 from langchain.embeddings import OpenAIEmbeddings
 from langchain.llms import AzureOpenAI
 from llama_index import GPTVectorStoreIndex, LLMPredictor, LangchainEmbedding, ServiceContext, SimpleDirectoryReader
 from llama_index.indices.base import BaseGPTIndex
 
+import gpt_review.constants as C
+
 
 def _ask_doc(question: str, files: List[str], fast: bool = False, large: bool = False) -> str:
     """
     Ask GPT a question.
     Args:
         question (List[str]): The question to ask.
         files (List[str]): The files to search.
@@ -50,15 +52,15 @@
         deployment_name=llm_name,
         model_kwargs={
             "api_key": openai.api_key,
             "api_base": openai.api_base,
             "api_type": "azure",
             "api_version": "2023-03-15-preview",
         },
-        max_retries=10,
+        max_retries=C.MAX_RETRIES,
     )
 
     llm_predictor = LLMPredictor(llm=llm)
 
     embedding_llm = LangchainEmbedding(
         OpenAIEmbeddings(
             model="text-embedding-ada-002",
```

### Comparing `gpt-review-0.8.0rc517.post1/src/gpt_review/_repository.py` & `gpt-review-0.8.0rc518.post1/src/gpt_review/_repository.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/src/gpt_review/_review.py` & `gpt-review-0.8.0rc518.post1/src/gpt_review/_review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/src/gpt_review/main.py` & `gpt-review-0.8.0rc518.post1/src/gpt_review/main.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/tests/conftest.py` & `gpt-review-0.8.0rc518.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/tests/mock.diff` & `gpt-review-0.8.0rc518.post1/tests/mock.diff`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/tests/test_github.py` & `gpt-review-0.8.0rc518.post1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/tests/test_gpt_cli.py` & `gpt-review-0.8.0rc518.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/tests/test_llama_index.py` & `gpt-review-0.8.0rc518.post1/tests/test_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/tests/test_report.py` & `gpt-review-0.8.0rc518.post1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc517.post1/PKG-INFO` & `gpt-review-0.8.0rc518.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.8.0rc517.post1
+Version: 0.8.0rc518.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gpt-review Version: 0.8.0rc517.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.8.0rc518.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.8.1 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

