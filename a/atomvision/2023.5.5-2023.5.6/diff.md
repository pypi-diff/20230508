# Comparing `tmp/atomvision-2023.5.5.tar.gz` & `tmp/atomvision-2023.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomvision-2023.5.5.tar", last modified: Mon May  8 02:48:15 2023, max compression
+gzip compressed data, was "atomvision-2023.5.6.tar", last modified: Mon May  8 03:09:17 2023, max compression
```

## Comparing `atomvision-2023.5.5.tar` & `atomvision-2023.5.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-05-08 02:48:15.258959 atomvision-2023.5.5/
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2128 2023-05-07 14:06:49.000000 atomvision-2023.5.5/LICENSE.md
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5108 2023-05-08 02:48:15.258959 atomvision-2023.5.5/PKG-INFO
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4631 2023-05-07 14:06:49.000000 atomvision-2023.5.5/README.md
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-05-08 02:48:15.174960 atomvision-2023.5.5/atomvision/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2023-05-07 14:12:03.000000 atomvision-2023.5.5/atomvision/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-05-08 02:48:15.198959 atomvision-2023.5.5/atomvision/data/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       36 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/data/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3244 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/data/graph.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    13492 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/data/stem.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7333 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/data/stemconv.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-05-08 02:48:15.222959 atomvision-2023.5.5/atomvision/models/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       42 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/models/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7862 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/models/alignn_classifier.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1667 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/models/cnn_classifiers.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    12426 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/models/gcn.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      586 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/models/plotting.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1004 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/models/segmentation_utils.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2105 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/models/training_metrics.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5735 2023-05-07 14:06:49.000000 atomvision-2023.5.5/atomvision/models/training_utils.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-05-08 02:48:15.254959 atomvision-2023.5.5/atomvision/scripts/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       40 2023-05-07 14:06:50.000000 atomvision-2023.5.5/atomvision/scripts/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    11705 2023-05-07 14:06:50.000000 atomvision-2023.5.5/atomvision/scripts/focal_loss.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6315 2023-05-07 14:06:50.000000 atomvision-2023.5.5/atomvision/scripts/generate_stem.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6685 2023-05-07 14:06:50.000000 atomvision-2023.5.5/atomvision/scripts/image_to_graph.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2508 2023-05-07 14:24:30.000000 atomvision-2023.5.5/atomvision/scripts/stem_conv.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7599 2023-05-07 14:24:09.000000 atomvision-2023.5.5/atomvision/scripts/train_autoencoder.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    11111 2023-05-07 14:23:19.000000 atomvision-2023.5.5/atomvision/scripts/train_classifier_alignn.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    17467 2023-05-07 14:23:04.000000 atomvision-2023.5.5/atomvision/scripts/train_classifier_cnn.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    16607 2023-05-07 14:23:59.000000 atomvision-2023.5.5/atomvision/scripts/train_gan.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    20002 2023-05-07 14:06:50.000000 atomvision-2023.5.5/atomvision/scripts/train_gnn_old.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    17654 2023-05-07 14:24:22.000000 atomvision-2023.5.5/atomvision/scripts/train_segmentation.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6327 2023-05-07 14:23:52.000000 atomvision-2023.5.5/atomvision/scripts/train_tsne.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5779 2023-05-07 14:06:50.000000 atomvision-2023.5.5/atomvision/scripts/train_variational_autoencoder.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-05-08 02:48:15.186960 atomvision-2023.5.5/atomvision.egg-info/
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5108 2023-05-08 02:48:14.000000 atomvision-2023.5.5/atomvision.egg-info/PKG-INFO
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1093 2023-05-08 02:48:15.000000 atomvision-2023.5.5/atomvision.egg-info/SOURCES.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)        1 2023-05-08 02:48:14.000000 atomvision-2023.5.5/atomvision.egg-info/dependency_links.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)      442 2023-05-08 02:48:14.000000 atomvision-2023.5.5/atomvision.egg-info/requires.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)       11 2023-05-08 02:48:14.000000 atomvision-2023.5.5/atomvision.egg-info/top_level.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)       38 2023-05-08 02:48:15.262959 atomvision-2023.5.5/setup.cfg
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1811 2023-05-07 14:22:28.000000 atomvision-2023.5.5/setup.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-05-08 03:09:17.077654 atomvision-2023.5.6/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2128 2023-05-07 14:06:49.000000 atomvision-2023.5.6/LICENSE.md
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5108 2023-05-08 03:09:17.073654 atomvision-2023.5.6/PKG-INFO
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4631 2023-05-07 14:06:49.000000 atomvision-2023.5.6/README.md
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-05-08 03:09:16.965655 atomvision-2023.5.6/atomvision/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2023-05-08 02:57:48.000000 atomvision-2023.5.6/atomvision/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-05-08 03:09:16.989655 atomvision-2023.5.6/atomvision/data/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       36 2023-05-07 14:06:49.000000 atomvision-2023.5.6/atomvision/data/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3244 2023-05-07 14:06:49.000000 atomvision-2023.5.6/atomvision/data/graph.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    13492 2023-05-07 14:06:49.000000 atomvision-2023.5.6/atomvision/data/stem.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     7333 2023-05-07 14:06:49.000000 atomvision-2023.5.6/atomvision/data/stemconv.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-05-08 03:09:17.009655 atomvision-2023.5.6/atomvision/models/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       42 2023-05-07 14:06:49.000000 atomvision-2023.5.6/atomvision/models/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     7862 2023-05-07 14:06:49.000000 atomvision-2023.5.6/atomvision/models/alignn_classifier.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1667 2023-05-07 14:06:49.000000 atomvision-2023.5.6/atomvision/models/cnn_classifiers.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    12426 2023-05-07 14:06:49.000000 atomvision-2023.5.6/atomvision/models/gcn.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      586 2023-05-07 14:06:49.000000 atomvision-2023.5.6/atomvision/models/plotting.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1004 2023-05-07 14:06:49.000000 atomvision-2023.5.6/atomvision/models/segmentation_utils.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2105 2023-05-07 14:06:49.000000 atomvision-2023.5.6/atomvision/models/training_metrics.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5735 2023-05-07 14:06:49.000000 atomvision-2023.5.6/atomvision/models/training_utils.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-05-08 03:09:17.073654 atomvision-2023.5.6/atomvision/scripts/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       40 2023-05-07 14:06:50.000000 atomvision-2023.5.6/atomvision/scripts/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    11705 2023-05-07 14:06:50.000000 atomvision-2023.5.6/atomvision/scripts/focal_loss.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6315 2023-05-07 14:06:50.000000 atomvision-2023.5.6/atomvision/scripts/generate_stem.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6685 2023-05-07 14:06:50.000000 atomvision-2023.5.6/atomvision/scripts/image_to_graph.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2508 2023-05-07 14:24:30.000000 atomvision-2023.5.6/atomvision/scripts/stem_conv.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     7599 2023-05-07 14:24:09.000000 atomvision-2023.5.6/atomvision/scripts/train_autoencoder.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    11111 2023-05-07 14:23:19.000000 atomvision-2023.5.6/atomvision/scripts/train_classifier_alignn.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    17468 2023-05-08 02:58:57.000000 atomvision-2023.5.6/atomvision/scripts/train_classifier_cnn.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    16607 2023-05-07 14:23:59.000000 atomvision-2023.5.6/atomvision/scripts/train_gan.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    20002 2023-05-07 14:06:50.000000 atomvision-2023.5.6/atomvision/scripts/train_gnn_old.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    17654 2023-05-07 14:24:22.000000 atomvision-2023.5.6/atomvision/scripts/train_segmentation.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6327 2023-05-07 14:23:52.000000 atomvision-2023.5.6/atomvision/scripts/train_tsne.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5779 2023-05-07 14:06:50.000000 atomvision-2023.5.6/atomvision/scripts/train_variational_autoencoder.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-05-08 03:09:16.981655 atomvision-2023.5.6/atomvision.egg-info/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5108 2023-05-08 03:09:16.000000 atomvision-2023.5.6/atomvision.egg-info/PKG-INFO
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1093 2023-05-08 03:09:16.000000 atomvision-2023.5.6/atomvision.egg-info/SOURCES.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        1 2023-05-08 03:09:16.000000 atomvision-2023.5.6/atomvision.egg-info/dependency_links.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      442 2023-05-08 03:09:16.000000 atomvision-2023.5.6/atomvision.egg-info/requires.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       11 2023-05-08 03:09:16.000000 atomvision-2023.5.6/atomvision.egg-info/top_level.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       38 2023-05-08 03:09:17.077654 atomvision-2023.5.6/setup.cfg
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1811 2023-05-08 02:57:35.000000 atomvision-2023.5.6/setup.py
```

### Comparing `atomvision-2023.5.5/LICENSE.md` & `atomvision-2023.5.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/PKG-INFO` & `atomvision-2023.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomvision
-Version: 2023.5.5
+Version: 2023.5.6
 Summary: atomvision
 Home-page: https://github.com/usnistgov/atomvision
 Author: Kamal Choudhary, Brian DeCost
 Author-email: kamal.choudhary@nist.gov
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atomvision-2023.5.5/README.md` & `atomvision-2023.5.6/README.md`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/data/graph.py` & `atomvision-2023.5.6/atomvision/data/graph.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/data/stem.py` & `atomvision-2023.5.6/atomvision/data/stem.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/data/stemconv.py` & `atomvision-2023.5.6/atomvision/data/stemconv.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/models/alignn_classifier.py` & `atomvision-2023.5.6/atomvision/models/alignn_classifier.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/models/cnn_classifiers.py` & `atomvision-2023.5.6/atomvision/models/cnn_classifiers.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/models/gcn.py` & `atomvision-2023.5.6/atomvision/models/gcn.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/models/plotting.py` & `atomvision-2023.5.6/atomvision/models/plotting.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/models/segmentation_utils.py` & `atomvision-2023.5.6/atomvision/models/segmentation_utils.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/models/training_metrics.py` & `atomvision-2023.5.6/atomvision/models/training_metrics.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/models/training_utils.py` & `atomvision-2023.5.6/atomvision/models/training_utils.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/scripts/focal_loss.py` & `atomvision-2023.5.6/atomvision/scripts/focal_loss.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/scripts/generate_stem.py` & `atomvision-2023.5.6/atomvision/scripts/generate_stem.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/scripts/image_to_graph.py` & `atomvision-2023.5.6/atomvision/scripts/image_to_graph.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/scripts/stem_conv.py` & `atomvision-2023.5.6/atomvision/scripts/stem_conv.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/scripts/train_autoencoder.py` & `atomvision-2023.5.6/atomvision/scripts/train_autoencoder.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/scripts/train_classifier_alignn.py` & `atomvision-2023.5.6/atomvision/scripts/train_classifier_alignn.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/scripts/train_classifier_cnn.py` & `atomvision-2023.5.6/atomvision/scripts/train_classifier_cnn.py`

 * *Files 0% similar despite different names*

