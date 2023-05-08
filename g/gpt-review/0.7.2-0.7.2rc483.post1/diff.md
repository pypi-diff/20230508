# Comparing `tmp/gpt-review-0.7.2.tar.gz` & `tmp/gpt-review-0.7.2rc483.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.7.2.tar", last modified: Mon May  8 19:08:11 2023, max compression
+gzip compressed data, was "gpt-review-0.7.2rc483.post1.tar", last modified: Mon May  8 17:17:20 2023, max compression
```

## Comparing `gpt-review-0.7.2.tar` & `gpt-review-0.7.2rc483.post1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      336 2023-05-08 19:08:05.704089 gpt-review-0.7.2/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-05-08 19:08:05.704089 gpt-review-0.7.2/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-08 19:08:05.704089 gpt-review-0.7.2/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-08 19:08:05.704089 gpt-review-0.7.2/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-08 19:08:05.704089 gpt-review-0.7.2/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-08 19:08:05.704089 gpt-review-0.7.2/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-08 19:08:05.704089 gpt-review-0.7.2/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     2153 2023-05-08 19:08:05.704089 gpt-review-0.7.2/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4172 2023-05-08 19:08:05.704089 gpt-review-0.7.2/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-08 19:08:05.704089 gpt-review-0.7.2/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1761 2023-05-08 19:08:05.704089 gpt-review-0.7.2/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1808 2023-05-08 19:08:05.704089 gpt-review-0.7.2/.gitignore
--rw-r--r--   0        0        0      158 2023-05-08 19:08:05.704089 gpt-review-0.7.2/.pypirc
--rw-r--r--   0        0        0     1125 2023-05-08 19:08:05.704089 gpt-review-0.7.2/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-08 19:08:05.704089 gpt-review-0.7.2/LICENSE
--rw-r--r--   0        0        0     3251 2023-05-08 19:08:05.704089 gpt-review-0.7.2/README.md
--rw-r--r--   0        0        0     3561 2023-05-08 19:08:05.704089 gpt-review-0.7.2/action.yml
--rw-r--r--   0        0        0      218 2023-05-08 19:08:05.704089 gpt-review-0.7.2/config.summary.template.yml
--rw-r--r--   0        0        0     8346 2023-05-08 19:08:05.704089 gpt-review-0.7.2/pyproject.toml
--rw-r--r--   0        0        0        1 2023-05-08 19:08:11.148137 gpt-review-0.7.2/src/gpt/__init__.py
--rw-r--r--   0        0        0      171 2023-05-08 19:08:05.704089 gpt-review-0.7.2/src/gpt/__main__.py
--rw-r--r--   0        0        0      354 2023-05-08 19:08:11.148137 gpt-review-0.7.2/src/gpt_review/__init__.py
--rw-r--r--   0        0        0      171 2023-05-08 19:08:05.704089 gpt-review-0.7.2/src/gpt_review/__main__.py
--rw-r--r--   0        0        0    10048 2023-05-08 19:08:05.704089 gpt-review-0.7.2/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-08 19:08:05.704089 gpt-review-0.7.2/src/gpt_review/_command.py
--rw-r--r--   0        0        0     1924 2023-05-08 19:08:05.704089 gpt-review-0.7.2/src/gpt_review/_git.py
--rw-r--r--   0        0        0     5738 2023-05-08 19:08:05.708089 gpt-review-0.7.2/src/gpt_review/_github.py
--rw-r--r--   0        0        0     1441 2023-05-08 19:08:05.708089 gpt-review-0.7.2/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0     3221 2023-05-08 19:08:05.708089 gpt-review-0.7.2/src/gpt_review/_llama_index.py
--rw-r--r--   0        0        0      788 2023-05-08 19:08:05.708089 gpt-review-0.7.2/src/gpt_review/_repository.py
--rw-r--r--   0        0        0     9707 2023-05-08 19:08:05.708089 gpt-review-0.7.2/src/gpt_review/_review.py
--rw-r--r--   0        0        0      464 2023-05-08 19:08:05.708089 gpt-review-0.7.2/src/gpt_review/constants.py
--rw-r--r--   0        0        0      568 2023-05-08 19:08:05.708089 gpt-review-0.7.2/src/gpt_review/main.py
--rw-r--r--   0        0        0      218 2023-05-08 19:08:05.708089 gpt-review-0.7.2/tests/config.summary.test.yml
--rw-r--r--   0        0        0     3124 2023-05-08 19:08:05.708089 gpt-review-0.7.2/tests/conftest.py
--rw-r--r--   0        0        0      639 2023-05-08 19:08:05.708089 gpt-review-0.7.2/tests/mock.diff
--rw-r--r--   0        0        0      462 2023-05-08 19:08:05.708089 gpt-review-0.7.2/tests/test_git.py
--rw-r--r--   0        0        0     1363 2023-05-08 19:08:05.708089 gpt-review-0.7.2/tests/test_github.py
--rw-r--r--   0        0        0     6707 2023-05-08 19:08:05.708089 gpt-review-0.7.2/tests/test_gpt_cli.py
--rw-r--r--   0        0        0      590 2023-05-08 19:08:05.708089 gpt-review-0.7.2/tests/test_llama_index.py
--rw-r--r--   0        0        0     1015 2023-05-08 19:08:05.708089 gpt-review-0.7.2/tests/test_report.py
--rw-r--r--   0        0        0      420 2023-05-08 19:08:05.708089 gpt-review-0.7.2/tests/test_review.py
--rw-r--r--   0        0        0     5414 1970-01-01 00:00:00.000000 gpt-review-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-08 17:17:09.192258 gpt-review-0.7.2rc483.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-08 17:17:09.192258 gpt-review-0.7.2rc483.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-08 17:17:09.192258 gpt-review-0.7.2rc483.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-08 17:17:09.192258 gpt-review-0.7.2rc483.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-08 17:17:09.192258 gpt-review-0.7.2rc483.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     2153 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4172 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1761 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1808 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/.pypirc
+-rw-r--r--   0        0        0     1125 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/LICENSE
+-rw-r--r--   0        0        0     3251 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/README.md
+-rw-r--r--   0        0        0     3561 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/action.yml
+-rw-r--r--   0        0        0      218 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/config.summary.template.yml
+-rw-r--r--   0        0        0     8346 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-05-08 17:17:19.496328 gpt-review-0.7.2rc483.post1/src/gpt/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/src/gpt/__main__.py
+-rw-r--r--   0        0        0      366 2023-05-08 17:17:19.496328 gpt-review-0.7.2rc483.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/src/gpt_review/__main__.py
+-rw-r--r--   0        0        0    10048 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     1924 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/src/gpt_review/_git.py
+-rw-r--r--   0        0        0     5738 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/src/gpt_review/_github.py
+-rw-r--r--   0        0        0     1441 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0     3221 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/src/gpt_review/_llama_index.py
+-rw-r--r--   0        0        0      788 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/src/gpt_review/_repository.py
+-rw-r--r--   0        0        0     9707 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/src/gpt_review/_review.py
+-rw-r--r--   0        0        0      464 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0      568 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0      218 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/tests/config.summary.test.yml
+-rw-r--r--   0        0        0     3124 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/tests/conftest.py
+-rw-r--r--   0        0        0      639 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/tests/mock.diff
+-rw-r--r--   0        0        0      462 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/tests/test_git.py
+-rw-r--r--   0        0        0     1363 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/tests/test_github.py
+-rw-r--r--   0        0        0     6707 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0      590 2023-05-08 17:17:09.196258 gpt-review-0.7.2rc483.post1/tests/test_llama_index.py
+-rw-r--r--   0        0        0     1015 2023-05-08 17:17:09.200258 gpt-review-0.7.2rc483.post1/tests/test_report.py
+-rw-r--r--   0        0        0      420 2023-05-08 17:17:09.200258 gpt-review-0.7.2rc483.post1/tests/test_review.py
+-rw-r--r--   0        0        0     5425 1970-01-01 00:00:00.000000 gpt-review-0.7.2rc483.post1/PKG-INFO
```

### Comparing `gpt-review-0.7.2/.devcontainer/devcontainer.json` & `gpt-review-0.7.2rc483.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.7.2rc483.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/.github/dependabot.yml` & `gpt-review-0.7.2rc483.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/.github/pull_request_template.md` & `gpt-review-0.7.2rc483.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/.github/workflows/codeql.yml` & `gpt-review-0.7.2rc483.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/.github/workflows/dependency-review.yml` & `gpt-review-0.7.2rc483.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/.github/workflows/on-push-create-draft-release.yml` & `gpt-review-0.7.2rc483.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/.github/workflows/python.yml` & `gpt-review-0.7.2rc483.post1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/.github/workflows/test-action.yml` & `gpt-review-0.7.2rc483.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/.gitignore` & `gpt-review-0.7.2rc483.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/.vscode/settings.json` & `gpt-review-0.7.2rc483.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/LICENSE` & `gpt-review-0.7.2rc483.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/README.md` & `gpt-review-0.7.2rc483.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/action.yml` & `gpt-review-0.7.2rc483.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/pyproject.toml` & `gpt-review-0.7.2rc483.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/src/gpt_review/_ask.py` & `gpt-review-0.7.2rc483.post1/src/gpt_review/_ask.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/src/gpt_review/_git.py` & `gpt-review-0.7.2rc483.post1/src/gpt_review/_git.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/src/gpt_review/_github.py` & `gpt-review-0.7.2rc483.post1/src/gpt_review/_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/src/gpt_review/_gpt_cli.py` & `gpt-review-0.7.2rc483.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/src/gpt_review/_llama_index.py` & `gpt-review-0.7.2rc483.post1/src/gpt_review/_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/src/gpt_review/_repository.py` & `gpt-review-0.7.2rc483.post1/src/gpt_review/_repository.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/src/gpt_review/_review.py` & `gpt-review-0.7.2rc483.post1/src/gpt_review/_review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/src/gpt_review/main.py` & `gpt-review-0.7.2rc483.post1/src/gpt_review/main.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/tests/conftest.py` & `gpt-review-0.7.2rc483.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/tests/mock.diff` & `gpt-review-0.7.2rc483.post1/tests/mock.diff`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/tests/test_github.py` & `gpt-review-0.7.2rc483.post1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/tests/test_gpt_cli.py` & `gpt-review-0.7.2rc483.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/tests/test_llama_index.py` & `gpt-review-0.7.2rc483.post1/tests/test_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/tests/test_report.py` & `gpt-review-0.7.2rc483.post1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.7.2/PKG-INFO` & `gpt-review-0.7.2rc483.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.7.2
+Version: 0.7.2rc483.post1
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
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: gpt-review Version: 0.7.2 Summary: Python Project
-for reviewing GitHub PRs with Open AI and Chat-GPT. Author-email: Daniel
-Ciborowski
+Metadata-Version: 2.1 Name: gpt-review Version: 0.7.2rc483.post1 Summary:
+Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
+email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.8.1 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: azure-identity Requires-Dist: azure-keyvault-
```

