# Comparing `tmp/code-loader-0.2.8.tar.gz` & `tmp/code-loader-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code-loader-0.2.8.tar", max compression
+gzip compressed data, was "code-loader-0.2.9.tar", max compression
```

## Comparing `code-loader-0.2.8.tar` & `code-loader-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1067 2021-12-01 12:49:40.221608 code-loader-0.2.8/LICENSE
--rw-r--r--   0        0        0       63 2021-12-01 12:49:40.221888 code-loader-0.2.8/README.md
--rw-r--r--   0        0        0      131 2021-12-02 13:04:01.154724 code-loader-0.2.8/code_loader/__init__.py
--rw-r--r--   0        0        0        0 2021-12-01 12:49:40.222215 code-loader-0.2.8/code_loader/contract/__init__.py
--rw-r--r--   0        0        0     2335 2022-03-27 16:13:55.814631 code-loader-0.2.8/code_loader/contract/datasetclasses.py
--rw-r--r--   0        0        0     1073 2022-01-30 17:03:35.077863 code-loader-0.2.8/code_loader/contract/decoder_classes.py
--rw-r--r--   0        0        0      752 2022-01-30 17:03:35.078224 code-loader-0.2.8/code_loader/contract/enums.py
--rw-r--r--   0        0        0     1352 2022-03-27 16:06:31.786773 code-loader-0.2.8/code_loader/contract/responsedataclasses.py
--rw-r--r--   0        0        0      108 2021-12-02 13:04:01.155417 code-loader-0.2.8/code_loader/dataset_binder/__init__.py
--rw-r--r--   0        0        0     3204 2022-03-27 15:51:17.625404 code-loader-0.2.8/code_loader/dataset_binder/datasetbinder.py
--rw-r--r--   0        0        0     9205 2022-03-27 15:51:17.618246 code-loader-0.2.8/code_loader/datasetloader.py
--rw-r--r--   0        0        0        0 2022-01-02 09:30:24.026399 code-loader-0.2.8/code_loader/decoders/__init__.py
--rw-r--r--   0        0        0     2320 2022-01-11 15:15:30.813571 code-loader-0.2.8/code_loader/decoders/default_decoders.py
--rw-r--r--   0        0        0     1548 2022-01-02 09:30:24.027864 code-loader-0.2.8/code_loader/utils.py
--rw-r--r--   0        0        0      702 2022-03-27 16:07:12.820469 code-loader-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      797 2022-03-27 16:34:59.525914 code-loader-0.2.8/setup.py
--rw-r--r--   0        0        0      562 2022-03-27 16:34:59.526149 code-loader-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2021-12-01 12:49:40.221608 code-loader-0.2.9/LICENSE
+-rw-r--r--   0        0        0       63 2021-12-01 12:49:40.221888 code-loader-0.2.9/README.md
+-rw-r--r--   0        0        0      131 2021-12-02 13:04:01.154724 code-loader-0.2.9/code_loader/__init__.py
+-rw-r--r--   0        0        0        0 2021-12-01 12:49:40.222215 code-loader-0.2.9/code_loader/contract/__init__.py
+-rw-r--r--   0        0        0     2357 2022-03-28 13:14:06.363969 code-loader-0.2.9/code_loader/contract/datasetclasses.py
+-rw-r--r--   0        0        0     1073 2022-01-30 17:03:35.077863 code-loader-0.2.9/code_loader/contract/decoder_classes.py
+-rw-r--r--   0        0        0      752 2022-01-30 17:03:35.078224 code-loader-0.2.9/code_loader/contract/enums.py
+-rw-r--r--   0        0        0     1409 2022-03-28 13:14:06.364283 code-loader-0.2.9/code_loader/contract/responsedataclasses.py
+-rw-r--r--   0        0        0      108 2021-12-02 13:04:01.155417 code-loader-0.2.9/code_loader/dataset_binder/__init__.py
+-rw-r--r--   0        0        0     3410 2022-03-28 13:14:06.364597 code-loader-0.2.9/code_loader/dataset_binder/datasetbinder.py
+-rw-r--r--   0        0        0     9242 2022-03-28 13:14:06.364931 code-loader-0.2.9/code_loader/datasetloader.py
+-rw-r--r--   0        0        0        0 2022-01-02 09:30:24.026399 code-loader-0.2.9/code_loader/decoders/__init__.py
+-rw-r--r--   0        0        0     2320 2022-01-11 15:15:30.813571 code-loader-0.2.9/code_loader/decoders/default_decoders.py
+-rw-r--r--   0        0        0     1548 2022-01-02 09:30:24.027864 code-loader-0.2.9/code_loader/utils.py
+-rw-r--r--   0        0        0      702 2022-03-28 13:14:39.404244 code-loader-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      797 2022-03-29 08:59:48.662325 code-loader-0.2.9/setup.py
+-rw-r--r--   0        0        0      562 2022-03-29 08:59:48.662571 code-loader-0.2.9/PKG-INFO
```

### Comparing `code-loader-0.2.8/LICENSE` & `code-loader-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `code-loader-0.2.8/code_loader/contract/datasetclasses.py` & `code-loader-0.2.9/code_loader/contract/datasetclasses.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Any, Callable, List, Optional, Dict, Union
-from typing_extensions import Protocol
 
 import numpy as np  # type: ignore
 from dataclasses import dataclass, field
 
 from code_loader.contract.decoder_classes import LeapImage, LeapText, LeapNumeric, LeapGraph, LeapHorizontalBar, \
     LeapTextMask, LeapImageMask
 from code_loader.contract.enums import DataStateType, DatasetMetadataType, \
     DataStateEnum, LeapDataType
+from code_loader.contract.responsedataclasses import HeatmapBlockInstance
 
 
 @dataclass
 class PreprocessResponse:
     length: int
     data: Any
 
@@ -55,20 +55,14 @@
 
 @dataclass
 class InputHandler(DatasetBaseHandler):
     shape: Optional[List[int]] = None
 
 
 @dataclass
-class ConnectionInstance:
-    decoder_name: str
-    encoder_names: List[str]
-
-
-@dataclass
 class GroundTruthHandler(DatasetBaseHandler):
     shape: Optional[List[int]] = None
 
 
 @dataclass
 class MetadataHandler(DatasetBaseHandler):
     type: DatasetMetadataType
@@ -77,14 +71,15 @@
 @dataclass
 class DatasetIntegrationSetup:
     preprocess: Optional[PreprocessHandler] = None
     decoders: List[DecoderHandler] = field(default_factory=list)
     inputs: List[InputHandler] = field(default_factory=list)
     ground_truths: List[GroundTruthHandler] = field(default_factory=list)
     metadata: List[MetadataHandler] = field(default_factory=list)
+    heatmap_blocks: List[HeatmapBlockInstance] = field(default_factory=list)
 
 
 @dataclass
 class DatasetSample:
     inputs: Dict[str, np.ndarray]
     gt: Dict[str, np.ndarray]
     metadata: Dict[str, np.ndarray]
```

