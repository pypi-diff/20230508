# Comparing `tmp/general_text_classifier-0.1.24-py3-none-any.whl.zip` & `tmp/general_text_classifier-0.1.25-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 12541 bytes, number of entries: 6
--rw-r--r--  2.0 unx    52989 b- defN 23-May-02 09:04 general_text_classifier/__init__.py
--rw-------  2.0 unx     1062 b- defN 23-May-02 09:05 general_text_classifier-0.1.24.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1188 b- defN 23-May-02 09:05 general_text_classifier-0.1.24.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-02 09:05 general_text_classifier-0.1.24.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-May-02 09:05 general_text_classifier-0.1.24.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      568 b- defN 23-May-02 09:05 general_text_classifier-0.1.24.dist-info/RECORD
-6 files, 55923 bytes uncompressed, 11497 bytes compressed:  79.4%
+Zip file size: 12905 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    56551 b- defN 23-May-08 05:44 general_text_classifier/__init__.py
+-rw-------  2.0 unx     1062 b- defN 23-May-08 05:45 general_text_classifier-0.1.25.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1188 b- defN 23-May-08 05:45 general_text_classifier-0.1.25.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-08 05:45 general_text_classifier-0.1.25.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-May-08 05:45 general_text_classifier-0.1.25.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      568 b- defN 23-May-08 05:45 general_text_classifier-0.1.25.dist-info/RECORD
+6 files, 59485 bytes uncompressed, 11861 bytes compressed:  80.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: general_text_classifier/__init__.py
 Comment: 
 
-Filename: general_text_classifier-0.1.24.dist-info/LICENSE.txt
+Filename: general_text_classifier-0.1.25.dist-info/LICENSE.txt
 Comment: 
 
-Filename: general_text_classifier-0.1.24.dist-info/METADATA
+Filename: general_text_classifier-0.1.25.dist-info/METADATA
 Comment: 
 
-Filename: general_text_classifier-0.1.24.dist-info/WHEEL
+Filename: general_text_classifier-0.1.25.dist-info/WHEEL
 Comment: 
 
-Filename: general_text_classifier-0.1.24.dist-info/top_level.txt
+Filename: general_text_classifier-0.1.25.dist-info/top_level.txt
 Comment: 
 
