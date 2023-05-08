# Comparing `tmp/onvif-gui-1.0.6.tar.gz` & `tmp/onvif-gui-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-gui-1.0.6.tar", last modified: Thu May  4 00:05:39 2023, max compression
+gzip compressed data, was "onvif-gui-1.0.7.tar", last modified: Mon May  8 16:45:39 2023, max compression
```

## Comparing `onvif-gui-1.0.6.tar` & `onvif-gui-1.0.7.tar`

### file list

```diff
@@ -1,276 +1,280 @@
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.936091 onvif-gui-1.0.6/
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11357 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/LICENSE
--rw-r--r--   0 stephen   (1000) stephen   (1000)       59 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/MANIFEST.in
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-04 00:05:39.936091 onvif-gui-1.0.6/PKG-INFO
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8170 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/README.md
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.900091 onvif-gui-1.0.6/detectron2/
--rw-r--r--   0 stephen   (1000) stephen   (1000)       67 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.900091 onvif-gui-1.0.6/detectron2/checkpoint/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      347 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/checkpoint/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    17770 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/checkpoint/c2_model_loading.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5685 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/checkpoint/catalog.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5258 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/checkpoint/detection_checkpoint.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.900091 onvif-gui-1.0.6/detectron2/config/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      599 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/config/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7890 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/config/compat.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9211 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/config/config.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    29512 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/config/defaults.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3015 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/config/instantiate.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15378 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/config/lazy.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.900091 onvif-gui-1.0.6/detectron2/configs/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/configs/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.900091 onvif-gui-1.0.6/detectron2/data/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      644 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7378 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/benchmark.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    21231 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7224 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/catalog.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9162 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/common.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8169 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/dataset_mapper.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.904091 onvif-gui-1.0.6/detectron2/data/datasets/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      523 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/datasets/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10174 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/datasets/builtin.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    21841 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/datasets/builtin_meta.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13167 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/datasets/cityscapes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7821 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/datasets/cityscapes_panoptic.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23465 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/datasets/coco.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8977 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/datasets/coco_panoptic.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9623 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/datasets/lvis.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)   223757 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/datasets/lvis_v0_5_categories.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)   219177 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/datasets/lvis_v1_categories.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    39414 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/datasets/lvis_v1_category_image_count.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3128 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/datasets/pascal_voc.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      169 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/datasets/register_coco.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    22841 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/detection_utils.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.904091 onvif-gui-1.0.6/detectron2/data/samplers/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      412 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/samplers/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11789 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/samplers/distributed_sampler.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1944 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/samplers/grouped_batch_sampler.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.904091 onvif-gui-1.0.6/detectron2/data/transforms/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      466 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/transforms/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14112 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/transforms/augmentation.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23069 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/transforms/augmentation_impl.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12629 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/data/transforms/transform.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.908091 onvif-gui-1.0.6/detectron2/layers/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      874 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/layers/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5764 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/layers/aspp.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12131 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/layers/batch_norm.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3024 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/layers/blocks.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    16978 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/layers/deform_conv.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4202 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/layers/losses.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10879 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/layers/mask_ops.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6490 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/layers/nms.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3098 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/layers/roi_align.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3302 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/layers/roi_align_rotated.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      652 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/layers/rotated_boxes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      537 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/layers/shape_spec.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5123 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/layers/wrappers.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.908091 onvif-gui-1.0.6/detectron2/modeling/
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1568 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15439 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/anchor_generator.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.912091 onvif-gui-1.0.6/detectron2/modeling/backbone/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      598 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/backbone/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2512 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/backbone/backbone.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1015 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/backbone/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10360 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/backbone/fpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15988 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/backbone/mvit.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    16656 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/backbone/regnet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23658 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/backbone/resnet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    25095 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/backbone/swin.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6360 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/backbone/utils.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    19338 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/backbone/vit.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15123 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/box_regression.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6264 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/matcher.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.912091 onvif-gui-1.0.6/detectron2/modeling/meta_arch/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      508 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/meta_arch/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      814 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/meta_arch/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11651 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/meta_arch/dense_detector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13213 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/meta_arch/fcos.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10407 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/meta_arch/panoptic_fpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13896 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/meta_arch/rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    18265 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/meta_arch/retinanet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9906 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/meta_arch/semantic_seg.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10832 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/mmdet_wrapper.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11316 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/poolers.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4045 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/postprocessing.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.912091 onvif-gui-1.0.6/detectron2/modeling/proposal_generator/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      231 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/proposal_generator/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      836 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/proposal_generator/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8128 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/proposal_generator/proposal_utils.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23814 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/proposal_generator/rpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8807 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/proposal_generator/rrpn.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.912091 onvif-gui-1.0.6/detectron2/modeling/roi_heads/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      768 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/roi_heads/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4077 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/roi_heads/box_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12990 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/roi_heads/cascade_rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    25390 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/roi_heads/fast_rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11156 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/roi_heads/keypoint_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12169 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/roi_heads/mask_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    37701 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/roi_heads/roi_heads.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11175 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2334 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/sampling.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12416 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/modeling/test_time_augmentation.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1780 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/predictor.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.916091 onvif-gui-1.0.6/detectron2/structures/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      645 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/structures/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14429 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/structures/boxes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5520 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/structures/image_list.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6613 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/structures/instances.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9030 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/structures/keypoints.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    19802 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/structures/masks.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    18853 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/structures/rotated_boxes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2707 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/tracker.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.920091 onvif-gui-1.0.6/detectron2/utils/
--rw-r--r--   0 stephen   (1000) stephen   (1000)       51 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/utils/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6017 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/utils/analysis.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8391 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/utils/collect_env.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4096 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/utils/colormap.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5608 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/utils/comm.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1852 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/utils/develop.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5644 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/utils/env.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    17022 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/utils/events.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1189 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/utils/file_io.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7807 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/utils/logger.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2583 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/utils/memory.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1874 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/utils/registry.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1064 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/utils/serialize.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    18113 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/utils/testing.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11319 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/utils/video_visualizer.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    51159 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/detectron2/utils/visualizer.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.920091 onvif-gui-1.0.6/gui/
--rw-r--r--   0 stephen   (1000) stephen   (1000)       28 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.920091 onvif-gui-1.0.6/gui/components/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      245 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/components/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1738 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/components/comboselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2397 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/components/directoryselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2118 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/components/fileselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5315 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/components/labelselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4077 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/components/progress.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1918 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/components/thresholdslider.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1996 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/glwidget.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14377 2023-05-04 00:03:29.000000 onvif-gui-1.0.6/gui/main.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.920091 onvif-gui-1.0.6/gui/onvif/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      191 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/onvif/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5743 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/onvif/admintab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3959 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/onvif/imagetab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2425 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/onvif/logindialog.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5247 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/onvif/networktab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5118 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/onvif/ptztab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4527 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/onvif/videotab.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.920091 onvif-gui-1.0.6/gui/panels/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      180 2023-05-03 01:49:37.000000 onvif-gui-1.0.6/gui/panels/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3624 2023-05-03 02:34:01.000000 onvif-gui-1.0.6/gui/panels/audiopanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13463 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/panels/camerapanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14483 2023-05-03 15:52:33.000000 onvif-gui-1.0.6/gui/panels/filepanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12913 2023-05-02 23:52:13.000000 onvif-gui-1.0.6/gui/panels/settingspanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3627 2023-05-03 02:39:24.000000 onvif-gui-1.0.6/gui/panels/videopanel.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.932091 onvif-gui-1.0.6/gui/resources/
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1936 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/LICENSE
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      252 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/apply.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      245 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/apply_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      244 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/apply_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      911 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/audio.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      536 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/audio_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      920 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/audio_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      203 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/branch_closed.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      219 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/branch_closed_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      211 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/branch_closed_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      199 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/branch_open.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      168 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/branch_open_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/branch_open_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      267 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/checked.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      235 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/checked_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      246 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/checked_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12716 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/darkstyle.qss
--rw-r--r--   0 stephen   (1000) stephen   (1000)      910 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/discover.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      849 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/discover_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      937 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/discover_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      425 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/fast-forward.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      253 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/fast-forward_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      433 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/fast-forward_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      641 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/mute.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      346 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/mute_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      618 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/mute_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      347 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/next.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      225 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/next_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      348 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/next_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)    46084 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/onvif-gui.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/pause.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      144 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/pause_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      149 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/pause_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      321 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/play.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      209 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/play_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      316 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/play_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      349 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/previous.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      232 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/previous_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      348 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/previous_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      324 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/radio-off.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      250 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/radio-off_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      324 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/radio-off_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      350 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/radio-on.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      263 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/radio-on_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      343 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/radio-on_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      395 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/record.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      394 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/record_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      425 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/record_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      408 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/recording.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      435 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/recording_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      532 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/recording_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      454 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/rewind.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      250 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/rewind_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      457 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/rewind_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      187 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/small_arrow_left.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      183 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/small_arrow_left_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      189 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/small_arrow_left_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      162 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/small_arrow_up.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      160 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/small_arrow_up_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      161 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/small_arrow_up_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      158 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/stop.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      140 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/stop_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      151 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/stop_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      143 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/unchecked.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      142 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/unchecked_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      143 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/gui/resources/unchecked_lo.png
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.932091 onvif-gui-1.0.6/modules/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:45:47.000000 onvif-gui-1.0.6/modules/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.932091 onvif-gui-1.0.6/modules/audio/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-05-03 02:36:19.000000 onvif-gui-1.0.6/modules/audio/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3404 2023-05-03 19:20:32.000000 onvif-gui-1.0.6/modules/audio/sample.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.932091 onvif-gui-1.0.6/modules/video/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/modules/video/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6518 2023-05-03 02:24:57.000000 onvif-gui-1.0.6/modules/video/keypoint.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4796 2023-05-03 02:51:04.000000 onvif-gui-1.0.6/modules/video/retinanet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3016 2023-05-03 02:51:12.000000 onvif-gui-1.0.6/modules/video/sample.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7106 2023-05-03 02:25:21.000000 onvif-gui-1.0.6/modules/video/segment.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11751 2023-05-03 02:51:21.000000 onvif-gui-1.0.6/modules/video/yolox.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.936091 onvif-gui-1.0.6/onvif_gui.egg-info/
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-04 00:05:39.000000 onvif-gui-1.0.6/onvif_gui.egg-info/PKG-INFO
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7636 2023-05-04 00:05:39.000000 onvif-gui-1.0.6/onvif_gui.egg-info/SOURCES.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)        1 2023-05-04 00:05:39.000000 onvif-gui-1.0.6/onvif_gui.egg-info/dependency_links.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)       39 2023-05-04 00:05:39.000000 onvif-gui-1.0.6/onvif_gui.egg-info/entry_points.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)       47 2023-05-04 00:05:39.000000 onvif-gui-1.0.6/onvif_gui.egg-info/requires.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)       29 2023-05-04 00:05:39.000000 onvif-gui-1.0.6/onvif_gui.egg-info/top_level.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1659 2023-05-04 00:03:08.000000 onvif-gui-1.0.6/pyproject.toml
--rw-r--r--   0 stephen   (1000) stephen   (1000)       38 2023-05-04 00:05:39.936091 onvif-gui-1.0.6/setup.cfg
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1504 2023-05-04 00:02:59.000000 onvif-gui-1.0.6/setup.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.936091 onvif-gui-1.0.6/yolox/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/yolox/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.936091 onvif-gui-1.0.6/yolox/models/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      936 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/yolox/models/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4894 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/yolox/models/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6647 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/yolox/models/darknet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2305 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/yolox/models/losses.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6720 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/yolox/models/network_blocks.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3104 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/yolox/models/yolo_fpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    25526 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/yolox/models/yolo_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4158 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/yolox/models/yolo_pafpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1992 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/yolox/models/yolox.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.936091 onvif-gui-1.0.6/yolox/tracker/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/yolox/tracker/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      951 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/yolox/tracker/basetrack.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12172 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/yolox/tracker/byte_tracker.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9547 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/yolox/tracker/kalman_filter.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6158 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/yolox/tracker/matching.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-04 00:05:39.936091 onvif-gui-1.0.6/yolox/utils/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      126 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/yolox/utils/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1580 2023-04-30 20:27:50.000000 onvif-gui-1.0.6/yolox/utils/utils.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.836831 onvif-gui-1.0.7/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11357 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/LICENSE
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       59 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/MANIFEST.in
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-08 16:45:39.836831 onvif-gui-1.0.7/PKG-INFO
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8170 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/README.md
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.816831 onvif-gui-1.0.7/detectron2/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       67 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.816831 onvif-gui-1.0.7/detectron2/checkpoint/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      347 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/checkpoint/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17770 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/checkpoint/c2_model_loading.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5685 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/checkpoint/catalog.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5258 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/checkpoint/detection_checkpoint.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.816831 onvif-gui-1.0.7/detectron2/config/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      599 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/config/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7890 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/config/compat.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9211 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/config/config.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    29512 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/config/defaults.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3015 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/config/instantiate.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15378 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/config/lazy.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.816831 onvif-gui-1.0.7/detectron2/configs/
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.816831 onvif-gui-1.0.7/detectron2/configs/COCO-InstanceSegmentation/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:40:11.000000 onvif-gui-1.0.7/detectron2/configs/COCO-InstanceSegmentation/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.816831 onvif-gui-1.0.7/detectron2/configs/COCO-Keypoints/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:40:01.000000 onvif-gui-1.0.7/detectron2/configs/COCO-Keypoints/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/configs/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.820831 onvif-gui-1.0.7/detectron2/data/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      644 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7378 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/benchmark.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    21231 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7224 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/catalog.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9162 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/common.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8169 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/dataset_mapper.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.820831 onvif-gui-1.0.7/detectron2/data/datasets/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      523 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/datasets/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10174 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/datasets/builtin.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    21841 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/datasets/builtin_meta.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13167 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/datasets/cityscapes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7821 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/datasets/cityscapes_panoptic.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23465 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/datasets/coco.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8977 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/datasets/coco_panoptic.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9623 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/datasets/lvis.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)   223757 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/datasets/lvis_v0_5_categories.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)   219177 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/datasets/lvis_v1_categories.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    39414 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/datasets/lvis_v1_category_image_count.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3128 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/datasets/pascal_voc.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      169 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/datasets/register_coco.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    22841 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/detection_utils.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.820831 onvif-gui-1.0.7/detectron2/data/samplers/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      412 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/samplers/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11789 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/samplers/distributed_sampler.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1944 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/samplers/grouped_batch_sampler.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.820831 onvif-gui-1.0.7/detectron2/data/transforms/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      466 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/transforms/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14112 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/transforms/augmentation.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23069 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/transforms/augmentation_impl.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12629 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/data/transforms/transform.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.820831 onvif-gui-1.0.7/detectron2/layers/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      874 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/layers/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5764 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/layers/aspp.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12131 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/layers/batch_norm.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3024 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/layers/blocks.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    16978 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/layers/deform_conv.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4202 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/layers/losses.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10879 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/layers/mask_ops.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6490 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/layers/nms.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3098 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/layers/roi_align.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3302 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/layers/roi_align_rotated.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      652 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/layers/rotated_boxes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      537 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/layers/shape_spec.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5123 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/layers/wrappers.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.820831 onvif-gui-1.0.7/detectron2/modeling/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1568 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15439 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/anchor_generator.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.824831 onvif-gui-1.0.7/detectron2/modeling/backbone/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      598 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/backbone/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2512 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/backbone/backbone.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1015 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/backbone/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10360 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/backbone/fpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15988 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/backbone/mvit.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    16656 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/backbone/regnet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23658 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/backbone/resnet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    25095 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/backbone/swin.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6360 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/backbone/utils.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    19338 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/backbone/vit.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15123 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/box_regression.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6264 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/matcher.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.824831 onvif-gui-1.0.7/detectron2/modeling/meta_arch/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      508 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/meta_arch/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      814 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/meta_arch/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11651 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/meta_arch/dense_detector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13213 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/meta_arch/fcos.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10407 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/meta_arch/panoptic_fpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13896 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/meta_arch/rcnn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18265 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/meta_arch/retinanet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9906 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/meta_arch/semantic_seg.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10832 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/mmdet_wrapper.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11316 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/poolers.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4045 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/postprocessing.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.824831 onvif-gui-1.0.7/detectron2/modeling/proposal_generator/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      231 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/proposal_generator/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      836 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/proposal_generator/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8128 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/proposal_generator/proposal_utils.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23814 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/proposal_generator/rpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8807 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/proposal_generator/rrpn.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.824831 onvif-gui-1.0.7/detectron2/modeling/roi_heads/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      768 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/roi_heads/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4077 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/roi_heads/box_head.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12990 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/roi_heads/cascade_rcnn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    25390 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/roi_heads/fast_rcnn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11156 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/roi_heads/keypoint_head.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12169 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/roi_heads/mask_head.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    37701 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/roi_heads/roi_heads.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11175 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2334 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/sampling.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12416 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/modeling/test_time_augmentation.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1780 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/predictor.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.824831 onvif-gui-1.0.7/detectron2/structures/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      645 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/structures/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14429 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/structures/boxes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5520 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/structures/image_list.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6613 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/structures/instances.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9030 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/structures/keypoints.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    19802 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/structures/masks.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18853 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/structures/rotated_boxes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2707 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/tracker.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.828831 onvif-gui-1.0.7/detectron2/utils/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       51 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/utils/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6017 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/utils/analysis.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8391 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/utils/collect_env.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4096 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/utils/colormap.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5608 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/utils/comm.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1852 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/utils/develop.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5644 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/utils/env.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17022 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/utils/events.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1189 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/utils/file_io.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7807 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/utils/logger.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2583 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/utils/memory.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1874 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/utils/registry.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1064 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/utils/serialize.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18113 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/utils/testing.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11319 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/utils/video_visualizer.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    51159 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/detectron2/utils/visualizer.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.828831 onvif-gui-1.0.7/gui/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       28 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.828831 onvif-gui-1.0.7/gui/components/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      245 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/components/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1738 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/components/comboselector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2397 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/components/directoryselector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2118 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/components/fileselector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5315 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/components/labelselector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4077 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/components/progress.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1918 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/components/thresholdslider.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1996 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/glwidget.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14377 2023-05-08 16:43:40.000000 onvif-gui-1.0.7/gui/main.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.828831 onvif-gui-1.0.7/gui/onvif/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      191 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/onvif/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5743 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/onvif/admintab.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3959 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/onvif/imagetab.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2425 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/onvif/logindialog.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5247 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/onvif/networktab.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5118 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/onvif/ptztab.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4527 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/onvif/videotab.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.828831 onvif-gui-1.0.7/gui/panels/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      180 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/panels/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3624 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/panels/audiopanel.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13463 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/panels/camerapanel.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14483 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/panels/filepanel.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12913 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/panels/settingspanel.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3627 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/panels/videopanel.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.836831 onvif-gui-1.0.7/gui/resources/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1936 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/LICENSE
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      252 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/apply.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      245 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/apply_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      244 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/apply_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      911 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/audio.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      536 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/audio_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      920 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/audio_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      203 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/branch_closed.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      219 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/branch_closed_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      211 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/branch_closed_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      199 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/branch_open.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      168 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/branch_open_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/branch_open_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      267 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/checked.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      235 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/checked_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      246 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/checked_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12716 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/darkstyle.qss
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      910 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/discover.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      849 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/discover_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      937 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/discover_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      425 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/fast-forward.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      253 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/fast-forward_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      433 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/fast-forward_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      641 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/mute.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      346 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/mute_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      618 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/mute_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      347 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/next.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      225 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/next_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      348 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/next_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    46084 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/onvif-gui.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/pause.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      144 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/pause_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      149 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/pause_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      321 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/play.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      209 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/play_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      316 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/play_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      349 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/previous.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      232 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/previous_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      348 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/previous_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      324 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/radio-off.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      250 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/radio-off_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      324 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/radio-off_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      350 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/radio-on.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      263 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/radio-on_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      343 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/radio-on_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      395 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/record.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      394 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/record_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      425 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/record_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      408 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/recording.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      435 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/recording_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      532 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/recording_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      454 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/rewind.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      250 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/rewind_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      457 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/rewind_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      187 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/small_arrow_left.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      183 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/small_arrow_left_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      189 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/small_arrow_left_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      162 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/small_arrow_up.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      160 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/small_arrow_up_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      161 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/small_arrow_up_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      158 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/stop.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      140 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/stop_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      151 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/stop_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      143 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/unchecked.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      142 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/unchecked_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      143 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/gui/resources/unchecked_lo.png
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.836831 onvif-gui-1.0.7/modules/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/modules/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.836831 onvif-gui-1.0.7/modules/audio/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/modules/audio/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3404 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/modules/audio/sample.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.836831 onvif-gui-1.0.7/modules/video/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/modules/video/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6518 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/modules/video/keypoint.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4796 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/modules/video/retinanet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3016 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/modules/video/sample.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7106 2023-05-05 16:51:13.000000 onvif-gui-1.0.7/modules/video/segment.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11751 2023-05-08 16:34:27.000000 onvif-gui-1.0.7/modules/video/yolox.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.836831 onvif-gui-1.0.7/onvif_gui.egg-info/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-08 16:45:39.000000 onvif-gui-1.0.7/onvif_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7739 2023-05-08 16:45:39.000000 onvif-gui-1.0.7/onvif_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-05-08 16:45:39.000000 onvif-gui-1.0.7/onvif_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       39 2023-05-08 16:45:39.000000 onvif-gui-1.0.7/onvif_gui.egg-info/entry_points.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       47 2023-05-08 16:45:39.000000 onvif-gui-1.0.7/onvif_gui.egg-info/requires.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       29 2023-05-08 16:45:39.000000 onvif-gui-1.0.7/onvif_gui.egg-info/top_level.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1659 2023-05-08 16:43:27.000000 onvif-gui-1.0.7/pyproject.toml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       38 2023-05-08 16:45:39.836831 onvif-gui-1.0.7/setup.cfg
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1504 2023-05-08 16:43:19.000000 onvif-gui-1.0.7/setup.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.836831 onvif-gui-1.0.7/yolox/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:34:27.000000 onvif-gui-1.0.7/yolox/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.836831 onvif-gui-1.0.7/yolox/models/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      936 2023-05-08 16:34:27.000000 onvif-gui-1.0.7/yolox/models/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4894 2023-05-08 16:34:27.000000 onvif-gui-1.0.7/yolox/models/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6647 2023-05-08 16:34:27.000000 onvif-gui-1.0.7/yolox/models/darknet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2305 2023-05-08 16:34:27.000000 onvif-gui-1.0.7/yolox/models/losses.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6720 2023-05-08 16:34:27.000000 onvif-gui-1.0.7/yolox/models/network_blocks.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3104 2023-05-08 16:34:27.000000 onvif-gui-1.0.7/yolox/models/yolo_fpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    25526 2023-05-08 16:34:27.000000 onvif-gui-1.0.7/yolox/models/yolo_head.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4158 2023-05-08 16:34:27.000000 onvif-gui-1.0.7/yolox/models/yolo_pafpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1992 2023-05-08 16:34:27.000000 onvif-gui-1.0.7/yolox/models/yolox.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.836831 onvif-gui-1.0.7/yolox/tracker/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:34:27.000000 onvif-gui-1.0.7/yolox/tracker/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      951 2023-05-08 16:34:27.000000 onvif-gui-1.0.7/yolox/tracker/basetrack.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12172 2023-05-08 16:34:27.000000 onvif-gui-1.0.7/yolox/tracker/byte_tracker.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9547 2023-05-08 16:34:27.000000 onvif-gui-1.0.7/yolox/tracker/kalman_filter.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6158 2023-05-08 16:34:27.000000 onvif-gui-1.0.7/yolox/tracker/matching.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:45:39.836831 onvif-gui-1.0.7/yolox/utils/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      126 2023-05-08 16:34:27.000000 onvif-gui-1.0.7/yolox/utils/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1580 2023-05-08 16:34:27.000000 onvif-gui-1.0.7/yolox/utils/utils.py
```

### Comparing `onvif-gui-1.0.6/LICENSE` & `onvif-gui-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/PKG-INFO` & `onvif-gui-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-gui
-Version: 1.0.6
+Version: 1.0.7
 Summary: A client gui for Onvif
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libonvif
 Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `onvif-gui-1.0.6/README.md` & `onvif-gui-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/checkpoint/c2_model_loading.py` & `onvif-gui-1.0.7/detectron2/checkpoint/c2_model_loading.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/checkpoint/catalog.py` & `onvif-gui-1.0.7/detectron2/checkpoint/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/checkpoint/detection_checkpoint.py` & `onvif-gui-1.0.7/detectron2/checkpoint/detection_checkpoint.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/config/__init__.py` & `onvif-gui-1.0.7/detectron2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/config/compat.py` & `onvif-gui-1.0.7/detectron2/config/compat.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/config/config.py` & `onvif-gui-1.0.7/detectron2/config/config.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/config/defaults.py` & `onvif-gui-1.0.7/detectron2/config/defaults.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/config/instantiate.py` & `onvif-gui-1.0.7/detectron2/config/instantiate.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/config/lazy.py` & `onvif-gui-1.0.7/detectron2/config/lazy.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/__init__.py` & `onvif-gui-1.0.7/detectron2/data/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/benchmark.py` & `onvif-gui-1.0.7/detectron2/data/benchmark.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/build.py` & `onvif-gui-1.0.7/detectron2/data/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/catalog.py` & `onvif-gui-1.0.7/detectron2/data/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/common.py` & `onvif-gui-1.0.7/detectron2/data/common.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/dataset_mapper.py` & `onvif-gui-1.0.7/detectron2/data/dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/datasets/__init__.py` & `onvif-gui-1.0.7/detectron2/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/datasets/builtin.py` & `onvif-gui-1.0.7/detectron2/data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/datasets/builtin_meta.py` & `onvif-gui-1.0.7/detectron2/data/datasets/builtin_meta.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/datasets/cityscapes.py` & `onvif-gui-1.0.7/detectron2/data/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/datasets/cityscapes_panoptic.py` & `onvif-gui-1.0.7/detectron2/data/datasets/cityscapes_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/datasets/coco.py` & `onvif-gui-1.0.7/detectron2/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/datasets/coco_panoptic.py` & `onvif-gui-1.0.7/detectron2/data/datasets/coco_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/datasets/lvis.py` & `onvif-gui-1.0.7/detectron2/data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/datasets/lvis_v0_5_categories.py` & `onvif-gui-1.0.7/detectron2/data/datasets/lvis_v0_5_categories.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/datasets/lvis_v1_categories.py` & `onvif-gui-1.0.7/detectron2/data/datasets/lvis_v1_categories.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/datasets/lvis_v1_category_image_count.py` & `onvif-gui-1.0.7/detectron2/data/datasets/lvis_v1_category_image_count.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/datasets/pascal_voc.py` & `onvif-gui-1.0.7/detectron2/data/datasets/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/detection_utils.py` & `onvif-gui-1.0.7/detectron2/data/detection_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/samplers/distributed_sampler.py` & `onvif-gui-1.0.7/detectron2/data/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/samplers/grouped_batch_sampler.py` & `onvif-gui-1.0.7/detectron2/data/samplers/grouped_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/transforms/augmentation.py` & `onvif-gui-1.0.7/detectron2/data/transforms/augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/transforms/augmentation_impl.py` & `onvif-gui-1.0.7/detectron2/data/transforms/augmentation_impl.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/data/transforms/transform.py` & `onvif-gui-1.0.7/detectron2/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/layers/__init__.py` & `onvif-gui-1.0.7/detectron2/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/layers/aspp.py` & `onvif-gui-1.0.7/detectron2/layers/aspp.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/layers/batch_norm.py` & `onvif-gui-1.0.7/detectron2/layers/batch_norm.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/layers/blocks.py` & `onvif-gui-1.0.7/detectron2/layers/blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/layers/deform_conv.py` & `onvif-gui-1.0.7/detectron2/layers/deform_conv.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/layers/losses.py` & `onvif-gui-1.0.7/detectron2/layers/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/layers/mask_ops.py` & `onvif-gui-1.0.7/detectron2/layers/mask_ops.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/layers/nms.py` & `onvif-gui-1.0.7/detectron2/layers/nms.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/layers/roi_align.py` & `onvif-gui-1.0.7/detectron2/layers/roi_align.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/layers/roi_align_rotated.py` & `onvif-gui-1.0.7/detectron2/layers/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/layers/rotated_boxes.py` & `onvif-gui-1.0.7/detectron2/layers/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/layers/shape_spec.py` & `onvif-gui-1.0.7/detectron2/layers/shape_spec.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/layers/wrappers.py` & `onvif-gui-1.0.7/detectron2/layers/wrappers.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/__init__.py` & `onvif-gui-1.0.7/detectron2/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/anchor_generator.py` & `onvif-gui-1.0.7/detectron2/modeling/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/backbone/__init__.py` & `onvif-gui-1.0.7/detectron2/modeling/backbone/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/backbone/backbone.py` & `onvif-gui-1.0.7/detectron2/modeling/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/backbone/build.py` & `onvif-gui-1.0.7/detectron2/modeling/backbone/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/backbone/fpn.py` & `onvif-gui-1.0.7/detectron2/modeling/backbone/fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/backbone/mvit.py` & `onvif-gui-1.0.7/detectron2/modeling/backbone/mvit.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/backbone/regnet.py` & `onvif-gui-1.0.7/detectron2/modeling/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/backbone/resnet.py` & `onvif-gui-1.0.7/detectron2/modeling/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/backbone/swin.py` & `onvif-gui-1.0.7/detectron2/modeling/backbone/swin.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/backbone/utils.py` & `onvif-gui-1.0.7/detectron2/modeling/backbone/utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/backbone/vit.py` & `onvif-gui-1.0.7/detectron2/modeling/backbone/vit.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/box_regression.py` & `onvif-gui-1.0.7/detectron2/modeling/box_regression.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/matcher.py` & `onvif-gui-1.0.7/detectron2/modeling/matcher.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/meta_arch/build.py` & `onvif-gui-1.0.7/detectron2/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/meta_arch/dense_detector.py` & `onvif-gui-1.0.7/detectron2/modeling/meta_arch/dense_detector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/meta_arch/fcos.py` & `onvif-gui-1.0.7/detectron2/modeling/meta_arch/fcos.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/meta_arch/panoptic_fpn.py` & `onvif-gui-1.0.7/detectron2/modeling/meta_arch/panoptic_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/meta_arch/rcnn.py` & `onvif-gui-1.0.7/detectron2/modeling/meta_arch/rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/meta_arch/retinanet.py` & `onvif-gui-1.0.7/detectron2/modeling/meta_arch/retinanet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/meta_arch/semantic_seg.py` & `onvif-gui-1.0.7/detectron2/modeling/meta_arch/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/mmdet_wrapper.py` & `onvif-gui-1.0.7/detectron2/modeling/mmdet_wrapper.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/poolers.py` & `onvif-gui-1.0.7/detectron2/modeling/poolers.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/postprocessing.py` & `onvif-gui-1.0.7/detectron2/modeling/postprocessing.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/proposal_generator/build.py` & `onvif-gui-1.0.7/detectron2/modeling/proposal_generator/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/proposal_generator/proposal_utils.py` & `onvif-gui-1.0.7/detectron2/modeling/proposal_generator/proposal_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/proposal_generator/rpn.py` & `onvif-gui-1.0.7/detectron2/modeling/proposal_generator/rpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/proposal_generator/rrpn.py` & `onvif-gui-1.0.7/detectron2/modeling/proposal_generator/rrpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/roi_heads/__init__.py` & `onvif-gui-1.0.7/detectron2/modeling/roi_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/roi_heads/box_head.py` & `onvif-gui-1.0.7/detectron2/modeling/roi_heads/box_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/roi_heads/cascade_rcnn.py` & `onvif-gui-1.0.7/detectron2/modeling/roi_heads/cascade_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/roi_heads/fast_rcnn.py` & `onvif-gui-1.0.7/detectron2/modeling/roi_heads/fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/roi_heads/keypoint_head.py` & `onvif-gui-1.0.7/detectron2/modeling/roi_heads/keypoint_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/roi_heads/mask_head.py` & `onvif-gui-1.0.7/detectron2/modeling/roi_heads/mask_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/roi_heads/roi_heads.py` & `onvif-gui-1.0.7/detectron2/modeling/roi_heads/roi_heads.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/roi_heads/rotated_fast_rcnn.py` & `onvif-gui-1.0.7/detectron2/modeling/roi_heads/rotated_fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/sampling.py` & `onvif-gui-1.0.7/detectron2/modeling/sampling.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/modeling/test_time_augmentation.py` & `onvif-gui-1.0.7/detectron2/modeling/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/predictor.py` & `onvif-gui-1.0.7/detectron2/predictor.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/structures/__init__.py` & `onvif-gui-1.0.7/detectron2/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/structures/boxes.py` & `onvif-gui-1.0.7/detectron2/structures/boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/structures/image_list.py` & `onvif-gui-1.0.7/detectron2/structures/image_list.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/structures/instances.py` & `onvif-gui-1.0.7/detectron2/structures/instances.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/structures/keypoints.py` & `onvif-gui-1.0.7/detectron2/structures/keypoints.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/structures/masks.py` & `onvif-gui-1.0.7/detectron2/structures/masks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/structures/rotated_boxes.py` & `onvif-gui-1.0.7/detectron2/structures/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/tracker.py` & `onvif-gui-1.0.7/detectron2/tracker.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/utils/analysis.py` & `onvif-gui-1.0.7/detectron2/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/utils/collect_env.py` & `onvif-gui-1.0.7/detectron2/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/utils/colormap.py` & `onvif-gui-1.0.7/detectron2/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/utils/comm.py` & `onvif-gui-1.0.7/detectron2/utils/comm.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/utils/develop.py` & `onvif-gui-1.0.7/detectron2/utils/develop.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/utils/env.py` & `onvif-gui-1.0.7/detectron2/utils/env.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/utils/events.py` & `onvif-gui-1.0.7/detectron2/utils/events.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/utils/file_io.py` & `onvif-gui-1.0.7/detectron2/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/utils/logger.py` & `onvif-gui-1.0.7/detectron2/utils/logger.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/utils/memory.py` & `onvif-gui-1.0.7/detectron2/utils/memory.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/utils/registry.py` & `onvif-gui-1.0.7/detectron2/utils/registry.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/utils/serialize.py` & `onvif-gui-1.0.7/detectron2/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/utils/testing.py` & `onvif-gui-1.0.7/detectron2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/utils/video_visualizer.py` & `onvif-gui-1.0.7/detectron2/utils/video_visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/detectron2/utils/visualizer.py` & `onvif-gui-1.0.7/detectron2/utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/components/comboselector.py` & `onvif-gui-1.0.7/gui/components/comboselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/components/directoryselector.py` & `onvif-gui-1.0.7/gui/components/directoryselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/components/fileselector.py` & `onvif-gui-1.0.7/gui/components/fileselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/components/labelselector.py` & `onvif-gui-1.0.7/gui/components/labelselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/components/progress.py` & `onvif-gui-1.0.7/gui/components/progress.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/components/thresholdslider.py` & `onvif-gui-1.0.7/gui/components/thresholdslider.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/glwidget.py` & `onvif-gui-1.0.7/gui/glwidget.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/main.py` & `onvif-gui-1.0.7/gui/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 class MainWindow(QMainWindow):
     def __init__(self, clear_settings=False):
         super().__init__()
         os.environ["QT_FILESYSTEMMODEL_WATCH_FILES"] = "ON"
         QDir.addSearchPath("image", self.getLocation() + "/gui/resources/")
         self.style()
-        self.program_name = "onvif gui version 1.0.6"
+        self.program_name = "onvif gui version 1.0.7"
         self.setWindowTitle(self.program_name)
         self.setWindowIcon(QIcon('image:onvif-gui.png'))
         self.settings = QSettings("onvif", "gui")
         if clear_settings:
             self.settings.clear()
         self.volumeKey = "MainWindow/volume"
         self.muteKey = "MainWindow/mute"
```

