# Comparing `tmp/spacy-to-hf-0.0.1.tar.gz` & `tmp/spacy-to-hf-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-to-hf-0.0.1.tar", last modified: Sat May  6 15:46:39 2023, max compression
+gzip compressed data, was "spacy-to-hf-0.0.2.tar", last modified: Mon May  8 17:33:10 2023, max compression
```

## Comparing `spacy-to-hf-0.0.1.tar` & `spacy-to-hf-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:46:39.618241 spacy-to-hf-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-06 15:46:17.000000 spacy-to-hf-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-06 15:46:39.618241 spacy-to-hf-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-06 15:46:17.000000 spacy-to-hf-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-06 15:46:17.000000 spacy-to-hf-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-06 15:46:39.618241 spacy-to-hf-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:46:39.614241 spacy-to-hf-0.0.1/spacy_to_hf/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-06 15:46:17.000000 spacy-to-hf-0.0.1/spacy_to_hf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-06 15:46:17.000000 spacy-to-hf-0.0.1/spacy_to_hf/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-06 15:46:17.000000 spacy-to-hf-0.0.1/spacy_to_hf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:46:39.618241 spacy-to-hf-0.0.1/spacy_to_hf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-06 15:46:39.000000 spacy-to-hf-0.0.1/spacy_to_hf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-06 15:46:39.000000 spacy-to-hf-0.0.1/spacy_to_hf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:46:39.000000 spacy-to-hf-0.0.1/spacy_to_hf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-06 15:46:39.000000 spacy-to-hf-0.0.1/spacy_to_hf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-06 15:46:39.000000 spacy-to-hf-0.0.1/spacy_to_hf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:46:39.618241 spacy-to-hf-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-06 15:46:17.000000 spacy-to-hf-0.0.1/tests/test_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:33:10.385719 spacy-to-hf-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 17:32:49.000000 spacy-to-hf-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-08 17:33:10.385719 spacy-to-hf-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-08 17:32:49.000000 spacy-to-hf-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-08 17:32:49.000000 spacy-to-hf-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-08 17:33:10.385719 spacy-to-hf-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:33:10.385719 spacy-to-hf-0.0.2/spacy_to_hf/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-08 17:32:49.000000 spacy-to-hf-0.0.2/spacy_to_hf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-08 17:32:49.000000 spacy-to-hf-0.0.2/spacy_to_hf/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-05-08 17:32:49.000000 spacy-to-hf-0.0.2/spacy_to_hf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:33:10.385719 spacy-to-hf-0.0.2/spacy_to_hf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-08 17:33:10.000000 spacy-to-hf-0.0.2/spacy_to_hf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-08 17:33:10.000000 spacy-to-hf-0.0.2/spacy_to_hf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:33:10.000000 spacy-to-hf-0.0.2/spacy_to_hf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-08 17:33:10.000000 spacy-to-hf-0.0.2/spacy_to_hf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 17:33:10.000000 spacy-to-hf-0.0.2/spacy_to_hf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:33:10.385719 spacy-to-hf-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-08 17:32:49.000000 spacy-to-hf-0.0.2/tests/test_conversion.py
```

### Comparing `spacy-to-hf-0.0.1/LICENSE` & `spacy-to-hf-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-to-hf-0.0.1/pyproject.toml` & `spacy-to-hf-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 license = {text = 'Apache 2.0'}
 description = "Spacy to HF converter"
 requires-python = ">=3.7"
 dependencies = [
     "spacy <3",
     "pytokenizations",
     "transformers",
+    "datasets",
     "flax"  # As the backend for transformers. Smaller/Faster than torch or tf
 ]
 [[project.authors]]
 name = "Ben Epstein"
 email = "ben.epstein97+spacy-hf@gmail.com"
 
 [project.optional-dependencies]
