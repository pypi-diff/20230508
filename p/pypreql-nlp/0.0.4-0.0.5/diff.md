# Comparing `tmp/pypreql-nlp-0.0.4.tar.gz` & `tmp/pypreql-nlp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypreql-nlp-0.0.4.tar", last modified: Sat May  6 21:50:45 2023, max compression
+gzip compressed data, was "pypreql-nlp-0.0.5.tar", last modified: Mon May  8 13:51:30 2023, max compression
```

## Comparing `pypreql-nlp-0.0.4.tar` & `pypreql-nlp-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:45.892298 pypreql-nlp-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-06 21:50:45.892298 pypreql-nlp-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:45.888298 pypreql-nlp-0.0.4/preql_nlp/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/preql_nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/preql_nlp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/preql_nlp/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/preql_nlp/monkeypatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:45.888298 pypreql-nlp-0.0.4/preql_nlp/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/preql_nlp/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/preql_nlp/prompts/final_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/preql_nlp/prompts/prompt_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/preql_nlp/prompts/query_semantic_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/preql_nlp/prompts/semantic_to_tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:45.892298 pypreql-nlp-0.0.4/pypreql_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-06 21:50:45.000000 pypreql-nlp-0.0.4/pypreql_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-06 21:50:45.000000 pypreql-nlp-0.0.4/pypreql_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 21:50:45.000000 pypreql-nlp-0.0.4/pypreql_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-06 21:50:45.000000 pypreql-nlp-0.0.4/pypreql_nlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 21:50:45.000000 pypreql-nlp-0.0.4/pypreql_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 21:50:45.892298 pypreql-nlp-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:51:30.223676 pypreql-nlp-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-08 13:51:30.223676 pypreql-nlp-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-08 13:51:18.000000 pypreql-nlp-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:51:30.223676 pypreql-nlp-0.0.5/preql_nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 13:51:18.000000 pypreql-nlp-0.0.5/preql_nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-08 13:51:18.000000 pypreql-nlp-0.0.5/preql_nlp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-05-08 13:51:18.000000 pypreql-nlp-0.0.5/preql_nlp/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-08 13:51:18.000000 pypreql-nlp-0.0.5/preql_nlp/monkeypatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:51:30.223676 pypreql-nlp-0.0.5/preql_nlp/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-08 13:51:18.000000 pypreql-nlp-0.0.5/preql_nlp/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-08 13:51:18.000000 pypreql-nlp-0.0.5/preql_nlp/prompts/final_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-08 13:51:18.000000 pypreql-nlp-0.0.5/preql_nlp/prompts/prompt_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-08 13:51:18.000000 pypreql-nlp-0.0.5/preql_nlp/prompts/query_semantic_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-08 13:51:18.000000 pypreql-nlp-0.0.5/preql_nlp/prompts/semantic_to_tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:51:30.223676 pypreql-nlp-0.0.5/pypreql_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-08 13:51:30.000000 pypreql-nlp-0.0.5/pypreql_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-08 13:51:30.000000 pypreql-nlp-0.0.5/pypreql_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:51:30.000000 pypreql-nlp-0.0.5/pypreql_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 13:51:30.000000 pypreql-nlp-0.0.5/pypreql_nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 13:51:30.000000 pypreql-nlp-0.0.5/pypreql_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-08 13:51:18.000000 pypreql-nlp-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:51:30.223676 pypreql-nlp-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-08 13:51:18.000000 pypreql-nlp-0.0.5/setup.py
```

### Comparing `pypreql-nlp-0.0.4/PKG-INFO` & `pypreql-nlp-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypreql-nlp
-Version: 0.0.4
+Version: 0.0.5
 Summary: NLP interface for pypreql.
 Home-page: 
 Author: 
 Author-email: pypreql-community@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -30,23 +30,23 @@
 ## Examples
 
 ### Basic BQ example
 
 
 ```python
 from trilogy_public_models import models
-from preql import Executor, default_engine, Dialect
+from preql import Executor, Dialects
 from preql_nlp import build_query
 
 # define the model we want to parse
 environment = models["bigquery.stack_overflow"]
 
 # set up preql executor
 # default bigquery executor requires local default credentials configured
-executor = Dialect.BIGQUERY.default_executor(environment= environment)
+executor = Dialects.BIGQUERY.default_executor(environment= environment)
 
 # build a query off text and the selected model
 processed_query = build_query(
     "How many questions are asked per year?",
     environment,
 )
```

