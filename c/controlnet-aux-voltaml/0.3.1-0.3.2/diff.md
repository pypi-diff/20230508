# Comparing `tmp/controlnet_aux_voltaml-0.3.1.tar.gz` & `tmp/controlnet_aux_voltaml-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "controlnet_aux_voltaml-0.3.1.tar", last modified: Mon May  8 09:10:14 2023, max compression
+gzip compressed data, was "controlnet_aux_voltaml-0.3.2.tar", last modified: Mon May  8 09:20:09 2023, max compression
```

## Comparing `controlnet_aux_voltaml-0.3.1.tar` & `controlnet_aux_voltaml-0.3.2.tar`

### file list

```diff
@@ -1,161 +1,158 @@
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.888310 controlnet_aux_voltaml-0.3.1/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3203 2023-05-08 09:10:14.888310 controlnet_aux_voltaml-0.3.1/PKG-INFO
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2272 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/README.md
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)       38 2023-05-08 09:10:14.888310 controlnet_aux_voltaml-0.3.1/setup.cfg
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     8853 2023-05-08 09:09:49.000000 controlnet_aux_voltaml-0.3.1/setup.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.872310 controlnet_aux_voltaml-0.3.1/src/
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.872310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      472 2023-05-08 09:05:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/__init__.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.872310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/canny/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      547 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/canny/__init__.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.872310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/hed/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     7994 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/hed/__init__.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.872310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/lineart/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     5293 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/lineart/__init__.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.872310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/lineart_anime/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     7718 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/lineart_anime/__init__.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.872310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/mediapipe_face/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      645 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/mediapipe_face/__init__.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     6713 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/mediapipe_face/mediapipe_face_common.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.872310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2992 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/__init__.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     5276 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/api.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.872310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/midas/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/midas/__init__.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      367 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/midas/base_model.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     9242 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/midas/blocks.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3154 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/midas/dpt_depth.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2709 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/midas/midas_net.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     5207 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/midas/midas_net_custom.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     7869 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/midas/transforms.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    14625 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/midas/vit.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     4582 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/utils.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.872310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/mlsd/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2314 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/mlsd/__init__.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.876310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/mlsd/models/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/mlsd/models/__init__.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     9678 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     9180 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    24134 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/mlsd/utils.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.876310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2662 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/__init__.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.876310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      597 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/NNET.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/__init__.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2980 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/baseline.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.876310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/__init__.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    10480 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/decoder.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.876310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/__init__.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2428 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     5993 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.876310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)       89 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/__init__.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3000 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/dataset.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3113 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/loader.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     9187 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/tf_preprocessing.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     4760 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/transforms.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.876310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      206 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/__init__.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.880310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     4170 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2690 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2294 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     4549 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3350 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    12093 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    26514 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    59925 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2833 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    15009 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      707 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)       22 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/version.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2730 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     5821 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2932 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      843 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     4905 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1737 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1297 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     6632 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1060 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/encoder.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     5703 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/submodules.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.880310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/utils/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/utils/__init__.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     7570 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/utils/losses.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     6725 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/utils/utils.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.880310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/open_pose/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     5563 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/open_pose/__init__.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    10883 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/open_pose/body.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    15314 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/open_pose/face.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     6530 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/open_pose/hand.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     8743 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/open_pose/model.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     7934 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/open_pose/util.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.880310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/pidi/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2978 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/pidi/__init__.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    21794 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/pidi/model.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.880310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/shuffle/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3468 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/shuffle/__init__.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3890 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/util.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.880310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2192 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/__init__.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.880310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/__init__.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.880310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1154 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/__init__.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.880310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1154 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    15248 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.884310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/__init__.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    13757 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.884310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/__init__.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.884310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/__init__.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     6909 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3436 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1045 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      333 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      931 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1576 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     7284 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     6899 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      367 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/base_model.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    12792 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     6099 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2709 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     5207 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     8552 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     7869 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2390 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/builder.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     7362 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/depth_model.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.884310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/layers/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1153 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/layers/__init__.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     8693 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/layers/attractor.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     4838 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     6733 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     4163 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3438 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/model_io.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.884310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/zoedepth/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1270 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1587 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth.json
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      556 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth_kitti.json
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    12630 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.884310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1276 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1968 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/config_zoedepth_nk.json
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    16363 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.884310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/utils/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1154 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/utils/__init__.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      624 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/utils/arg_utils.py
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    16310 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/utils/config.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.888310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/utils/easydict/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3426 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py
-drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:10:14.888310 controlnet_aux_voltaml-0.3.1/src/controlnet_aux_voltaml.egg-info/
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3203 2023-05-08 09:10:14.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux_voltaml.egg-info/PKG-INFO
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     7550 2023-05-08 09:10:14.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux_voltaml.egg-info/SOURCES.txt
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        1 2023-05-08 09:10:14.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux_voltaml.egg-info/dependency_links.txt
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      120 2023-05-08 09:10:14.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux_voltaml.egg-info/requires.txt
--rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)       15 2023-05-08 09:10:14.000000 controlnet_aux_voltaml-0.3.1/src/controlnet_aux_voltaml.egg-info/top_level.txt
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.997061 controlnet_aux_voltaml-0.3.2/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3203 2023-05-08 09:20:08.997061 controlnet_aux_voltaml-0.3.2/PKG-INFO
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2272 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/README.md
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)       38 2023-05-08 09:20:08.997061 controlnet_aux_voltaml-0.3.2/setup.cfg
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     8853 2023-05-08 09:19:57.000000 controlnet_aux_voltaml-0.3.2/setup.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.985061 controlnet_aux_voltaml-0.3.2/src/
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.989061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      472 2023-05-08 09:20:03.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/__init__.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.989061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/canny/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      547 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/canny/__init__.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.989061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/hed/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     7994 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/hed/__init__.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.989061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/lineart/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     5293 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/lineart/__init__.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.989061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/lineart_anime/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     7718 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/lineart_anime/__init__.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.989061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/mediapipe_face/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      645 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/mediapipe_face/__init__.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     6713 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/mediapipe_face/mediapipe_face_common.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.989061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2992 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/__init__.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     5276 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/api.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.989061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/midas/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/midas/__init__.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      367 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/midas/base_model.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     9242 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/midas/blocks.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3154 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/midas/dpt_depth.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2709 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/midas/midas_net.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     5207 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/midas/midas_net_custom.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     7869 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/midas/transforms.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    14625 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/midas/vit.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     4582 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/utils.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.989061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/mlsd/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2314 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/mlsd/__init__.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.989061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/mlsd/models/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/mlsd/models/__init__.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     9678 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/mlsd/models/mbv2_mlsd_large.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     9180 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/mlsd/models/mbv2_mlsd_tiny.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    24134 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/mlsd/utils.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.989061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2662 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/__init__.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.989061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      597 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/NNET.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/__init__.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2980 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/baseline.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.989061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/__init__.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    10480 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/decoder.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.993061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/__init__.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2428 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     5993 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.993061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/data/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)       89 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/data/__init__.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3000 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/data/dataset.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3113 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/data/loader.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     9187 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/data/tf_preprocessing.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     4760 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/data/transforms.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.993061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      206 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/__init__.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.993061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     4170 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2690 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2294 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     4549 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3350 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    12093 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    26514 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    59925 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2833 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    15009 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      707 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)       22 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/version.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2730 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/hubconf.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     5821 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/onnx_export.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2932 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      843 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     4905 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1737 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/setup.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1297 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/utils.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     6632 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/validate.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1060 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/encoder.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     5703 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/submodules.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.993061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/utils/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/utils/__init__.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     7570 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/utils/losses.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     6725 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/utils/utils.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.993061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/open_pose/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     5563 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/open_pose/__init__.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    10883 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/open_pose/body.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    15314 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/open_pose/face.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     6530 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/open_pose/hand.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     8743 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/open_pose/model.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     7934 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/open_pose/util.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.993061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/pidi/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2978 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/pidi/__init__.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    21794 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/pidi/model.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.993061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/shuffle/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3468 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/shuffle/__init__.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3890 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/util.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.993061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2192 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/__init__.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.993061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/__init__.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.993061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1154 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/__init__.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.993061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1154 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/__init__.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    15248 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.993061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/__init__.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    13757 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/hubconf.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.997061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/__init__.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.997061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/__init__.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     6909 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3436 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1045 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      333 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      931 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1576 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     7284 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     6899 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      367 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/base_model.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    12792 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     6099 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2709 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     5207 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     8552 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     7869 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     2390 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/builder.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     7362 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/depth_model.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.997061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/layers/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1153 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/layers/__init__.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     8693 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/layers/attractor.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     4838 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/layers/dist_layers.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     6733 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/layers/localbins_layers.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     4163 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/layers/patch_transformer.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3438 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/model_io.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.997061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/zoedepth/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1270 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/zoedepth/__init__.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    12630 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/zoedepth/zoedepth_v1.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.997061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/zoedepth_nk/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1276 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/zoedepth_nk/__init__.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    16363 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.997061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/utils/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     1154 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/utils/__init__.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      624 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/utils/arg_utils.py
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)    16310 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/utils/config.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.997061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/utils/easydict/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3426 2023-05-08 09:04:44.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/utils/easydict/__init__.py
+drwxrwxr-x   0 kubuntu   (1000) kubuntu   (1000)        0 2023-05-08 09:20:08.989061 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml.egg-info/
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     3203 2023-05-08 09:20:08.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml.egg-info/PKG-INFO
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)     8235 2023-05-08 09:20:08.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml.egg-info/SOURCES.txt
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)        1 2023-05-08 09:20:08.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml.egg-info/dependency_links.txt
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)      120 2023-05-08 09:20:08.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml.egg-info/requires.txt
+-rw-rw-r--   0 kubuntu   (1000) kubuntu   (1000)       23 2023-05-08 09:20:08.000000 controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml.egg-info/top_level.txt
```

### Comparing `controlnet_aux_voltaml-0.3.1/PKG-INFO` & `controlnet_aux_voltaml-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: controlnet_aux_voltaml
-Version: 0.3.1
+Version: 0.3.2
 Summary: Utilities for preprocessing images for controlnet
 Home-page: https://github.com/patrickvonplaten/controlnet_aux
 Author: The HuggingFace team
 Author-email: patrick@huggingface.co
 License: Apache
 Keywords: deep learning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `controlnet_aux_voltaml-0.3.1/README.md` & `controlnet_aux_voltaml-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/setup.py` & `controlnet_aux_voltaml-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
     deps["torchvision"],
     deps["timm"],
     deps["scikit-image"],
 ]
 
 setup(
     name="controlnet_aux_voltaml",
-    version="0.3.1",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
+    version="0.3.2",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
     description="Utilities for preprocessing images for controlnet",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning",
     license="Apache",
     author="The HuggingFace team",
     author_email="patrick@huggingface.co",
```

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/canny/__init__.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/canny/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/hed/__init__.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/hed/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/lineart/__init__.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/lineart/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/lineart_anime/__init__.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/lineart_anime/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/mediapipe_face/__init__.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/mediapipe_face/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/mediapipe_face/mediapipe_face_common.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/mediapipe_face/mediapipe_face_common.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/__init__.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/api.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/api.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/midas/blocks.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/midas/dpt_depth.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/midas/midas_net.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/midas/midas_net_custom.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/midas/transforms.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/midas/vit.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/midas/utils.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/midas/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/mlsd/__init__.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/mlsd/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/mlsd/utils.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/__init__.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/NNET.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/NNET.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/baseline.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/baseline.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/decoder.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/decoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/dataset.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/data/dataset.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/loader.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/data/loader.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/tf_preprocessing.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/data/tf_preprocessing.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/transforms.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/data/transforms.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/hubconf.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/onnx_export.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/setup.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/efficientnet_repo/validate.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/encoder.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/encoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/nets/submodules/submodules.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/nets/submodules/submodules.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/utils/losses.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/utils/losses.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/normalbae/utils/utils.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/normalbae/utils/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/open_pose/__init__.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/open_pose/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/open_pose/body.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/open_pose/body.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/open_pose/face.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/open_pose/face.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/open_pose/hand.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/open_pose/hand.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/open_pose/model.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/open_pose/model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/open_pose/util.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/open_pose/util.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/pidi/__init__.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/pidi/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/pidi/model.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/pidi/model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/shuffle/__init__.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/shuffle/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/util.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/util.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/__init__.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/__init__.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/hubconf.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/builder.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/builder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/depth_model.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/depth_model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/layers/__init__.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/layers/attractor.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/layers/attractor.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/layers/dist_layers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/layers/localbins_layers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/layers/patch_transformer.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/model_io.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/model_io.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/zoedepth/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/zoedepth/zoedepth_v1.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/zoedepth_nk/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/utils/__init__.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/utils/arg_utils.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/utils/config.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/utils/config.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml/zoe/zoedepth/utils/easydict/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux_voltaml-0.3.1/src/controlnet_aux_voltaml.egg-info/PKG-INFO` & `controlnet_aux_voltaml-0.3.2/src/controlnet_aux_voltaml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: controlnet-aux-voltaml
-Version: 0.3.1
+Version: 0.3.2
 Summary: Utilities for preprocessing images for controlnet
 Home-page: https://github.com/patrickvonplaten/controlnet_aux
 Author: The HuggingFace team
 Author-email: patrick@huggingface.co
 License: Apache
 Keywords: deep learning
 Classifier: Development Status :: 5 - Production/Stable
```