```

### Comparing `spacy-to-hf-0.0.1/spacy_to_hf/utils.py` & `spacy-to-hf-0.0.2/spacy_to_hf/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from typing import List
+from itertools import chain
+from typing import Dict, List
+
+from datasets import ClassLabel, Dataset, Sequence
 
 
 def next_token_is_same(tokens: List[List[int]], cur_idx: int, tok_num: int) -> bool:
     if cur_idx >= len(tokens) - 1:
         return False
     next_idx = cur_idx + 1
     return tok_num == tokens[next_idx][0]
@@ -124,7 +127,37 @@
             elif _is_last_tag(tag):
                 clean_tag = _handle_last_tag(tag, hf_to_spacy, cur_idx, tok_num)
 
             clean_hf_tags.append(clean_tag)
 
         hf_tags.extend(clean_hf_tags)
     return hf_tags
+
+
+def dict_to_dataset(hf_data: Dict[str, List[str]]) -> Dataset:
+    """Converts a dictionary of huggingface data into a well-formed Dataset
+
+    ex input:
+        {
+            "tokens": [["sentence", "1"], ["sentence", "Apple"]],
+            "ner_tags": [["U-word", "O"], ["U-word", "U-ORG"]]
+        }
+
+    This will create a huggingface dataset from the input, and also map the `ner_tags`
+    into a ClassLabel object which is required for training.
+    """
+    labels = sorted(set(chain.from_iterable(hf_data["ner_tags"])))
+    # O is typically the first tag. Move it there
+    if "O" in labels:
+        labels.remove("O")
+        labels.insert(0, "O")
+    ds = Dataset.from_dict(hf_data)
+    # https://github.com/python/mypy/issues/6239
+    class_label = Sequence(feature=ClassLabel(num_classes=len(labels), names=labels))
+    # First need to string index the ner_tags
+    label_to_idx = dict(zip(labels, range(len(labels))))
+    ds = ds.map(
+        lambda row: {"ner_tags": [label_to_idx[tag] for tag in row["ner_tags"]]}
+    )
+    # Then we can create the ClassLabel
+    ds = ds.cast_column("ner_tags", class_label)
+    return ds
```

### Comparing `spacy-to-hf-0.0.1/tests/test_conversion.py` & `spacy-to-hf-0.0.2/tests/test_conversion.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Dict, List
 
 import pytest
+from datasets import Dataset
 
 from spacy_to_hf import spacy_to_hf
 from tests.constants import (
     HF_TAGS_1,
     HF_TAGS_2,
     HF_TOKENS_1,
     HF_TOKENS_2,
@@ -24,14 +25,33 @@
     spacy_data: List[Dict], hf_tokens: List[str], hf_tags: List[str]
 ) -> None:
     hf_data = spacy_to_hf(spacy_data, "bert-base-cased")
     assert hf_data["tokens"][0] == hf_tokens
     assert hf_data["ner_tags"][0] == hf_tags
 
 
+@pytest.mark.parametrize(
+    "spacy_data,hf_tokens,hf_tags",
+    [
+        (SPACY_DATA_1, HF_TOKENS_1, HF_TAGS_1),
+        (SPACY_DATA_2, HF_TOKENS_2, HF_TAGS_2),
+    ],
+)
+def test_spacy_to_hf_as_dataset(
+    spacy_data: List[Dict], hf_tokens: List[str], hf_tags: List[str]
+) -> None:
+    hf_data = spacy_to_hf(spacy_data, "bert-base-cased", as_hf_dataset=True)
+    hf_non_o_tags = [i for i in hf_tags if i != "O"]
+    sorted_tags = ["O"] + sorted(set(hf_non_o_tags))
+    assert isinstance(hf_data, Dataset)
+    assert hf_data.features["ner_tags"].feature.names == sorted_tags
+    assert hf_data["tokens"][0] == hf_tokens
+    assert hf_data["ner_tags"][0] == [sorted_tags.index(tag) for tag in hf_tags]
+
+
 def test_spacy_to_hf_spans_not_list() -> None:
     spacy_data = [
         {
             "text": "I have a BSc (Bachelors of Computer Sciences) from NYU",
             "spans": dict(start=9, end=12, label="degree"),
         }
     ]
```