### Comparing `pypreql-nlp-0.0.4/README.md` & `pypreql-nlp-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 ## Examples
 
 ### Basic BQ example
 
 
 ```python
 from trilogy_public_models import models
-from preql import Executor, default_engine, Dialect
+from preql import Executor, Dialects
 from preql_nlp import build_query
 
 # define the model we want to parse
 environment = models["bigquery.stack_overflow"]
 
 # set up preql executor
 # default bigquery executor requires local default credentials configured
-executor = Dialect.BIGQUERY.default_executor(environment= environment)
+executor = Dialects.BIGQUERY.default_executor(environment= environment)
 
 # build a query off text and the selected model
 processed_query = build_query(
     "How many questions are asked per year?",
     environment,
 )
```

### Comparing `pypreql-nlp-0.0.4/preql_nlp/main.py` & `pypreql-nlp-0.0.5/preql_nlp/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 from preql.core.enums import Purpose
 from typing import Iterable, List
 from collections import defaultdict
 
 from preql.core.models import Environment
 from preql_nlp.prompts import (
     run_prompt,
-    gen_extraction_prompt_v1,
-    gen_structured_prompt_v1,
-    gen_selection_v1,
+    SemanticToTokensPromptCase,
+    SelectionPromptCase,
+    SemanticExtractionPromptCase,
 )
 from preql_nlp.constants import logger, DEFAULT_LIMIT
 
 from dataclasses import dataclass
 from typing import Any
 
 import re
-
+import uuid
 
 def split_to_tokens(input_text: str) -> list[str]:
     return list(set(re.split("\.|\_", input_text)))
 
 
 def build_token_list_by_purpose(concepts, purposes: Iterable[Purpose]):
     concepts = {k: v for k, v in concepts.items() if v.purpose in purposes}
@@ -102,47 +102,51 @@
     for x in input:
         if not isinstance(x, str):
             raise ValueError("Input must be a list of dicts")
     return input
 
 
 def discover_inputs(
-    input_text: str, input_environment: Environment, debug: bool = False
+    input_text: str, input_environment: Environment, debug: bool = False, log_info: bool = True
 ) -> IntermediateParseResults:
-    # we work around promopt size issues and hallucination by doing a two phase discovery
+    # we work around prompt size issues and hallucination by doing a two phase discovery
     # first we parse the question into metrics/dimensions
     # then for each one, we match those to a token list
     # and then we deterministically map the tokens back to the most relevant concept
     # TODO: turn the third pass into a prompt
     concepts = input_environment.concepts
     debug = True
     final_concept_list = list(concepts.keys())
     metrics = build_token_list_by_purpose(concepts, (Purpose.METRIC,))
     dimensions = build_token_list_by_purpose(
         concepts, (Purpose.KEY, Purpose.PROPERTY, Purpose.CONSTANT)
     )
 