### Comparing `code-loader-0.2.8/code_loader/contract/decoder_classes.py` & `code-loader-0.2.9/code_loader/contract/decoder_classes.py`

 * *Files identical despite different names*

### Comparing `code-loader-0.2.8/code_loader/contract/enums.py` & `code-loader-0.2.9/code_loader/contract/enums.py`

 * *Files identical despite different names*

### Comparing `code-loader-0.2.8/code_loader/contract/responsedataclasses.py` & `code-loader-0.2.9/code_loader/contract/responsedataclasses.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import List, Optional, Dict
 
 from dataclasses import dataclass, field
 
-from code_loader.contract.datasetclasses import ConnectionInstance
 from code_loader.contract.enums import DatasetMetadataType, LeapDataType
 
 
 @dataclass
 class DatasetPreprocess:
     training_length: int
     validation_length: int
@@ -36,20 +35,27 @@
 @dataclass
 class DecoderInstance:
     name: str
     type: LeapDataType
 
 
 @dataclass
+class HeatmapBlockInstance:
+    name: str
+    labels: List[str]
+
+
+@dataclass
 class DatasetSetup:
     preprocess: DatasetPreprocess
     inputs: List[DatasetInputInstance]
     metadata: List[DatasetMetadataInstance]
     outputs: List[DatasetOutputInstance]
     decoders: List[DecoderInstance]
+    heatmap_blocks: List[HeatmapBlockInstance]
 
 
 @dataclass
 class DatasetTestResultPayload:
     name: str
     display: Dict[str, str] = field(default_factory=dict)
     is_passed: bool = True
