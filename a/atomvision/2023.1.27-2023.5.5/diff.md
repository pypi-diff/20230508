# Comparing `tmp/atomvision-2023.1.27.tar.gz` & `tmp/atomvision-2023.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomvision-2023.1.27.tar", last modified: Sat Jan 28 15:27:54 2023, max compression
+gzip compressed data, was "atomvision-2023.5.5.tar", last modified: Mon May  8 02:48:15 2023, max compression
```

## Comparing `atomvision-2023.1.27.tar` & `atomvision-2023.5.5.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-01-28 15:27:54.102857 atomvision-2023.1.27/
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2128 2022-09-14 16:07:02.000000 atomvision-2023.1.27/LICENSE.md
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5072 2023-01-28 15:27:54.102857 atomvision-2023.1.27/PKG-INFO
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4631 2023-01-28 14:56:04.000000 atomvision-2023.1.27/README.md
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-01-28 15:27:54.046852 atomvision-2023.1.27/atomvision/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       48 2023-01-28 15:23:27.000000 atomvision-2023.1.27/atomvision/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-01-28 15:27:54.062854 atomvision-2023.1.27/atomvision/data/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       36 2022-09-14 16:07:02.000000 atomvision-2023.1.27/atomvision/data/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3244 2022-11-21 02:00:04.000000 atomvision-2023.1.27/atomvision/data/graph.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    13492 2022-11-21 02:00:04.000000 atomvision-2023.1.27/atomvision/data/stem.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7333 2022-09-14 16:07:44.000000 atomvision-2023.1.27/atomvision/data/stemconv.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-01-28 15:27:54.074855 atomvision-2023.1.27/atomvision/models/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       42 2022-09-14 16:07:04.000000 atomvision-2023.1.27/atomvision/models/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7862 2022-11-21 02:00:05.000000 atomvision-2023.1.27/atomvision/models/alignn_classifier.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1667 2022-09-14 16:07:44.000000 atomvision-2023.1.27/atomvision/models/cnn_classifiers.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    12426 2022-09-14 16:07:44.000000 atomvision-2023.1.27/atomvision/models/gcn.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      586 2022-09-14 16:07:44.000000 atomvision-2023.1.27/atomvision/models/plotting.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1004 2022-09-14 16:07:44.000000 atomvision-2023.1.27/atomvision/models/segmentation_utils.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2105 2022-11-21 02:00:05.000000 atomvision-2023.1.27/atomvision/models/training_metrics.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5735 2022-11-21 02:00:05.000000 atomvision-2023.1.27/atomvision/models/training_utils.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-01-28 15:27:54.102857 atomvision-2023.1.27/atomvision/scripts/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       40 2022-09-14 16:07:04.000000 atomvision-2023.1.27/atomvision/scripts/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    11705 2022-11-21 02:00:05.000000 atomvision-2023.1.27/atomvision/scripts/focal_loss.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6315 2022-11-21 02:00:05.000000 atomvision-2023.1.27/atomvision/scripts/generate_stem.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6685 2022-11-21 02:00:05.000000 atomvision-2023.1.27/atomvision/scripts/image_to_graph.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2486 2022-11-21 02:33:33.000000 atomvision-2023.1.27/atomvision/scripts/stem_conv.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7577 2023-01-28 14:52:22.000000 atomvision-2023.1.27/atomvision/scripts/train_autoencoder.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7565 2022-10-25 03:13:54.000000 atomvision-2023.1.27/atomvision/scripts/train_autoencoder2.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    11089 2022-11-21 02:00:05.000000 atomvision-2023.1.27/atomvision/scripts/train_classifier_alignn.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    16250 2022-11-21 02:00:05.000000 atomvision-2023.1.27/atomvision/scripts/train_classifier_cnn.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    16585 2022-11-21 02:00:05.000000 atomvision-2023.1.27/atomvision/scripts/train_gan.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    20002 2022-11-21 02:00:05.000000 atomvision-2023.1.27/atomvision/scripts/train_gnn_old.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    17632 2022-11-21 02:00:05.000000 atomvision-2023.1.27/atomvision/scripts/train_segmentation.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6305 2023-01-28 14:59:22.000000 atomvision-2023.1.27/atomvision/scripts/train_tsne.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5779 2023-01-28 15:12:10.000000 atomvision-2023.1.27/atomvision/scripts/train_variational_autoencoder.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-01-28 15:27:54.054853 atomvision-2023.1.27/atomvision.egg-info/
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5072 2023-01-28 15:27:53.000000 atomvision-2023.1.27/atomvision.egg-info/PKG-INFO
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1134 2023-01-28 15:27:53.000000 atomvision-2023.1.27/atomvision.egg-info/SOURCES.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)        1 2023-01-28 15:27:53.000000 atomvision-2023.1.27/atomvision.egg-info/dependency_links.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)      442 2023-01-28 15:27:53.000000 atomvision-2023.1.27/atomvision.egg-info/requires.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)       11 2023-01-28 15:27:53.000000 atomvision-2023.1.27/atomvision.egg-info/top_level.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)       38 2023-01-28 15:27:54.102857 atomvision-2023.1.27/setup.cfg
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1812 2023-01-28 15:23:14.000000 atomvision-2023.1.27/setup.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-05-08 02:48:15.258959 atomvision-2023.5.5/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2128 2023-05-07 14:06:49.000000 atomvision-2023.5.5/LICENSE.md
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5108 2023-05-08 02:48:15.258959 atomvision-2023.5.5/PKG-INFO
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4631 2023-05-07 14:06:49.000000 atomvision-2023.5.5/README.md
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-05-08 02:48:15.174960 atomvision-2023.5.5/atomvision/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2023-05-07 14:12:03.000000 atomvision-2023.5.5/atomvision/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-05-08 02:48:15.198959 atomvision-2023.5.5/atomvision/data/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       36 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/data/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3244 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/data/graph.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    13492 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/data/stem.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     7333 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/data/stemconv.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-05-08 02:48:15.222959 atomvision-2023.5.5/atomvision/models/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       42 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/models/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     7862 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/models/alignn_classifier.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1667 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/models/cnn_classifiers.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    12426 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/models/gcn.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      586 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/models/plotting.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1004 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/models/segmentation_utils.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2105 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/models/training_metrics.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5735 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/models/training_utils.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-05-08 02:48:15.254959 atomvision-2023.5.5/atomvision/scripts/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       40 2023-05-07 14:06:50.000000 atomvision-2023.5.5/atomvision/scripts/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    11705 2023-05-07 14:06:50.000000 atomvision-2023.5.5/atomvision/scripts/focal_loss.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6315 2023-05-07 14:06:50.000000 atomvision-2023.5.5/atomvision/scripts/generate_stem.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6685 2023-05-07 14:06:50.000000 atomvision-2023.5.5/atomvision/scripts/image_to_graph.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2508 2023-05-07 14:24:30.000000 atomvision-2023.5.5/atomvision/scripts/stem_conv.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     7599 2023-05-07 14:24:09.000000 atomvision-2023.5.5/atomvision/scripts/train_autoencoder.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    11111 2023-05-07 14:23:19.000000 atomvision-2023.5.5/atomvision/scripts/train_classifier_alignn.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    17467 2023-05-07 14:23:04.000000 atomvision-2023.5.5/atomvision/scripts/train_classifier_cnn.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    16607 2023-05-07 14:23:59.000000 atomvision-2023.5.5/atomvision/scripts/train_gan.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    20002 2023-05-07 14:06:50.000000 atomvision-2023.5.5/atomvision/scripts/train_gnn_old.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    17654 2023-05-07 14:24:22.000000 atomvision-2023.5.5/atomvision/scripts/train_segmentation.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6327 2023-05-07 14:23:52.000000 atomvision-2023.5.5/atomvision/scripts/train_tsne.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5779 2023-05-07 14:06:50.000000 atomvision-2023.5.5/atomvision/scripts/train_variational_autoencoder.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-05-08 02:48:15.186960 atomvision-2023.5.5/atomvision.egg-info/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5108 2023-05-08 02:48:14.000000 atomvision-2023.5.5/atomvision.egg-info/PKG-INFO
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1093 2023-05-08 02:48:15.000000 atomvision-2023.5.5/atomvision.egg-info/SOURCES.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        1 2023-05-08 02:48:14.000000 atomvision-2023.5.5/atomvision.egg-info/dependency_links.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      442 2023-05-08 02:48:14.000000 atomvision-2023.5.5/atomvision.egg-info/requires.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       11 2023-05-08 02:48:14.000000 atomvision-2023.5.5/atomvision.egg-info/top_level.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       38 2023-05-08 02:48:15.262959 atomvision-2023.5.5/setup.cfg
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1811 2023-05-07 14:22:28.000000 atomvision-2023.5.5/setup.py
```

### Comparing `atomvision-2023.1.27/LICENSE.md` & `atomvision-2023.5.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `atomvision-2023.1.27/PKG-INFO` & `atomvision-2023.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: atomvision
-Version: 2023.1.27
+Version: 2023.5.5
 Summary: atomvision
 Home-page: https://github.com/usnistgov/atomvision
 Author: Kamal Choudhary, Brian DeCost
 Author-email: kamal.choudhary@nist.gov
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
@@ -154,7 +156,9 @@
 NIST-MGI (https://www.nist.gov/mgi).
 
 Code of conduct
 --------------------
 
 Please see [Code of conduct](https://github.com/usnistgov/jarvis/blob/master/CODE_OF_CONDUCT.md)
 
+
+
```

