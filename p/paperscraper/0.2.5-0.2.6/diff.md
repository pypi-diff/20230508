# Comparing `tmp/paperscraper-0.2.5.tar.gz` & `tmp/paperscraper-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paperscraper-0.2.5.tar", last modified: Wed Apr 19 16:30:47 2023, max compression
+gzip compressed data, was "paperscraper-0.2.6.tar", last modified: Sun May  7 22:40:04 2023, max compression
```

## Comparing `paperscraper-0.2.5.tar` & `paperscraper-0.2.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.327613 paperscraper-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-04-19 16:30:33.000000 paperscraper-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    11386 2023-04-19 16:30:47.327613 paperscraper-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10554 2023-04-19 16:30:33.000000 paperscraper-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.323613 paperscraper-0.2.5/paperscraper/
--rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.323613 paperscraper-0.2.5/paperscraper/arxiv/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/arxiv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3148 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/arxiv/arxiv.py
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/arxiv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.323613 paperscraper-0.2.5/paperscraper/get_dumps/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/get_dumps/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1484 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/get_dumps/biorxiv.py
--rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/get_dumps/chemrxiv.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1508 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/get_dumps/medrxiv.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.323613 paperscraper-0.2.5/paperscraper/get_dumps/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/get_dumps/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.323613 paperscraper-0.2.5/paperscraper/get_dumps/utils/chemrxiv/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/get_dumps/utils/chemrxiv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4173 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/get_dumps/utils/chemrxiv/chemrxiv_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4482 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/get_dumps/utils/chemrxiv/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5428 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/journal_if.py
--rw-r--r--   0 runner    (1001) docker     (122)     1491 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/load_dumps.py
--rw-r--r--   0 runner    (1001) docker     (122)     3603 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)    16483 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/plotting.py
--rw-r--r--   0 runner    (1001) docker     (122)     4830 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/postprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.327613 paperscraper-0.2.5/paperscraper/pubmed/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/pubmed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3505 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/pubmed/pubmed.py
--rw-r--r--   0 runner    (1001) docker     (122)     4107 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/pubmed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.327613 paperscraper-0.2.5/paperscraper/scholar/
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/scholar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3140 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/scholar/scholar.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.327613 paperscraper-0.2.5/paperscraper/server_dumps/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/server_dumps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2166 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.327613 paperscraper-0.2.5/paperscraper/xrxiv/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/xrxiv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/xrxiv/xrxiv_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3264 2023-04-19 16:30:33.000000 paperscraper-0.2.5/paperscraper/xrxiv/xrxiv_query.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:30:47.323613 paperscraper-0.2.5/paperscraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11386 2023-04-19 16:30:47.000000 paperscraper-0.2.5/paperscraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-04-19 16:30:47.000000 paperscraper-0.2.5/paperscraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 16:30:47.000000 paperscraper-0.2.5/paperscraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 16:30:47.000000 paperscraper-0.2.5/paperscraper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-04-19 16:30:47.000000 paperscraper-0.2.5/paperscraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-19 16:30:47.000000 paperscraper-0.2.5/paperscraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-19 16:30:47.327613 paperscraper-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-04-19 16:30:33.000000 paperscraper-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.292587 paperscraper-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-05-07 22:39:50.000000 paperscraper-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    11386 2023-05-07 22:40:04.292587 paperscraper-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10554 2023-05-07 22:39:50.000000 paperscraper-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.284587 paperscraper-0.2.6/paperscraper/
+-rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.288587 paperscraper-0.2.6/paperscraper/arxiv/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/arxiv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3333 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/arxiv/arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/arxiv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.288587 paperscraper-0.2.6/paperscraper/get_dumps/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/get_dumps/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1484 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/get_dumps/biorxiv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/get_dumps/chemrxiv.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1508 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/get_dumps/medrxiv.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.288587 paperscraper-0.2.6/paperscraper/get_dumps/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/get_dumps/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.288587 paperscraper-0.2.6/paperscraper/get_dumps/utils/chemrxiv/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/get_dumps/utils/chemrxiv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4173 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/get_dumps/utils/chemrxiv/chemrxiv_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4482 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/get_dumps/utils/chemrxiv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5428 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/journal_if.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1491 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/load_dumps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3603 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16483 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4830 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.292587 paperscraper-0.2.6/paperscraper/pubmed/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/pubmed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3505 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/pubmed/pubmed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4107 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/pubmed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.292587 paperscraper-0.2.6/paperscraper/scholar/
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/scholar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3140 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/scholar/scholar.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.292587 paperscraper-0.2.6/paperscraper/server_dumps/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/server_dumps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2166 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.292587 paperscraper-0.2.6/paperscraper/xrxiv/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/xrxiv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/xrxiv/xrxiv_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3264 2023-05-07 22:39:50.000000 paperscraper-0.2.6/paperscraper/xrxiv/xrxiv_query.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 22:40:04.288587 paperscraper-0.2.6/paperscraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11386 2023-05-07 22:40:04.000000 paperscraper-0.2.6/paperscraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-05-07 22:40:04.000000 paperscraper-0.2.6/paperscraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-07 22:40:04.000000 paperscraper-0.2.6/paperscraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-07 22:40:04.000000 paperscraper-0.2.6/paperscraper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-05-07 22:40:04.000000 paperscraper-0.2.6/paperscraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-07 22:40:04.000000 paperscraper-0.2.6/paperscraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-07 22:40:04.292587 paperscraper-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-05-07 22:39:50.000000 paperscraper-0.2.6/setup.py
```

### Comparing `paperscraper-0.2.5/LICENSE` & `paperscraper-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.5/PKG-INFO` & `paperscraper-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paperscraper
-Version: 0.2.5
+Version: 0.2.6
 Summary: paperscraper: Package to scrape papers.
 Home-page: https://github.com/PhosphorylatedRabbits/paperscraper
 Author: Jannis Born, Matteo Manica
 Author-email: jannis.born@gmx.de, drugilsberg@gmail.com
 License: MIT
 Keywords: Academics,Science,Publication,Search,PubMed,Arxiv,Medrxiv,Biorxiv,Chemrxiv
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `paperscraper-0.2.5/README.md` & `paperscraper-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.5/paperscraper/__init__.py` & `paperscraper-0.2.6/paperscraper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Initialize the module."""
 __name__ = "paperscraper"
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 
 import logging
 import os
 import sys
 from typing import List, Union
 
 from .load_dumps import QUERY_FN_DICT
```