### Comparing `onvif-gui-1.0.6/gui/onvif/admintab.py` & `onvif-gui-1.0.7/gui/onvif/admintab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/onvif/imagetab.py` & `onvif-gui-1.0.7/gui/onvif/imagetab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/onvif/logindialog.py` & `onvif-gui-1.0.7/gui/onvif/logindialog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/onvif/networktab.py` & `onvif-gui-1.0.7/gui/onvif/networktab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/onvif/ptztab.py` & `onvif-gui-1.0.7/gui/onvif/ptztab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/onvif/videotab.py` & `onvif-gui-1.0.7/gui/onvif/videotab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/panels/audiopanel.py` & `onvif-gui-1.0.7/gui/panels/audiopanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/panels/camerapanel.py` & `onvif-gui-1.0.7/gui/panels/camerapanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/panels/filepanel.py` & `onvif-gui-1.0.7/gui/panels/filepanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/panels/settingspanel.py` & `onvif-gui-1.0.7/gui/panels/settingspanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/panels/videopanel.py` & `onvif-gui-1.0.7/gui/panels/videopanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/resources/LICENSE` & `onvif-gui-1.0.7/gui/resources/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/resources/audio.png` & `onvif-gui-1.0.7/gui/resources/audio.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/resources/audio_hi.png` & `onvif-gui-1.0.7/gui/resources/audio_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/resources/audio_lo.png` & `onvif-gui-1.0.7/gui/resources/audio_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/resources/darkstyle.qss` & `onvif-gui-1.0.7/gui/resources/darkstyle.qss`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/resources/discover.png` & `onvif-gui-1.0.7/gui/resources/discover.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/resources/discover_hi.png` & `onvif-gui-1.0.7/gui/resources/discover_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/resources/discover_lo.png` & `onvif-gui-1.0.7/gui/resources/discover_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/resources/mute.png` & `onvif-gui-1.0.7/gui/resources/mute.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/resources/mute_lo.png` & `onvif-gui-1.0.7/gui/resources/mute_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/resources/onvif-gui.png` & `onvif-gui-1.0.7/gui/resources/onvif-gui.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/gui/resources/recording_lo.png` & `onvif-gui-1.0.7/gui/resources/recording_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/modules/audio/sample.py` & `onvif-gui-1.0.7/modules/audio/sample.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/modules/video/keypoint.py` & `onvif-gui-1.0.7/modules/video/keypoint.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/modules/video/retinanet.py` & `onvif-gui-1.0.7/modules/video/retinanet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/modules/video/sample.py` & `onvif-gui-1.0.7/modules/video/sample.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/modules/video/segment.py` & `onvif-gui-1.0.7/modules/video/segment.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/modules/video/yolox.py` & `onvif-gui-1.0.7/modules/video/yolox.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/onvif_gui.egg-info/PKG-INFO` & `onvif-gui-1.0.7/onvif_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-gui
-Version: 1.0.6
+Version: 1.0.7
 Summary: A client gui for Onvif
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libonvif
 Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `onvif-gui-1.0.6/onvif_gui.egg-info/SOURCES.txt` & `onvif-gui-1.0.7/onvif_gui.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 detectron2/config/__init__.py
 detectron2/config/compat.py
 detectron2/config/config.py
 detectron2/config/defaults.py
 detectron2/config/instantiate.py
 detectron2/config/lazy.py
 detectron2/configs/__init__.py
+detectron2/configs/COCO-InstanceSegmentation/__init__.py
+detectron2/configs/COCO-Keypoints/__init__.py
 detectron2/data/__init__.py
 detectron2/data/benchmark.py
 detectron2/data/build.py
 detectron2/data/catalog.py
 detectron2/data/common.py
 detectron2/data/dataset_mapper.py
 detectron2/data/detection_utils.py
```