### Comparing `atomvision-2023.1.27/README.md` & `atomvision-2023.5.5/README.md`

 * *Files identical despite different names*

### Comparing `atomvision-2023.1.27/atomvision/data/graph.py` & `atomvision-2023.5.5/atomvision/data/graph.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.1.27/atomvision/data/stem.py` & `atomvision-2023.5.5/atomvision/data/stem.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.1.27/atomvision/data/stemconv.py` & `atomvision-2023.5.5/atomvision/data/stemconv.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.1.27/atomvision/models/alignn_classifier.py` & `atomvision-2023.5.5/atomvision/models/alignn_classifier.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.1.27/atomvision/models/cnn_classifiers.py` & `atomvision-2023.5.5/atomvision/models/cnn_classifiers.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.1.27/atomvision/models/gcn.py` & `atomvision-2023.5.5/atomvision/models/gcn.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.1.27/atomvision/models/plotting.py` & `atomvision-2023.5.5/atomvision/models/plotting.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.1.27/atomvision/models/segmentation_utils.py` & `atomvision-2023.5.5/atomvision/models/segmentation_utils.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.1.27/atomvision/models/training_metrics.py` & `atomvision-2023.5.5/atomvision/models/training_metrics.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.1.27/atomvision/models/training_utils.py` & `atomvision-2023.5.5/atomvision/models/training_utils.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.1.27/atomvision/scripts/focal_loss.py` & `atomvision-2023.5.5/atomvision/scripts/focal_loss.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.1.27/atomvision/scripts/generate_stem.py` & `atomvision-2023.5.5/atomvision/scripts/generate_stem.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.1.27/atomvision/scripts/image_to_graph.py` & `atomvision-2023.5.5/atomvision/scripts/image_to_graph.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.1.27/atomvision/scripts/stem_conv.py` & `atomvision-2023.5.5/atomvision/scripts/stem_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python
 from atomvision.data.stemconv import STEMConv
 import sys
 import argparse
 from jarvis.core.atoms import Atoms
 import matplotlib.pyplot as plt
 from jarvis.analysis.defects.surface import Surface