### Comparing `paperscraper-0.2.5/paperscraper/arxiv/arxiv.py` & `paperscraper-0.2.6/paperscraper/arxiv/arxiv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from typing import Dict, List, Union
 
-import arxiv
 import pandas as pd
+from tqdm import tqdm
+
+import arxiv
 
 from ..utils import dump_papers
 from .utils import get_query_from_keywords
 
 arxiv_field_mapper = {
     "published": "date",
     "journal_ref": "journal",
     "summary": "abstract",
+    "entry_id": "doi",
 }
 
 # Authors, date, and journal fields need specific processing
 process_fields = {
     "authors": lambda authors: ", ".join([a.name for a in authors]),
     "date": lambda date: date.strftime("%Y-%m-%d"),
     "journal": lambda j: j if j is not None else "",
+    "doi": lambda entry_id: f"10.48550/arXiv.{entry_id.split('/')[-1].split('v')[0]}",
 }
 
 
 def get_arxiv_papers(
     query: str,
     fields: List = ["title", "authors", "date", "abstract", "journal", "doi"],
     max_results: int = 99999,
@@ -53,28 +57,28 @@
     processed = pd.DataFrame(
         [
             {
                 arxiv_field_mapper.get(key, key): process_fields.get(
                     arxiv_field_mapper.get(key, key), lambda x: x
                 )(value)
                 for key, value in vars(paper).items()
-                if arxiv_field_mapper.get(key, key) in fields
+                if arxiv_field_mapper.get(key, key) in fields and key != "doi"
             }
-            for paper in results
+            for paper in tqdm(results, desc=f"Processing {query}")
         ]
     )
     return processed
 
 
 def get_and_dump_arxiv_papers(
     keywords: List[Union[str, List[str]]],
     output_filepath: str,
     fields: List = ["title", "authors", "date", "abstract", "journal", "doi"],
     *args,
-    **kwargs
+    **kwargs,
 ):
     """
     Combines get_arxiv_papers and dump_papers.
 
     Args:
         keywords (List[str, List[str]]): List of keywords to request arxiv API.
             The outer list level will be considered as AND separated keys, the
```

### Comparing `paperscraper-0.2.5/paperscraper/arxiv/utils.py` & `paperscraper-0.2.6/paperscraper/arxiv/utils.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.5/paperscraper/get_dumps/biorxiv.py` & `paperscraper-0.2.6/paperscraper/get_dumps/biorxiv.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.5/paperscraper/get_dumps/chemrxiv.py` & `paperscraper-0.2.6/paperscraper/get_dumps/chemrxiv.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.5/paperscraper/get_dumps/medrxiv.py` & `paperscraper-0.2.6/paperscraper/get_dumps/medrxiv.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.5/paperscraper/get_dumps/utils/chemrxiv/chemrxiv_api.py` & `paperscraper-0.2.6/paperscraper/get_dumps/utils/chemrxiv/chemrxiv_api.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.5/paperscraper/get_dumps/utils/chemrxiv/utils.py` & `paperscraper-0.2.6/paperscraper/get_dumps/utils/chemrxiv/utils.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.5/paperscraper/journal_if.py` & `paperscraper-0.2.6/paperscraper/journal_if.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.5/paperscraper/load_dumps.py` & `paperscraper-0.2.6/paperscraper/load_dumps.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.5/paperscraper/pdf.py` & `paperscraper-0.2.6/paperscraper/pdf.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.5/paperscraper/plotting.py` & `paperscraper-0.2.6/paperscraper/plotting.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.5/paperscraper/postprocessing.py` & `paperscraper-0.2.6/paperscraper/postprocessing.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.5/paperscraper/pubmed/pubmed.py` & `paperscraper-0.2.6/paperscraper/pubmed/pubmed.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.5/paperscraper/pubmed/utils.py` & `paperscraper-0.2.6/paperscraper/pubmed/utils.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.5/paperscraper/scholar/scholar.py` & `paperscraper-0.2.6/paperscraper/scholar/scholar.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.5/paperscraper/utils.py` & `paperscraper-0.2.6/paperscraper/utils.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.5/paperscraper/xrxiv/xrxiv_api.py` & `paperscraper-0.2.6/paperscraper/xrxiv/xrxiv_api.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.5/paperscraper/xrxiv/xrxiv_query.py` & `paperscraper-0.2.6/paperscraper/xrxiv/xrxiv_query.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.5/paperscraper.egg-info/PKG-INFO` & `paperscraper-0.2.6/paperscraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paperscraper
-Version: 0.2.5
+Version: 0.2.6
 Summary: paperscraper: Package to scrape papers.
 Home-page: https://github.com/PhosphorylatedRabbits/paperscraper
 Author: Jannis Born, Matteo Manica
 Author-email: jannis.born@gmx.de, drugilsberg@gmail.com
 License: MIT
 Keywords: Academics,Science,Publication,Search,PubMed,Arxiv,Medrxiv,Biorxiv,Chemrxiv
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `paperscraper-0.2.5/paperscraper.egg-info/SOURCES.txt` & `paperscraper-0.2.6/paperscraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.5/setup.py` & `paperscraper-0.2.6/setup.py`

 * *Files identical despite different names*