+    session_uuid = uuid.uuid4()
+
     parsed = coerce_list_dict(
-        run_prompt(gen_extraction_prompt_v1(input_text), debug=debug)
+        run_prompt(SemanticExtractionPromptCase(input_text), debug=debug, log_info=log_info, session_uuid=session_uuid)
     )[0]
     order = parsed.get("order", [])
     token_inputs = {"metrics": metrics, "dimensions": dimensions}
 
     output: List[str] = []
     for field in [
         "metrics",
         "dimensions",
     ]:
         local_phrases = [x for x in parsed[field]]
         phrase_tokens = coerce_list_dict(
             run_prompt(
-                gen_structured_prompt_v1(
+                SemanticToTokensPromptCase(
                     phrases=local_phrases, tokens=token_inputs[field]
                 ),
                 debug=True,
+                session_uuid=session_uuid,
+                log_info=log_info
             )
         )
         token_universe = []
         for mapping in phrase_tokens:
             for k, v in mapping.items():
                 token_universe += v
         for mapping in phrase_tokens:
@@ -157,15 +161,15 @@
                 if concepts:
                     output += concepts
                 else:
                     raise ValueError(
                         f"Could not find concept for input {k} with tokens {v}"
                     )
     selections = coerce_list_dict(
-        run_prompt(gen_selection_v1(concepts=output, question=input_text), debug=debug)
+        run_prompt(SelectionPromptCase(concepts=output, question=input_text), debug=debug, session_uuid=session_uuid, log_info=log_info)
     )[0]
     final = list(set(selections.get("matches", [])))
 
     return IntermediateParseResults(
         select=final, limit=parsed.get("limit", 20), order=order
     )
 
@@ -208,26 +212,29 @@
     return OrderBy(items=final)
 
 
 def parse_query(
     input_text: str,
     input_environment: Environment,
     debug: bool = False,
+    log_info: bool=True
 ):
-    results = discover_inputs(input_text, input_environment, debug=debug)
+    results = discover_inputs(input_text, input_environment, debug=debug, log_info=log_info)
     concepts = [input_environment.concepts[x] for x in results.select]
     order = parse_order(concepts, results.order)
     if debug:
         print("Concepts found")
         for c in concepts:
             print(c.address)
     query = Select(selection=concepts, limit=safe_limit(results.limit), order_by=order)
     return query
 
 
+
 def build_query(
     input_text: str,
     input_environment: Environment,
     debug: bool = False,
+    log_info: bool = True
 ) -> ProcessedQuery:
-    query = parse_query(input_text, input_environment, debug=debug)
+    query = parse_query(input_text, input_environment, debug=debug, log_info=log_info)
     return process_query_v2(statement=query, environment=input_environment)
```

### Comparing `pypreql-nlp-0.0.4/preql_nlp/monkeypatch.py` & `pypreql-nlp-0.0.5/preql_nlp/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.4/preql_nlp/prompts/final_selection.py` & `pypreql-nlp-0.0.5/preql_nlp/prompts/final_selection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,29 @@
-def process_concept(concept: str):
-    return concept
-
-
-def gen_selection_v1(concepts: list[str], question: str):
-    concept_string = ", ".join(
-        [f'"{process_concept(concept)}"' for concept in concepts]
-    )
-    return f"""
+SELECTION_TEMPLATE_V1 = """
 System: You are a helpful AI that selects the most relevant matching concepts to answer a question from a provided list.
 
 Guidelines:
 * you can assume the user will always provide a list of phrases
 * you can assume the user will always provide a question
 * only return concepts provided by the user
 * concepts are dot seperated and in quotes, e.g. "sales" or "product.revenue"
 * return the concepts that together best match the user question
 * reason about each match step by step, e.g. "first match the concept 'product' to the word 'product' in the question, then match the concept 'revenue' to the word 'revenue' in the question, and together these enable aggregating revenue by year"
 The output should be a VALID JSON blob with the following keys and values:
 * matches: a list of concepts from the user provided list that together best match the 
 * reasoning: a string explaining your step by step reasoning for the matches
 User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"] question: "what product colors had the most revenue in 2024?"]
 System:
-{{"matches": ["product.color", "order.revenue.sum", "order.year" ],
-"reasoning": "product.color matches the user request for product colors, and order revenue sum would enable aggregating revenue to the color. Order year is required to filter to 2024." }}
+{% raw %}{"matches": ["product.color", "order.revenue.sum", "order.year" ],
+"reasoning": "product.color matches the user request for product colors, and order revenue sum would enable aggregating revenue to the color. Order year is required to filter to 2024." }
 User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"] question: "What are the sales by state?"
 System:
-{{"matches": ["order.state", "order.revenue.sum"],
-"reasoning": "order.state is the best match for state when looking at revenue, and order.revenue.sum would enable aggregating revenue." }}
+{"matches": ["order.state", "order.revenue.sum"],
+"reasoning": "order.state is the best match for state when looking at revenue, and order.revenue.sum would enable aggregating revenue." }
 User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"]  question: "What are the average sales by state?"
 System:
-{{"matches": ["order.state", "order.revenue.avg"],
-"reasoning": "order.state is the best match for state, and order.revenue.avg would capture average revenue." }}
-User: concepts:"[{concept_string}]" question: "{question}"
+{"matches": ["order.state", "order.revenue.avg"],
+"reasoning": "order.state is the best match for state, and order.revenue.avg would capture average revenue." }{% endraw %}
+User: concepts:"[{{ concept_string }}]" question: "{{ question }}"
 System:
 
 """
```

### Comparing `pypreql-nlp-0.0.4/preql_nlp/prompts/query_semantic_extraction.py` & `pypreql-nlp-0.0.5/preql_nlp/prompts/query_semantic_extraction.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,49 @@
-def gen_extraction_prompt_v1(input: str):
-    return f"""
+
+
+EXTRACTION_PROMPT_V1 = """
 System: You are a helpful AI that translates ambiguous business questions into structured outputs.
 For a provided question, you will determine if there are metrics or aggregates or dimensions,
-as well as any limit, order, of filtering. 
+as well as any limit, order, or filtering. 
 
 The output should be a VALID JSON blob with the following keys and values:
 - metrics: a list of concepts from the question that should be aggregated
 - dimensions: a list of concepts from the question which are not metrics
 - limit: a number of records to limit the results to, -1 if none specified
 - order: a list of fields to order the results by, with the option to specify ascending or descending
 - filtering: a list of criteria to restrict the results by
 
 
 User: "What are the top 10 products by sales?"
 System:
-{{
+{% raw %}{
 "metrics":["sales"],
 "dimensions": ["products"],
 "limit": 10,
 "order": ["sales desc"],
 "filtering": []
-}}
+}
 
 User: "What are the sales by line of business and state?"
 System:
-{{
+{
 "metrics":["average sales"],
 "dimensions": ["line of business", "state],
 "limit": -1,
 "order": [],
 "filtering": []
-}}
+}
 
 User: "What is the average sales by state?"
 System:
-{{
+{
 "metrics":["average state sales"],
 "dimensions": [],
 "limit": -1,
 "order": [],
 "filtering": []
-}}
+}{% endraw %}
 
-User: "{input}"
+User: "{{ question }}"
 System:
 
-"""
+"""
```

### Comparing `pypreql-nlp-0.0.4/preql_nlp/prompts/semantic_to_tokens.py` & `pypreql-nlp-0.0.5/preql_nlp/prompts/semantic_to_tokens.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,28 @@
-from typing import List
 
-
-def gen_structured_prompt_v1(phrases:List[str], tokens:str)->str:
-    phrase_str = ', '.join(phrases)
-    user_input = f"Given the tokens {tokens}, match tokens to the phrases {phrase_str}"
-    template = f"""\
+STRUCTURED_PROMPT_V1 = """\
 System: you are an AI that helps a user map phrases to tokens by associating a phrase with tokens related to the words
 in the phrase.
 Guidelines:
 * you can assume the user will always provide a list of phrases
 * you can assume the user will always provide a list of tokens
 * only return tokens provided by the user
 The output should be a VALID JSON blob with the phrases as keys and arrays of tokens as values:
 * If a phrase has no matches, return an empty array
 User: given the tokens ["color", "product", "year", "revenue"], match tokens to the phrases ["product revenue", "product color", "product revenue by year", "yearly revenue"]
 System:
-{{
+{% raw %}{
     "product revenue": ["product", "revenue"],
     "product color": ["product", "color"],
     "product revenue by year": ["product", "revenue", "year"],
     "yearly revenue": ["year", "revenue"]
-}}
+}
 User: given the tokens ["product", "count", "order", "year"], match tokens to the phrases ["products sold", "orders"]
 System:
-{{
+{
     "products sold": ["product", "count"],
     "orders": ["order", "count"]
-}}
-User: { user_input }
+}{% endraw %}
+User: Given the tokens {{ tokens }}, match tokens to the phrases {{ phrase_str }}
 System:
-"""  # noqa"""
-    return template
+"""
```

### Comparing `pypreql-nlp-0.0.4/pypreql_nlp.egg-info/PKG-INFO` & `pypreql-nlp-0.0.5/pypreql_nlp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypreql-nlp
-Version: 0.0.4
+Version: 0.0.5
 Summary: NLP interface for pypreql.
 Home-page: 
 Author: 
 Author-email: pypreql-community@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -30,23 +30,23 @@
 ## Examples
 
 ### Basic BQ example
 
 
 ```python
 from trilogy_public_models import models
-from preql import Executor, default_engine, Dialect
+from preql import Executor, Dialects
 from preql_nlp import build_query
 
 # define the model we want to parse
 environment = models["bigquery.stack_overflow"]
 
 # set up preql executor
 # default bigquery executor requires local default credentials configured
-executor = Dialect.BIGQUERY.default_executor(environment= environment)
+executor = Dialects.BIGQUERY.default_executor(environment= environment)
 
 # build a query off text and the selected model
 processed_query = build_query(
     "How many questions are asked per year?",
     environment,
 )
```

### Comparing `pypreql-nlp-0.0.4/setup.py` & `pypreql-nlp-0.0.5/setup.py`

 * *Files identical despite different names*