```

### Comparing `atomvision-2023.1.27/atomvision/scripts/train_autoencoder.py` & `atomvision-2023.5.5/atomvision/scripts/train_autoencoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python
 """Module for PyTorch autoencoder training."""
 import torch
 import torchvision
 import torchvision.transforms as transforms
 import torchvision.datasets as datasets
 import torch.nn as nn
 import torch.optim as optim
```

### Comparing `atomvision-2023.1.27/atomvision/scripts/train_classifier_alignn.py` & `atomvision-2023.5.5/atomvision/scripts/train_classifier_alignn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python
 """Module for ALIGNN Image Classifier."""
 import numpy as np
 from jarvis.db.figshare import data
 from atomvision.data.stem import write_image_directory
 import os
 from alignn.models import alignn
 from atomvision.data.graph import GraphDataset
```

### Comparing `atomvision-2023.1.27/atomvision/scripts/train_classifier_cnn.py` & `atomvision-2023.5.5/atomvision/scripts/train_classifier_cnn.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
+#!/usr/bin/env python
 """Module to train image classification models."""
 import torch
 import torchvision.transforms as transforms
 import torchvision.datasets as datasets
 import torch.nn as nn
 import torch.optim as optim
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
+import os
 import sys
 import random
 import argparse
 import ignite
 from ignite.engine import (
     Events,
     create_supervised_trainer,
     create_supervised_evaluator,
 )
 from ignite.metrics import Accuracy, Loss, RunningAverage, ConfusionMatrix