```diff
@@ -454,15 +454,15 @@
                 trainer.state.epoch, accuracy, loss
             )
         )
 
     trainer.add_event_handler(Events.EPOCH_COMPLETED, log_validation_results)
 
     @trainer.on(Events.COMPLETED)
-    def og_confusion_matrix(trainer):
+    def log_confusion_matrix(trainer):
         val_evaluator.run(val_loader)
         metrics = val_evaluator.state.metrics
         cm = metrics["cm"]
         cm = cm.numpy()
         cm = cm.astype(int)
         classes = val_loader.dataset.classes
         # classes = ["0", "1", "2", "3", "4"]
```

### Comparing `atomvision-2023.5.5/atomvision/scripts/train_gan.py` & `atomvision-2023.5.6/atomvision/scripts/train_gan.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/scripts/train_gnn_old.py` & `atomvision-2023.5.6/atomvision/scripts/train_gnn_old.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/scripts/train_segmentation.py` & `atomvision-2023.5.6/atomvision/scripts/train_segmentation.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/scripts/train_tsne.py` & `atomvision-2023.5.6/atomvision/scripts/train_tsne.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision/scripts/train_variational_autoencoder.py` & `atomvision-2023.5.6/atomvision/scripts/train_variational_autoencoder.py`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/atomvision.egg-info/PKG-INFO` & `atomvision-2023.5.6/atomvision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomvision
-Version: 2023.5.5
+Version: 2023.5.6
 Summary: atomvision
 Home-page: https://github.com/usnistgov/atomvision
 Author: Kamal Choudhary, Brian DeCost
 Author-email: kamal.choudhary@nist.gov
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atomvision-2023.5.5/atomvision.egg-info/SOURCES.txt` & `atomvision-2023.5.6/atomvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atomvision-2023.5.5/setup.py` & `atomvision-2023.5.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="atomvision",
-    version="2023.5.5",
+    version="2023.5.6",
     author="Kamal Choudhary, Brian DeCost",
     author_email="kamal.choudhary@nist.gov",
     description="atomvision",
     install_requires=[
         "numpy>=1.19.5",
         "scipy>=1.6.3",
         "jarvis-tools>=2021.07.19",
```

