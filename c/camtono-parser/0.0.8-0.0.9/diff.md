# Comparing `tmp/camtono-parser-0.0.8.tar.gz` & `tmp/camtono-parser-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/camtono-parser-0.0.8.tar", last modified: Fri Mar 19 15:17:53 2021, max compression
+gzip compressed data, was "dist/camtono-parser-0.0.9.tar", last modified: Fri Mar 19 16:45:49 2021, max compression
```

## Comparing `camtono-parser-0.0.8.tar` & `camtono-parser-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-19 15:17:53.000000 camtono-parser-0.0.8/
--rw-rw-rw-   0 root         (0) root         (0)       34 2021-03-19 15:17:22.000000 camtono-parser-0.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      458 2021-03-19 15:17:53.000000 camtono-parser-0.0.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-19 15:17:53.000000 camtono-parser-0.0.8/camtono/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-19 15:17:53.000000 camtono-parser-0.0.8/camtono/parser/
--rw-rw-rw-   0 root         (0) root         (0)      108 2021-03-19 15:17:22.000000 camtono-parser-0.0.8/camtono/parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4666 2021-03-19 15:17:22.000000 camtono-parser-0.0.8/camtono/parser/clean.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2021-03-19 15:17:22.000000 camtono-parser-0.0.8/camtono/parser/dialects.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2021-03-19 15:17:22.000000 camtono-parser-0.0.8/camtono/parser/feature.py
--rw-rw-rw-   0 root         (0) root         (0)     2425 2021-03-19 15:17:22.000000 camtono-parser-0.0.8/camtono/parser/format.py
--rw-rw-rw-   0 root         (0) root         (0)     1476 2021-03-19 15:17:22.000000 camtono-parser-0.0.8/camtono/parser/keywords.py
--rw-rw-rw-   0 root         (0) root         (0)    14235 2021-03-19 15:17:22.000000 camtono-parser-0.0.8/camtono/parser/parse.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2021-03-19 15:17:22.000000 camtono-parser-0.0.8/camtono/parser/standard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-19 15:17:53.000000 camtono-parser-0.0.8/camtono_parser.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      458 2021-03-19 15:17:53.000000 camtono-parser-0.0.8/camtono_parser.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      426 2021-03-19 15:17:53.000000 camtono-parser-0.0.8/camtono_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2021-03-19 15:17:53.000000 camtono-parser-0.0.8/camtono_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       27 2021-03-19 15:17:53.000000 camtono-parser-0.0.8/camtono_parser.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        8 2021-03-19 15:17:53.000000 camtono-parser-0.0.8/camtono_parser.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      210 2021-03-19 15:17:53.000000 camtono-parser-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      865 2021-03-19 15:17:22.000000 camtono-parser-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-19 16:45:49.000000 camtono-parser-0.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2021-03-19 16:45:23.000000 camtono-parser-0.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      458 2021-03-19 16:45:49.000000 camtono-parser-0.0.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-19 16:45:49.000000 camtono-parser-0.0.9/camtono/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-19 16:45:49.000000 camtono-parser-0.0.9/camtono/parser/
+-rw-rw-rw-   0 root         (0) root         (0)      108 2021-03-19 16:45:23.000000 camtono-parser-0.0.9/camtono/parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4652 2021-03-19 16:45:23.000000 camtono-parser-0.0.9/camtono/parser/clean.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2021-03-19 16:45:23.000000 camtono-parser-0.0.9/camtono/parser/dialects.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2021-03-19 16:45:23.000000 camtono-parser-0.0.9/camtono/parser/feature.py
+-rw-rw-rw-   0 root         (0) root         (0)     2425 2021-03-19 16:45:23.000000 camtono-parser-0.0.9/camtono/parser/format.py
+-rw-rw-rw-   0 root         (0) root         (0)     1476 2021-03-19 16:45:23.000000 camtono-parser-0.0.9/camtono/parser/keywords.py
+-rw-rw-rw-   0 root         (0) root         (0)    14383 2021-03-19 16:45:23.000000 camtono-parser-0.0.9/camtono/parser/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2021-03-19 16:45:23.000000 camtono-parser-0.0.9/camtono/parser/standard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-19 16:45:49.000000 camtono-parser-0.0.9/camtono_parser.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      458 2021-03-19 16:45:49.000000 camtono-parser-0.0.9/camtono_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      426 2021-03-19 16:45:49.000000 camtono-parser-0.0.9/camtono_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2021-03-19 16:45:49.000000 camtono-parser-0.0.9/camtono_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       27 2021-03-19 16:45:49.000000 camtono-parser-0.0.9/camtono_parser.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        8 2021-03-19 16:45:49.000000 camtono-parser-0.0.9/camtono_parser.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      210 2021-03-19 16:45:49.000000 camtono-parser-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      865 2021-03-19 16:45:23.000000 camtono-parser-0.0.9/setup.py
```

### Comparing `camtono-parser-0.0.8/camtono/parser/clean.py` & `camtono-parser-0.0.9/camtono/parser/clean.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,24 +14,19 @@
     cleaned_query = pad_comparisons(query=cleaned_query)
     cleaned_query = clean_spaces(query=cleaned_query)
     return cleaned_query.lower()
 
 
 def pad_comparisons(query):
     import re