-
-# from ignite.handlers import ModelCheckpoint, EarlyStopping
 from ignite.handlers import EarlyStopping
 from ignite.handlers import Checkpoint, DiskSaver
 from atomvision.models.cnn_classifiers import (
     densenet,
     googlenet,
     vgg,
     mobilenet,
@@ -41,14 +41,15 @@
     ALIGNNConfig,
     MLPLayer,
     ALIGNNConv,
     EdgeGatedGraphConv,
 )
 from dgl.nn import AvgPooling
 from alignn.models.utils import RBFExpansion
+from sklearn.metrics import confusion_matrix
 
 # import dgl
 # import dgl.function as fn
 # import numpy as np
 # import torch
 # from dgl.nn.functional import edge_softmax
 # from pydantic.typing import Literal
@@ -398,15 +399,16 @@
     # creating trainer,evaluator
     trainer = create_supervised_trainer(
         model, optimizer, criterion, device=device
     )
     metrics = {
         "accuracy": Accuracy(),
         "nll": Loss(criterion),
-        "cm": ConfusionMatrix(num_classes=5),
+        "cm": ConfusionMatrix(num_classes=int(args.num_classes)),
+        # "cm": ConfusionMatrix(num_classes=5),
     }
     train_evaluator = create_supervised_evaluator(
         model, metrics=metrics, device=device
     )
     val_evaluator = create_supervised_evaluator(
         model, metrics=metrics, device=device
     )
@@ -452,21 +454,22 @@
                 trainer.state.epoch, accuracy, loss
             )
         )
 
     trainer.add_event_handler(Events.EPOCH_COMPLETED, log_validation_results)
 
     @trainer.on(Events.COMPLETED)
-    def log_confusion_matrix(trainer):
+    def og_confusion_matrix(trainer):
         val_evaluator.run(val_loader)
         metrics = val_evaluator.state.metrics
         cm = metrics["cm"]
         cm = cm.numpy()
         cm = cm.astype(int)
