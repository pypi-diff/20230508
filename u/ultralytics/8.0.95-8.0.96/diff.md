# Comparing `tmp/ultralytics-8.0.95.tar.gz` & `tmp/ultralytics-8.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics-8.0.95.tar", last modified: Mon May  8 20:36:59 2023, max compression
+gzip compressed data, was "ultralytics-8.0.96.tar", last modified: Mon May  8 21:43:39 2023, max compression
```

## Comparing `ultralytics-8.0.95.tar` & `ultralytics-8.0.96.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.357214 ultralytics-8.0.95/
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-08 20:35:18.000000 ultralytics-8.0.95/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-08 20:35:18.000000 ultralytics-8.0.95/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-08 20:35:18.000000 ultralytics-8.0.95/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-05-08 20:36:59.357214 ultralytics-8.0.95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-05-08 20:35:18.000000 ultralytics-8.0.95/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    23225 2023-05-08 20:35:18.000000 ultralytics-8.0.95/README.zh-CN.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-08 20:35:18.000000 ultralytics-8.0.95/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-08 20:36:59.357214 ultralytics-8.0.95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-08 20:35:18.000000 ultralytics-8.0.95/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.337214 ultralytics-8.0.95/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-08 20:35:18.000000 ultralytics-8.0.95/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-08 20:35:18.000000 ultralytics-8.0.95/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-08 20:35:18.000000 ultralytics-8.0.95/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.337214 ultralytics-8.0.95/ultralytics/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.337214 ultralytics-8.0.95/ultralytics/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/assets/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    50427 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.341214 ultralytics-8.0.95/ultralytics/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/datasets/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    42439 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/datasets/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/datasets/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/datasets/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/datasets/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/datasets/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/datasets/coco-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/datasets/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/datasets/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/datasets/coco128.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/datasets/coco8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/datasets/coco8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/datasets/coco8.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/datasets/xView.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.341214 ultralytics-8.0.95/ultralytics/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/hub/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.333213 ultralytics-8.0.95/ultralytics/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.341214 ultralytics-8.0.95/ultralytics/models/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/models/v3/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/models/v3/yolov3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.341214 ultralytics-8.0.95/ultralytics/models/v5/
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/models/v5/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/models/v5/yolov5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.341214 ultralytics-8.0.95/ultralytics/models/v8/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/models/v8/yolov8-cls.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/models/v8/yolov8-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/models/v8/yolov8-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/models/v8/yolov8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/models/v8/yolov8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/models/v8/yolov8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.341214 ultralytics-8.0.95/ultralytics/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24243 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/nn/autobackend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/nn/autoshape.py
--rw-r--r--   0 runner    (1001) docker     (123)    25079 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/nn/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    27170 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/nn/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.345214 ultralytics-8.0.95/ultralytics/tracker/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/tracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.345214 ultralytics-8.0.95/ultralytics/tracker/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/tracker/cfg/botsort.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/tracker/cfg/bytetrack.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/tracker/track.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.345214 ultralytics-8.0.95/ultralytics/tracker/trackers/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/tracker/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/tracker/trackers/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/tracker/trackers/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/tracker/trackers/byte_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.345214 ultralytics-8.0.95/ultralytics/tracker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/tracker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/tracker/utils/gmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/tracker/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/tracker/utils/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.345214 ultralytics-8.0.95/ultralytics/vit/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/vit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.345214 ultralytics-8.0.95/ultralytics/vit/sam/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/vit/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/vit/sam/amg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/vit/sam/autosize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/vit/sam/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/vit/sam/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.345214 ultralytics-8.0.95/ultralytics/vit/sam/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/vit/sam/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/vit/sam/modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22502 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/vit/sam/modules/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/vit/sam/modules/mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/vit/sam/modules/prompt_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/vit/sam/modules/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/vit/sam/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/vit/sam/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.345214 ultralytics-8.0.95/ultralytics/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.345214 ultralytics-8.0.95/ultralytics/yolo/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)    17817 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/cfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/cfg/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.349214 ultralytics-8.0.95/ultralytics/yolo/data/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/data/annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)    33512 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/data/augment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/data/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/data/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.349214 ultralytics-8.0.95/ultralytics/yolo/data/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/data/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/data/dataloaders/stream_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/data/dataloaders/v5augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)    51260 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/data/dataloaders/v5loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/data/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    23582 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.349214 ultralytics-8.0.95/ultralytics/yolo/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40265 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/engine/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/engine/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15927 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/engine/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20634 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/engine/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    31310 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/engine/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/engine/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.353214 ultralytics-8.0.95/ultralytics/yolo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.353214 ultralytics-8.0.95/ultralytics/yolo/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/callbacks/clearml.py
--rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/callbacks/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/callbacks/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/callbacks/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/callbacks/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/callbacks/raytune.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/callbacks/wb.py
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    41903 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    28191 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    24037 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/tal.py
--rw-r--r--   0 runner    (1001) docker     (123)    20019 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/utils/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.353214 ultralytics-8.0.95/ultralytics/yolo/v8/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/v8/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.353214 ultralytics-8.0.95/ultralytics/yolo/v8/classify/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/v8/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/v8/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/v8/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/v8/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.353214 ultralytics-8.0.95/ultralytics/yolo/v8/detect/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/v8/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/v8/detect/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/v8/detect/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/v8/detect/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.353214 ultralytics-8.0.95/ultralytics/yolo/v8/pose/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/v8/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/v8/pose/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/v8/pose/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/v8/pose/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.357214 ultralytics-8.0.95/ultralytics/yolo/v8/segment/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/v8/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/v8/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/v8/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-05-08 20:35:18.000000 ultralytics-8.0.95/ultralytics/yolo/v8/segment/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:36:59.337214 ultralytics-8.0.95/ultralytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-05-08 20:36:59.000000 ultralytics-8.0.95/ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-08 20:36:59.000000 ultralytics-8.0.95/ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:36:59.000000 ultralytics-8.0.95/ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-08 20:36:59.000000 ultralytics-8.0.95/ultralytics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-08 20:36:59.000000 ultralytics-8.0.95/ultralytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 20:36:59.000000 ultralytics-8.0.95/ultralytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.374660 ultralytics-8.0.96/
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-08 21:41:42.000000 ultralytics-8.0.96/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-08 21:41:42.000000 ultralytics-8.0.96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-08 21:41:42.000000 ultralytics-8.0.96/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25911 2023-05-08 21:43:39.374660 ultralytics-8.0.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-05-08 21:41:42.000000 ultralytics-8.0.96/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23225 2023-05-08 21:41:42.000000 ultralytics-8.0.96/README.zh-CN.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-08 21:41:42.000000 ultralytics-8.0.96/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-08 21:43:39.374660 ultralytics-8.0.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-08 21:41:42.000000 ultralytics-8.0.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.342659 ultralytics-8.0.96/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-08 21:41:42.000000 ultralytics-8.0.96/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-08 21:41:42.000000 ultralytics-8.0.96/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-08 21:41:42.000000 ultralytics-8.0.96/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.342659 ultralytics-8.0.96/ultralytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.342659 ultralytics-8.0.96/ultralytics/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/assets/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    50427 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.346659 ultralytics-8.0.96/ultralytics/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/datasets/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    42439 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/datasets/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/datasets/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/datasets/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/datasets/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/datasets/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/datasets/coco-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/datasets/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/datasets/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/datasets/coco128.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/datasets/coco8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/datasets/coco8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/datasets/coco8.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/datasets/xView.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.346659 ultralytics-8.0.96/ultralytics/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/hub/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.338659 ultralytics-8.0.96/ultralytics/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.350659 ultralytics-8.0.96/ultralytics/models/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/models/v3/yolov3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.350659 ultralytics-8.0.96/ultralytics/models/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/models/v5/yolov5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.350659 ultralytics-8.0.96/ultralytics/models/v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/models/v8/yolov8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.350659 ultralytics-8.0.96/ultralytics/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24243 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/nn/autobackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/nn/autoshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25079 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/nn/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27170 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/nn/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.354659 ultralytics-8.0.96/ultralytics/tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/tracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.354659 ultralytics-8.0.96/ultralytics/tracker/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/tracker/cfg/botsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/tracker/cfg/bytetrack.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/tracker/track.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.354659 ultralytics-8.0.96/ultralytics/tracker/trackers/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/tracker/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/tracker/trackers/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/tracker/trackers/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/tracker/trackers/byte_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.354659 ultralytics-8.0.96/ultralytics/tracker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/tracker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/tracker/utils/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/tracker/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/tracker/utils/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.354659 ultralytics-8.0.96/ultralytics/vit/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/vit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.358660 ultralytics-8.0.96/ultralytics/vit/sam/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/vit/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/vit/sam/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/vit/sam/autosize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/vit/sam/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/vit/sam/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.358660 ultralytics-8.0.96/ultralytics/vit/sam/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/vit/sam/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/vit/sam/modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22502 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/vit/sam/modules/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/vit/sam/modules/mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/vit/sam/modules/prompt_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/vit/sam/modules/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/vit/sam/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/vit/sam/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.358660 ultralytics-8.0.96/ultralytics/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.358660 ultralytics-8.0.96/ultralytics/yolo/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)    17817 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/cfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/cfg/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.362660 ultralytics-8.0.96/ultralytics/yolo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/data/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33512 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/data/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.362660 ultralytics-8.0.96/ultralytics/yolo/data/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/data/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/data/dataloaders/stream_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/data/dataloaders/v5augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51260 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/data/dataloaders/v5loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/data/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23582 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.362660 ultralytics-8.0.96/ultralytics/yolo/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40265 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/engine/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/engine/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15927 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/engine/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20634 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/engine/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31310 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/engine/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/engine/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.366659 ultralytics-8.0.96/ultralytics/yolo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.370660 ultralytics-8.0.96/ultralytics/yolo/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/callbacks/clearml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/callbacks/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/callbacks/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/callbacks/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/callbacks/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/callbacks/raytune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/callbacks/wb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41908 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28191 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24037 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/tal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20019 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/utils/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.370660 ultralytics-8.0.96/ultralytics/yolo/v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/v8/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.370660 ultralytics-8.0.96/ultralytics/yolo/v8/classify/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/v8/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/v8/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/v8/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/v8/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.370660 ultralytics-8.0.96/ultralytics/yolo/v8/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/v8/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/v8/detect/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/v8/detect/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/v8/detect/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.370660 ultralytics-8.0.96/ultralytics/yolo/v8/pose/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/v8/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/v8/pose/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/v8/pose/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/v8/pose/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.374660 ultralytics-8.0.96/ultralytics/yolo/v8/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/v8/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/v8/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/v8/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-05-08 21:41:42.000000 ultralytics-8.0.96/ultralytics/yolo/v8/segment/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:43:39.342659 ultralytics-8.0.96/ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25911 2023-05-08 21:43:39.000000 ultralytics-8.0.96/ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-08 21:43:39.000000 ultralytics-8.0.96/ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:43:39.000000 ultralytics-8.0.96/ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-08 21:43:39.000000 ultralytics-8.0.96/ultralytics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-08 21:43:39.000000 ultralytics-8.0.96/ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 21:43:39.000000 ultralytics-8.0.96/ultralytics.egg-info/top_level.txt
```

### Comparing `ultralytics-8.0.95/CONTRIBUTING.md` & `ultralytics-8.0.96/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/LICENSE` & `ultralytics-8.0.96/LICENSE`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/PKG-INFO` & `ultralytics-8.0.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.0.95
-Summary: Ultralytics YOLOv8
+Version: 8.0.96
+Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Home-page: https://github.com/ultralytics/ultralytics
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/ultralytics
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.0.95 Summary: Ultralytics
-YOLOv8 Home-page: https://github.com/ultralytics/ultralytics Author:
-Ultralytics Author-email: hello@ultralytics.com License: AGPL-3.0 Project-URL:
-Bug Reports, https://github.com/ultralytics/ultralytics/issues Project-URL:
-Funding, https://ultralytics.com Project-URL: Source, https://github.com/
-ultralytics/ultralytics Keywords: machine-learning,deep-
+Metadata-Version: 2.1 Name: ultralytics Version: 8.0.96 Summary: Ultralytics
+YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
+pose estimation and image classification. Home-page: https://github.com/
+ultralytics/ultralytics Author: Ultralytics Author-email: hello@ultralytics.com
+License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
+ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
+Source, https://github.com/ultralytics/ultralytics Keywords: machine-
+learning,deep-
 learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: GNU Affero General
 Public License v3 or later (AGPLv3+) Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ultralytics-8.0.95/README.md` & `ultralytics-8.0.96/README.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/README.zh-CN.md` & `ultralytics-8.0.96/README.zh-CN.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/requirements.txt` & `ultralytics-8.0.96/requirements.txt`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/setup.cfg` & `ultralytics-8.0.96/setup.cfg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/setup.py` & `ultralytics-8.0.96/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 
 
 setup(
     name='ultralytics',  # name of pypi package
     version=get_version(),  # version of pypi package
     python_requires='>=3.7',
     license='AGPL-3.0',
-    description='Ultralytics YOLOv8',
+    description=('Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, '
+                 'pose estimation and image classification.'),
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/ultralytics/ultralytics',
     project_urls={
         'Bug Reports': 'https://github.com/ultralytics/ultralytics/issues',
         'Funding': 'https://ultralytics.com',
         'Source': 'https://github.com/ultralytics/ultralytics'},
@@ -43,14 +44,15 @@
             'pytest',
             'pytest-cov',
             'coverage',
             'mkdocs-material',
             'mkdocstrings[python]',
             'mkdocs-redirects',  # for 301 redirects
             'mkdocs-git-revision-date-localized-plugin',  # for created/updated dates
+            'mkdocs-ultralytics-plugin',  # for meta descriptions and images
         ],
         'export': ['coremltools>=6.0', 'openvino-dev>=2022.3', 'tensorflowjs'],  # automatically installs tensorflow
     },
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
```

### Comparing `ultralytics-8.0.95/tests/test_cli.py` & `ultralytics-8.0.96/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/tests/test_engine.py` & `ultralytics-8.0.96/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/tests/test_python.py` & `ultralytics-8.0.96/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/assets/bus.jpg` & `ultralytics-8.0.96/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/assets/zidane.jpg` & `ultralytics-8.0.96/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/datasets/Argoverse.yaml` & `ultralytics-8.0.96/ultralytics/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/datasets/GlobalWheat2020.yaml` & `ultralytics-8.0.96/ultralytics/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/datasets/ImageNet.yaml` & `ultralytics-8.0.96/ultralytics/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/datasets/Objects365.yaml` & `ultralytics-8.0.96/ultralytics/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/datasets/SKU-110K.yaml` & `ultralytics-8.0.96/ultralytics/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/datasets/VOC.yaml` & `ultralytics-8.0.96/ultralytics/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/datasets/VisDrone.yaml` & `ultralytics-8.0.96/ultralytics/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/datasets/coco-pose.yaml` & `ultralytics-8.0.96/ultralytics/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/datasets/coco.yaml` & `ultralytics-8.0.96/ultralytics/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/datasets/coco128-seg.yaml` & `ultralytics-8.0.96/ultralytics/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/datasets/coco128.yaml` & `ultralytics-8.0.96/ultralytics/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/datasets/coco8-pose.yaml` & `ultralytics-8.0.96/ultralytics/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/datasets/coco8-seg.yaml` & `ultralytics-8.0.96/ultralytics/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/datasets/coco8.yaml` & `ultralytics-8.0.96/ultralytics/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/datasets/xView.yaml` & `ultralytics-8.0.96/ultralytics/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/hub/__init__.py` & `ultralytics-8.0.96/ultralytics/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/hub/auth.py` & `ultralytics-8.0.96/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/hub/session.py` & `ultralytics-8.0.96/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/hub/utils.py` & `ultralytics-8.0.96/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/models/v3/yolov3-spp.yaml` & `ultralytics-8.0.96/ultralytics/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/models/v3/yolov3-tiny.yaml` & `ultralytics-8.0.96/ultralytics/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/models/v3/yolov3.yaml` & `ultralytics-8.0.96/ultralytics/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/models/v5/yolov5-p6.yaml` & `ultralytics-8.0.96/ultralytics/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/models/v5/yolov5.yaml` & `ultralytics-8.0.96/ultralytics/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/models/v8/yolov8-cls.yaml` & `ultralytics-8.0.96/ultralytics/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/models/v8/yolov8-p2.yaml` & `ultralytics-8.0.96/ultralytics/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/models/v8/yolov8-p6.yaml` & `ultralytics-8.0.96/ultralytics/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/models/v8/yolov8-pose-p6.yaml` & `ultralytics-8.0.96/ultralytics/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/models/v8/yolov8-pose.yaml` & `ultralytics-8.0.96/ultralytics/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/models/v8/yolov8-seg.yaml` & `ultralytics-8.0.96/ultralytics/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/models/v8/yolov8.yaml` & `ultralytics-8.0.96/ultralytics/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/nn/autobackend.py` & `ultralytics-8.0.96/ultralytics/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/nn/autoshape.py` & `ultralytics-8.0.96/ultralytics/nn/autoshape.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/nn/modules.py` & `ultralytics-8.0.96/ultralytics/nn/modules.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/nn/tasks.py` & `ultralytics-8.0.96/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/tracker/cfg/botsort.yaml` & `ultralytics-8.0.96/ultralytics/tracker/cfg/botsort.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/tracker/cfg/bytetrack.yaml` & `ultralytics-8.0.96/ultralytics/tracker/cfg/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/tracker/track.py` & `ultralytics-8.0.96/ultralytics/tracker/track.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/tracker/trackers/basetrack.py` & `ultralytics-8.0.96/ultralytics/tracker/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/tracker/trackers/bot_sort.py` & `ultralytics-8.0.96/ultralytics/tracker/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/tracker/trackers/byte_tracker.py` & `ultralytics-8.0.96/ultralytics/tracker/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/tracker/utils/gmc.py` & `ultralytics-8.0.96/ultralytics/tracker/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/tracker/utils/kalman_filter.py` & `ultralytics-8.0.96/ultralytics/tracker/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/tracker/utils/matching.py` & `ultralytics-8.0.96/ultralytics/tracker/utils/matching.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/vit/sam/amg.py` & `ultralytics-8.0.96/ultralytics/vit/sam/amg.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/vit/sam/autosize.py` & `ultralytics-8.0.96/ultralytics/vit/sam/autosize.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/vit/sam/build.py` & `ultralytics-8.0.96/ultralytics/vit/sam/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/vit/sam/model.py` & `ultralytics-8.0.96/ultralytics/vit/sam/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/vit/sam/modules/decoders.py` & `ultralytics-8.0.96/ultralytics/vit/sam/modules/decoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/vit/sam/modules/encoders.py` & `ultralytics-8.0.96/ultralytics/vit/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/vit/sam/modules/mask_generator.py` & `ultralytics-8.0.96/ultralytics/vit/sam/modules/mask_generator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/vit/sam/modules/prompt_predictor.py` & `ultralytics-8.0.96/ultralytics/vit/sam/modules/prompt_predictor.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/vit/sam/modules/sam.py` & `ultralytics-8.0.96/ultralytics/vit/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/vit/sam/modules/transformer.py` & `ultralytics-8.0.96/ultralytics/vit/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/vit/sam/predict.py` & `ultralytics-8.0.96/ultralytics/vit/sam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/cfg/__init__.py` & `ultralytics-8.0.96/ultralytics/yolo/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/cfg/default.yaml` & `ultralytics-8.0.96/ultralytics/yolo/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/data/annotator.py` & `ultralytics-8.0.96/ultralytics/yolo/data/annotator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/data/augment.py` & `ultralytics-8.0.96/ultralytics/yolo/data/augment.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/data/base.py` & `ultralytics-8.0.96/ultralytics/yolo/data/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/data/build.py` & `ultralytics-8.0.96/ultralytics/yolo/data/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/data/converter.py` & `ultralytics-8.0.96/ultralytics/yolo/data/converter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/data/dataloaders/stream_loaders.py` & `ultralytics-8.0.96/ultralytics/yolo/data/dataloaders/stream_loaders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/data/dataloaders/v5augmentations.py` & `ultralytics-8.0.96/ultralytics/yolo/data/dataloaders/v5augmentations.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/data/dataloaders/v5loader.py` & `ultralytics-8.0.96/ultralytics/yolo/data/dataloaders/v5loader.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/data/dataset.py` & `ultralytics-8.0.96/ultralytics/yolo/data/dataset.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/data/dataset_wrappers.py` & `ultralytics-8.0.96/ultralytics/yolo/data/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/data/utils.py` & `ultralytics-8.0.96/ultralytics/yolo/data/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/engine/exporter.py` & `ultralytics-8.0.96/ultralytics/yolo/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/engine/model.py` & `ultralytics-8.0.96/ultralytics/yolo/engine/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/engine/predictor.py` & `ultralytics-8.0.96/ultralytics/yolo/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/engine/results.py` & `ultralytics-8.0.96/ultralytics/yolo/engine/results.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/engine/trainer.py` & `ultralytics-8.0.96/ultralytics/yolo/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/engine/validator.py` & `ultralytics-8.0.96/ultralytics/yolo/engine/validator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/__init__.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/autobatch.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/benchmarks.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/callbacks/base.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/callbacks/clearml.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/callbacks/clearml.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,17 +80,23 @@
                            'please add clearml-init and connect your arguments before initializing YOLO.')
         task.connect(vars(trainer.args), name='General')
     except Exception as e:
         LOGGER.warning(f'WARNING ⚠️ ClearML installed but not initialized correctly, not logging this run. {e}')
 
 
 def on_train_epoch_end(trainer):
