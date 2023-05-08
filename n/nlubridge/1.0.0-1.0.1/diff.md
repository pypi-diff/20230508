# Comparing `tmp/nlubridge-1.0.0.tar.gz` & `tmp/nlubridge-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlubridge-1.0.0.tar", last modified: Fri Mar 10 14:08:04 2023, max compression
+gzip compressed data, was "nlubridge-1.0.1.tar", last modified: Mon May  8 12:56:19 2023, max compression
```

## Comparing `nlubridge-1.0.0.tar` & `nlubridge-1.0.1.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:08:04.658209 nlubridge-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-03-10 14:07:55.000000 nlubridge-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-10 14:07:55.000000 nlubridge-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-03-10 14:08:04.658209 nlubridge-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-03-10 14:07:55.000000 nlubridge-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:08:04.658209 nlubridge-1.0.0/nlubridge/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:08:04.658209 nlubridge-1.0.0/nlubridge/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/dataloaders/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/dataloaders/luis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/dataloaders/rasa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/dataloaders/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/dataloaders/watson_assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)    18334 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/nlu_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:08:04.658209 nlubridge-1.0.0/nlubridge/vendors/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/vendors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/vendors/char_ngram_intent_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:08:04.658209 nlubridge-1.0.0/nlubridge/vendors/config/
--rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/vendors/config/rasa_nlu_config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     3522 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/vendors/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/vendors/luis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10788 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/vendors/rasa.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7316 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/vendors/rasa2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7000 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/vendors/rasa3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/vendors/spacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/vendors/tfidf_intent_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/vendors/vendor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-03-10 14:07:55.000000 nlubridge-1.0.0/nlubridge/vendors/watson_assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:08:04.658209 nlubridge-1.0.0/nlubridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-03-10 14:08:04.000000 nlubridge-1.0.0/nlubridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-10 14:08:04.000000 nlubridge-1.0.0/nlubridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 14:08:04.000000 nlubridge-1.0.0/nlubridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-10 14:08:04.000000 nlubridge-1.0.0/nlubridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-10 14:08:04.000000 nlubridge-1.0.0/nlubridge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-10 14:07:55.000000 nlubridge-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-10 14:08:04.662209 nlubridge-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-03-10 14:07:55.000000 nlubridge-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:08:04.658209 nlubridge-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-03-10 14:07:55.000000 nlubridge-1.0.0/tests/test_dataset_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-03-10 14:07:55.000000 nlubridge-1.0.0/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-03-10 14:07:55.000000 nlubridge-1.0.0/tests/test_vendors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-10 14:07:55.000000 nlubridge-1.0.0/tests/test_watson_vendor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-03-10 14:07:55.000000 nlubridge-1.0.0/tests/test_watson_vendor_mocked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-03-10 14:07:55.000000 nlubridge-1.0.0/tests/testing_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:56:19.050644 nlubridge-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-08 12:56:05.000000 nlubridge-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 12:56:05.000000 nlubridge-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-05-08 12:56:19.050644 nlubridge-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-05-08 12:56:05.000000 nlubridge-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:56:19.046643 nlubridge-1.0.1/nlubridge/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:56:19.046643 nlubridge-1.0.1/nlubridge/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/dataloaders/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/dataloaders/luis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/dataloaders/rasa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/dataloaders/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/dataloaders/watson_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18334 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/nlu_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:56:19.050644 nlubridge-1.0.1/nlubridge/vendors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/char_ngram_intent_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:56:19.050644 nlubridge-1.0.1/nlubridge/vendors/config/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/config/rasa_nlu_config.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3522 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/luis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7122 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/rasa2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6715 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/rasa3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/spacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/tfidf_intent_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/watson_assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:56:19.046643 nlubridge-1.0.1/nlubridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-05-08 12:56:19.000000 nlubridge-1.0.1/nlubridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-08 12:56:19.000000 nlubridge-1.0.1/nlubridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:56:19.000000 nlubridge-1.0.1/nlubridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-08 12:56:19.000000 nlubridge-1.0.1/nlubridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 12:56:19.000000 nlubridge-1.0.1/nlubridge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-08 12:56:05.000000 nlubridge-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-08 12:56:19.050644 nlubridge-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-08 12:56:05.000000 nlubridge-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:56:19.050644 nlubridge-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-08 12:56:05.000000 nlubridge-1.0.1/tests/test_dataset_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-05-08 12:56:05.000000 nlubridge-1.0.1/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-08 12:56:05.000000 nlubridge-1.0.1/tests/test_vendors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-08 12:56:05.000000 nlubridge-1.0.1/tests/test_watson_vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-05-08 12:56:05.000000 nlubridge-1.0.1/tests/test_watson_vendor_mocked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-08 12:56:05.000000 nlubridge-1.0.1/tests/testing_data.py
```

### Comparing `nlubridge-1.0.0/LICENSE` & `nlubridge-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/PKG-INFO` & `nlubridge-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlubridge
-Version: 1.0.0
+Version: 1.0.1
 Summary: Provides a unified API to several popular intent recognition applications
 Home-page: https://github.com/telekom/nlu-bridge
 Author: Klaus-Peter Engelbrecht
 Author-email: k.engelbrecht@telekom.de
 Maintainer: Klaus-Peter Engelbrecht
 Project-URL: Bug Tracker, https://github.com/telekom/nlu-bridge/issues
 Project-URL: Source Code, https://github.com/telekom/nlu-bridge
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nlubridge Version: 1.0.0 Summary: Provides a
+Metadata-Version: 2.1 Name: nlubridge Version: 1.0.1 Summary: Provides a
 unified API to several popular intent recognition applications Home-page:
 https://github.com/telekom/nlu-bridge Author: Klaus-Peter Engelbrecht Author-
 email: k.engelbrecht@telekom.de Maintainer: Klaus-Peter Engelbrecht Project-
 URL: Bug Tracker, https://github.com/telekom/nlu-bridge/issues Project-URL:
 Source Code, https://github.com/telekom/nlu-bridge Project-URL: Contributing,
 https://github.com/telekom/nlu-bridge/blob/main/CONTRIBUTING.md Project-URL:
 Code of Conduct, https://github.com/telekom/nlu-bridge/blob/main/