-        classes = ["0", "1", "2", "3", "4"]
+        classes = val_loader.dataset.classes
+        # classes = ["0", "1", "2", "3", "4"]
         plt.rcParams.update({"font.size": 20})
         fig, ax = plt.subplots(figsize=(16, 16))
         ax = plt.subplot()
         cm1 = cm / cm.sum(axis=1)[:, np.newaxis]
         sns.heatmap(
             cm1,
             annot=True,
@@ -516,7 +519,41 @@
     plt.plot(training_history["loss"], label="Training Loss")
     plt.plot(validation_history["loss"], label="Validation Loss")
     plt.xlabel("No. of Epochs")
     plt.ylabel("Loss")
     plt.legend(frameon=False)
     plt.savefig("Loss.png")
     plt.close()
+
+    f = open(
+        os.path.join(output_dir, "prediction_results_test_set.csv"),
+        "w",
+    )
+    f.write("id,target,prediction\n")
+    targets = []
+    predictions = []
+    with torch.no_grad():
+        ids = [os.path.basename(i[0]) for i in val_loader.dataset.imgs]
+        for dat, id in zip(val_dataset, ids):
+            # print (dat[0],dat[0].shape,type(dat[0]))
+            # print (id,model([dat[0].to(device)]))
+            pred = (
+                torch.argmax(model(dat[0][None, :].to(device)))
+                .cpu()
+                .detach()
+                .numpy()
+            )
+            target = dat[1]  # .numpy()
+            targets.append(dat[1])
+            predictions.append(pred)
+            # print(id,pred,target,(pred))
+            f.write("%s, %d, %d\n" % (id, target, pred))
+    cm_sk = np.array(
+        confusion_matrix(
+            targets,
+            predictions,
+            labels=np.arange(int(args.num_classes), dtype="int"),
+        )
+    )
+    cm_sk1 = cm_sk / cm_sk.sum(axis=1)[:, np.newaxis]
+    # print("cm_sk", cm_sk1)
+    f.close()
```

### Comparing `atomvision-2023.1.27/atomvision/scripts/train_gan.py` & `atomvision-2023.5.5/atomvision/scripts/train_gan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python
 """Module to train GAN."""
 # https://www.kaggle.com/code/balraj98/
 # single-image-super-resolution-gan-srgan-pytorch
 import numpy as np
 import os
 import sys
 import glob
```

### Comparing `atomvision-2023.1.27/atomvision/scripts/train_gnn_old.py` & `atomvision-2023.5.5/atomvision/scripts/train_gnn_old.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.1.27/atomvision/scripts/train_segmentation.py` & `atomvision-2023.5.5/atomvision/scripts/train_segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python
 """Module to perform segmentation on atomistic dataset."""
 import torch
 import os
 from segmentation_models_pytorch.encoders import get_preprocessing_fn
 from jarvis.core.lattice import get_2d_lattice
 import numpy as np
 import pandas as pd
```

### Comparing `atomvision-2023.1.27/atomvision/scripts/train_tsne.py` & `atomvision-2023.5.5/atomvision/scripts/train_tsne.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python
 """Module to perform t-SNE on imamges."""
 import sys
 import argparse
 import cv2
 import torchvision.datasets as dset
 from sklearn.manifold import TSNE
 import numpy as np
```

### Comparing `atomvision-2023.1.27/atomvision/scripts/train_variational_autoencoder.py` & `atomvision-2023.5.5/atomvision/scripts/train_variational_autoencoder.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.1.27/atomvision.egg-info/PKG-INFO` & `atomvision-2023.5.5/atomvision.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: atomvision
-Version: 2023.1.27
+Version: 2023.5.5
 Summary: atomvision
 Home-page: https://github.com/usnistgov/atomvision
 Author: Kamal Choudhary, Brian DeCost
 Author-email: kamal.choudhary@nist.gov
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
@@ -154,7 +156,9 @@
 NIST-MGI (https://www.nist.gov/mgi).
 
 Code of conduct
 --------------------
 
 Please see [Code of conduct](https://github.com/usnistgov/jarvis/blob/master/CODE_OF_CONDUCT.md)
 
+
+
```

### Comparing `atomvision-2023.1.27/atomvision.egg-info/SOURCES.txt` & `atomvision-2023.5.5/atomvision.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 atomvision/models/training_utils.py
 atomvision/scripts/__init__.py
 atomvision/scripts/focal_loss.py
 atomvision/scripts/generate_stem.py
 atomvision/scripts/image_to_graph.py
 atomvision/scripts/stem_conv.py
 atomvision/scripts/train_autoencoder.py
-atomvision/scripts/train_autoencoder2.py
 atomvision/scripts/train_classifier_alignn.py
 atomvision/scripts/train_classifier_cnn.py
 atomvision/scripts/train_gan.py
 atomvision/scripts/train_gnn_old.py
 atomvision/scripts/train_segmentation.py
 atomvision/scripts/train_tsne.py
 atomvision/scripts/train_variational_autoencoder.py
```

### Comparing `atomvision-2023.1.27/setup.py` & `atomvision-2023.5.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="atomvision",
-    version="2023.1.27",
+    version="2023.5.5",
     author="Kamal Choudhary, Brian DeCost",
     author_email="kamal.choudhary@nist.gov",
     description="atomvision",
     install_requires=[
         "numpy>=1.19.5",
         "scipy>=1.6.3",
         "jarvis-tools>=2021.07.19",
         "alignn>=2022.10.23",
         "beautifulsoup4>=4.11.1",
         "scikit-image>=0.19.3",
-        "torch==1.12.0",
+        "torch>=1.12.0",
         "pyparsing==2.2.1",
         "opencv-python>=4.6.0.66",
         "typer",
         "python-dotenv",
         "segmentation-models-pytorch>=0.2.1",
         # "torchvision>=0.10.0+cu111",
         "Pillow>=9.2.0",
-        "torchvision==0.13.0",
+        "torchvision>=0.13.0",
         "scikit-learn>=0.24.1",
         "matplotlib>=3.4.1",
         "seaborn>=0.11.2",
         "tqdm>=4.60.0",
-        "pandas==1.2.4",
-        "pytorch-ignite==0.5.0.dev20221024",
-        "pydantic>=1.8.1",
+        "pandas>=1.2.4",
+        "pytorch-ignite>=0.5.0.dev20221024",
+        "pydantic==1.8.1",
         "flake8>=3.9.1",
         "pycodestyle>=2.7.0",
         "pydocstyle>=6.0.0",
     ],
     scripts=[
         "atomvision/scripts/train_tsne.py",
         "atomvision/scripts/train_gan.py",
```