-    """Logs debug samples for the first epoch of YOLO training."""
-    if trainer.epoch == 1 and Task.current_task():
-        _log_debug_samples(sorted(trainer.save_dir.glob('train_batch*.jpg')), 'Mosaic')
+    task = Task.current_task()
+
+    if task:
+        """Logs debug samples for the first epoch of YOLO training."""
+        if trainer.epoch == 1:
+            _log_debug_samples(sorted(trainer.save_dir.glob('train_batch*.jpg')), 'Mosaic')
+        """Report the current training progress."""
+        for k, v in trainer.validator.metrics.results_dict.items():
+            task.get_logger().report_scalar('train', k, v, iteration=trainer.epoch)
 
 
 def on_fit_epoch_end(trainer):
     """Reports model information to logger at the end of an epoch."""
     task = Task.current_task()
     if task:
         # You should have access to the validation bboxes under jdict
@@ -115,15 +121,17 @@
 
 
 def on_train_end(trainer):
     """Logs final model and its name on training completion."""
     task = Task.current_task()
     if task:
         # Log final results, CM matrix + PR plots
-        files = ['results.png', 'confusion_matrix.png', *(f'{x}_curve.png' for x in ('F1', 'PR', 'P', 'R'))]
+        files = [
+            'results.png', 'confusion_matrix.png', 'confusion_matrix_normalized.png',
+            *(f'{x}_curve.png' for x in ('F1', 'PR', 'P', 'R'))]
         files = [(trainer.save_dir / f) for f in files if (trainer.save_dir / f).exists()]  # filter
         for f in files:
             _log_plot(title=f.stem, plot_path=f)
         # Report final metrics
         for k, v in trainer.validator.metrics.results_dict.items():
             task.get_logger().report_single_value(k, v)
         # Log the final model
