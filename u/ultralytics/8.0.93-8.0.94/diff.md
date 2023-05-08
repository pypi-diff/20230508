# Comparing `tmp/ultralytics-8.0.93.tar.gz` & `tmp/ultralytics-8.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics-8.0.93.tar", last modified: Fri May  5 23:14:31 2023, max compression
+gzip compressed data, was "ultralytics-8.0.94.tar", last modified: Mon May  8 00:01:02 2023, max compression
```

## Comparing `ultralytics-8.0.93.tar` & `ultralytics-8.0.94.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.110600 ultralytics-8.0.93/
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-05 23:12:57.000000 ultralytics-8.0.93/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-05 23:12:57.000000 ultralytics-8.0.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-05 23:12:57.000000 ultralytics-8.0.93/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-05-05 23:14:31.110600 ultralytics-8.0.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-05-05 23:12:57.000000 ultralytics-8.0.93/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    23225 2023-05-05 23:12:57.000000 ultralytics-8.0.93/README.zh-CN.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-05 23:12:57.000000 ultralytics-8.0.93/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-05 23:14:31.110600 ultralytics-8.0.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-05 23:12:57.000000 ultralytics-8.0.93/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.090600 ultralytics-8.0.93/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-05 23:12:57.000000 ultralytics-8.0.93/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-05 23:12:57.000000 ultralytics-8.0.93/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-05 23:12:57.000000 ultralytics-8.0.93/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.090600 ultralytics-8.0.93/ultralytics/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.090600 ultralytics-8.0.93/ultralytics/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/assets/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    50427 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.094600 ultralytics-8.0.93/ultralytics/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    42439 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/coco-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/coco128.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/coco8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/coco8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/coco8.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/xView.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.094600 ultralytics-8.0.93/ultralytics/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/hub/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.086599 ultralytics-8.0.93/ultralytics/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.094600 ultralytics-8.0.93/ultralytics/models/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v3/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v3/yolov3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.094600 ultralytics-8.0.93/ultralytics/models/v5/
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v5/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v5/yolov5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.094600 ultralytics-8.0.93/ultralytics/models/v8/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v8/yolov8-cls.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v8/yolov8-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v8/yolov8-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v8/yolov8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v8/yolov8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v8/yolov8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.098600 ultralytics-8.0.93/ultralytics/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24243 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/nn/autobackend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/nn/autoshape.py
--rw-r--r--   0 runner    (1001) docker     (123)    25079 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/nn/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    27170 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/nn/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.098600 ultralytics-8.0.93/ultralytics/tracker/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.098600 ultralytics-8.0.93/ultralytics/tracker/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/cfg/botsort.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/cfg/bytetrack.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/track.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.098600 ultralytics-8.0.93/ultralytics/tracker/trackers/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/trackers/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/trackers/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/trackers/byte_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.098600 ultralytics-8.0.93/ultralytics/tracker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/utils/gmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/utils/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.098600 ultralytics-8.0.93/ultralytics/vit/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.098600 ultralytics-8.0.93/ultralytics/vit/sam/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/amg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/autosize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.102600 ultralytics-8.0.93/ultralytics/vit/sam/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22502 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/modules/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/modules/mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/modules/prompt_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/modules/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.102600 ultralytics-8.0.93/ultralytics/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.102600 ultralytics-8.0.93/ultralytics/yolo/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)    17819 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/cfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/cfg/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.102600 ultralytics-8.0.93/ultralytics/yolo/data/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)    33512 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/augment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.102600 ultralytics-8.0.93/ultralytics/yolo/data/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/dataloaders/stream_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/dataloaders/v5augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)    51260 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/dataloaders/v5loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22741 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.102600 ultralytics-8.0.93/ultralytics/yolo/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40265 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/engine/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/engine/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15927 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/engine/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20634 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/engine/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    31310 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/engine/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/engine/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.106600 ultralytics-8.0.93/ultralytics/yolo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.106600 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/clearml.py
--rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/raytune.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/wb.py
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    41829 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    28191 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    24037 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/tal.py
--rw-r--r--   0 runner    (1001) docker     (123)    20019 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.106600 ultralytics-8.0.93/ultralytics/yolo/v8/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.110600 ultralytics-8.0.93/ultralytics/yolo/v8/classify/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.110600 ultralytics-8.0.93/ultralytics/yolo/v8/detect/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/detect/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    12199 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/detect/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/detect/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.110600 ultralytics-8.0.93/ultralytics/yolo/v8/pose/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/pose/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/pose/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/pose/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.110600 ultralytics-8.0.93/ultralytics/yolo/v8/segment/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/segment/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.090600 ultralytics-8.0.93/ultralytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-05-05 23:14:31.000000 ultralytics-8.0.93/ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-05 23:14:31.000000 ultralytics-8.0.93/ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 23:14:31.000000 ultralytics-8.0.93/ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 23:14:31.000000 ultralytics-8.0.93/ultralytics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-05 23:14:31.000000 ultralytics-8.0.93/ultralytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 23:14:31.000000 ultralytics-8.0.93/ultralytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:02.003672 ultralytics-8.0.94/
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-07 23:59:29.000000 ultralytics-8.0.94/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-07 23:59:29.000000 ultralytics-8.0.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-07 23:59:29.000000 ultralytics-8.0.94/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-05-08 00:01:02.007673 ultralytics-8.0.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-05-07 23:59:29.000000 ultralytics-8.0.94/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23225 2023-05-07 23:59:29.000000 ultralytics-8.0.94/README.zh-CN.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-07 23:59:29.000000 ultralytics-8.0.94/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-08 00:01:02.007673 ultralytics-8.0.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-07 23:59:29.000000 ultralytics-8.0.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.983672 ultralytics-8.0.94/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-07 23:59:29.000000 ultralytics-8.0.94/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-07 23:59:29.000000 ultralytics-8.0.94/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-07 23:59:29.000000 ultralytics-8.0.94/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.983672 ultralytics-8.0.94/ultralytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.987672 ultralytics-8.0.94/ultralytics/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/assets/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    50427 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.987672 ultralytics-8.0.94/ultralytics/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/datasets/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    42439 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/datasets/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/datasets/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/datasets/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/datasets/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/datasets/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/datasets/coco-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/datasets/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/datasets/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/datasets/coco128.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/datasets/coco8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/datasets/coco8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/datasets/coco8.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/datasets/xView.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.987672 ultralytics-8.0.94/ultralytics/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/hub/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.983672 ultralytics-8.0.94/ultralytics/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.991672 ultralytics-8.0.94/ultralytics/models/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/models/v3/yolov3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.991672 ultralytics-8.0.94/ultralytics/models/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/models/v5/yolov5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.991672 ultralytics-8.0.94/ultralytics/models/v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/models/v8/yolov8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.991672 ultralytics-8.0.94/ultralytics/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24243 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/nn/autobackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/nn/autoshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25079 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/nn/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27170 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/nn/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.991672 ultralytics-8.0.94/ultralytics/tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/tracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.991672 ultralytics-8.0.94/ultralytics/tracker/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/tracker/cfg/botsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/tracker/cfg/bytetrack.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/tracker/track.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.991672 ultralytics-8.0.94/ultralytics/tracker/trackers/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/tracker/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/tracker/trackers/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/tracker/trackers/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/tracker/trackers/byte_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.995672 ultralytics-8.0.94/ultralytics/tracker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/tracker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/tracker/utils/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/tracker/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/tracker/utils/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.995672 ultralytics-8.0.94/ultralytics/vit/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/vit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.995672 ultralytics-8.0.94/ultralytics/vit/sam/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/vit/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/vit/sam/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/vit/sam/autosize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/vit/sam/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/vit/sam/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.995672 ultralytics-8.0.94/ultralytics/vit/sam/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/vit/sam/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/vit/sam/modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22502 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/vit/sam/modules/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/vit/sam/modules/mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/vit/sam/modules/prompt_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/vit/sam/modules/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/vit/sam/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/vit/sam/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.995672 ultralytics-8.0.94/ultralytics/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.995672 ultralytics-8.0.94/ultralytics/yolo/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)    17817 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/cfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/cfg/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.995672 ultralytics-8.0.94/ultralytics/yolo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/data/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33512 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/data/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.999673 ultralytics-8.0.94/ultralytics/yolo/data/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/data/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/data/dataloaders/stream_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/data/dataloaders/v5augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51260 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/data/dataloaders/v5loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/data/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23582 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.999673 ultralytics-8.0.94/ultralytics/yolo/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40265 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/engine/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/engine/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15927 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/engine/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20634 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/engine/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31310 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/engine/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/engine/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:02.003672 ultralytics-8.0.94/ultralytics/yolo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:02.003672 ultralytics-8.0.94/ultralytics/yolo/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/callbacks/clearml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/callbacks/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/callbacks/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/callbacks/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/callbacks/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/callbacks/raytune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/callbacks/wb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41903 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28191 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24037 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/tal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20019 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/utils/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:02.003672 ultralytics-8.0.94/ultralytics/yolo/v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/v8/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:02.003672 ultralytics-8.0.94/ultralytics/yolo/v8/classify/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/v8/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/v8/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/v8/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/v8/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:02.003672 ultralytics-8.0.94/ultralytics/yolo/v8/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/v8/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/v8/detect/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/v8/detect/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/v8/detect/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:02.003672 ultralytics-8.0.94/ultralytics/yolo/v8/pose/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/v8/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/v8/pose/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/v8/pose/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/v8/pose/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:02.003672 ultralytics-8.0.94/ultralytics/yolo/v8/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/v8/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/v8/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/v8/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-05-07 23:59:29.000000 ultralytics-8.0.94/ultralytics/yolo/v8/segment/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:01:01.987672 ultralytics-8.0.94/ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-05-08 00:01:01.000000 ultralytics-8.0.94/ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-08 00:01:01.000000 ultralytics-8.0.94/ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 00:01:01.000000 ultralytics-8.0.94/ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-08 00:01:01.000000 ultralytics-8.0.94/ultralytics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-08 00:01:01.000000 ultralytics-8.0.94/ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 00:01:01.000000 ultralytics-8.0.94/ultralytics.egg-info/top_level.txt
```

### Comparing `ultralytics-8.0.93/CONTRIBUTING.md` & `ultralytics-8.0.94/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/LICENSE` & `ultralytics-8.0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/PKG-INFO` & `ultralytics-8.0.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.0.93
+Version: 8.0.94
 Summary: Ultralytics YOLOv8
 Home-page: https://github.com/ultralytics/ultralytics
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.0.93 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.0.94 Summary: Ultralytics
 YOLOv8 Home-page: https://github.com/ultralytics/ultralytics Author:
 Ultralytics Author-email: hello@ultralytics.com License: AGPL-3.0 Project-URL:
 Bug Reports, https://github.com/ultralytics/ultralytics/issues Project-URL:
 Funding, https://ultralytics.com Project-URL: Source, https://github.com/
 ultralytics/ultralytics Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