### Comparing `onvif-gui-1.0.6/pyproject.toml` & `onvif-gui-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #*********************************************************************/
 
 [project]
 name = "onvif-gui" 
-version = "1.0.6"  
+version = "1.0.7"  
 description = "A client gui for Onvif"  
 readme = "README.md" 
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["sample", "setuptools", "development"]  
 authors = [
   {name = "Stephen Rhodes", email = "sr99622@gmail.com" }
```

### Comparing `onvif-gui-1.0.6/setup.py` & `onvif-gui-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from setuptools.command.install import install
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="onvif-gui",
-    version="1.0.6",
+    version="1.0.7",
     author="Stephen Rhodes",
     author_email="sr99622@gmail.com",
     description="GUI program for onvif",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

### Comparing `onvif-gui-1.0.6/yolox/models/__init__.py` & `onvif-gui-1.0.7/yolox/models/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/yolox/models/build.py` & `onvif-gui-1.0.7/yolox/models/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/yolox/models/darknet.py` & `onvif-gui-1.0.7/yolox/models/darknet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/yolox/models/losses.py` & `onvif-gui-1.0.7/yolox/models/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/yolox/models/network_blocks.py` & `onvif-gui-1.0.7/yolox/models/network_blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/yolox/models/yolo_fpn.py` & `onvif-gui-1.0.7/yolox/models/yolo_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/yolox/models/yolo_head.py` & `onvif-gui-1.0.7/yolox/models/yolo_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/yolox/models/yolo_pafpn.py` & `onvif-gui-1.0.7/yolox/models/yolo_pafpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/yolox/models/yolox.py` & `onvif-gui-1.0.7/yolox/models/yolox.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/yolox/tracker/basetrack.py` & `onvif-gui-1.0.7/yolox/tracker/basetrack.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/yolox/tracker/byte_tracker.py` & `onvif-gui-1.0.7/yolox/tracker/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/yolox/tracker/kalman_filter.py` & `onvif-gui-1.0.7/yolox/tracker/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/yolox/tracker/matching.py` & `onvif-gui-1.0.7/yolox/tracker/matching.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.0.6/yolox/utils/utils.py` & `onvif-gui-1.0.7/yolox/utils/utils.py`

 * *Files identical despite different names*

