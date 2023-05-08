# Comparing `tmp/journal-prompts-0.1.4.tar.gz` & `tmp/journal-prompts-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "journal-prompts-0.1.4.tar", max compression
+gzip compressed data, was "journal-prompts-0.1.6.tar", max compression
```

## Comparing `journal-prompts-0.1.4.tar` & `journal-prompts-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      486 2022-09-15 00:22:49.161967 journal-prompts-0.1.4/journal_prompts/__init__.py
--rw-r--r--   0        0        0      168 2022-09-15 00:21:39.628966 journal-prompts-0.1.4/journal_prompts/dto/__init__.py
--rw-r--r--   0        0        0    43344 2022-09-14 23:36:05.672467 journal-prompts-0.1.4/journal_prompts/dto/journal_prompts_500_kb.py
--rw-r--r--   0        0        0     9859 2022-09-15 00:21:33.652468 journal-prompts-0.1.4/journal_prompts/dto/journal_prompts_random_kb.py
--rw-r--r--   0        0        0   223969 2022-11-21 03:18:54.078845 journal-prompts-0.1.4/journal_prompts/dto/random_questions_kb.py
--rw-r--r--   0        0        0        0 2022-09-14 21:02:10.039422 journal-prompts-0.1.4/journal_prompts/svc/__init__.py
--rw-r--r--   0        0        0      830 2022-09-15 00:22:26.600468 journal-prompts-0.1.4/journal_prompts/svc/find_random_question.py
--rw-r--r--   0        0        0     1390 2022-11-21 03:11:36.876989 journal-prompts-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      612 2022-09-15 00:23:16.047967 journal-prompts-0.1.4/README.md
--rw-r--r--   0        0        0     1345 2022-11-21 03:19:55.860594 journal-prompts-0.1.4/setup.py
--rw-r--r--   0        0        0     1466 2022-11-21 03:19:55.860594 journal-prompts-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      486 2022-09-15 00:22:49.161967 journal-prompts-0.1.6/journal_prompts/__init__.py
+-rw-r--r--   0        0        0      254 2023-05-08 19:00:00.564529 journal-prompts-0.1.6/journal_prompts/dto/__init__.py
+-rw-r--r--   0        0        0    43344 2022-09-14 23:36:05.672467 journal-prompts-0.1.6/journal_prompts/dto/journal_prompts_500_kb.py
+-rw-r--r--   0        0        0     9859 2022-09-15 00:21:33.652468 journal-prompts-0.1.6/journal_prompts/dto/journal_prompts_random_kb.py
+-rw-r--r--   0        0        0   223969 2022-11-21 03:18:54.078845 journal-prompts-0.1.6/journal_prompts/dto/random_questions_kb.py
+-rw-r--r--   0        0        0     5583 2023-05-08 19:04:29.723027 journal-prompts-0.1.6/journal_prompts/dto/sarcastic_questions_kb.py
+-rw-r--r--   0        0        0        0 2022-09-14 21:02:10.039422 journal-prompts-0.1.6/journal_prompts/svc/__init__.py
+-rw-r--r--   0        0        0     1239 2023-05-08 19:01:17.877028 journal-prompts-0.1.6/journal_prompts/svc/find_random_question.py
+-rw-r--r--   0        0        0     1390 2023-05-08 19:04:55.497528 journal-prompts-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      612 2022-09-15 00:23:16.047967 journal-prompts-0.1.6/README.md
+-rw-r--r--   0        0        0     1345 2023-05-08 19:05:47.401028 journal-prompts-0.1.6/setup.py
+-rw-r--r--   0        0        0     1466 2023-05-08 19:05:47.401528 journal-prompts-0.1.6/PKG-INFO
```

### Comparing `journal-prompts-0.1.4/journal_prompts/dto/journal_prompts_500_kb.py` & `journal-prompts-0.1.6/journal_prompts/dto/journal_prompts_500_kb.py`

 * *Files identical despite different names*

### Comparing `journal-prompts-0.1.4/journal_prompts/dto/journal_prompts_random_kb.py` & `journal-prompts-0.1.6/journal_prompts/dto/journal_prompts_random_kb.py`

 * *Files identical despite different names*

### Comparing `journal-prompts-0.1.4/journal_prompts/dto/random_questions_kb.py` & `journal-prompts-0.1.6/journal_prompts/dto/random_questions_kb.py`

 * *Files identical despite different names*

### Comparing `journal-prompts-0.1.4/pyproject.toml` & `journal-prompts-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "Craig Trim <craigtrim@gmail.com>",
 ]
 
 description = "Corpus of Random Journal Prompts"
 license = "None"
 name = "journal-prompts"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.6"
 
 keywords = ["nlp", "text", "corpus", "prompts"]
 repository = "https://github.com/craigtrim/journal-prompts"
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `journal-prompts-0.1.4/README.md` & `journal-prompts-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `journal-prompts-0.1.4/setup.py` & `journal-prompts-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['baseblock']
 
 setup_kwargs = {
     'name': 'journal-prompts',
-    'version': '0.1.4',
+    'version': '0.1.6',
     'description': 'Corpus of Random Journal Prompts',
     'long_description': "# Journal Prompts\nA corpus of journal prompts with a finder facade\n\n### Usage\n```python\nfrom journal_prompts import find_random_question\n\nfind_random_question()\n```\nEach function call returns a single random question.\n\n### Results\n```\nWhat's the funniest brand name you've ever seen?\nHave you ever broken a safety rule? What was it?\nWhat's the most ridiculous warning sign you've ever seen?\nHave you ever tried to lick your elbow?\n...\nDo you believe in UFOs, and have you seen one?\n```\n\n### Corpus Size\n```python\nfrom journal_prompts import corpus_size\nassert corpus_size() == 3642\n```\n",
     'author': 'Craig Trim',
     'author_email': 'craigtrim@gmail.com',
     'maintainer': 'Craig Trim',
     'maintainer_email': 'craigtrim@gmail.com',
     'url': 'https://github.com/craigtrim/journal-prompts',
```

### Comparing `journal-prompts-0.1.4/PKG-INFO` & `journal-prompts-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: journal-prompts
-Version: 0.1.4
+Version: 0.1.6
 Summary: Corpus of Random Journal Prompts
 Home-page: https://github.com/craigtrim/journal-prompts
 License: None
 Keywords: nlp,text,corpus,prompts
 Author: Craig Trim
 Author-email: craigtrim@gmail.com
 Maintainer: Craig Trim
```