```

### Comparing `nlubridge-1.0.0/README.md` & `nlubridge-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/nlubridge/__init__.py` & `nlubridge-1.0.1/nlubridge/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import sys
 from typing import TYPE_CHECKING
 
 from lazy_imports import LazyImporter
 
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 
 if TYPE_CHECKING:
     from .dataloaders.huggingface import from_huggingface  # noqa: F401
     from .dataloaders.luis import from_luis  # noqa: F401
     from .dataloaders.rasa import from_rasa, to_rasa  # noqa: F401, F811
     from .dataloaders.utils import from_csv, from_json  # noqa: F401
```

### Comparing `nlubridge-1.0.0/nlubridge/dataloaders/huggingface.py` & `nlubridge-1.0.1/nlubridge/dataloaders/huggingface.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/nlubridge/dataloaders/luis.py` & `nlubridge-1.0.1/nlubridge/dataloaders/luis.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/nlubridge/dataloaders/rasa.py` & `nlubridge-1.0.1/nlubridge/dataloaders/rasa.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) 2021 Ralf Kirchherr, Deutsche Telekom AG
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 from __future__ import annotations
 
 import pathlib
-from typing import Union
+from typing import Dict, List, Union
 
 from rasa.shared.data import get_data_files, is_nlu_file
 from rasa.shared.importers.utils import training_data_from_paths
 from rasa.shared.nlu.constants import (
     ENTITIES,
     ENTITY_ATTRIBUTE_END,
     ENTITY_ATTRIBUTE_START,
@@ -55,35 +55,49 @@
 
     texts = []
     intents = []
     entities = []
     for message in training_data.training_examples:
         texts.append(message.get(TEXT))
         intents.append(message.get(INTENT))
-        es = []
-        for e in message.get(ENTITIES, []):
-            entity = {
-                EntityKeys.TYPE: e.get(ENTITY_ATTRIBUTE_TYPE),
-                EntityKeys.START: e.get(ENTITY_ATTRIBUTE_START),
-                EntityKeys.END: e.get(ENTITY_ATTRIBUTE_END),
-            }
-            # Add any custom keys defined in the source structure
-            for key in e.keys():
-                if key not in [
-                    ENTITY_ATTRIBUTE_TYPE,
-                    ENTITY_ATTRIBUTE_START,
-                    ENTITY_ATTRIBUTE_END,
-                ]:
-                    entity[key] = e[key]
-            es.append(entity)
+        es = convert_entities_to_nludataset(message)
         entities.append(es)
 
     return NluDataset(texts, intents, entities)
 
 
+def convert_entities_to_nludataset(message: Message) -> List[Dict]:
+    """
+    Convert entity dicts from Rasa format to NluDataset format.
+
+    It will change the key names for entity type, start index and end index to those
+    used in NluDataset and keep all additional keys from the Rasa formatted entity.
+
+    :param message: A Rasa Message object
+    :return: list of entities (dicts) in new format
+    """
+    es = []
+    for e in message.get(ENTITIES, []):
+        entity = {
+            EntityKeys.TYPE: e.get(ENTITY_ATTRIBUTE_TYPE),
+            EntityKeys.START: e.get(ENTITY_ATTRIBUTE_START),
+            EntityKeys.END: e.get(ENTITY_ATTRIBUTE_END),
+        }
+        # Add any custom keys defined in the source structure
+        for key in e.keys():
+            if key not in [
+                ENTITY_ATTRIBUTE_TYPE,
+                ENTITY_ATTRIBUTE_START,
+                ENTITY_ATTRIBUTE_END,
+            ]:
+                entity[key] = e[key]
+        es.append(entity)
+    return es
+
+
 def to_rasa(
     dataset: NluDataset, filepath: Union[str, pathlib.Path], format: str = "yml"
 ):
     """
     Write dataset in Rasa's yml- or json-format.
 
     :param dataset: Dataset to be converted
```

### Comparing `nlubridge-1.0.0/nlubridge/dataloaders/utils.py` & `nlubridge-1.0.1/nlubridge/dataloaders/utils.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/nlubridge/datasets.py` & `nlubridge-1.0.1/nlubridge/datasets.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/nlubridge/nlu_dataset.py` & `nlubridge-1.0.1/nlubridge/nlu_dataset.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/nlubridge/vendors/__init__.py` & `nlubridge-1.0.1/nlubridge/vendors/__init__.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/nlubridge/vendors/char_ngram_intent_classifier.py` & `nlubridge-1.0.1/nlubridge/vendors/char_ngram_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/nlubridge/vendors/config/rasa_nlu_config.yml` & `nlubridge-1.0.1/nlubridge/vendors/config/rasa_nlu_config.yml`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/nlubridge/vendors/fasttext.py` & `nlubridge-1.0.1/nlubridge/vendors/fasttext.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/nlubridge/vendors/luis.py` & `nlubridge-1.0.1/nlubridge/vendors/luis.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/nlubridge/vendors/rasa2.py` & `nlubridge-1.0.1/nlubridge/vendors/rasa2.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     INTENT_RANKING_KEY,
     PREDICTED_CONFIDENCE_KEY,
     TEXT,
 )
 from rasa.shared.nlu.training_data.formats.rasa import RasaReader
 from rasa.shared.nlu.training_data.training_data import TrainingData
 
+from nlubridge.dataloaders.rasa import convert_entities_to_nludataset
 from nlubridge.nlu_dataset import EntityKeys, NBestKeys, NluDataset
 from nlubridge.vendors import Vendor
 
 
 DEFAULT_INTENT_RASA_CONFIG_PATH = os.path.join(
     pathlib.Path(__file__).parent.absolute(), "config", "rasa_nlu_config.yml"
 )
@@ -92,22 +93,15 @@
         n_best_lists: List[List[dict]] = []
         entities_list: List[List[dict]] = []
         if self._interpreter is None:
             raise Exception("Rasa2 classifier has to be trained first!")
         for text in dataset.texts:
             result = self._interpreter.parse(text)
             intent = result.get(INTENT, {}).get(INTENT_NAME_KEY)
-            entities = [
-                {
-                    EntityKeys.TYPE: e.get(ENTITY_ATTRIBUTE_TYPE),
-                    EntityKeys.START: e.get(ENTITY_ATTRIBUTE_START),
-                    EntityKeys.END: e.get(ENTITY_ATTRIBUTE_END),
-                }
-                for e in result.get(ENTITIES, [])
-            ]
+            entities = convert_entities_to_nludataset(result)
             nbest = [
                 {
                     NBestKeys.INTENT: ranked.get(INTENT_NAME_KEY),
                     NBestKeys.CONFIDENCE: ranked.get(PREDICTED_CONFIDENCE_KEY),
                 }
                 for ranked in result.get(INTENT_RANKING_KEY, [])
             ]
```

### Comparing `nlubridge-1.0.0/nlubridge/vendors/rasa3.py` & `nlubridge-1.0.1/nlubridge/vendors/rasa3.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,27 +10,23 @@
 from typing import List, Optional, Tuple, Union
 
 from rasa.core.agent import Agent
 from rasa.core.channels.channel import UserMessage
 from rasa.model import get_local_model
 from rasa.model_training import train_nlu
 from rasa.shared.nlu.constants import (
-    ENTITIES,
-    ENTITY_ATTRIBUTE_END,
-    ENTITY_ATTRIBUTE_START,
-    ENTITY_ATTRIBUTE_TYPE,
     INTENT,
     INTENT_NAME_KEY,
     INTENT_RANKING_KEY,
     PREDICTED_CONFIDENCE_KEY,
 )
 
-from nlubridge import EntityKeys, NBestKeys, NluDataset, to_rasa
-
-from .vendor import Vendor
+from nlubridge import NBestKeys, NluDataset, to_rasa
+from nlubridge.dataloaders.rasa import convert_entities_to_nludataset
+from nlubridge.vendors.vendor import Vendor
 
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_INTENT_RASA_CONFIG_PATH = os.path.join(
     pathlib.Path(__file__).parent.absolute(), "config", "rasa_nlu_config.yml"
 )
@@ -135,22 +131,15 @@
             raise RuntimeError("Rasa3 classifier has to be trained first!")
         intents = []
         n_best_lists = []
         entities_list = []
         for text in dataset.texts:
             result = self._parse_message(text)
             intent = result.get(INTENT, {}).get(INTENT_NAME_KEY)
-            entities = [
-                {
-                    EntityKeys.TYPE: e.get(ENTITY_ATTRIBUTE_TYPE),
-                    EntityKeys.START: e.get(ENTITY_ATTRIBUTE_START),
-                    EntityKeys.END: e.get(ENTITY_ATTRIBUTE_END),
-                }
-                for e in result.get(ENTITIES, [])
-            ]
+            entities = convert_entities_to_nludataset(result)
             nbest = [
                 {
                     NBestKeys.INTENT: ranked.get(INTENT_NAME_KEY),
                     NBestKeys.CONFIDENCE: ranked.get(PREDICTED_CONFIDENCE_KEY),
                 }
                 for ranked in result.get(INTENT_RANKING_KEY, [])
             ]
```

### Comparing `nlubridge-1.0.0/nlubridge/vendors/spacy.py` & `nlubridge-1.0.1/nlubridge/vendors/spacy.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/nlubridge/vendors/tfidf_intent_classifier.py` & `nlubridge-1.0.1/nlubridge/vendors/tfidf_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/nlubridge/vendors/vendor.py` & `nlubridge-1.0.1/nlubridge/vendors/vendor.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/nlubridge/vendors/watson_assistant.py` & `nlubridge-1.0.1/nlubridge/vendors/watson_assistant.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/nlubridge.egg-info/PKG-INFO` & `nlubridge-1.0.1/nlubridge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlubridge
-Version: 1.0.0
+Version: 1.0.1
 Summary: Provides a unified API to several popular intent recognition applications
 Home-page: https://github.com/telekom/nlu-bridge
 Author: Klaus-Peter Engelbrecht
 Author-email: k.engelbrecht@telekom.de
 Maintainer: Klaus-Peter Engelbrecht
 Project-URL: Bug Tracker, https://github.com/telekom/nlu-bridge/issues
 Project-URL: Source Code, https://github.com/telekom/nlu-bridge
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nlubridge Version: 1.0.0 Summary: Provides a
+Metadata-Version: 2.1 Name: nlubridge Version: 1.0.1 Summary: Provides a
 unified API to several popular intent recognition applications Home-page:
 https://github.com/telekom/nlu-bridge Author: Klaus-Peter Engelbrecht Author-
 email: k.engelbrecht@telekom.de Maintainer: Klaus-Peter Engelbrecht Project-
 URL: Bug Tracker, https://github.com/telekom/nlu-bridge/issues Project-URL:
 Source Code, https://github.com/telekom/nlu-bridge Project-URL: Contributing,
 https://github.com/telekom/nlu-bridge/blob/main/CONTRIBUTING.md Project-URL:
 Code of Conduct, https://github.com/telekom/nlu-bridge/blob/main/
```

### Comparing `nlubridge-1.0.0/nlubridge.egg-info/SOURCES.txt` & `nlubridge-1.0.1/nlubridge.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 nlubridge/dataloaders/rasa.py
 nlubridge/dataloaders/utils.py
 nlubridge/dataloaders/watson_assistant.py
 nlubridge/vendors/__init__.py
 nlubridge/vendors/char_ngram_intent_classifier.py
 nlubridge/vendors/fasttext.py
 nlubridge/vendors/luis.py
-nlubridge/vendors/rasa.py
 nlubridge/vendors/rasa2.py
 nlubridge/vendors/rasa3.py
 nlubridge/vendors/spacy.py
 nlubridge/vendors/tfidf_intent_classifier.py
 nlubridge/vendors/vendor.py
 nlubridge/vendors/watson_assistant.py
 nlubridge/vendors/config/rasa_nlu_config.yml
```

### Comparing `nlubridge-1.0.0/setup.py` & `nlubridge-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,18 +59,18 @@
     packages=find_packages(),
     python_requires=">=3, <3.9",
     install_requires=["scikit-learn", "python-dotenv", "lazy-imports", "ratelimit"],
     extras_require={
         "watson": ["ibm_watson", "tqdm", "requests"],
         "fasttext": ["fasttext"],
         "luis": ["requests", "ratelimit"],
-        "rasa2": ["rasa~=2.0"],
+        "rasa2": ["rasa~=2.0", "websockets~=10.4"],
         "rasa3": ["rasa~=3.0"],
         "spacy": ["spacy==3.1.3"],
-        "huggingface": ["datasets"],
+        "huggingface": ["datasets~=1.0"],
         "develop": [
             "pytest-cov",
             "pytest-mock",
             "flake8",
             "black",
             "pydocstyle",
             "setuptools",
```

### Comparing `nlubridge-1.0.0/tests/test_dataset_loaders.py` & `nlubridge-1.0.1/tests/test_dataset_loaders.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/tests/test_datasets.py` & `nlubridge-1.0.1/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/tests/test_vendors.py` & `nlubridge-1.0.1/tests/test_vendors.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/tests/test_watson_vendor.py` & `nlubridge-1.0.1/tests/test_watson_vendor.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/tests/test_watson_vendor_mocked.py` & `nlubridge-1.0.1/tests/test_watson_vendor_mocked.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.0/tests/testing_data.py` & `nlubridge-1.0.1/tests/testing_data.py`

 * *Files identical despite different names*

