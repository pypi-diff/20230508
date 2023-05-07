# Comparing `tmp/xztrainer-0.9.5.tar.gz` & `tmp/xztrainer-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xztrainer-0.9.5.tar", max compression
+gzip compressed data, was "xztrainer-0.9.6.tar", max compression
```

## Comparing `xztrainer-0.9.5.tar` & `xztrainer-0.9.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      894 2023-04-23 16:11:10.258766 xztrainer-0.9.5/pyproject.toml
--rw-r--r--   0        0        0       46 1970-01-01 00:00:00.000000 xztrainer-0.9.5/src/xztrainer/__init__.py
--rw-r--r--   0        0        0      256 2023-03-14 15:54:26.631822 xztrainer-0.9.5/src/xztrainer/functional.py
--rw-r--r--   0        0        0     1414 1970-01-01 00:00:00.000000 xztrainer-0.9.5/src/xztrainer/logger/__init__.py
--rw-r--r--   0        0        0     1590 1970-01-01 00:00:00.000000 xztrainer-0.9.5/src/xztrainer/logger/compose.py
--rw-r--r--   0        0        0      384 1970-01-01 00:00:00.000000 xztrainer-0.9.5/src/xztrainer/logger/null.py
--rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 xztrainer-0.9.5/src/xztrainer/logger/stream.py
--rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 xztrainer-0.9.5/src/xztrainer/logger/tensorboard.py
--rw-r--r--   0        0        0     1614 2023-04-23 16:06:34.685368 xztrainer-0.9.5/src/xztrainer/model.py
--rw-r--r--   0        0        0      743 2023-03-10 15:49:26.715934 xztrainer-0.9.5/src/xztrainer/rng.py
--rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 xztrainer-0.9.5/src/xztrainer/sampler.py
--rw-r--r--   0        0        0      409 2023-03-10 15:49:26.707934 xztrainer-0.9.5/src/xztrainer/setup_helper.py
--rw-r--r--   0        0        0    24069 2023-04-23 16:12:03.787658 xztrainer-0.9.5/src/xztrainer/xztrainer.py
--rw-r--r--   0        0        0      908 1970-01-01 00:00:00.000000 xztrainer-0.9.5/setup.py
--rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 xztrainer-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0      894 2023-05-07 23:51:55.750566 xztrainer-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0       46 1970-01-01 00:00:00.000000 xztrainer-0.9.6/src/xztrainer/__init__.py
+-rw-r--r--   0        0        0      256 2023-03-14 15:54:26.631822 xztrainer-0.9.6/src/xztrainer/functional.py
+-rw-r--r--   0        0        0     1414 1970-01-01 00:00:00.000000 xztrainer-0.9.6/src/xztrainer/logger/__init__.py
+-rw-r--r--   0        0        0     1590 1970-01-01 00:00:00.000000 xztrainer-0.9.6/src/xztrainer/logger/compose.py
+-rw-r--r--   0        0        0      384 1970-01-01 00:00:00.000000 xztrainer-0.9.6/src/xztrainer/logger/null.py
+-rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 xztrainer-0.9.6/src/xztrainer/logger/stream.py
+-rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 xztrainer-0.9.6/src/xztrainer/logger/tensorboard.py
+-rw-r--r--   0        0        0     1652 2023-05-07 23:51:35.263746 xztrainer-0.9.6/src/xztrainer/model.py
+-rw-r--r--   0        0        0      743 2023-03-10 15:49:26.715934 xztrainer-0.9.6/src/xztrainer/rng.py
+-rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 xztrainer-0.9.6/src/xztrainer/sampler.py
+-rw-r--r--   0        0        0      409 2023-03-10 15:49:26.707934 xztrainer-0.9.6/src/xztrainer/setup_helper.py
+-rw-r--r--   0        0        0    24069 2023-04-23 16:12:03.787658 xztrainer-0.9.6/src/xztrainer/xztrainer.py
+-rw-r--r--   0        0        0      908 1970-01-01 00:00:00.000000 xztrainer-0.9.6/setup.py
+-rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 xztrainer-0.9.6/PKG-INFO
```

### Comparing `xztrainer-0.9.5/pyproject.toml` & `xztrainer-0.9.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xztrainer"
-version = "0.9.5"
+version = "0.9.6"
 description = "A customizable training pipeline for PyTorch"
 authors = ["Maxim Afanasyev <mr.applexz@gmail.com>"]
 license = "MPL-2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 tqdm = ">=4.62.3"
```

### Comparing `xztrainer-0.9.5/src/xztrainer/logger/__init__.py` & `xztrainer-0.9.6/src/xztrainer/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.5/src/xztrainer/logger/compose.py` & `xztrainer-0.9.6/src/xztrainer/logger/compose.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.5/src/xztrainer/logger/stream.py` & `xztrainer-0.9.6/src/xztrainer/logger/stream.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.5/src/xztrainer/logger/tensorboard.py` & `xztrainer-0.9.6/src/xztrainer/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.5/src/xztrainer/model.py` & `xztrainer-0.9.6/src/xztrainer/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import multiprocessing
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from enum import Enum
 from typing import Protocol, Callable, List, Optional, Any, Union, Tuple
 
 from torch import nn, dtype
 from torch.optim import Optimizer
 from torch.utils.data.dataloader import default_collate
 
@@ -51,8 +51,8 @@
     print_steps: int = 100
     eval_steps: int = 0
     skip_nan_loss: bool = True
     save_steps: int = 100
     save_keep_n: int = -1
     save_dir: str = 'checkpoint'
     collate_fn: Callable[[List[object]], Any] = default_collate
-    logger: LoggingEngineConfig = StreamLoggingEngineConfig()
+    logger: LoggingEngineConfig = field(default_factory=lambda: StreamLoggingEngineConfig())
```

### Comparing `xztrainer-0.9.5/src/xztrainer/rng.py` & `xztrainer-0.9.6/src/xztrainer/rng.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.5/src/xztrainer/sampler.py` & `xztrainer-0.9.6/src/xztrainer/sampler.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.5/src/xztrainer/xztrainer.py` & `xztrainer-0.9.6/src/xztrainer/xztrainer.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.5/setup.py` & `xztrainer-0.9.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 extras_require = \
 {'numpy': ['numpy>=1.24.2'],
  'tensorboard': ['tensorboard>=2.8.0'],
  'torch': ['torch>=1.10.0']}
 
 setup_kwargs = {
     'name': 'xztrainer',
-    'version': '0.9.5',
+    'version': '0.9.6',
     'description': 'A customizable training pipeline for PyTorch',
     'long_description': 'None',
     'author': 'Maxim Afanasyev',
     'author_email': 'mr.applexz@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `xztrainer-0.9.5/PKG-INFO` & `xztrainer-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xztrainer
-Version: 0.9.5
+Version: 0.9.6
 Summary: A customizable training pipeline for PyTorch
 License: MPL-2.0
 Author: Maxim Afanasyev
 Author-email: mr.applexz@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