```

### Comparing `ultralytics-8.0.93/README.md` & `ultralytics-8.0.94/README.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/README.zh-CN.md` & `ultralytics-8.0.94/README.zh-CN.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/requirements.txt` & `ultralytics-8.0.94/requirements.txt`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/setup.cfg` & `ultralytics-8.0.94/setup.cfg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/setup.py` & `ultralytics-8.0.94/setup.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/tests/test_cli.py` & `ultralytics-8.0.94/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/tests/test_engine.py` & `ultralytics-8.0.94/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/tests/test_python.py` & `ultralytics-8.0.94/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/assets/bus.jpg` & `ultralytics-8.0.94/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/assets/zidane.jpg` & `ultralytics-8.0.94/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/datasets/Argoverse.yaml` & `ultralytics-8.0.94/ultralytics/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/datasets/GlobalWheat2020.yaml` & `ultralytics-8.0.94/ultralytics/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/datasets/ImageNet.yaml` & `ultralytics-8.0.94/ultralytics/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/datasets/Objects365.yaml` & `ultralytics-8.0.94/ultralytics/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/datasets/SKU-110K.yaml` & `ultralytics-8.0.94/ultralytics/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/datasets/VOC.yaml` & `ultralytics-8.0.94/ultralytics/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/datasets/VisDrone.yaml` & `ultralytics-8.0.94/ultralytics/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/datasets/coco-pose.yaml` & `ultralytics-8.0.94/ultralytics/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/datasets/coco.yaml` & `ultralytics-8.0.94/ultralytics/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/datasets/coco128-seg.yaml` & `ultralytics-8.0.94/ultralytics/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/datasets/coco128.yaml` & `ultralytics-8.0.94/ultralytics/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/datasets/coco8-pose.yaml` & `ultralytics-8.0.94/ultralytics/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/datasets/coco8-seg.yaml` & `ultralytics-8.0.94/ultralytics/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/datasets/coco8.yaml` & `ultralytics-8.0.94/ultralytics/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/datasets/xView.yaml` & `ultralytics-8.0.94/ultralytics/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/hub/__init__.py` & `ultralytics-8.0.94/ultralytics/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/hub/auth.py` & `ultralytics-8.0.94/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/hub/session.py` & `ultralytics-8.0.94/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/hub/utils.py` & `ultralytics-8.0.94/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/models/v3/yolov3-spp.yaml` & `ultralytics-8.0.94/ultralytics/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/models/v3/yolov3-tiny.yaml` & `ultralytics-8.0.94/ultralytics/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/models/v3/yolov3.yaml` & `ultralytics-8.0.94/ultralytics/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/models/v5/yolov5-p6.yaml` & `ultralytics-8.0.94/ultralytics/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/models/v5/yolov5.yaml` & `ultralytics-8.0.94/ultralytics/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/models/v8/yolov8-cls.yaml` & `ultralytics-8.0.94/ultralytics/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/models/v8/yolov8-p2.yaml` & `ultralytics-8.0.94/ultralytics/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/models/v8/yolov8-p6.yaml` & `ultralytics-8.0.94/ultralytics/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/models/v8/yolov8-pose-p6.yaml` & `ultralytics-8.0.94/ultralytics/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/models/v8/yolov8-pose.yaml` & `ultralytics-8.0.94/ultralytics/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/models/v8/yolov8-seg.yaml` & `ultralytics-8.0.94/ultralytics/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/models/v8/yolov8.yaml` & `ultralytics-8.0.94/ultralytics/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/nn/autobackend.py` & `ultralytics-8.0.94/ultralytics/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/nn/autoshape.py` & `ultralytics-8.0.94/ultralytics/nn/autoshape.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/nn/modules.py` & `ultralytics-8.0.94/ultralytics/nn/modules.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/nn/tasks.py` & `ultralytics-8.0.94/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/tracker/cfg/botsort.yaml` & `ultralytics-8.0.94/ultralytics/tracker/cfg/botsort.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/tracker/cfg/bytetrack.yaml` & `ultralytics-8.0.94/ultralytics/tracker/cfg/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/tracker/track.py` & `ultralytics-8.0.94/ultralytics/tracker/track.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/tracker/trackers/basetrack.py` & `ultralytics-8.0.94/ultralytics/tracker/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/tracker/trackers/bot_sort.py` & `ultralytics-8.0.94/ultralytics/tracker/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/tracker/trackers/byte_tracker.py` & `ultralytics-8.0.94/ultralytics/tracker/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/tracker/utils/gmc.py` & `ultralytics-8.0.94/ultralytics/tracker/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/tracker/utils/kalman_filter.py` & `ultralytics-8.0.94/ultralytics/tracker/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/tracker/utils/matching.py` & `ultralytics-8.0.94/ultralytics/tracker/utils/matching.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/vit/sam/amg.py` & `ultralytics-8.0.94/ultralytics/vit/sam/amg.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/vit/sam/autosize.py` & `ultralytics-8.0.94/ultralytics/vit/sam/autosize.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/vit/sam/build.py` & `ultralytics-8.0.94/ultralytics/vit/sam/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/vit/sam/model.py` & `ultralytics-8.0.94/ultralytics/vit/sam/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/vit/sam/modules/decoders.py` & `ultralytics-8.0.94/ultralytics/vit/sam/modules/decoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/vit/sam/modules/encoders.py` & `ultralytics-8.0.94/ultralytics/vit/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/vit/sam/modules/mask_generator.py` & `ultralytics-8.0.94/ultralytics/vit/sam/modules/mask_generator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/vit/sam/modules/prompt_predictor.py` & `ultralytics-8.0.94/ultralytics/vit/sam/modules/prompt_predictor.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/vit/sam/modules/sam.py` & `ultralytics-8.0.94/ultralytics/vit/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/vit/sam/modules/transformer.py` & `ultralytics-8.0.94/ultralytics/vit/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/vit/sam/predict.py` & `ultralytics-8.0.94/ultralytics/vit/sam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/cfg/__init__.py` & `ultralytics-8.0.94/ultralytics/yolo/cfg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'segment': 'coco128-seg.yaml',
     'classify': 'imagenet100',
     'pose': 'coco8-pose.yaml'}
 TASK2MODEL = {
     'detect': 'yolov8n.pt',
     'segment': 'yolov8n-seg.pt',
     'classify': 'yolov8n-cls.pt',
-    'pose': 'yolov8n-pose.yaml'}
+    'pose': 'yolov8n-pose.pt'}
 
 CLI_HELP_MSG = \
     f"""
     Arguments received: {str(['yolo'] + sys.argv[1:])}. Ultralytics 'yolo' commands use the following syntax:
 
         yolo TASK MODE ARGS
```

