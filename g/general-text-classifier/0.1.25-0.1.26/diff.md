# Comparing `tmp/general_text_classifier-0.1.25-py3-none-any.whl.zip` & `tmp/general_text_classifier-0.1.26-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 12905 bytes, number of entries: 6
--rw-r--r--  2.0 unx    56551 b- defN 23-May-08 05:44 general_text_classifier/__init__.py
--rw-------  2.0 unx     1062 b- defN 23-May-08 05:45 general_text_classifier-0.1.25.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1188 b- defN 23-May-08 05:45 general_text_classifier-0.1.25.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-08 05:45 general_text_classifier-0.1.25.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-May-08 05:45 general_text_classifier-0.1.25.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      568 b- defN 23-May-08 05:45 general_text_classifier-0.1.25.dist-info/RECORD
-6 files, 59485 bytes uncompressed, 11861 bytes compressed:  80.1%
+-rw-r--r--  2.0 unx    56550 b- defN 23-May-08 11:06 general_text_classifier/__init__.py
+-rw-------  2.0 unx     1062 b- defN 23-May-08 11:07 general_text_classifier-0.1.26.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1188 b- defN 23-May-08 11:07 general_text_classifier-0.1.26.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-08 11:07 general_text_classifier-0.1.26.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-May-08 11:07 general_text_classifier-0.1.26.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      568 b- defN 23-May-08 11:07 general_text_classifier-0.1.26.dist-info/RECORD
+6 files, 59484 bytes uncompressed, 11861 bytes compressed:  80.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: general_text_classifier/__init__.py
 Comment: 
 
-Filename: general_text_classifier-0.1.25.dist-info/LICENSE.txt
+Filename: general_text_classifier-0.1.26.dist-info/LICENSE.txt
 Comment: 
 
-Filename: general_text_classifier-0.1.25.dist-info/METADATA
+Filename: general_text_classifier-0.1.26.dist-info/METADATA
 Comment: 
 
-Filename: general_text_classifier-0.1.25.dist-info/WHEEL
+Filename: general_text_classifier-0.1.26.dist-info/WHEEL
 Comment: 
 
-Filename: general_text_classifier-0.1.25.dist-info/top_level.txt
+Filename: general_text_classifier-0.1.26.dist-info/top_level.txt
 Comment: 
 
-Filename: general_text_classifier-0.1.25.dist-info/RECORD
+Filename: general_text_classifier-0.1.26.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## general_text_classifier/__init__.py

```diff
@@ -1020,15 +1020,15 @@
                 self.print_log_messages(4)
                 self.train_data, self.val_data, self.label_encoder = self.encode_labels(
                     self.train_data
                 )
 
                 try:
                     msss = MultilabelStratifiedShuffleSplit(
-                        n_splits=3,
+                        n_splits=1,
                         test_size=self.split_size,
                         random_state=self.random_state,
                     )
 
                     X = self.train_data["text"].values
                     y = np.vstack(self.train_data["labels"].values[:])
                     msss.get_n_splits(X, y)
@@ -1437,15 +1437,15 @@
             )
         else:
             predictions_raw = []
             confidence_scores = []
 
             for i in range(len(self.raw_outputs)):
                 predictions_raw.append(
-                    ", ".join(
+                    ";".join(
                         self.label_encoder.inverse_transform(
                             np.array(self.predictions[i]).reshape(1, -1)
                         )[0]
                     )
                 )
                 confidence_scores.append(
                     self.raw_outputs[i][np.nonzero(self.predictions[i])[0]]
```

## Comparing `general_text_classifier-0.1.25.dist-info/LICENSE.txt` & `general_text_classifier-0.1.26.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `general_text_classifier-0.1.25.dist-info/METADATA` & `general_text_classifier-0.1.26.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: general-text-classifier
-Version: 0.1.25
+Version: 0.1.26
 Summary: General Text Classification Library
 Home-page: UNKNOWN
 Author: Trendyol NLP Team
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `general_text_classifier-0.1.25.dist-info/RECORD` & `general_text_classifier-0.1.26.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-general_text_classifier/__init__.py,sha256=-pBRKkPkyh6LLKwrtGyXpIyQ8Yt1nEZGE8oSlhWUEHI,56551
-general_text_classifier-0.1.25.dist-info/LICENSE.txt,sha256=39ifOUz0fv0QxPoscWvZ9z9ZkO1xtfvb8ze-KnkO3EE,1062
-general_text_classifier-0.1.25.dist-info/METADATA,sha256=QN0sFHHKcq_TJ1paQ2cRtjSbcoTQ2TdE1zK8FgQqYV0,1188
-general_text_classifier-0.1.25.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-general_text_classifier-0.1.25.dist-info/top_level.txt,sha256=8byuMM000m_1XjdHiOSw1VvLuoY7o1e8hk5siED7p_0,24
-general_text_classifier-0.1.25.dist-info/RECORD,,
+general_text_classifier/__init__.py,sha256=ZbtFd3MqUNGXaHpJ34zElbodQ7TMByx5ms4YujhiMtQ,56550
+general_text_classifier-0.1.26.dist-info/LICENSE.txt,sha256=39ifOUz0fv0QxPoscWvZ9z9ZkO1xtfvb8ze-KnkO3EE,1062
+general_text_classifier-0.1.26.dist-info/METADATA,sha256=3XBuxxHta0gEH0oEEHTUEeqYYz7np3mlYDnPHxgiJIY,1188
+general_text_classifier-0.1.26.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+general_text_classifier-0.1.26.dist-info/top_level.txt,sha256=8byuMM000m_1XjdHiOSw1VvLuoY7o1e8hk5siED7p_0,24
+general_text_classifier-0.1.26.dist-info/RECORD,,
```

