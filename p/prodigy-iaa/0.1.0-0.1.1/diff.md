# Comparing `tmp/prodigy_iaa-0.1.0.tar.gz` & `tmp/prodigy_iaa-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodigy_iaa-0.1.0.tar", max compression
+gzip compressed data, was "prodigy_iaa-0.1.1.tar", max compression
```

## Comparing `prodigy_iaa-0.1.0.tar` & `prodigy_iaa-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,8 @@
--rw-r--r--   0        0        0     6164 2022-12-08 16:43:42.346864 prodigy_iaa-0.1.0/README.md
--rw-r--r--   0        0        0      667 2022-11-21 20:22:09.646331 prodigy_iaa-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      166 2022-11-21 14:06:35.178530 prodigy_iaa-0.1.0/src/prodigy_iaa/__init__.py
--rw-r--r--   0        0        0     5503 2022-12-01 20:39:45.611724 prodigy_iaa-0.1.0/src/prodigy_iaa/measures.py
--rw-r--r--   0        0        0     3896 2022-11-22 20:06:29.075139 prodigy_iaa-0.1.0/src/prodigy_iaa/processors.py
--rw-r--r--   0        0        0     5522 2022-11-21 20:39:24.443613 prodigy_iaa-0.1.0/src/prodigy_iaa/recipe.py
--rw-r--r--   0        0        0     1460 2022-11-21 20:48:32.156057 prodigy_iaa-0.1.0/src/prodigy_iaa/render.py
--rw-r--r--   0        0        0     2625 2022-11-27 20:27:54.130806 prodigy_iaa-0.1.0/src/prodigy_iaa/spans.py
--rw-r--r--   0        0        0     7118 1970-01-01 00:00:00.000000 prodigy_iaa-0.1.0/setup.py
--rw-r--r--   0        0        0     6636 1970-01-01 00:00:00.000000 prodigy_iaa-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6433 2023-05-08 14:24:13.658721 prodigy_iaa-0.1.1/README.md
+-rw-r--r--   0        0        0      667 2023-05-08 14:27:44.235127 prodigy_iaa-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-05-08 14:24:13.659569 prodigy_iaa-0.1.1/src/prodigy_iaa/__init__.py
+-rw-r--r--   0        0        0     5503 2023-05-08 14:24:13.659741 prodigy_iaa-0.1.1/src/prodigy_iaa/measures.py
+-rw-r--r--   0        0        0     4015 2023-05-08 14:27:29.598535 prodigy_iaa-0.1.1/src/prodigy_iaa/processors.py
+-rw-r--r--   0        0        0     5522 2023-05-08 14:24:13.660037 prodigy_iaa-0.1.1/src/prodigy_iaa/recipe.py
+-rw-r--r--   0        0        0     1460 2023-05-08 14:24:13.662064 prodigy_iaa-0.1.1/src/prodigy_iaa/render.py
+-rw-r--r--   0        0        0     6905 1970-01-01 00:00:00.000000 prodigy_iaa-0.1.1/PKG-INFO
```

### Comparing `prodigy_iaa-0.1.0/README.md` & `prodigy_iaa-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,43 @@
+Metadata-Version: 2.1
+Name: prodigy-iaa
+Version: 0.1.1
+Summary: 
+Author: Peter Baumgartner
+Author-email: 5107405+pmbaumgartner@users.noreply.github.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
 # ✨ Prodigy - Inter-Annotator Agreement Recipes 🤝
 
 These recipes calculate [Inter-Annotator Agreement](https://en.wikipedia.org/wiki/Inter-rater_reliability) (aka Inter-Rater Reliability) measures for use with [Prodigy](https://prodi.gy/). The measures include Percent (Simple) Agreement, Krippendorff's `Alpha`, and Gwet's `AC2`. All calculations were derived using the equations in [this paper](https://agreestat.com/papers/onkrippendorffalpha_rev10052015.pdf)[^1], and this includes tests to match the values given on the datasets referenced in that paper. 
 
 Currently this package supports IAA metrics for binary classification, multiclass classification, and multilabel (binary per label) classification. Span-based IAA measures for NER and Span Categorization will be integrated in the future.
 
 Note that you can also use the measures included here w/o directly interfacing with Prodigy, see section on [other use cases](#other-use-cases--use-outside-prodigy).
 
+**Install**
+
+```
+pip install prodigy-iaa
+```
+
+For dev
+
+```
+pip install git+https://github.com/pmbaumgartner/prodigy-iaa
+```
+
+This package uses [entry points](https://prodi.gy/docs/install#entry-points) so you should just be able to install and run the commands below.
+
 ## Recipes
 
 Recipes depend the source data structure:
 - `iaa.datasets` will calculate measures assuming you have multiple datasets in prodigy, one dataset per annotator
 - `iaa.sessions` will calculate measures assuming you have multiple annotators, identified typically by `_session_id`, in a single dataset
 - `iaa.jsonl` operates the same as `iaa.sessions`, but on a file exported to JSONL with `prodigy db-out`.
 
@@ -84,7 +112,8 @@
 ## References
 
 
 [^1]: K. L. Gwet, “On Krippendorff’s Alpha Coefficient,” p. 16, 2015.
 [^2]: J. Lovejoy, B. R. Watson, S. Lacy, and D. Riffe, “Three Decades of Reliability in Communication Content Analyses: Reporting of Reliability Statistics and Coefficient Levels in Three Top Journals,” p. 44.
 [^3]: S. Lacy, B. R. Watson, D. Riffe, and J. Lovejoy, “Issues and Best Practices in Content Analysis,” Journalism & Mass Communication Quarterly, vol. 92, no. 4, pp. 791–811, Dec. 2015, doi: 10.1177/1077699015607338.
 [^4]: X. Zhao, J. S. Liu, and K. Deng, “Assumptions Behind Intercoder Reliability Indices,” Communication Yearbook, p. 83.
+
```

### Comparing `prodigy_iaa-0.1.0/pyproject.toml` & `prodigy_iaa-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prodigy-iaa"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Peter Baumgartner <5107405+pmbaumgartner@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "prodigy_iaa", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `prodigy_iaa-0.1.0/src/prodigy_iaa/measures.py` & `prodigy_iaa-0.1.1/src/prodigy_iaa/measures.py`

 * *Files identical despite different names*

### Comparing `prodigy_iaa-0.1.0/src/prodigy_iaa/processors.py` & `prodigy_iaa-0.1.1/src/prodigy_iaa/processors.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,19 @@
         return answer
     else:
         return None
 
 
 def get_choice(example) -> Optional[str]:
     if example["answer"] == "accept":
-        return example["accept"][0]
+        try:
+            # They could accept but have no choice
+            return example["accept"][0]
+        except IndexError:
+            return None
     else:
         return None
 
 
 def get_contains(example, value: str) -> int:
     """You'll need to use this with functools.partial to pass
     to examples_to_reliability in the multilabel case."""
```

### Comparing `prodigy_iaa-0.1.0/src/prodigy_iaa/recipe.py` & `prodigy_iaa-0.1.1/src/prodigy_iaa/recipe.py`

 * *Files identical despite different names*

### Comparing `prodigy_iaa-0.1.0/src/prodigy_iaa/render.py` & `prodigy_iaa-0.1.1/src/prodigy_iaa/render.py`

 * *Files identical despite different names*

### Comparing `prodigy_iaa-0.1.0/setup.py` & `prodigy_iaa-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,104 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+# ✨ Prodigy - Inter-Annotator Agreement Recipes 🤝
 
-package_dir = \
-{'': 'src'}
+These recipes calculate [Inter-Annotator Agreement](https://en.wikipedia.org/wiki/Inter-rater_reliability) (aka Inter-Rater Reliability) measures for use with [Prodigy](https://prodi.gy/). The measures include Percent (Simple) Agreement, Krippendorff's `Alpha`, and Gwet's `AC2`. All calculations were derived using the equations in [this paper](https://agreestat.com/papers/onkrippendorffalpha_rev10052015.pdf)[^1], and this includes tests to match the values given on the datasets referenced in that paper. 
 
-packages = \
-['prodigy_iaa']
+Currently this package supports IAA metrics for binary classification, multiclass classification, and multilabel (binary per label) classification. Span-based IAA measures for NER and Span Categorization will be integrated in the future.
 
-package_data = \
-{'': ['*']}
-
-entry_points = \
-{'prodigy_recipes': ['iaa.datasets = prodigy_iaa.recipe:iaa_datasets',
-                     'iaa.jsonl = prodigy_iaa.recipe:iaa_jsonl',
-                     'iaa.sessions = prodigy_iaa.recipe:iaa_jsonl']}
-
-setup_kwargs = {
-    'name': 'prodigy-iaa',
-    'version': '0.1.0',
-    'description': '',
-    'long_description': '# ✨ Prodigy - Inter-Annotator Agreement Recipes 🤝\n\nThese recipes calculate [Inter-Annotator Agreement](https://en.wikipedia.org/wiki/Inter-rater_reliability) (aka Inter-Rater Reliability) measures for use with [Prodigy](https://prodi.gy/). The measures include Percent (Simple) Agreement, Krippendorff\'s `Alpha`, and Gwet\'s `AC2`. All calculations were derived using the equations in [this paper](https://agreestat.com/papers/onkrippendorffalpha_rev10052015.pdf)[^1], and this includes tests to match the values given on the datasets referenced in that paper. \n\nCurrently this package supports IAA metrics for binary classification, multiclass classification, and multilabel (binary per label) classification. Span-based IAA measures for NER and Span Categorization will be integrated in the future.\n\nNote that you can also use the measures included here w/o directly interfacing with Prodigy, see section on [other use cases](#other-use-cases--use-outside-prodigy).\n\n## Recipes\n\nRecipes depend the source data structure:\n- `iaa.datasets` will calculate measures assuming you have multiple datasets in prodigy, one dataset per annotator\n- `iaa.sessions` will calculate measures assuming you have multiple annotators, identified typically by `_session_id`, in a single dataset\n- `iaa.jsonl` operates the same as `iaa.sessions`, but on a file exported to JSONL with `prodigy db-out`.\n\nℹ️ **Get details on each recipe\'s arguments with `prodigy <recipe> --help`**\n\n## Example\n\nIn this toy example, the command calculates agreement using dataset `my-dataset`, which is a `multiclass` problem -- meaning it\'s data is generated using the `choice` interface, exclusive choices, storing choices in the "accept" key. In this example, there are 5 total examples, 4 of them have co-incident annotations (i.e. any overlap), and 3 unique annotators.\n\n```\n$ prodigy iaa.sessions my-dataset multiclass\n\nℹ Annotation Statistics\n\nAttribute                      Value\n----------------------------   -----\nExamples                           5\nCategories                         3\nCo-Incident Examples*              4\nSingle Annotation Examples         1\nAnnotators                         3\nAvg. Annotations per Example    2.60\n\n* (>1 annotation)\n\nℹ Agreement Statistics\n\nStatistic                     Value\n--------------------------   ------\nPercent (Simple) Agreement   0.4167\nKrippendorff\'s Alpha         0.1809\nGwet\'s AC2                   0.1640\n```\n\n## Validations & Practical Use\n\nAll recipes depend on examples being hashed uniquely and stored under `_task_hash` on the example. There are other validations involved as well:\n- Checks if `view_id` is the same for all examples\n- Checks if `label` is the same for all examples\n- Checks that each annotator has not double-annotated the same `_task_hash`\n\n**If any validations fail, or your data is unique in some way, `iaa.jsonl` is the recipe you want.** Export your data, identify any issues and remedy them, and then calculate your measures on the cleaned exported data.\n\n\n## Theory\n\nThere is no single measure across all datasets to give a reasonable measurement of agreement - often times the measures are conditional on qualities of the data. The metrics included in these recipes have nice properties that make them flexible to various annotation situations: they can handle missing values (i.e. incomplete overlap), scale to any number of annotators, scale to any number of categories, and can be customized with your own weighting functions. In addition, the choice of metrics available within this package follow the recommendations in the literature[^2][^3], plus theoretical analysis[^4] demonstrating when certain metrics might be most useful.\n\nTable 13 in [this paper](https://scholar.google.com/scholar?cluster=17269958574032994585&hl=en&as_sdt=0,34&as_vis=1)[^4] highlights systematic issues with each metric. They are as follows:\n\n- **When there is _low agreement_**: Percent (Simple) Agreement can produce high scores.\n  - Imagine a binary classification problem with a very low base rate. Annotators can often agree on the negative case, but rarely agree on the positive.\n- **When there are _highly uneven sizes of categories_**: `AC2` can produce low scores, `Alpha` can produce high scores.\n- **When there are _N < 20_ co-incident annotated examples**: `Alpha` can produce high scores.\n  - You probably shouldn\'t trust _N < 100_ generally.\n- **When there are _3 or more categories_**: `AC2` can produce high scores.\n\n**Summary**: Use simple agreement and `Alpha`. If simple agreement is high, and `Alpha` is low, verify with `AC2`[^3]. In general these numbers correlate, if you\'re getting contradictory or unclear information increase the number of examples and explore your data.\n\n## Other Use-Cases / Use Outside Prodigy\n\nIf you want to calculate these measures in a custom script on your own data, you can use `from prodigy_iaa.measures import calculate_agreement`. See tests in `tests/test_measures.py` for an example. The docstrings for each function should indicate the expected data structures.\n\nYou could also use this, for example, to print out some nice output during an `update` callback and get annotation statistics as each user submits examples.\n\nIf you want to calcualte more precise statistics, e.g. comparing two annotators pairwise, you could write a script to do that as well with these existing functions.\n\n\n## Tests\n\nTests require a working version of `prodigy`, so they are not run in CI and must be run locally. \n## References\n\n\n[^1]: K. L. Gwet, “On Krippendorff’s Alpha Coefficient,” p. 16, 2015.\n[^2]: J. Lovejoy, B. R. Watson, S. Lacy, and D. Riffe, “Three Decades of Reliability in Communication Content Analyses: Reporting of Reliability Statistics and Coefficient Levels in Three Top Journals,” p. 44.\n[^3]: S. Lacy, B. R. Watson, D. Riffe, and J. Lovejoy, “Issues and Best Practices in Content Analysis,” Journalism & Mass Communication Quarterly, vol. 92, no. 4, pp. 791–811, Dec. 2015, doi: 10.1177/1077699015607338.\n[^4]: X. Zhao, J. S. Liu, and K. Deng, “Assumptions Behind Intercoder Reliability Indices,” Communication Yearbook, p. 83.\n',
-    'author': 'Peter Baumgartner',
-    'author_email': '5107405+pmbaumgartner@users.noreply.github.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+Note that you can also use the measures included here w/o directly interfacing with Prodigy, see section on [other use cases](#other-use-cases--use-outside-prodigy).
 
+**Install**
 
-setup(**setup_kwargs)
+```
+pip install prodigy-iaa
+```
+
+For dev
+
+```
+pip install git+https://github.com/pmbaumgartner/prodigy-iaa
+```
+
+This package uses [entry points](https://prodi.gy/docs/install#entry-points) so you should just be able to install and run the commands below.
+
+## Recipes
+
+Recipes depend the source data structure:
+- `iaa.datasets` will calculate measures assuming you have multiple datasets in prodigy, one dataset per annotator
+- `iaa.sessions` will calculate measures assuming you have multiple annotators, identified typically by `_session_id`, in a single dataset
+- `iaa.jsonl` operates the same as `iaa.sessions`, but on a file exported to JSONL with `prodigy db-out`.
+
+ℹ️ **Get details on each recipe's arguments with `prodigy <recipe> --help`**
+
+## Example
+
+In this toy example, the command calculates agreement using dataset `my-dataset`, which is a `multiclass` problem -- meaning it's data is generated using the `choice` interface, exclusive choices, storing choices in the "accept" key. In this example, there are 5 total examples, 4 of them have co-incident annotations (i.e. any overlap), and 3 unique annotators.
+
+```
+$ prodigy iaa.sessions my-dataset multiclass
+
+ℹ Annotation Statistics
+
+Attribute                      Value
+----------------------------   -----
+Examples                           5
+Categories                         3
+Co-Incident Examples*              4
+Single Annotation Examples         1
+Annotators                         3
+Avg. Annotations per Example    2.60
+
+* (>1 annotation)
+
+ℹ Agreement Statistics
+
+Statistic                     Value
+--------------------------   ------
+Percent (Simple) Agreement   0.4167
+Krippendorff's Alpha         0.1809
+Gwet's AC2                   0.1640
+```
+
+## Validations & Practical Use
+
+All recipes depend on examples being hashed uniquely and stored under `_task_hash` on the example. There are other validations involved as well:
+- Checks if `view_id` is the same for all examples
+- Checks if `label` is the same for all examples
+- Checks that each annotator has not double-annotated the same `_task_hash`
+
+**If any validations fail, or your data is unique in some way, `iaa.jsonl` is the recipe you want.** Export your data, identify any issues and remedy them, and then calculate your measures on the cleaned exported data.
+
+
+## Theory
+
+There is no single measure across all datasets to give a reasonable measurement of agreement - often times the measures are conditional on qualities of the data. The metrics included in these recipes have nice properties that make them flexible to various annotation situations: they can handle missing values (i.e. incomplete overlap), scale to any number of annotators, scale to any number of categories, and can be customized with your own weighting functions. In addition, the choice of metrics available within this package follow the recommendations in the literature[^2][^3], plus theoretical analysis[^4] demonstrating when certain metrics might be most useful.
+
+Table 13 in [this paper](https://scholar.google.com/scholar?cluster=17269958574032994585&hl=en&as_sdt=0,34&as_vis=1)[^4] highlights systematic issues with each metric. They are as follows:
+
+- **When there is _low agreement_**: Percent (Simple) Agreement can produce high scores.
+  - Imagine a binary classification problem with a very low base rate. Annotators can often agree on the negative case, but rarely agree on the positive.
+- **When there are _highly uneven sizes of categories_**: `AC2` can produce low scores, `Alpha` can produce high scores.
+- **When there are _N < 20_ co-incident annotated examples**: `Alpha` can produce high scores.
+  - You probably shouldn't trust _N < 100_ generally.
+- **When there are _3 or more categories_**: `AC2` can produce high scores.
+
+**Summary**: Use simple agreement and `Alpha`. If simple agreement is high, and `Alpha` is low, verify with `AC2`[^3]. In general these numbers correlate, if you're getting contradictory or unclear information increase the number of examples and explore your data.
+
+## Other Use-Cases / Use Outside Prodigy
+
+If you want to calculate these measures in a custom script on your own data, you can use `from prodigy_iaa.measures import calculate_agreement`. See tests in `tests/test_measures.py` for an example. The docstrings for each function should indicate the expected data structures.
+
+You could also use this, for example, to print out some nice output during an `update` callback and get annotation statistics as each user submits examples.
+
+If you want to calcualte more precise statistics, e.g. comparing two annotators pairwise, you could write a script to do that as well with these existing functions.
+
+
+## Tests
+
+Tests require a working version of `prodigy`, so they are not run in CI and must be run locally. 
+## References
+
+
+[^1]: K. L. Gwet, “On Krippendorff’s Alpha Coefficient,” p. 16, 2015.
+[^2]: J. Lovejoy, B. R. Watson, S. Lacy, and D. Riffe, “Three Decades of Reliability in Communication Content Analyses: Reporting of Reliability Statistics and Coefficient Levels in Three Top Journals,” p. 44.
+[^3]: S. Lacy, B. R. Watson, D. Riffe, and J. Lovejoy, “Issues and Best Practices in Content Analysis,” Journalism & Mass Communication Quarterly, vol. 92, no. 4, pp. 791–811, Dec. 2015, doi: 10.1177/1077699015607338.
+[^4]: X. Zhao, J. S. Liu, and K. Deng, “Assumptions Behind Intercoder Reliability Indices,” Communication Yearbook, p. 83.
```

