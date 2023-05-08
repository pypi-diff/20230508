# Comparing `tmp/gradio_client-0.2.0.tar.gz` & `tmp/gradio_client-0.2.1.tar.gz`

## Comparing `gradio_client-0.2.0.tar` & `gradio_client-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.2.0/README.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.2.0/requirements.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.2.0/gradio_client/__init__.py
--rw-r--r--   0        0        0    46849 2020-02-02 00:00:00.000000 gradio_client-0.2.0/gradio_client/client.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.2.0/gradio_client/data_classes.py
--rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 gradio_client-0.2.0/gradio_client/documentation.py
--rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.2.0/gradio_client/media_data.py
--rw-r--r--   0        0        0    18574 2020-02-02 00:00:00.000000 gradio_client-0.2.0/gradio_client/serializing.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 gradio_client-0.2.0/gradio_client/types.json
--rw-r--r--   0        0        0    16272 2020-02-02 00:00:00.000000 gradio_client-0.2.0/gradio_client/utils.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.2.0/gradio_client/version.txt
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gradio_client-0.2.0/.gitignore
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 gradio_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.2.1/README.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.2.1/requirements.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.2.1/gradio_client/__init__.py
+-rw-r--r--   0        0        0    46849 2020-02-02 00:00:00.000000 gradio_client-0.2.1/gradio_client/client.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.2.1/gradio_client/data_classes.py
+-rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 gradio_client-0.2.1/gradio_client/documentation.py
+-rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.2.1/gradio_client/media_data.py
+-rw-r--r--   0        0        0    18591 2020-02-02 00:00:00.000000 gradio_client-0.2.1/gradio_client/serializing.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 gradio_client-0.2.1/gradio_client/types.json
+-rw-r--r--   0        0        0    16272 2020-02-02 00:00:00.000000 gradio_client-0.2.1/gradio_client/utils.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.2.1/gradio_client/version.txt
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gradio_client-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 gradio_client-0.2.1/PKG-INFO
```

### Comparing `gradio_client-0.2.0/README.md` & `gradio_client-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.0/gradio_client/client.py` & `gradio_client-0.2.1/gradio_client/client.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.0/gradio_client/documentation.py` & `gradio_client-0.2.1/gradio_client/documentation.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.0/gradio_client/media_data.py` & `gradio_client-0.2.1/gradio_client/media_data.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.0/gradio_client/serializing.py` & `gradio_client-0.2.1/gradio_client/serializing.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import uuid
 from pathlib import Path
 from typing import Any
 
 from gradio_client import media_data, utils
 from gradio_client.data_classes import FileData
 
-serializer_types = json.load(open(Path(__file__).parent / "types.json"))
+with open(Path(__file__).parent / "types.json") as f:
+    serializer_types = json.load(f)
 
 
 class Serializable:
     def serialized_info(self):
         """
         The typing information for this component as a dictionary whose values are a list of 2 strings: [Python type, language-agnostic description].
         Keys of the dictionary are: raw_input, raw_output, serialized_input, serialized_output
```

### Comparing `gradio_client-0.2.0/gradio_client/types.json` & `gradio_client-0.2.1/gradio_client/types.json`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.0/gradio_client/utils.py` & `gradio_client-0.2.1/gradio_client/utils.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.0/.gitignore` & `gradio_client-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.0/pyproject.toml` & `gradio_client-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.0/PKG-INFO` & `gradio_client-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradio_client
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python library for easily interacting with trained machine learning models
 Project-URL: Homepage, https://github.com/gradio-app/gradio
 Author-email: Abubakar Abid <team@gradio.app>, Ali Abid <team@gradio.app>, Ali Abdalla <team@gradio.app>, Dawood Khan <team@gradio.app>, Ahsen Khaliq <team@gradio.app>, Pete Allen <team@gradio.app>, Freddy Boulton <team@gradio.app>
 License-Expression: Apache-2.0
 Keywords: API,client,machine learning
 Requires-Python: >=3.7
 Requires-Dist: fsspec
```