-
-    re.sub('(?:\S*)(<|>|<=|>=|=|==|\|\||\:\:|\+|\-|\!=|<>|\/|\*|\~)(?:\S*)', pad, query)
-    cleaned_query = query
+    cleaned_query = re.sub(
+        '([\s\(][\d\w\.\_\{\}]*)(<=|>=|<>|==|!=|<|>|=|\|\||::|\+|-|/|\*|~)([\d\w\.\_\{\}]*[\)\s]*)', r' \1 \2 \3', query)
     return cleaned_query
 
 
-def pad(m, ):
-    return ' ' + m.string + " "
-
-
 def clean_spaces(query) -> str:
     """
 
     :param query:
     :return:
     """
     cleaned_query = re.sub('\s+', ' ', query)
```

### Comparing `camtono-parser-0.0.8/camtono/parser/dialects.py` & `camtono-parser-0.0.9/camtono/parser/dialects.py`

 * *Files identical despite different names*

### Comparing `camtono-parser-0.0.8/camtono/parser/feature.py` & `camtono-parser-0.0.9/camtono/parser/feature.py`

 * *Files identical despite different names*

### Comparing `camtono-parser-0.0.8/camtono/parser/format.py` & `camtono-parser-0.0.9/camtono/parser/format.py`

 * *Files identical despite different names*

### Comparing `camtono-parser-0.0.8/camtono/parser/keywords.py` & `camtono-parser-0.0.9/camtono/parser/keywords.py`

 * *Files identical despite different names*

### Comparing `camtono-parser-0.0.8/camtono/parser/parse.py` & `camtono-parser-0.0.9/camtono/parser/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import absolute_import, division, unicode_literals
 
 from mo_parsing.engine import Engine
 from mo_parsing.helpers import delimitedList, restOfLine
 from moz_sql_parser.windows import sortColumn, window
 
-from .keywords import *
-from .dialects import load_dialect_module
-from .clean import strip_comments, encapsulate_variables, pad_comparisons, ENCODING_CHARACTER
+from camtono.parser.keywords import *
+from camtono.parser.dialects import load_dialect_module
+from camtono.parser.clean import strip_comments, encapsulate_variables, pad_comparisons, ENCODING_CHARACTER
 
 HINT_STRING = "|"
 
 
 def parse_query(query, sql_dialect, feature_name=None) -> tuple:
     """
 
@@ -18,18 +18,22 @@
     :param sql_dialect:
     :param feature_name:
     :return:
     """
     dialect = load_dialect_module(dialect_name=sql_dialect)
     standardized_query = strip_comments(query=query)
     standardized_query = pad_comparisons(query = standardized_query)
+    print('padded')
+    print(standardized_query)
     standardized_query, variables = encapsulate_variables(
         query=standardized_query, encoding_character='', wrap_character=ENCODING_CHARACTER,
         skip_characters=0, encoded=False, feature_name=feature_name
     )
+    print('encapsulated')
+    print(standardized_query)
     query_ast = dialect.parse_query(query=standardized_query)
     query_input = label_input(variable_set=variables, query_ast=query_ast)
 
     output = label_output(query_ast=query_ast)
     dependencies = []
     return query_ast, query_input, output, dependencies
```

### Comparing `camtono-parser-0.0.8/setup.py` & `camtono-parser-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # with open("README.md", "r") as fh:
 #     long_description = fh.read()
 # with open('requirements.txt') as f:
 #     requirements = f.readlines()
 
 setuptools.setup(
     name="camtono-parser",  # Replace with your own username
-    version="0.0.8",
+    version="0.0.9",
     author="DOT",
     author_email="dot@adara.com",
     description="SQL parser and formatter",
     long_description="",
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://bitbucket.org/adarainc/camtono-parser-pkg",
```