-Filename: general_text_classifier-0.1.24.dist-info/RECORD
+Filename: general_text_classifier-0.1.25.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## general_text_classifier/__init__.py

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from scipy.special import softmax
 from shutil import make_archive, unpack_archive
 from simpletransformers.classification import (
     ClassificationModel,
     ClassificationArgs,
     MultiLabelClassificationModel,
-    MultiLabelClassificationArgs,
+    MultiLabelClassificationArgs
 )
 from sklearn.metrics import (
     classification_report,
     f1_score,
     precision_score,
     recall_score,
     accuracy_score,
@@ -34,36 +34,116 @@
 
 logging.basicConfig(level=logging.INFO)
 transformers_logger = logging.getLogger("transformers")
 transformers_logger.setLevel(logging.WARNING)
 
 
 def f1_multiclass(labels, preds):
+    """
+    Computes the F1 score of a multi-class classification problem.
+    Args:
+        labels (np.ndarray): ground-truth labels, shape (n_samples, n_classes).
+        preds (np.ndarray): predicted labels, shape (n_samples, n_classes).
+    Returns:
+        float: the F1 score.
+    """
     return (
         f1_score(labels, preds, average="macro")
         if len(np.unique(labels)) > 2
         else f1_score(labels, preds, average="binary")
     )
 
-
 def precision_multiclass(labels, preds):
+    """
+    Computes the precision score of a multi-class classification problem.
+    Args:
+        labels (np.ndarray): ground-truth labels, shape (n_samples, n_classes).
+        preds (np.ndarray): predicted labels, shape (n_samples, n_classes).
+    Returns:
+        float: the precision score.
+    """
     return (
         precision_score(labels, preds, average="macro")
         if len(np.unique(labels)) > 2
         else precision_score(labels, preds, average="binary")
     )
 
 
 def recall_multiclass(labels, preds):
+    """
+    Computes the recall score of a multi-class classification problem.
+    Args:
+        labels (np.ndarray): ground-truth labels, shape (n_samples, n_classes).
+        preds (np.ndarray): predicted labels, shape (n_samples, n_classes).
+    Returns:
+        float: the recall score.
+    """
     return (
         recall_score(labels, preds, average="macro")
         if len(np.unique(labels)) > 2
         else recall_score(labels, preds, average="binary")
     )
 
+def precision_multilabel(labels, preds, threshold=0.5, average="macro"):
+    """
+    Computes the precision score of a multi-label classification problem.
+    Args:
+        labels (np.ndarray): ground-truth labels, shape (n_samples, n_classes).
+        preds (np.ndarray): predicted labels, shape (n_samples, n_classes).
+        threshold (float): probability threshold to consider a label as positive.
+        average (str): averaging strategy to use, either "macro" or "micro".
+    Returns:
+        float: the precision score.
+    """
+    preds = (preds > threshold).astype(np.int32)
+    return precision_score(labels, preds, average=average)
+
+def recall_multilabel(labels, preds, threshold=0.5, average="macro"):
+    """
+    Computes the recall score of a multi-label classification problem.
+    Args:
+        labels (np.ndarray): ground-truth labels, shape (n_samples, n_classes).
+        preds (np.ndarray): predicted labels, shape (n_samples, n_classes).
+        threshold (float): probability threshold to consider a label as positive.
+        average (str): averaging strategy to use, either "macro" or "micro".
+    Returns:
+        float: the recall score.
+    """
+    preds = (preds > threshold).astype(np.int32)
+    return recall_score(labels, preds, average=average)
+
+def accuracy_multilabel(labels, preds, threshold=0.5):
+    """
+    Computes the accuracy score of a multi-label classification problem.
+    Args:
+        labels (np.ndarray): ground-truth labels, shape (n_samples, n_classes).
+        preds (np.ndarray): predicted labels, shape (n_samples, n_classes).
+        threshold (float): probability threshold to consider a label as positive.
+    Returns:
+        float: the accuracy score.
+    """
+    preds = (preds > threshold).astype(np.int32)
+    return accuracy_score(labels, preds)
+
+
+def f1_multilabel(labels, preds, threshold=0.5, average="macro"):
+    """
+    Computes the F1 score of a multi-label classification problem.
+    Args:
+        labels (np.ndarray): ground-truth labels, shape (n_samples, n_classes).
+        preds (np.ndarray): predicted labels, shape (n_samples, n_classes).
+        threshold (float): probability threshold to consider a label as positive.
+        average (str): averaging strategy to use, either "macro" or "micro".
+    Returns:
+        float: the F1 score.
+    """
+    preds = (preds > threshold).astype(np.int32)
+    return f1_score(labels, preds, average=average)
+
+
 
 def create_model_card(
     model_card_path="model_card.md",
     model_title="Model Title",
     model_summary="",
     team="",
     contact_persons="",
@@ -441,18 +521,18 @@
                 self.classification_args_obj = ClassificationArgs
 
             elif self.classification_type == "multi":
                 self.classification_model_obj = MultiLabelClassificationModel
                 self.classification_args_obj = MultiLabelClassificationArgs
 
             self.model_args = {
-                "use_early_stopping": False,
                 "do_lower_case": self.do_lowercase if self.data_lang != "tr" else False,
+                "use_early_stopping": True,
                 "early_stopping_consider_epochs": False,
-                "early_stopping_delta": 0.0001,
+                "early_stopping_delta": 0.001,
                 "early_stopping_metric": "eval_loss",
                 "early_stopping_metric_minimize": True,
                 "early_stopping_patience": 5,
                 "eval_batch_size": 16,
                 "train_batch_size": 16,
                 "n_gpu": len(self.gpus_to_use),
                 "evaluate_during_training": True,
@@ -464,14 +544,15 @@
                 "output_dir": os.path.join(self.model_dir, "outputs/"),
                 "best_model_dir": os.path.join(self.model_dir, "best_model/"),
                 "cache_dir": os.path.join(self.model_dir, "cache_dir/"),
                 "overwrite_output_dir": True,
                 "use_multiprocessing": False,
                 "use_multiprocessing_for_evaluation": False,
                 "manual_seed": self.random_state,
+                "save_eval_checkpoints": True
             }
 
             self.model_args = {**self.model_args, **exp_args}
             self.model_type = model_type
             self.model_version = model_version
             self.save_onnx_model = save_onnx_model
             self.split_size = split_size
@@ -833,20 +914,20 @@
 
             if self.classification_type == "single":
                 label_encoder = LabelEncoder()
 
             else:
                 label_encoder = MultiLabelBinarizer()
                 train_data["labels"] = train_data["labels"].apply(
-                    lambda x: [elem.strip() for elem in x.split(",")]
+                    lambda x: [elem.strip() for elem in x.split(";")]
                 )
 
                 if val_data is not None:
                     val_data["labels"] = val_data["labels"].apply(
-                        lambda x: [elem.strip() for elem in x.split(",")]
+                        lambda x: [elem.strip() for elem in x.split(";")]
                     )
 
             train_data["labels"] = label_encoder.fit_transform(
                 train_data["labels"].tolist()
             ).tolist()
 
             if val_data is not None:
@@ -857,15 +938,15 @@
             return [train_data, val_data, label_encoder]
 
         else:
             val_data["labels_original"] = val_data["labels"].tolist()
 
             if self.classification_type == "multi":
                 val_data["labels"] = val_data["labels"].apply(
-                    lambda x: [elem.strip() for elem in x.split(",")]
+                    lambda x: [elem.strip() for elem in x.split(";")]
                 )
 
             val_data["labels"] = self.label_encoder.transform(
                 val_data["labels"].tolist()
             ).tolist()
             return val_data
 
@@ -1163,15 +1244,20 @@
                 self.model_version,
                 use_cuda=True if len(self.gpus_to_use) else False,
                 args=self.model_args,
                 num_labels=len(list(self.label_encoder.classes_)),
             )
 
             _, self.training_details = self.model.train_model(
-                self.model_train_data[["text", "labels"]], eval_df=eval_df
+                self.model_train_data[["text", "labels"]], 
+                eval_df=eval_df,
+                f1=f1_multilabel,
+                acc=accuracy_multilabel,
+                precision=precision_multilabel,
+                recall=recall_multilabel
             )
 
         # save model metadata & label encoder
         self.model_metadata = {
             "model_type": self.model_type,
             "task_type": self.classification_type,
             "do_eval": eval_df is not None,
@@ -1218,15 +1304,15 @@
             except:
                 pass
 
         make_archive(model_save_path, "gztar", root_dir=model_save_path)
 
         if self.gcloud_bucket_name is not None:
             self.print_log_messages(7)
-
+            
             self.upload_to_gcs(
                 self.storage_client,
                 model_save_path + ".tar.gz",
                 self.gcloud_bucket_name,
                 self.model_bigq_dir,
             )
 
@@ -1379,28 +1465,28 @@
             self.print_log_messages(12)
 
             self.test_data = self.encode_labels(val_data=self.test_data)
             print(
                 classification_report(
                     self.test_data["labels"].tolist(),
                     self.test_data["predictions_encoded"].tolist(),
-                    digits=3,
+                    digits=4,
                     target_names=[
                         str(elem) for elem in self.label_encoder.classes_.tolist()
                     ],
                 )
             )
 
             self.cls_report = classification_report(
                 self.test_data["labels"].tolist(),
                 self.test_data["predictions_encoded"].tolist(),
                 target_names=[
                     str(elem) for elem in self.label_encoder.classes_.tolist()
                 ],
-                digits=3,
+                digits=4,
                 output_dict=True,
             )
 
             self.cls_report = pd.DataFrame(self.cls_report).T
             self.cls_report_path = (
                 os.path.join(self.model_dir, "best_model", "cls_report.csv")
                 if self.model_metadata["do_eval"]
```

## Comparing `general_text_classifier-0.1.24.dist-info/LICENSE.txt` & `general_text_classifier-0.1.25.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `general_text_classifier-0.1.24.dist-info/METADATA` & `general_text_classifier-0.1.25.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: general-text-classifier
-Version: 0.1.24
+Version: 0.1.25
 Summary: General Text Classification Library
 Home-page: UNKNOWN
 Author: Trendyol NLP Team
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `general_text_classifier-0.1.24.dist-info/RECORD` & `general_text_classifier-0.1.25.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-general_text_classifier/__init__.py,sha256=ttV2r05WWlicIYGKPYXBERC0NorWdCfjOcgRuoALSQA,52989
-general_text_classifier-0.1.24.dist-info/LICENSE.txt,sha256=39ifOUz0fv0QxPoscWvZ9z9ZkO1xtfvb8ze-KnkO3EE,1062
-general_text_classifier-0.1.24.dist-info/METADATA,sha256=HQVl3Kc_Jg2Ff8JJC435g-k2iNqADEjvrzj0FgXFFyw,1188
-general_text_classifier-0.1.24.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-general_text_classifier-0.1.24.dist-info/top_level.txt,sha256=8byuMM000m_1XjdHiOSw1VvLuoY7o1e8hk5siED7p_0,24
-general_text_classifier-0.1.24.dist-info/RECORD,,
+general_text_classifier/__init__.py,sha256=-pBRKkPkyh6LLKwrtGyXpIyQ8Yt1nEZGE8oSlhWUEHI,56551
+general_text_classifier-0.1.25.dist-info/LICENSE.txt,sha256=39ifOUz0fv0QxPoscWvZ9z9ZkO1xtfvb8ze-KnkO3EE,1062
+general_text_classifier-0.1.25.dist-info/METADATA,sha256=QN0sFHHKcq_TJ1paQ2cRtjSbcoTQ2TdE1zK8FgQqYV0,1188
+general_text_classifier-0.1.25.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+general_text_classifier-0.1.25.dist-info/top_level.txt,sha256=8byuMM000m_1XjdHiOSw1VvLuoY7o1e8hk5siED7p_0,24
+general_text_classifier-0.1.25.dist-info/RECORD,,
```

