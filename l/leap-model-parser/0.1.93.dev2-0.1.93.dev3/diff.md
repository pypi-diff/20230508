# Comparing `tmp/leap_model_parser-0.1.93.dev2.tar.gz` & `tmp/leap_model_parser-0.1.93.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leap_model_parser-0.1.93.dev2.tar", max compression
+gzip compressed data, was "leap_model_parser-0.1.93.dev3.tar", max compression
```

## Comparing `leap_model_parser-0.1.93.dev2.tar` & `leap_model_parser-0.1.93.dev3.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1067 2022-02-10 15:52:31.114426 leap_model_parser-0.1.93.dev2/LICENSE
--rw-r--r--   0        0        0       68 2022-02-13 12:20:32.223194 leap_model_parser-0.1.93.dev2/README.md
--rw-r--r--   0        0        0      132 2022-05-26 14:22:41.518359 leap_model_parser-0.1.93.dev2/leap_model_parser/__init__.py
--rw-r--r--   0        0        0        0 2022-02-10 15:52:31.865328 leap_model_parser-0.1.93.dev2/leap_model_parser/contract/__init__.py
--rw-r--r--   0        0        0      691 2023-03-06 12:05:13.379795 leap_model_parser-0.1.93.dev2/leap_model_parser/contract/importmodelresponse.py
--rw-r--r--   0        0        0    44142 2023-05-02 07:42:26.775061 leap_model_parser-0.1.93.dev2/leap_model_parser/contract/nodedata.py
--rw-r--r--   0        0        0   421621 2023-05-02 07:42:26.773903 leap_model_parser-0.1.93.dev2/leap_model_parser/contract/ui_components.json
--rw-r--r--   0        0        0    15485 2023-04-02 14:14:25.101809 leap_model_parser-0.1.93.dev2/leap_model_parser/keras_json_model_import.py
--rw-r--r--   0        0        0     6766 2023-03-29 10:33:06.573801 leap_model_parser-0.1.93.dev2/leap_model_parser/model_parser.py
--rw-r--r--   0        0        0        0 2022-05-26 14:22:41.520554 leap_model_parser-0.1.93.dev2/leap_model_parser/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-05-26 14:22:41.520732 leap_model_parser-0.1.93.dev2/leap_model_parser/utils/layerpedia/__init__.py
--rw-r--r--   0        0        0     9291 2022-05-26 14:22:41.520971 leap_model_parser-0.1.93.dev2/leap_model_parser/utils/layerpedia/layerpedia.py
--rw-r--r--   0        0        0        1 2022-05-26 14:22:41.521197 leap_model_parser-0.1.93.dev2/leap_model_parser/utils/tlinspection/__init__.py
--rw-r--r--   0        0        0     2786 2022-05-26 14:22:41.521396 leap_model_parser-0.1.93.dev2/leap_model_parser/utils/tlinspection/leapinspection.py
--rw-r--r--   0        0        0      111 2022-05-26 14:22:41.521654 leap_model_parser-0.1.93.dev2/leap_model_parser/utils/uicomponents/__init__.py
--rw-r--r--   0        0        0     3035 2022-05-26 14:22:41.521847 leap_model_parser-0.1.93.dev2/leap_model_parser/utils/uicomponents/generatenodedata.py
--rw-r--r--   0        0        0     5799 2022-06-13 10:57:06.739900 leap_model_parser-0.1.93.dev2/leap_model_parser/utils/uicomponents/tensorflowinscpection.py
--rw-r--r--   0        0        0    19604 2023-04-30 15:00:43.099004 leap_model_parser-0.1.93.dev2/leap_model_parser/utils/uicomponents/ui_components_config.yaml
--rw-r--r--   0        0        0     1072 2023-05-02 07:47:53.236993 leap_model_parser-0.1.93.dev2/pyproject.toml
--rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 leap_model_parser-0.1.93.dev2/setup.py
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 leap_model_parser-0.1.93.dev2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-02-10 15:52:31.114426 leap_model_parser-0.1.93.dev3/LICENSE
+-rw-r--r--   0        0        0       68 2022-02-13 12:20:32.223194 leap_model_parser-0.1.93.dev3/README.md
+-rw-r--r--   0        0        0      132 2022-05-26 14:22:41.518359 leap_model_parser-0.1.93.dev3/leap_model_parser/__init__.py
+-rw-r--r--   0        0        0        0 2022-02-10 15:52:31.865328 leap_model_parser-0.1.93.dev3/leap_model_parser/contract/__init__.py
+-rw-r--r--   0        0        0      691 2023-03-06 12:05:13.379795 leap_model_parser-0.1.93.dev3/leap_model_parser/contract/importmodelresponse.py
+-rw-r--r--   0        0        0    44142 2023-05-02 07:42:26.775061 leap_model_parser-0.1.93.dev3/leap_model_parser/contract/nodedata.py
+-rw-r--r--   0        0        0   421621 2023-05-02 07:42:26.773903 leap_model_parser-0.1.93.dev3/leap_model_parser/contract/ui_components.json
+-rw-r--r--   0        0        0    15485 2023-04-02 14:14:25.101809 leap_model_parser-0.1.93.dev3/leap_model_parser/keras_json_model_import.py
+-rw-r--r--   0        0        0     6766 2023-03-29 10:33:06.573801 leap_model_parser-0.1.93.dev3/leap_model_parser/model_parser.py
+-rw-r--r--   0        0        0        0 2022-05-26 14:22:41.520554 leap_model_parser-0.1.93.dev3/leap_model_parser/utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-26 14:22:41.520732 leap_model_parser-0.1.93.dev3/leap_model_parser/utils/layerpedia/__init__.py
+-rw-r--r--   0        0        0     9291 2022-05-26 14:22:41.520971 leap_model_parser-0.1.93.dev3/leap_model_parser/utils/layerpedia/layerpedia.py
+-rw-r--r--   0        0        0        1 2022-05-26 14:22:41.521197 leap_model_parser-0.1.93.dev3/leap_model_parser/utils/tlinspection/__init__.py
+-rw-r--r--   0        0        0     2786 2022-05-26 14:22:41.521396 leap_model_parser-0.1.93.dev3/leap_model_parser/utils/tlinspection/leapinspection.py
+-rw-r--r--   0        0        0      111 2022-05-26 14:22:41.521654 leap_model_parser-0.1.93.dev3/leap_model_parser/utils/uicomponents/__init__.py
+-rw-r--r--   0        0        0     3035 2022-05-26 14:22:41.521847 leap_model_parser-0.1.93.dev3/leap_model_parser/utils/uicomponents/generatenodedata.py
+-rw-r--r--   0        0        0     5799 2022-06-13 10:57:06.739900 leap_model_parser-0.1.93.dev3/leap_model_parser/utils/uicomponents/tensorflowinscpection.py
+-rw-r--r--   0        0        0    19604 2023-04-30 15:00:43.099004 leap_model_parser-0.1.93.dev3/leap_model_parser/utils/uicomponents/ui_components_config.yaml
+-rw-r--r--   0        0        0     1072 2023-05-07 07:07:38.837689 leap_model_parser-0.1.93.dev3/pyproject.toml
+-rw-r--r--   0        0        0     1028 1970-01-01 00:00:00.000000 leap_model_parser-0.1.93.dev3/PKG-INFO
```

### Comparing `leap_model_parser-0.1.93.dev2/LICENSE` & `leap_model_parser-0.1.93.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.93.dev2/leap_model_parser/contract/importmodelresponse.py` & `leap_model_parser-0.1.93.dev3/leap_model_parser/contract/importmodelresponse.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.93.dev2/leap_model_parser/contract/nodedata.py` & `leap_model_parser-0.1.93.dev3/leap_model_parser/contract/nodedata.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.93.dev2/leap_model_parser/contract/ui_components.json` & `leap_model_parser-0.1.93.dev3/leap_model_parser/contract/ui_components.json`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.93.dev2/leap_model_parser/keras_json_model_import.py` & `leap_model_parser-0.1.93.dev3/leap_model_parser/keras_json_model_import.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.93.dev2/leap_model_parser/model_parser.py` & `leap_model_parser-0.1.93.dev3/leap_model_parser/model_parser.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.93.dev2/leap_model_parser/utils/layerpedia/layerpedia.py` & `leap_model_parser-0.1.93.dev3/leap_model_parser/utils/layerpedia/layerpedia.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.93.dev2/leap_model_parser/utils/tlinspection/leapinspection.py` & `leap_model_parser-0.1.93.dev3/leap_model_parser/utils/tlinspection/leapinspection.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.93.dev2/leap_model_parser/utils/uicomponents/generatenodedata.py` & `leap_model_parser-0.1.93.dev3/leap_model_parser/utils/uicomponents/generatenodedata.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.93.dev2/leap_model_parser/utils/uicomponents/tensorflowinscpection.py` & `leap_model_parser-0.1.93.dev3/leap_model_parser/utils/uicomponents/tensorflowinscpection.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.93.dev2/leap_model_parser/utils/uicomponents/ui_components_config.yaml` & `leap_model_parser-0.1.93.dev3/leap_model_parser/utils/uicomponents/ui_components_config.yaml`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.93.dev2/pyproject.toml` & `leap_model_parser-0.1.93.dev3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "leap-model-parser"
-version = "0.1.93.dev2"
+version = "0.1.93.dev3"
 description = ""
 authors = ["idan <idan.yogev@tensorleap.ai>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/tensorleap/leap-model-parser"
 homepage = "https://github.com/tensorleap/leap-model-parser"
 include = [
@@ -14,17 +14,17 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.12.0", markers = "platform_machine  == 'x86_64'"}
 tensorflow-macos = {version = "2.12.0", markers = "platform_machine  == 'arm64'"}
 numpy = "^1.22.3"
 onnx = "1.10.1"
-onnx2kerastl = "0.0.84.dev1"
-keras-data-format-converter = "0.1.15.dev1"
-leap-model-rebuilder = "0.1.6.dev2"
+onnx2kerastl = "0.0.84.dev2"
+keras-data-format-converter = "0.1.15.dev2"
+leap-model-rebuilder = "0.1.6.dev3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 mypy = "^0.941"
 grappa = "^1.0.1"
 pytest-cov = "^3.0.0"
 pytest-watch = "^4.2.0"
```

### Comparing `leap_model_parser-0.1.93.dev2/PKG-INFO` & `leap_model_parser-0.1.93.dev3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: leap-model-parser
-Version: 0.1.93.dev2
+Version: 0.1.93.dev3
 Summary: 
 Home-page: https://github.com/tensorleap/leap-model-parser
 License: MIT
 Author: idan
 Author-email: idan.yogev@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: keras-data-format-converter (==0.1.15.dev1)
-Requires-Dist: leap-model-rebuilder (==0.1.6.dev2)
+Requires-Dist: keras-data-format-converter (==0.1.15.dev2)
+Requires-Dist: leap-model-rebuilder (==0.1.6.dev3)
 Requires-Dist: numpy (>=1.22.3,<2.0.0)
 Requires-Dist: onnx (==1.10.1)
-Requires-Dist: onnx2kerastl (==0.0.84.dev1)
-Requires-Dist: tensorflow (==2.12.0); platform_machine == "x86_64"
-Requires-Dist: tensorflow-macos (==2.12.0); platform_machine == "arm64"
+Requires-Dist: onnx2kerastl (==0.0.84.dev2)
+Requires-Dist: tensorflow (==2.12.0) ; platform_machine == "x86_64"
+Requires-Dist: tensorflow-macos (==2.12.0) ; platform_machine == "arm64"
 Project-URL: Repository, https://github.com/tensorleap/leap-model-parser
 Description-Content-Type: text/markdown
 
 # Tensorleap model parser
 Used to parse model to the import format
```