```

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/callbacks/comet.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/callbacks/hub.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/callbacks/mlflow.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/callbacks/neptune.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/callbacks/neptune.py`

 * *Files 8% similar despite different names*

```diff
@@ -83,15 +83,17 @@
         _log_images({f.stem: str(f) for f in validator.save_dir.glob('val*.jpg')}, 'Validation')
 
 
 def on_train_end(trainer):
     """Callback function called at end of training."""
     if run:
         # Log final results, CM matrix + PR plots
-        files = ['results.png', 'confusion_matrix.png', *(f'{x}_curve.png' for x in ('F1', 'PR', 'P', 'R'))]
+        files = [
+            'results.png', 'confusion_matrix.png', 'confusion_matrix_normalized.png',
+            *(f'{x}_curve.png' for x in ('F1', 'PR', 'P', 'R'))]
         files = [(trainer.save_dir / f) for f in files if (trainer.save_dir / f).exists()]  # filter
         for f in files:
             _log_plot(title=f.stem, plot_path=f)
         # Log the final model
         run[f'weights/{trainer.args.name or trainer.args.task}/{str(trainer.best.name)}'].upload(File(str(
             trainer.best)))
         run.stop()
```

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/callbacks/tensorboard.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/callbacks/wb.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/checks.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/checks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/dist.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/dist.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/downloads.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/files.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/files.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/instance.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/instance.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/loss.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/loss.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/metrics.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,25 +317,26 @@
         fig, ax = plt.subplots(1, 1, figsize=(12, 9), tight_layout=True)
         nc, nn = self.nc, len(names)  # number of classes, names
         sn.set(font_scale=1.0 if nc < 50 else 0.8)  # for label size
         labels = (0 < nn < 99) and (nn == nc)  # apply names to ticklabels
         ticklabels = (list(names) + ['background']) if labels else 'auto'
         with warnings.catch_warnings():
             warnings.simplefilter('ignore')  # suppress empty matrix RuntimeWarning: All-NaN slice encountered