```

### Comparing `code-loader-0.2.8/code_loader/dataset_binder/datasetbinder.py` & `code-loader-0.2.9/code_loader/dataset_binder/datasetbinder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from typing import Callable, List, Optional, Dict, Any, Union
+from typing import Callable, List, Optional, Dict, Any
 
 import numpy as np  # type: ignore
 
 from code_loader.contract.datasetclasses import SectionCallableInterface, InputHandler, \
     GroundTruthHandler, MetadataHandler, DatasetIntegrationSetup, DecoderHandler, PreprocessResponse, \
-    PreprocessHandler, DecoderCallableInterface, ConnectionInstance
+    PreprocessHandler, DecoderCallableInterface
 from code_loader.contract.enums import DatasetMetadataType, LeapDataType
+from code_loader.contract.responsedataclasses import HeatmapBlockInstance
 from code_loader.decoders.default_decoders import DefaultDecoder, default_numeric_decoder, default_graph_decoder, \
     default_image_decoder, default_horizontal_bar_decoder, default_word_decoder, \
     default_image_mask_decoder, default_text_mask_decoder
 from code_loader.utils import to_numpy_return_wrapper
 
 
 class DatasetBinder:
@@ -42,14 +43,17 @@
 
     def set_input(self, function: SectionCallableInterface, input_name: str) -> None:
         function = to_numpy_return_wrapper(function)
         self.setup_container.inputs.append(InputHandler(input_name, function))
 
         self._encoder_names.append(input_name)
 
+    def set_heatmap_block(self, name: str, labels: List[str]) -> None:
+        self.setup_container.heatmap_blocks.append(HeatmapBlockInstance(name, labels))
+
     def set_ground_truth(self, function: SectionCallableInterface, gt_name: str) -> None:
         function = to_numpy_return_wrapper(function)
         self.setup_container.ground_truths.append(GroundTruthHandler(gt_name, function))
 
         self._encoder_names.append(gt_name)
 
     def set_metadata(self, function: SectionCallableInterface,
```

### Comparing `code-loader-0.2.8/code_loader/datasetloader.py` & `code-loader-0.2.9/code_loader/datasetloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         metadata = [DatasetMetadataInstance(name=metadata.name, type=metadata.type)
                     for metadata in setup.metadata]
 
         decoders = [DecoderInstance(name=decoder_handler.name, type=decoder_handler.type)
                     for decoder_handler in setup.decoders]
 
         return DatasetSetup(preprocess=dataset_preprocess, inputs=inputs, outputs=ground_truths, metadata=metadata,
-                            decoders=decoders)
+                            decoders=decoders, heatmap_blocks=setup.heatmap_blocks)
 
     @lru_cache()
     def _preprocess_result(self) -> List[PreprocessResponse]:
         preprocess = global_dataset_binder.setup_container.preprocess
         # TODO: add caching of subset result
         assert preprocess is not None
         preprocess_result = preprocess.function()
```

### Comparing `code-loader-0.2.8/code_loader/decoders/default_decoders.py` & `code-loader-0.2.9/code_loader/decoders/default_decoders.py`

 * *Files identical despite different names*

### Comparing `code-loader-0.2.8/code_loader/utils.py` & `code-loader-0.2.9/code_loader/utils.py`

 * *Files identical despite different names*

### Comparing `code-loader-0.2.8/pyproject.toml` & `code-loader-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "code-loader"
-version = "0.2.8"
+version = "0.2.9"
 description = ""
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/tensorleap/code-loader"
 homepage = "https://github.com/tensorleap/code-loader"
 include = [
```

### Comparing `code-loader-0.2.8/setup.py` & `code-loader-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['dataclasses==0.8', 'numpy>=1.19.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'code-loader',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': '',
     'long_description': '# tensorleap code loader\nUsed to load user code to tensorleap \n',
     'author': 'dorhar',
     'author_email': 'doron.harnoy@tensorleap.ai',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/tensorleap/code-loader',
```

### Comparing `code-loader-0.2.8/PKG-INFO` & `code-loader-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-loader
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Home-page: https://github.com/tensorleap/code-loader
 License: MIT
 Author: dorhar
 Author-email: doron.harnoy@tensorleap.ai
 Requires-Python: >=3.6.1,<3.7
 Classifier: License :: OSI Approved :: MIT License
```