### Comparing `ultralytics-8.0.93/ultralytics/yolo/cfg/default.yaml` & `ultralytics-8.0.94/ultralytics/yolo/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/data/annotator.py` & `ultralytics-8.0.94/ultralytics/yolo/data/annotator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/data/augment.py` & `ultralytics-8.0.94/ultralytics/yolo/data/augment.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/data/base.py` & `ultralytics-8.0.94/ultralytics/yolo/data/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import cv2
 import numpy as np
 import psutil
 from torch.utils.data import Dataset
 from tqdm import tqdm
 
-from ..utils import LOCAL_RANK, LOGGER, NUM_THREADS, TQDM_BAR_FORMAT
+from ..utils import DEFAULT_CFG, LOCAL_RANK, LOGGER, NUM_THREADS, TQDM_BAR_FORMAT
 from .utils import HELP_URL, IMG_FORMATS
 
 
 class BaseDataset(Dataset):
     """
     Base dataset class for loading and processing image data.
 
@@ -47,15 +47,15 @@
     """
 
     def __init__(self,
                  img_path,
                  imgsz=640,
                  cache=False,
                  augment=True,
-                 hyp=None,
+                 hyp=DEFAULT_CFG,
                  prefix='',
                  rect=False,
                  batch_size=None,
                  stride=32,
                  pad=0.5,
                  single_cls=False,
                  classes=None):