-            sn.heatmap(array,
-                       ax=ax,
-                       annot=nc < 30,
-                       annot_kws={
-                           'size': 8},
-                       cmap='Blues',
-                       fmt='.2f',
-                       square=True,
-                       vmin=0.0,
-                       xticklabels=ticklabels,
-                       yticklabels=ticklabels).set_facecolor((1, 1, 1))
+            sn.heatmap(
+                array,
+                ax=ax,
+                annot=nc < 30,
+                annot_kws={
+                    'size': 8},
+                cmap='Blues',
+                fmt='.2f' if normalize else '%d',  # float if normalize else integer
+                square=True,
+                vmin=0.0,
+                xticklabels=ticklabels,
+                yticklabels=ticklabels).set_facecolor((1, 1, 1))
         title = 'Confusion Matrix' + ' Normalized' * normalize
         ax.set_xlabel('True')
         ax.set_ylabel('Predicted')
         ax.set_title(title)
         fig.savefig(Path(save_dir) / f'{title.lower().replace(" ", "_")}.png', dpi=250)
         plt.close(fig)
```

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/ops.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/ops.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/plotting.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/tal.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/tal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import torch
 import torch.nn as nn
-import torch.nn.functional as F
 
 from .checks import check_version
 from .metrics import bbox_iou
 
 TORCH_1_10 = check_version(torch.__version__, '1.10.0')
 
 
@@ -40,17 +39,19 @@
         mask_pos (Tensor): shape(b, n_max_boxes, h*w)
     """
     # (b, n_max_boxes, h*w) -> (b, h*w)
     fg_mask = mask_pos.sum(-2)
     if fg_mask.max() > 1:  # one anchor is assigned to multiple gt_bboxes
         mask_multi_gts = (fg_mask.unsqueeze(1) > 1).repeat([1, n_max_boxes, 1])  # (b, n_max_boxes, h*w)
         max_overlaps_idx = overlaps.argmax(1)  # (b, h*w)
-        is_max_overlaps = F.one_hot(max_overlaps_idx, n_max_boxes)  # (b, h*w, n_max_boxes)
-        is_max_overlaps = is_max_overlaps.permute(0, 2, 1).to(overlaps.dtype)  # (b, n_max_boxes, h*w)
-        mask_pos = torch.where(mask_multi_gts, is_max_overlaps, mask_pos)  # (b, n_max_boxes, h*w)
+
+        is_max_overlaps = torch.zeros(mask_pos.shape, dtype=mask_pos.dtype, device=mask_pos.device)
+        is_max_overlaps.scatter_(1, max_overlaps_idx.unsqueeze(1), 1)
+
+        mask_pos = torch.where(mask_multi_gts, is_max_overlaps, mask_pos).float()  # (b, n_max_boxes, h*w)
         fg_mask = mask_pos.sum(-2)
     # Find each grid serve which gt(index)
     target_gt_idx = mask_pos.argmax(-2)  # (b, h*w)
     return target_gt_idx, fg_mask, mask_pos
 
 
 class TaskAlignedAssigner(nn.Module):
@@ -171,29 +172,31 @@
                                 topk is the number of top candidates to consider. If not provided,
                                 the top-k values are automatically computed based on the given metrics.
 
         Returns:
             (Tensor): A tensor of shape (b, max_num_obj, h*w) containing the selected top-k candidates.
         """
 
-        num_anchors = metrics.shape[-1]  # h*w
         # (b, max_num_obj, topk)
         topk_metrics, topk_idxs = torch.topk(metrics, self.topk, dim=-1, largest=largest)
         if topk_mask is None:
-            topk_mask = (topk_metrics.max(-1, keepdim=True) > self.eps).tile([1, 1, self.topk])
+            topk_mask = (topk_metrics.max(-1, keepdim=True)[0] > self.eps).expand_as(topk_idxs)
         # (b, max_num_obj, topk)
-        topk_idxs[~topk_mask] = 0
+        topk_idxs.masked_fill_(~topk_mask, 0)
+
         # (b, max_num_obj, topk, h*w) -> (b, max_num_obj, h*w)
-        is_in_topk = torch.zeros(metrics.shape, dtype=torch.long, device=metrics.device)
-        for it in range(self.topk):
-            is_in_topk += F.one_hot(topk_idxs[:, :, it], num_anchors)
-        # is_in_topk = F.one_hot(topk_idxs, num_anchors).sum(-2)
+        count_tensor = torch.zeros(metrics.shape, dtype=torch.int8, device=topk_idxs.device)
+        ones = torch.ones_like(topk_idxs[:, :, :1], dtype=torch.int8, device=topk_idxs.device)
+        for k in range(self.topk):
+            # Expand topk_idxs for each value of k and add 1 at the specified positions
+            count_tensor.scatter_add_(-1, topk_idxs[:, :, k:k + 1], ones)
         # filter invalid bboxes
-        is_in_topk = torch.where(is_in_topk > 1, 0, is_in_topk)
-        return is_in_topk.to(metrics.dtype)
+        count_tensor.masked_fill_(count_tensor > 1, 0)
+
+        return count_tensor.to(metrics.dtype)
 
     def get_targets(self, gt_labels, gt_bboxes, target_gt_idx, fg_mask):
         """
         Compute target labels, target bounding boxes, and target scores for the positive anchor points.
 
         Args:
             gt_labels (Tensor): Ground truth labels of shape (b, max_num_obj, 1), where b is the
@@ -222,15 +225,21 @@
         target_labels = gt_labels.long().flatten()[target_gt_idx]  # (b, h*w)
 
         # Assigned target boxes, (b, max_num_obj, 4) -> (b, h*w)
         target_bboxes = gt_bboxes.view(-1, 4)[target_gt_idx]
 
         # Assigned target scores
         target_labels.clamp_(0)
-        target_scores = F.one_hot(target_labels, self.num_classes)  # (b, h*w, 80)
+
+        # 10x faster than F.one_hot()
+        target_scores = torch.zeros((target_labels.shape[0], target_labels.shape[1], self.num_classes),
+                                    dtype=torch.int64,
+                                    device=target_labels.device)  # (b, h*w, 80)
+        target_scores.scatter_(2, target_labels.unsqueeze(-1), 1)
+
         fg_scores_mask = fg_mask[:, :, None].repeat(1, 1, self.num_classes)  # (b, h*w, 80)
         target_scores = torch.where(fg_scores_mask > 0, target_scores, 0)
 
         return target_labels, target_bboxes, target_scores
 
 
 def make_anchors(feats, strides, grid_cell_offset=0.5):
```

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/torch_utils.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/utils/tuner.py` & `ultralytics-8.0.96/ultralytics/yolo/utils/tuner.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/v8/classify/predict.py` & `ultralytics-8.0.96/ultralytics/yolo/v8/classify/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/v8/classify/train.py` & `ultralytics-8.0.96/ultralytics/yolo/v8/classify/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/v8/classify/val.py` & `ultralytics-8.0.96/ultralytics/yolo/v8/classify/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/v8/detect/predict.py` & `ultralytics-8.0.96/ultralytics/yolo/v8/detect/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/v8/detect/train.py` & `ultralytics-8.0.96/ultralytics/yolo/v8/detect/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/v8/detect/val.py` & `ultralytics-8.0.96/ultralytics/yolo/v8/detect/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/v8/pose/predict.py` & `ultralytics-8.0.96/ultralytics/yolo/v8/pose/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/v8/pose/train.py` & `ultralytics-8.0.96/ultralytics/yolo/v8/pose/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/v8/pose/val.py` & `ultralytics-8.0.96/ultralytics/yolo/v8/pose/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/v8/segment/predict.py` & `ultralytics-8.0.96/ultralytics/yolo/v8/segment/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/v8/segment/train.py` & `ultralytics-8.0.96/ultralytics/yolo/v8/segment/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics/yolo/v8/segment/val.py` & `ultralytics-8.0.96/ultralytics/yolo/v8/segment/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.95/ultralytics.egg-info/PKG-INFO` & `ultralytics-8.0.96/ultralytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.0.95
-Summary: Ultralytics YOLOv8
+Version: 8.0.96
+Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Home-page: https://github.com/ultralytics/ultralytics
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/ultralytics
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.0.95 Summary: Ultralytics
-YOLOv8 Home-page: https://github.com/ultralytics/ultralytics Author:
-Ultralytics Author-email: hello@ultralytics.com License: AGPL-3.0 Project-URL:
-Bug Reports, https://github.com/ultralytics/ultralytics/issues Project-URL:
-Funding, https://ultralytics.com Project-URL: Source, https://github.com/
-ultralytics/ultralytics Keywords: machine-learning,deep-
+Metadata-Version: 2.1 Name: ultralytics Version: 8.0.96 Summary: Ultralytics
+YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
+pose estimation and image classification. Home-page: https://github.com/
+ultralytics/ultralytics Author: Ultralytics Author-email: hello@ultralytics.com
+License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
+ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
+Source, https://github.com/ultralytics/ultralytics Keywords: machine-
+learning,deep-
 learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: GNU Affero General
 Public License v3 or later (AGPLv3+) Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ultralytics-8.0.95/ultralytics.egg-info/SOURCES.txt` & `ultralytics-8.0.96/ultralytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

