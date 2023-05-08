# Comparing `tmp/globox-2.1.1.tar.gz` & `tmp/globox-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globox-2.1.1.tar", last modified: Wed Mar  8 08:53:10 2023, max compression
+gzip compressed data, was "globox-2.1.2.tar", last modified: Mon May  8 17:04:46 2023, max compression
```

## Comparing `globox-2.1.1.tar` & `globox-2.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 louislac   (501) staff       (20)        0 2023-03-08 08:53:10.919946 globox-2.1.1/
--rw-r--r--   0 louislac   (501) staff       (20)     1048 2022-09-12 14:17:20.000000 globox-2.1.1/LICENCE
--rw-r--r--   0 louislac   (501) staff       (20)     9991 2023-03-08 08:53:10.919726 globox-2.1.1/PKG-INFO
--rw-r--r--   0 louislac   (501) staff       (20)     9193 2023-02-22 20:49:42.000000 globox-2.1.1/README.md
--rw-r--r--   0 louislac   (501) staff       (20)       80 2022-10-03 20:55:21.000000 globox-2.1.1/pyproject.toml
--rw-r--r--   0 louislac   (501) staff       (20)       38 2023-03-08 08:53:10.919997 globox-2.1.1/setup.cfg
--rw-r--r--   0 louislac   (501) staff       (20)     1745 2023-02-22 20:52:00.000000 globox-2.1.1/setup.py
-drwxr-xr-x   0 louislac   (501) staff       (20)        0 2023-03-08 08:53:10.914130 globox-2.1.1/src/
-drwxr-xr-x   0 louislac   (501) staff       (20)        0 2023-03-08 08:53:10.917496 globox-2.1.1/src/globox/
--rw-r--r--   0 louislac   (501) staff       (20)      273 2022-12-13 08:25:32.000000 globox-2.1.1/src/globox/__init__.py
--rw-r--r--   0 louislac   (501) staff       (20)       30 2022-10-26 18:29:42.000000 globox-2.1.1/src/globox/__main__.py
--rw-r--r--   0 louislac   (501) staff       (20)       63 2023-03-08 08:52:05.000000 globox-2.1.1/src/globox/__version__.py
--rw-r--r--   0 louislac   (501) staff       (20)    18551 2023-02-02 16:27:25.000000 globox-2.1.1/src/globox/annotation.py
--rw-r--r--   0 louislac   (501) staff       (20)    33234 2023-02-02 16:30:38.000000 globox-2.1.1/src/globox/annotationset.py
--rw-r--r--   0 louislac   (501) staff       (20)     1015 2023-02-02 16:31:14.000000 globox-2.1.1/src/globox/atomic.py
--rw-r--r--   0 louislac   (501) staff       (20)    17250 2023-03-08 08:48:11.000000 globox-2.1.1/src/globox/boundingbox.py
--rw-r--r--   0 louislac   (501) staff       (20)    14247 2023-02-02 16:31:37.000000 globox-2.1.1/src/globox/cli.py
--rw-r--r--   0 louislac   (501) staff       (20)      539 2023-02-02 16:31:45.000000 globox-2.1.1/src/globox/errors.py
--rw-r--r--   0 louislac   (501) staff       (20)    21347 2023-02-02 16:31:53.000000 globox-2.1.1/src/globox/evaluation.py
--rw-r--r--   0 louislac   (501) staff       (20)      699 2023-02-02 16:31:55.000000 globox-2.1.1/src/globox/file_utils.py
--rw-r--r--   0 louislac   (501) staff       (20)     6983 2023-02-02 16:32:02.000000 globox-2.1.1/src/globox/image_utils.py
--rw-r--r--   0 louislac   (501) staff       (20)      880 2023-02-02 16:32:05.000000 globox-2.1.1/src/globox/thread_utils.py
--rw-r--r--   0 louislac   (501) staff       (20)      747 2023-02-02 16:32:09.000000 globox-2.1.1/src/globox/utils.py
-drwxr-xr-x   0 louislac   (501) staff       (20)        0 2023-03-08 08:53:10.918390 globox-2.1.1/src/globox.egg-info/
--rw-r--r--   0 louislac   (501) staff       (20)     9991 2023-03-08 08:53:10.000000 globox-2.1.1/src/globox.egg-info/PKG-INFO
--rw-r--r--   0 louislac   (501) staff       (20)      755 2023-03-08 08:53:10.000000 globox-2.1.1/src/globox.egg-info/SOURCES.txt
--rw-r--r--   0 louislac   (501) staff       (20)        1 2023-03-08 08:53:10.000000 globox-2.1.1/src/globox.egg-info/dependency_links.txt
--rw-r--r--   0 louislac   (501) staff       (20)       43 2023-03-08 08:53:10.000000 globox-2.1.1/src/globox.egg-info/entry_points.txt
--rw-r--r--   0 louislac   (501) staff       (20)       65 2023-03-08 08:53:10.000000 globox-2.1.1/src/globox.egg-info/requires.txt
--rw-r--r--   0 louislac   (501) staff       (20)        7 2023-03-08 08:53:10.000000 globox-2.1.1/src/globox.egg-info/top_level.txt
-drwxr-xr-x   0 louislac   (501) staff       (20)        0 2023-03-08 08:53:10.919454 globox-2.1.1/tests/
--rw-r--r--   0 louislac   (501) staff       (20)     7607 2023-02-02 16:32:39.000000 globox-2.1.1/tests/test_annotation.py
--rw-r--r--   0 louislac   (501) staff       (20)     8505 2023-02-02 16:32:45.000000 globox-2.1.1/tests/test_annotationset.py
--rw-r--r--   0 louislac   (501) staff       (20)     7846 2023-03-08 08:50:04.000000 globox-2.1.1/tests/test_bbox.py
--rw-r--r--   0 louislac   (501) staff       (20)     5168 2023-02-02 16:32:56.000000 globox-2.1.1/tests/test_coco_evaluation.py
--rw-r--r--   0 louislac   (501) staff       (20)     2151 2023-02-02 16:33:01.000000 globox-2.1.1/tests/test_conversion.py
--rw-r--r--   0 louislac   (501) staff       (20)      226 2023-02-02 16:33:05.000000 globox-2.1.1/tests/test_evaluation.py
--rw-r--r--   0 louislac   (501) staff       (20)     2867 2023-02-02 16:33:08.000000 globox-2.1.1/tests/test_parsing.py
+drwxr-xr-x   0 louislac   (501) staff       (20)        0 2023-05-08 17:04:46.766928 globox-2.1.2/
+-rw-r--r--   0 louislac   (501) staff       (20)     1048 2022-09-12 14:17:20.000000 globox-2.1.2/LICENCE
+-rw-r--r--   0 louislac   (501) staff       (20)    10259 2023-05-08 17:04:46.766661 globox-2.1.2/PKG-INFO
+-rw-r--r--   0 louislac   (501) staff       (20)     9461 2023-05-04 12:47:54.000000 globox-2.1.2/README.md
+-rw-r--r--   0 louislac   (501) staff       (20)       80 2022-10-03 20:55:21.000000 globox-2.1.2/pyproject.toml
+-rw-r--r--   0 louislac   (501) staff       (20)       38 2023-05-08 17:04:46.767027 globox-2.1.2/setup.cfg
+-rw-r--r--   0 louislac   (501) staff       (20)     1745 2023-04-27 15:10:15.000000 globox-2.1.2/setup.py
+drwxr-xr-x   0 louislac   (501) staff       (20)        0 2023-05-08 17:04:46.759871 globox-2.1.2/src/
+drwxr-xr-x   0 louislac   (501) staff       (20)        0 2023-05-08 17:04:46.764236 globox-2.1.2/src/globox/
+-rw-r--r--   0 louislac   (501) staff       (20)      273 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/__init__.py
+-rw-r--r--   0 louislac   (501) staff       (20)       30 2022-10-26 18:29:42.000000 globox-2.1.2/src/globox/__main__.py
+-rw-r--r--   0 louislac   (501) staff       (20)       63 2023-05-08 17:03:33.000000 globox-2.1.2/src/globox/__version__.py
+-rw-r--r--   0 louislac   (501) staff       (20)    18551 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/annotation.py
+-rw-r--r--   0 louislac   (501) staff       (20)    33312 2023-05-08 17:02:15.000000 globox-2.1.2/src/globox/annotationset.py
+-rw-r--r--   0 louislac   (501) staff       (20)     1015 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/atomic.py
+-rw-r--r--   0 louislac   (501) staff       (20)    17250 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/boundingbox.py
+-rw-r--r--   0 louislac   (501) staff       (20)    14247 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/cli.py
+-rw-r--r--   0 louislac   (501) staff       (20)      539 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/errors.py
+-rw-r--r--   0 louislac   (501) staff       (20)    21347 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/evaluation.py
+-rw-r--r--   0 louislac   (501) staff       (20)      699 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/file_utils.py
+-rw-r--r--   0 louislac   (501) staff       (20)     6983 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/image_utils.py
+-rw-r--r--   0 louislac   (501) staff       (20)      880 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/thread_utils.py
+-rw-r--r--   0 louislac   (501) staff       (20)      747 2023-04-27 15:10:15.000000 globox-2.1.2/src/globox/utils.py
+drwxr-xr-x   0 louislac   (501) staff       (20)        0 2023-05-08 17:04:46.765227 globox-2.1.2/src/globox.egg-info/
+-rw-r--r--   0 louislac   (501) staff       (20)    10259 2023-05-08 17:04:46.000000 globox-2.1.2/src/globox.egg-info/PKG-INFO
+-rw-r--r--   0 louislac   (501) staff       (20)      755 2023-05-08 17:04:46.000000 globox-2.1.2/src/globox.egg-info/SOURCES.txt
+-rw-r--r--   0 louislac   (501) staff       (20)        1 2023-05-08 17:04:46.000000 globox-2.1.2/src/globox.egg-info/dependency_links.txt
+-rw-r--r--   0 louislac   (501) staff       (20)       43 2023-05-08 17:04:46.000000 globox-2.1.2/src/globox.egg-info/entry_points.txt
+-rw-r--r--   0 louislac   (501) staff       (20)       65 2023-05-08 17:04:46.000000 globox-2.1.2/src/globox.egg-info/requires.txt
+-rw-r--r--   0 louislac   (501) staff       (20)        7 2023-05-08 17:04:46.000000 globox-2.1.2/src/globox.egg-info/top_level.txt
+drwxr-xr-x   0 louislac   (501) staff       (20)        0 2023-05-08 17:04:46.766427 globox-2.1.2/tests/
+-rw-r--r--   0 louislac   (501) staff       (20)     7607 2023-04-27 15:10:15.000000 globox-2.1.2/tests/test_annotation.py
+-rw-r--r--   0 louislac   (501) staff       (20)     8505 2023-04-27 15:10:15.000000 globox-2.1.2/tests/test_annotationset.py
+-rw-r--r--   0 louislac   (501) staff       (20)     7846 2023-04-27 15:10:15.000000 globox-2.1.2/tests/test_bbox.py
+-rw-r--r--   0 louislac   (501) staff       (20)     5168 2023-04-27 15:10:15.000000 globox-2.1.2/tests/test_coco_evaluation.py
+-rw-r--r--   0 louislac   (501) staff       (20)     2151 2023-04-27 15:10:15.000000 globox-2.1.2/tests/test_conversion.py
+-rw-r--r--   0 louislac   (501) staff       (20)      226 2023-04-27 15:10:15.000000 globox-2.1.2/tests/test_evaluation.py
+-rw-r--r--   0 louislac   (501) staff       (20)     2867 2023-04-27 15:10:15.000000 globox-2.1.2/tests/test_parsing.py
```

### Comparing `globox-2.1.1/LICENCE` & `globox-2.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `globox-2.1.1/PKG-INFO` & `globox-2.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globox
-Version: 2.1.1
+Version: 2.1.2
 Summary: Globox is a package and command line interface to read and convert object detection databases (COCO, YOLO, PascalVOC, LabelMe, CVAT, OpenImage, ...) and evaluate them with COCO and PascalVOC.
 Home-page: https://github.com/laclouis5/globox
 Author: Louis Lac
 Author-email: lac.louis5@gmail.com
 License: MIT
 Keywords: annotation,metrics,object detection,bounding boxes,yolo,openimages,cvat,coco,pascal voc,average precision,mean average precision
 Classifier: Programming Language :: Python
@@ -40,15 +40,15 @@
 
 The library has three main components:
 
 * `BoundingBox`: represents a bounding box with a label and an optional confidence score
 * `Annotation`: represent the bounding boxes annotations for one image
 * `AnnotationSet`: represents annotations for a set of images (a database)
 
-The `AnnotationSet` class contains static methods to read different databases:
+The `AnnotationSet` class contains static methods to read different dataset formats:
 
 ```python
 # COCO
 coco = AnnotationSet.from_coco(file_path="path/to/file.json")
 
 # YOLOv5
 yolo = AnnotationSet.from_yolo_v5(
@@ -90,15 +90,15 @@
     print(box.label, box.area, box.is_ground_truth)
 
 for annotation in gts:
     nb_boxes = len(annotation.boxes)
     print(f"{annotation.image_id}: {nb_boxes} boxes")
 ```
 
-Database stats can printed to the console:
+Datasets stats can printed to the console:
 
 ```python
 coco_gts.show_stats()
 ```
 
 ```shell
          Database Stats         
@@ -128,15 +128,15 @@
 ├─────────────┼────────┼───────┤
 │ Total       │    100 │   273 │
 └─────────────┴────────┴───────┘
 ```
 
 ### Convert and Save to Many Formats
 
-Datasets can be converted to and saved in other formats easily:
+Datasets can be converted to and saved in other formats:
 
 ```python
 # ImageNet
 gts.save_imagenet(save_dir="pascalVOC_db/")
 
 # YOLO Darknet
 gts.save_yolo_darknet(
@@ -152,15 +152,15 @@
 
 # CVAT
 gts.save_cvat(path="train.xml")
 ```
 
 ### COCO Evaluation
 
-Evaluating is as easy as:
+COCO Evaluation is also supported:
 
 ```python
 evaluator = COCOEvaluator(
     ground_truths=gts, 
     predictions=dets
 )
 
@@ -215,14 +215,24 @@
 cat_ar = evaluation["cat"].ar
 ```
 
 Evaluations are cached by `(iou_threshold, max_detections, size_range)` keys. This means that you should not care about about performance, repetead queries to the evaluator are fast!
 
 ## Use in Command Line
 
+If you only need to use Globox from the command line like an application, you can install the package through [pipx](https://pypa.github.io/pipx/):
+
+```shell
+pipx install globox
+```
+
+Globox will then be in your shell path and usable from anywhere.
+
+### Usage
+
 Get a summary of annotations for one dataset:
 
 ```shell
 globox summary /yolo/folder/ --format yolo
 ```
 
 Convert annotations from one format to another one:
```

### Comparing `globox-2.1.1/README.md` & `globox-2.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 The library has three main components:
 
 * `BoundingBox`: represents a bounding box with a label and an optional confidence score
 * `Annotation`: represent the bounding boxes annotations for one image
 * `AnnotationSet`: represents annotations for a set of images (a database)
 
-The `AnnotationSet` class contains static methods to read different databases:
+The `AnnotationSet` class contains static methods to read different dataset formats:
 
 ```python
 # COCO
 coco = AnnotationSet.from_coco(file_path="path/to/file.json")
 
 # YOLOv5
 yolo = AnnotationSet.from_yolo_v5(
@@ -72,15 +72,15 @@
     print(box.label, box.area, box.is_ground_truth)
 
 for annotation in gts:
     nb_boxes = len(annotation.boxes)
     print(f"{annotation.image_id}: {nb_boxes} boxes")
 ```
 
-Database stats can printed to the console:
+Datasets stats can printed to the console:
 
 ```python
 coco_gts.show_stats()
 ```
 
 ```shell
          Database Stats         
@@ -110,15 +110,15 @@
 ├─────────────┼────────┼───────┤
 │ Total       │    100 │   273 │
 └─────────────┴────────┴───────┘
 ```
 
 ### Convert and Save to Many Formats
 
-Datasets can be converted to and saved in other formats easily:
+Datasets can be converted to and saved in other formats:
 
 ```python
 # ImageNet
 gts.save_imagenet(save_dir="pascalVOC_db/")
 
 # YOLO Darknet
 gts.save_yolo_darknet(
@@ -134,15 +134,15 @@
 
 # CVAT
 gts.save_cvat(path="train.xml")
 ```
 
 ### COCO Evaluation
 
-Evaluating is as easy as:
+COCO Evaluation is also supported:
 
 ```python
 evaluator = COCOEvaluator(
     ground_truths=gts, 
     predictions=dets
 )
 
@@ -197,14 +197,24 @@
 cat_ar = evaluation["cat"].ar
 ```
 
 Evaluations are cached by `(iou_threshold, max_detections, size_range)` keys. This means that you should not care about about performance, repetead queries to the evaluator are fast!
 
 ## Use in Command Line
 
+If you only need to use Globox from the command line like an application, you can install the package through [pipx](https://pypa.github.io/pipx/):
+
+```shell
+pipx install globox
+```
+
+Globox will then be in your shell path and usable from anywhere.
+
+### Usage
+
 Get a summary of annotations for one dataset:
 
 ```shell
 globox summary /yolo/folder/ --format yolo
 ```
 
 Convert annotations from one format to another one:
```

### Comparing `globox-2.1.1/setup.py` & `globox-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.1/src/globox/annotation.py` & `globox-2.1.2/src/globox/annotation.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.1/src/globox/annotationset.py` & `globox-2.1.2/src/globox/annotationset.py`

 * *Files 0% similar despite different names*

```diff
@@ -748,14 +748,16 @@
         for annotation in tqdm(self, desc="Saving", disable=not verbose):
             for box in annotation.boxes:
                 box_annotation = {
                     "iscrowd": 0,
                     "ignore": 0,
                     "image_id": imageid_to_id[annotation.image_id],
                     "bbox": box.ltwh,
+                    "area": box.area,
+                    "segmentation": [],
                     "category_id": label_to_id[box.label],
                     "id": ann_id_count,
                 }
 
                 if box.is_detection:
                     box_annotation["score"] = box.confidence
```

### Comparing `globox-2.1.1/src/globox/atomic.py` & `globox-2.1.2/src/globox/atomic.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.1/src/globox/boundingbox.py` & `globox-2.1.2/src/globox/boundingbox.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.1/src/globox/cli.py` & `globox-2.1.2/src/globox/cli.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.1/src/globox/errors.py` & `globox-2.1.2/src/globox/errors.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.1/src/globox/evaluation.py` & `globox-2.1.2/src/globox/evaluation.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.1/src/globox/file_utils.py` & `globox-2.1.2/src/globox/file_utils.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.1/src/globox/image_utils.py` & `globox-2.1.2/src/globox/image_utils.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.1/src/globox/thread_utils.py` & `globox-2.1.2/src/globox/thread_utils.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.1/src/globox/utils.py` & `globox-2.1.2/src/globox/utils.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.1/src/globox.egg-info/PKG-INFO` & `globox-2.1.2/src/globox.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globox
-Version: 2.1.1
+Version: 2.1.2
 Summary: Globox is a package and command line interface to read and convert object detection databases (COCO, YOLO, PascalVOC, LabelMe, CVAT, OpenImage, ...) and evaluate them with COCO and PascalVOC.
 Home-page: https://github.com/laclouis5/globox
 Author: Louis Lac
 Author-email: lac.louis5@gmail.com
 License: MIT
 Keywords: annotation,metrics,object detection,bounding boxes,yolo,openimages,cvat,coco,pascal voc,average precision,mean average precision
 Classifier: Programming Language :: Python
@@ -40,15 +40,15 @@
 
 The library has three main components:
 
 * `BoundingBox`: represents a bounding box with a label and an optional confidence score
 * `Annotation`: represent the bounding boxes annotations for one image
 * `AnnotationSet`: represents annotations for a set of images (a database)
 
-The `AnnotationSet` class contains static methods to read different databases:
+The `AnnotationSet` class contains static methods to read different dataset formats:
 
 ```python
 # COCO
 coco = AnnotationSet.from_coco(file_path="path/to/file.json")
 
 # YOLOv5
 yolo = AnnotationSet.from_yolo_v5(
@@ -90,15 +90,15 @@
     print(box.label, box.area, box.is_ground_truth)
 
 for annotation in gts:
     nb_boxes = len(annotation.boxes)
     print(f"{annotation.image_id}: {nb_boxes} boxes")
 ```
 
-Database stats can printed to the console:
+Datasets stats can printed to the console:
 
 ```python
 coco_gts.show_stats()
 ```
 
 ```shell
          Database Stats         
@@ -128,15 +128,15 @@
 ├─────────────┼────────┼───────┤
 │ Total       │    100 │   273 │
 └─────────────┴────────┴───────┘
 ```
 
 ### Convert and Save to Many Formats
 
-Datasets can be converted to and saved in other formats easily:
+Datasets can be converted to and saved in other formats:
 
 ```python
 # ImageNet
 gts.save_imagenet(save_dir="pascalVOC_db/")
 
 # YOLO Darknet
 gts.save_yolo_darknet(
@@ -152,15 +152,15 @@
 
 # CVAT
 gts.save_cvat(path="train.xml")
 ```
 
 ### COCO Evaluation
 
-Evaluating is as easy as:
+COCO Evaluation is also supported:
 
 ```python
 evaluator = COCOEvaluator(
     ground_truths=gts, 
     predictions=dets
 )
 
@@ -215,14 +215,24 @@
 cat_ar = evaluation["cat"].ar
 ```
 
 Evaluations are cached by `(iou_threshold, max_detections, size_range)` keys. This means that you should not care about about performance, repetead queries to the evaluator are fast!
 
 ## Use in Command Line
 
+If you only need to use Globox from the command line like an application, you can install the package through [pipx](https://pypa.github.io/pipx/):
+
+```shell
+pipx install globox
+```
+
+Globox will then be in your shell path and usable from anywhere.
+
+### Usage
+
 Get a summary of annotations for one dataset:
 
 ```shell
 globox summary /yolo/folder/ --format yolo
 ```
 
 Convert annotations from one format to another one:
```

### Comparing `globox-2.1.1/src/globox.egg-info/SOURCES.txt` & `globox-2.1.2/src/globox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globox-2.1.1/tests/test_annotation.py` & `globox-2.1.2/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.1/tests/test_annotationset.py` & `globox-2.1.2/tests/test_annotationset.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.1/tests/test_bbox.py` & `globox-2.1.2/tests/test_bbox.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.1/tests/test_coco_evaluation.py` & `globox-2.1.2/tests/test_coco_evaluation.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.1/tests/test_conversion.py` & `globox-2.1.2/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `globox-2.1.1/tests/test_parsing.py` & `globox-2.1.2/tests/test_parsing.py`

 * *Files identical despite different names*