```

### Comparing `ultralytics-8.0.93/ultralytics/yolo/data/build.py` & `ultralytics-8.0.94/ultralytics/yolo/data/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     worker_seed = torch.initial_seed() % 2 ** 32
     np.random.seed(worker_seed)
     random.seed(worker_seed)
 
 
 def build_yolo_dataset(cfg, img_path, batch, data_info, mode='train', rect=False, stride=32):
     """Build YOLO Dataset"""
-    dataset = YOLODataset(
+    return YOLODataset(
         img_path=img_path,
         imgsz=cfg.imgsz,
         batch_size=batch,
         augment=mode == 'train',  # augmentation
         hyp=cfg,  # TODO: probably add a get_hyps_from_cfg function
         rect=cfg.rect or rect,  # rectangular batches
         cache=cfg.cache or None,
@@ -83,15 +83,14 @@
         stride=int(stride),
         pad=0.0 if mode == 'train' else 0.5,
         prefix=colorstr(f'{mode}: '),
         use_segments=cfg.task == 'segment',
         use_keypoints=cfg.task == 'pose',
         classes=cfg.classes,
         data=data_info)
-    return dataset
 
 
 def build_dataloader(dataset, batch, workers, shuffle=True, rank=-1):
     """Return an InfiniteDataLoader or DataLoader for training or validation set."""
     batch = min(batch, len(dataset))
     nd = torch.cuda.device_count()  # number of CUDA devices
     nw = min([os.cpu_count() // max(nd, 1), batch if batch > 1 else 0, workers])  # number of workers
```

### Comparing `ultralytics-8.0.93/ultralytics/yolo/data/converter.py` & `ultralytics-8.0.94/ultralytics/yolo/data/converter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/data/dataloaders/stream_loaders.py` & `ultralytics-8.0.94/ultralytics/yolo/data/dataloaders/stream_loaders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/data/dataloaders/v5augmentations.py` & `ultralytics-8.0.94/ultralytics/yolo/data/dataloaders/v5augmentations.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/data/dataloaders/v5loader.py` & `ultralytics-8.0.94/ultralytics/yolo/data/dataloaders/v5loader.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/data/dataset.py` & `ultralytics-8.0.94/ultralytics/yolo/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
     YOLOv5 Classification Dataset.
     Arguments
         root:  Dataset path
         transform:  torchvision transforms, used by default
         album_transform: Albumentations transforms, used if installed
     """
 
-    def __init__(self, root, augment, imgsz, cache=False):
+    def __init__(self, root, augment=False, imgsz=224, cache=False):
         """Initialize YOLO object with root, image size, augmentations, and cache settings"""
         super().__init__(root=root)
         self.torch_transforms = classify_transforms(imgsz)
         self.album_transforms = classify_albumentations(augment, imgsz) if augment else None
         self.cache_ram = cache is True or cache == 'ram'
         self.cache_disk = cache == 'disk'
         self.samples = [list(x) + [Path(x[0]).with_suffix('.npy'), None] for x in self.samples]  # file, index, npy, im
```

### Comparing `ultralytics-8.0.93/ultralytics/yolo/data/dataset_wrappers.py` & `ultralytics-8.0.94/ultralytics/yolo/data/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/data/utils.py` & `ultralytics-8.0.94/ultralytics/yolo/data/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -306,25 +306,27 @@
 
 class HUBDatasetStats():
     """
     Class for generating HUB dataset JSON and `-hub` dataset directory
 
     Arguments
         path:           Path to data.yaml or data.zip (with data.yaml inside data.zip)
+        task:           Dataset task. Options are 'detect', 'segment', 'pose', 'classify'.
         autodownload:   Attempt to download dataset if not found locally
 
     Usage
         from ultralytics.yolo.data.utils import HUBDatasetStats
-        stats = HUBDatasetStats('coco128.yaml', autodownload=True)  # usage 1
-        stats = HUBDatasetStats('/Users/glennjocher/Downloads/coco6.zip')  # usage 2
+        stats = HUBDatasetStats('/Users/glennjocher/Downloads/coco8.zip', task='detect')  # detect dataset
+        stats = HUBDatasetStats('/Users/glennjocher/Downloads/coco8-seg.zip', task='segment')  # segment dataset
+        stats = HUBDatasetStats('/Users/glennjocher/Downloads/coco8-pose.zip', task='pose')  # pose dataset
         stats.get_json(save=False)
         stats.process_images()
     """
 
-    def __init__(self, path='coco128.yaml', autodownload=False):
+    def __init__(self, path='coco128.yaml', task='detect', autodownload=False):
         """Initialize class."""
         zipped, data_dir, yaml_path = self._unzip(Path(path))
         try:
             # data = yaml_load(check_yaml(yaml_path))  # data dict
             data = check_det_dataset(yaml_path, autodownload)  # data dict
             if zipped:
                 data['path'] = data_dir
@@ -332,14 +334,15 @@
             raise Exception('error/HUB/dataset_stats/yaml_load') from e
 
         self.hub_dir = Path(str(data['path']) + '-hub')
         self.im_dir = self.hub_dir / 'images'
         self.im_dir.mkdir(parents=True, exist_ok=True)  # makes /images
         self.stats = {'nc': len(data['names']), 'names': list(data['names'].values())}  # statistics dictionary
         self.data = data
+        self.task = task  # detect, segment, pose, classify
 
     @staticmethod
     def _find_yaml(dir):
         """Return data.yaml file."""
         files = list(dir.glob('*.yaml')) or list(dir.rglob('*.yaml'))  # try root level first and then recursive
         assert files, f'No *.yaml file found in {dir}'
         if len(files) > 1:
@@ -348,71 +351,82 @@
         assert len(files) == 1, f'Multiple *.yaml files found: {files}, only 1 *.yaml file allowed in {dir}'
         return files[0]
 
     def _unzip(self, path):
         """Unzip data.zip."""
         if not str(path).endswith('.zip'):  # path is data.yaml
             return False, None, path
-        assert Path(path).is_file(), f'Error unzipping {path}, file not found'
-        unzip_file(path, path=path.parent)
-        dir = path.with_suffix('')  # dataset directory == zip name
-        assert dir.is_dir(), f'Error unzipping {path}, {dir} not found. path/to/abc.zip MUST unzip to path/to/abc/'
-        return True, str(dir), self._find_yaml(dir)  # zipped, data_dir, yaml_path
+        unzip_dir = unzip_file(path, path=path.parent)
+        assert unzip_dir.is_dir(), f'Error unzipping {path}, {unzip_dir} not found. ' \
+                                   f'path/to/abc.zip MUST unzip to path/to/abc/'
+        return True, str(unzip_dir), self._find_yaml(unzip_dir)  # zipped, data_dir, yaml_path
 
     def _hub_ops(self, f):
         """Saves a compressed image for HUB previews."""
         compress_one_image(f, self.im_dir / Path(f).name)  # save to dataset-hub
 
     def get_json(self, save=False, verbose=False):
         """Return dataset JSON for Ultralytics HUB."""
-        # from ultralytics.yolo.data import YOLODataset
-        from ultralytics.yolo.data.dataloaders.v5loader import LoadImagesAndLabels
+        from ultralytics.yolo.data import YOLODataset  # ClassificationDataset
 
         def _round(labels):
-            """Update labels to integer class and 6 decimal place floats."""
-            return [[int(c), *(round(x, 4) for x in points)] for c, *points in labels]
+            """Update labels to integer class and 4 decimal place floats."""
+            if self.task == 'detect':
+                coordinates = labels['bboxes']
+            elif self.task == 'segment':
+                coordinates = [x.flatten() for x in labels['segments']]
+            elif self.task == 'pose':
+                n = labels['keypoints'].shape[0]
+                coordinates = np.concatenate((labels['bboxes'], labels['keypoints'].reshape(n, -1)), 1)
+            else:
+                raise ValueError('Undefined dataset task.')
+            zipped = zip(labels['cls'], coordinates)
+            return [[int(c), *(round(float(x), 4) for x in points)] for c, points in zipped]
 
         for split in 'train', 'val', 'test':
             if self.data.get(split) is None:
                 self.stats[split] = None  # i.e. no test set
                 continue
-            dataset = LoadImagesAndLabels(self.data[split])  # load dataset
+
+            dataset = YOLODataset(img_path=self.data[split],
+                                  data=self.data,
+                                  use_segments=self.task == 'segment',
+                                  use_keypoints=self.task == 'pose')
             x = np.array([
-                np.bincount(label[:, 0].astype(int), minlength=self.data['nc'])
+                np.bincount(label['cls'].astype(int).flatten(), minlength=self.data['nc'])
                 for label in tqdm(dataset.labels, total=len(dataset), desc='Statistics')])  # shape(128x80)
             self.stats[split] = {
                 'instance_stats': {
                     'total': int(x.sum()),
                     'per_class': x.sum(0).tolist()},
                 'image_stats': {
                     'total': len(dataset),
                     'unlabelled': int(np.all(x == 0, 1).sum()),
                     'per_class': (x > 0).sum(0).tolist()},
                 'labels': [{
-                    str(Path(k).name): _round(v.tolist())} for k, v in zip(dataset.im_files, dataset.labels)]}
+                    Path(k).name: _round(v)} for k, v in zip(dataset.im_files, dataset.labels)]}
 
         # Save, print and return
         if save:
             stats_path = self.hub_dir / 'stats.json'
             LOGGER.info(f'Saving {stats_path.resolve()}...')
             with open(stats_path, 'w') as f:
                 json.dump(self.stats, f)  # save stats.json
         if verbose:
             LOGGER.info(json.dumps(self.stats, indent=2, sort_keys=False))
         return self.stats
 
     def process_images(self):
         """Compress images for Ultralytics HUB."""
-        # from ultralytics.yolo.data import YOLODataset
-        from ultralytics.yolo.data.dataloaders.v5loader import LoadImagesAndLabels
+        from ultralytics.yolo.data import YOLODataset  # ClassificationDataset
 
         for split in 'train', 'val', 'test':
             if self.data.get(split) is None:
                 continue
-            dataset = LoadImagesAndLabels(self.data[split])  # load dataset
+            dataset = YOLODataset(img_path=self.data[split], data=self.data)
             with ThreadPool(NUM_THREADS) as pool:
                 for _ in tqdm(pool.imap(self._hub_ops, dataset.im_files), total=len(dataset), desc=f'{split} images'):
                     pass
         LOGGER.info(f'Done. All images saved to {self.im_dir}')
         return self.im_dir
```

### Comparing `ultralytics-8.0.93/ultralytics/yolo/engine/exporter.py` & `ultralytics-8.0.94/ultralytics/yolo/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/engine/model.py` & `ultralytics-8.0.94/ultralytics/yolo/engine/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/engine/predictor.py` & `ultralytics-8.0.94/ultralytics/yolo/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/engine/results.py` & `ultralytics-8.0.94/ultralytics/yolo/engine/results.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/engine/trainer.py` & `ultralytics-8.0.94/ultralytics/yolo/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/engine/validator.py` & `ultralytics-8.0.94/ultralytics/yolo/engine/validator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/__init__.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/autobatch.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/benchmarks.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/base.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/clearml.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/comet.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/hub.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/mlflow.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/neptune.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/tensorboard.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/wb.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/checks.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/checks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/dist.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/dist.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/downloads.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/downloads.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,34 +33,47 @@
                 return response.getcode() == 200  # check if exists online
         return True
     return False
 
 
 def unzip_file(file, path=None, exclude=('.DS_Store', '__MACOSX')):
     """
-    Unzip a *.zip file to path/, excluding files containing strings in exclude list
-    Replaces: ZipFile(file).extractall(path=path)
+    Unzips a *.zip file to the specified path, excluding files containing strings in the exclude list.
+
+    If the zipfile does not contain a single top-level directory, the function will create a new
+    directory with the same name as the zipfile (without the extension) to extract its contents.
+    If a path is not provided, the function will use the parent directory of the zipfile as the default path.
+
+    Args:
+        file (str): The path to the zipfile to be extracted.
+        path (str, optional): The path to extract the zipfile to. Defaults to None.
+        exclude (tuple, optional): A tuple of filename strings to be excluded. Defaults to ('.DS_Store', '__MACOSX').
+
+    Raises:
+        BadZipFile: If the provided file does not exist or is not a valid zipfile.
+
+    Returns:
+        (Path): The path to the directory where the zipfile was extracted.
     """
     if not (Path(file).exists() and is_zipfile(file)):
         raise BadZipFile(f"File '{file}' does not exist or is a bad zip file.")
     if path is None:
         path = Path(file).parent  # default path
+
     with ZipFile(file) as zipObj:
-        for i, f in enumerate(zipObj.namelist()):  # list all archived filenames in the zip
-            # If zip does not expand into a directory create a new directory to expand into
-            if i == 0:
-                info = zipObj.getinfo(f)
-                if info.file_size > 0 or not info.filename.endswith('/'):  # element is a file and not a directory
-                    path = Path(path) / Path(file).stem  # define new unzip directory
-                    unzip_dir = path
-                else:
-                    unzip_dir = f
-            if all(x not in f for x in exclude):
-                zipObj.extract(f, path=path)
-        return unzip_dir  # return unzip dir
+        file_list = [f for f in zipObj.namelist() if all(x not in f for x in exclude)]
+        top_level_dirs = {Path(f).parts[0] for f in file_list}
+
+        if len(top_level_dirs) > 1 or not file_list[0].endswith('/'):
+            path = Path(path) / Path(file).stem  # define new unzip directory
+
+        for f in file_list:
+            zipObj.extract(f, path=path)
+
+    return path  # return unzip dir
 
 
 def check_disk_space(url='https://ultralytics.com/assets/coco128.zip', sf=1.5, hard=True):
     """
     Check if there is sufficient disk space to download and store a file.
 
     Args:
```

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/files.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/files.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/instance.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/instance.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/loss.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/loss.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/metrics.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,32 +314,33 @@
         array = self.matrix / ((self.matrix.sum(0).reshape(1, -1) + 1E-9) if normalize else 1)  # normalize columns
         array[array < 0.005] = np.nan  # don't annotate (would appear as 0.00)
 
         fig, ax = plt.subplots(1, 1, figsize=(12, 9), tight_layout=True)
         nc, nn = self.nc, len(names)  # number of classes, names
         sn.set(font_scale=1.0 if nc < 50 else 0.8)  # for label size
         labels = (0 < nn < 99) and (nn == nc)  # apply names to ticklabels
-        ticklabels = (names + ['background']) if labels else 'auto'
+        ticklabels = (list(names) + ['background']) if labels else 'auto'
         with warnings.catch_warnings():
             warnings.simplefilter('ignore')  # suppress empty matrix RuntimeWarning: All-NaN slice encountered
             sn.heatmap(array,
                        ax=ax,
                        annot=nc < 30,
                        annot_kws={
                            'size': 8},
                        cmap='Blues',
                        fmt='.2f',
                        square=True,
                        vmin=0.0,
                        xticklabels=ticklabels,
                        yticklabels=ticklabels).set_facecolor((1, 1, 1))
+        title = 'Confusion Matrix' + ' Normalized' * normalize
         ax.set_xlabel('True')
         ax.set_ylabel('Predicted')
-        ax.set_title('Confusion Matrix')
-        fig.savefig(Path(save_dir) / 'confusion_matrix.png', dpi=250)
+        ax.set_title(title)
+        fig.savefig(Path(save_dir) / f'{title.lower().replace(" ", "_")}.png', dpi=250)
         plt.close(fig)
 
     def print(self):
         """
         Print the confusion matrix to the console.
         """
         for i in range(self.nc + 1):
```

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/ops.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/ops.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/plotting.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/tal.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/tal.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/torch_utils.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/utils/tuner.py` & `ultralytics-8.0.94/ultralytics/yolo/utils/tuner.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,9 +34,9 @@
     'mosaic': tune.uniform(0.0, 1.0),  # image mixup (probability)
     'mixup': tune.uniform(0.0, 1.0),  # image mixup (probability)
     'copy_paste': tune.uniform(0.0, 1.0)}  # segment copy-paste (probability)
 
 task_metric_map = {
     'detect': 'metrics/mAP50-95(B)',
     'segment': 'metrics/mAP50-95(M)',
-    'classify': 'top1_acc',
-    'pose': None}
+    'classify': 'metrics/accuracy_top1',
+    'pose': 'metrics/mAP50-95(P)'}
```

### Comparing `ultralytics-8.0.93/ultralytics/yolo/v8/classify/predict.py` & `ultralytics-8.0.94/ultralytics/yolo/v8/classify/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/v8/classify/train.py` & `ultralytics-8.0.94/ultralytics/yolo/v8/classify/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,17 +68,16 @@
             self.model = torchvision.models.__dict__[model](weights='IMAGENET1K_V1' if pretrained else None)
         else:
             FileNotFoundError(f'ERROR: model={model} not found locally or online. Please check model name.')
         ClassificationModel.reshape_outputs(self.model, self.data['nc'])
 
         return  # dont return ckpt. Classification doesn't support resume
 
-    def build_dataset(self, img_path, mode='train'):
-        dataset = ClassificationDataset(root=img_path, imgsz=self.args.imgsz, augment=mode == 'train')
-        return dataset
+    def build_dataset(self, img_path, mode='train', batch=None):
+        return ClassificationDataset(root=img_path, imgsz=self.args.imgsz, augment=mode == 'train')
 
     def get_dataloader(self, dataset_path, batch_size=16, rank=0, mode='train'):
         """Returns PyTorch DataLoader with transforms to preprocess images for inference."""
         with torch_distributed_zero_first(rank):  # init dataset *.cache only once if DDP
             dataset = self.build_dataset(dataset_path, mode)
 
         loader = build_dataloader(dataset, batch_size, self.args.workers, rank=rank)
```

### Comparing `ultralytics-8.0.93/ultralytics/yolo/v8/classify/val.py` & `ultralytics-8.0.94/ultralytics/yolo/v8/classify/val.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,16 @@
         self.pred.append(preds.argsort(1, descending=True)[:, :n5])
         self.targets.append(batch['cls'])
 
     def finalize_metrics(self, *args, **kwargs):
         """Finalizes metrics of the model such as confusion_matrix and speed."""
         self.confusion_matrix.process_cls_preds(self.pred, self.targets)
         if self.args.plots:
-            self.confusion_matrix.plot(save_dir=self.save_dir, names=list(self.names.values()))
+            for normalize in True, False:
+                self.confusion_matrix.plot(save_dir=self.save_dir, names=self.names.values(), normalize=normalize)
         self.metrics.speed = self.speed
         self.metrics.confusion_matrix = self.confusion_matrix
 
     def get_stats(self):
         """Returns a dictionary of metrics obtained by processing targets and predictions."""
         self.metrics.process(self.targets, self.pred)
         return self.metrics.results_dict
```

### Comparing `ultralytics-8.0.93/ultralytics/yolo/v8/detect/predict.py` & `ultralytics-8.0.94/ultralytics/yolo/v8/detect/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/v8/detect/train.py` & `ultralytics-8.0.94/ultralytics/yolo/v8/detect/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             img_path (str): Path to the folder containing images.
             mode (str): `train` mode or `val` mode, users are able to customize different augmentations for each mode.
             batch (int, optional): Size of batches, this is for `rect`. Defaults to None.
         """
         gs = max(int(de_parallel(self.model).stride.max() if self.model else 0), 32)
         return build_yolo_dataset(self.args, img_path, batch, self.data, mode=mode, rect=mode == 'val', stride=gs)
 
-    def get_dataloader(self, dataset_path, batch_size, rank=0, mode='train'):
+    def get_dataloader(self, dataset_path, batch_size=16, rank=0, mode='train'):
         """TODO: manage splits differently."""
         # Calculate stride - check if model is initialized
         if self.args.v5loader:
             LOGGER.warning("WARNING ⚠️ 'v5loader' feature is deprecated and will be removed soon. You can train using "
                            'the default YOLOv8 dataloader instead, no argument is needed.')
             gs = max(int(de_parallel(self.model).stride.max() if self.model else 0), 32)
             return create_dataloader(path=dataset_path,
@@ -58,16 +58,15 @@
         with torch_distributed_zero_first(rank):  # init dataset *.cache only once if DDP
             dataset = self.build_dataset(dataset_path, mode, batch_size)
         shuffle = mode == 'train'
         if getattr(dataset, 'rect', False) and shuffle:
             LOGGER.warning("WARNING ⚠️ 'rect=True' is incompatible with DataLoader shuffle, setting shuffle=False")
             shuffle = False
         workers = self.args.workers if mode == 'train' else self.args.workers * 2
-        dataloader = build_dataloader(dataset, batch_size, workers, shuffle, rank)
-        return dataloader
+        return build_dataloader(dataset, batch_size, workers, shuffle, rank)  # return dataloader
 
     def preprocess_batch(self, batch):
         """Preprocesses a batch of images by scaling and converting to float."""
         batch['img'] = batch['img'].to(self.device, non_blocking=True).float() / 255
         return batch
 
     def set_model_attributes(self):
```

### Comparing `ultralytics-8.0.93/ultralytics/yolo/v8/detect/val.py` & `ultralytics-8.0.94/ultralytics/yolo/v8/detect/val.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,16 @@
 
         # Print results per class
         if self.args.verbose and not self.training and self.nc > 1 and len(self.stats):
             for i, c in enumerate(self.metrics.ap_class_index):
                 LOGGER.info(pf % (self.names[c], self.seen, self.nt_per_class[c], *self.metrics.class_result(i)))
 
         if self.args.plots:
-            self.confusion_matrix.plot(save_dir=self.save_dir, names=list(self.names.values()))
+            for normalize in True, False:
+                self.confusion_matrix.plot(save_dir=self.save_dir, names=self.names.values(), normalize=normalize)
 
     def _process_batch(self, detections, labels):
         """
         Return correct prediction matrix
         Arguments:
             detections (array[N, 6]), x1, y1, x2, y2, conf, class
             labels (array[M, 5]), class, x1, y1, x2, y2
```

### Comparing `ultralytics-8.0.93/ultralytics/yolo/v8/pose/predict.py` & `ultralytics-8.0.94/ultralytics/yolo/v8/pose/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/v8/pose/train.py` & `ultralytics-8.0.94/ultralytics/yolo/v8/pose/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/v8/pose/val.py` & `ultralytics-8.0.94/ultralytics/yolo/v8/pose/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/v8/segment/predict.py` & `ultralytics-8.0.94/ultralytics/yolo/v8/segment/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/v8/segment/train.py` & `ultralytics-8.0.94/ultralytics/yolo/v8/segment/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics/yolo/v8/segment/val.py` & `ultralytics-8.0.94/ultralytics/yolo/v8/segment/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.93/ultralytics.egg-info/PKG-INFO` & `ultralytics-8.0.94/ultralytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.0.93
+Version: 8.0.94
 Summary: Ultralytics YOLOv8
 Home-page: https://github.com/ultralytics/ultralytics
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.0.93 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.0.94 Summary: Ultralytics
 YOLOv8 Home-page: https://github.com/ultralytics/ultralytics Author:
 Ultralytics Author-email: hello@ultralytics.com License: AGPL-3.0 Project-URL:
 Bug Reports, https://github.com/ultralytics/ultralytics/issues Project-URL:
 Funding, https://ultralytics.com Project-URL: Source, https://github.com/
 ultralytics/ultralytics Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
```

### Comparing `ultralytics-8.0.93/ultralytics.egg-info/SOURCES.txt` & `ultralytics-8.0.94/ultralytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

