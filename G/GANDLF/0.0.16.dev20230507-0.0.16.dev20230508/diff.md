# Comparing `tmp/GANDLF-0.0.16.dev20230507.tar.gz` & `tmp/GANDLF-0.0.16.dev20230508.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GANDLF-0.0.16.dev20230507.tar", last modified: Sun May  7 03:12:45 2023, max compression
+gzip compressed data, was "GANDLF-0.0.16.dev20230508.tar", last modified: Mon May  8 03:13:25 2023, max compression
```

## Comparing `GANDLF-0.0.16.dev20230507.tar` & `GANDLF-0.0.16.dev20230508.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.457810 GANDLF-0.0.16.dev20230507/
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.421810 GANDLF-0.0.16.dev20230507/GANDLF/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.421810 GANDLF-0.0.16.dev20230507/GANDLF/anonymize/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/anonymize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/anonymize/convert_to_nifti.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.425810 GANDLF-0.0.16.dev20230507/GANDLF/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/cli/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/cli/main_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/cli/patch_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/cli/post_training_model_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/cli/preprocess_and_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/cli/recover_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.425810 GANDLF-0.0.16.dev20230507/GANDLF/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/compute/forward_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/compute/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/compute/inference_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/compute/loss_and_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/compute/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    21366 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/compute/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.429810 GANDLF-0.0.16.dev20230507/GANDLF/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/ImagesFromDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.429810 GANDLF-0.0.16.dev20230507/GANDLF/data/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/augmentation/blur_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/augmentation/noise_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/augmentation/rgb_augs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/augmentation/rotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/augmentation/wrap_torchio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/inference_dataloader_histopath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.429810 GANDLF-0.0.16.dev20230507/GANDLF/data/patch_miner/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/patch_miner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.429810 GANDLF-0.0.16.dev20230507/GANDLF/data/patch_miner/opm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/patch_miner/opm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/patch_miner/opm/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    21766 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/patch_miner/opm/patch_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/patch_miner/opm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.433810 GANDLF-0.0.16.dev20230507/GANDLF/data/post_process/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/post_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/post_process/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/post_process/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.433810 GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/crop_zero_planes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/non_zero_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/normalize_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/resample_minimum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/rgb_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.437811 GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/template_matching/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/template_matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/template_matching/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/template_matching/histogram_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/template_matching/stain_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/template_matching/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/threshold_and_clip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.437811 GANDLF-0.0.16.dev20230507/GANDLF/grad_clipping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/grad_clipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/grad_clipping/adaptive_gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/grad_clipping/clip_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/grad_clipping/grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/inference_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.437811 GANDLF-0.0.16.dev20230507/GANDLF/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/losses/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/losses/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/losses/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.441810 GANDLF-0.0.16.dev20230507/GANDLF/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/metrics/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.445810 GANDLF-0.0.16.dev20230507/GANDLF/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/MSDNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/brain_age.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/deep_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/imagenet_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/imagenet_vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/light_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/light_unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/modelBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/sdnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.453811 GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/DecodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/DownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/EncodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/FCNUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/IncConv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/IncDownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/IncDropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/IncUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/InceptionModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/InitialConv.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/Interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/ResNetModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/UpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/add_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/add_downsample_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/average_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/out_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/transunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/uinc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/models/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.453811 GANDLF-0.0.16.dev20230507/GANDLF/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/optimizers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    30843 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/parseConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.453811 GANDLF-0.0.16.dev20230507/GANDLF/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/schedulers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/training_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.457810 GANDLF-0.0.16.dev20230507/GANDLF/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/utils/handle_collisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/utils/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/utils/modelbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/utils/modelio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/utils/parameter_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/utils/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/GANDLF/utils/write_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-07 03:12:38.000000 GANDLF-0.0.16.dev20230507/GANDLF/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:12:45.421810 GANDLF-0.0.16.dev20230507/GANDLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-05-07 03:12:45.000000 GANDLF-0.0.16.dev20230507/GANDLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-07 03:12:45.000000 GANDLF-0.0.16.dev20230507/GANDLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 03:12:45.000000 GANDLF-0.0.16.dev20230507/GANDLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 03:10:29.000000 GANDLF-0.0.16.dev20230507/GANDLF.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-07 03:12:45.000000 GANDLF-0.0.16.dev20230507/GANDLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 03:12:45.000000 GANDLF-0.0.16.dev20230507/GANDLF.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-05-07 03:12:45.457810 GANDLF-0.0.16.dev20230507/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/gandlf_anonymizer
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/gandlf_collectStats
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/gandlf_configGenerator
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/gandlf_constructCSV
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/gandlf_deploy
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/gandlf_optimizeModel
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/gandlf_patchMiner
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/gandlf_preprocess
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/gandlf_recoverConfig
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/gandlf_run
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/gandlf_verifyInstall
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 03:12:45.457810 GANDLF-0.0.16.dev20230507/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-05-07 03:10:12.000000 GANDLF-0.0.16.dev20230507/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.902946 GANDLF-0.0.16.dev20230508/
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.846943 GANDLF-0.0.16.dev20230508/GANDLF/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.846943 GANDLF-0.0.16.dev20230508/GANDLF/anonymize/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/anonymize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/anonymize/convert_to_nifti.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.850943 GANDLF-0.0.16.dev20230508/GANDLF/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/cli/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/cli/main_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/cli/patch_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/cli/post_training_model_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/cli/preprocess_and_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/cli/recover_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.854943 GANDLF-0.0.16.dev20230508/GANDLF/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/compute/forward_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/compute/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/compute/inference_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/compute/loss_and_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/compute/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21366 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/compute/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.858943 GANDLF-0.0.16.dev20230508/GANDLF/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/ImagesFromDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.858943 GANDLF-0.0.16.dev20230508/GANDLF/data/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/augmentation/blur_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/augmentation/noise_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/augmentation/rgb_augs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/augmentation/rotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/augmentation/wrap_torchio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/inference_dataloader_histopath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.858943 GANDLF-0.0.16.dev20230508/GANDLF/data/patch_miner/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/patch_miner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.862944 GANDLF-0.0.16.dev20230508/GANDLF/data/patch_miner/opm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/patch_miner/opm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/patch_miner/opm/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21766 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/patch_miner/opm/patch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/patch_miner/opm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.862944 GANDLF-0.0.16.dev20230508/GANDLF/data/post_process/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/post_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/post_process/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/post_process/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.866944 GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/crop_zero_planes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/non_zero_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/normalize_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/resample_minimum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/rgb_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.870944 GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/template_matching/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/template_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/template_matching/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/template_matching/histogram_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/template_matching/stain_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/template_matching/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/threshold_and_clip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.870944 GANDLF-0.0.16.dev20230508/GANDLF/grad_clipping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/grad_clipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/grad_clipping/adaptive_gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/grad_clipping/clip_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/grad_clipping/grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/inference_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.874944 GANDLF-0.0.16.dev20230508/GANDLF/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/losses/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/losses/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/losses/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.874944 GANDLF-0.0.16.dev20230508/GANDLF/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/metrics/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.886945 GANDLF-0.0.16.dev20230508/GANDLF/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/MSDNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/brain_age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/deep_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/imagenet_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/imagenet_vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/light_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/light_unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/modelBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/sdnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.894946 GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/DecodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/DownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/EncodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/FCNUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/IncConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/IncDownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/IncDropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/IncUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/InceptionModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/InitialConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/Interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/ResNetModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/UpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/add_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/add_downsample_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/average_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/out_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/transunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/uinc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/models/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.894946 GANDLF-0.0.16.dev20230508/GANDLF/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/optimizers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30843 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/parseConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.894946 GANDLF-0.0.16.dev20230508/GANDLF/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/schedulers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/training_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.898946 GANDLF-0.0.16.dev20230508/GANDLF/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/utils/handle_collisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/utils/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/utils/modelbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/utils/modelio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/utils/parameter_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/utils/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/GANDLF/utils/write_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-08 03:13:17.000000 GANDLF-0.0.16.dev20230508/GANDLF/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:13:25.846943 GANDLF-0.0.16.dev20230508/GANDLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-05-08 03:13:25.000000 GANDLF-0.0.16.dev20230508/GANDLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-08 03:13:25.000000 GANDLF-0.0.16.dev20230508/GANDLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 03:13:25.000000 GANDLF-0.0.16.dev20230508/GANDLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 03:10:50.000000 GANDLF-0.0.16.dev20230508/GANDLF.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-08 03:13:25.000000 GANDLF-0.0.16.dev20230508/GANDLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 03:13:25.000000 GANDLF-0.0.16.dev20230508/GANDLF.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-05-08 03:13:25.898946 GANDLF-0.0.16.dev20230508/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/gandlf_anonymizer
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/gandlf_collectStats
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/gandlf_configGenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/gandlf_constructCSV
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/gandlf_deploy
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/gandlf_optimizeModel
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/gandlf_patchMiner
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/gandlf_preprocess
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/gandlf_recoverConfig
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/gandlf_run
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/gandlf_verifyInstall
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 03:13:25.902946 GANDLF-0.0.16.dev20230508/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-05-08 03:10:27.000000 GANDLF-0.0.16.dev20230508/setup.py
```

### Comparing `GANDLF-0.0.16.dev20230507/CODE_OF_CONDUCT.md` & `GANDLF-0.0.16.dev20230508/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/CONTRIBUTING.md` & `GANDLF-0.0.16.dev20230508/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/anonymize/__init__.py` & `GANDLF-0.0.16.dev20230508/GANDLF/anonymize/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/anonymize/convert_to_nifti.py` & `GANDLF-0.0.16.dev20230508/GANDLF/anonymize/convert_to_nifti.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/cli/__init__.py` & `GANDLF-0.0.16.dev20230508/GANDLF/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/cli/config_generator.py` & `GANDLF-0.0.16.dev20230508/GANDLF/cli/config_generator.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/cli/deploy.py` & `GANDLF-0.0.16.dev20230508/GANDLF/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/cli/main_run.py` & `GANDLF-0.0.16.dev20230508/GANDLF/cli/main_run.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/cli/patch_extraction.py` & `GANDLF-0.0.16.dev20230508/GANDLF/cli/patch_extraction.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/cli/post_training_model_optimization.py` & `GANDLF-0.0.16.dev20230508/GANDLF/cli/post_training_model_optimization.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/cli/preprocess_and_save.py` & `GANDLF-0.0.16.dev20230508/GANDLF/cli/preprocess_and_save.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/cli/recover_config.py` & `GANDLF-0.0.16.dev20230508/GANDLF/cli/recover_config.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/compute/forward_pass.py` & `GANDLF-0.0.16.dev20230508/GANDLF/compute/forward_pass.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/compute/generic.py` & `GANDLF-0.0.16.dev20230508/GANDLF/compute/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/compute/inference_loop.py` & `GANDLF-0.0.16.dev20230508/GANDLF/compute/inference_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/compute/loss_and_metric.py` & `GANDLF-0.0.16.dev20230508/GANDLF/compute/loss_and_metric.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/compute/step.py` & `GANDLF-0.0.16.dev20230508/GANDLF/compute/step.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/compute/training_loop.py` & `GANDLF-0.0.16.dev20230508/GANDLF/compute/training_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/ImagesFromDataFrame.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/ImagesFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/__init__.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/augmentation/__init__.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/augmentation/blur_enhanced.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/augmentation/blur_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/augmentation/noise_enhanced.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/augmentation/noise_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/augmentation/rgb_augs.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/augmentation/rgb_augs.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/augmentation/rotations.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/augmentation/rotations.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/augmentation/wrap_torchio.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/augmentation/wrap_torchio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/inference_dataloader_histopath.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/inference_dataloader_histopath.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/patch_miner/opm/patch.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/patch_miner/opm/patch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/patch_miner/opm/patch_manager.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/patch_miner/opm/patch_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/patch_miner/opm/utils.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/patch_miner/opm/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/post_process/morphology.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/post_process/morphology.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/post_process/tensor.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/post_process/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/__init__.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/crop_zero_planes.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/crop_zero_planes.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/non_zero_normalize.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/non_zero_normalize.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/normalize_rgb.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/normalize_rgb.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/resample_minimum.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/resample_minimum.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/rgb_conversion.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/rgb_conversion.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/template_matching/base.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/template_matching/base.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/template_matching/histogram_matching.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/template_matching/histogram_matching.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/template_matching/stain_extractors.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/template_matching/stain_extractors.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/template_matching/stain_normalizer.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/template_matching/stain_normalizer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/template_matching/utils.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/template_matching/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/data/preprocessing/threshold_and_clip.py` & `GANDLF-0.0.16.dev20230508/GANDLF/data/preprocessing/threshold_and_clip.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/grad_clipping/adaptive_gradient_clipping.py` & `GANDLF-0.0.16.dev20230508/GANDLF/grad_clipping/adaptive_gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/grad_clipping/clip_gradients.py` & `GANDLF-0.0.16.dev20230508/GANDLF/grad_clipping/clip_gradients.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/grad_clipping/grad_scaler.py` & `GANDLF-0.0.16.dev20230508/GANDLF/grad_clipping/grad_scaler.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/inference_manager.py` & `GANDLF-0.0.16.dev20230508/GANDLF/inference_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/logger.py` & `GANDLF-0.0.16.dev20230508/GANDLF/logger.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/losses/__init__.py` & `GANDLF-0.0.16.dev20230508/GANDLF/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/losses/hybrid.py` & `GANDLF-0.0.16.dev20230508/GANDLF/losses/hybrid.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/losses/regression.py` & `GANDLF-0.0.16.dev20230508/GANDLF/losses/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/losses/segmentation.py` & `GANDLF-0.0.16.dev20230508/GANDLF/losses/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/metrics/__init__.py` & `GANDLF-0.0.16.dev20230508/GANDLF/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/metrics/classification.py` & `GANDLF-0.0.16.dev20230508/GANDLF/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/metrics/generic.py` & `GANDLF-0.0.16.dev20230508/GANDLF/metrics/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/metrics/regression.py` & `GANDLF-0.0.16.dev20230508/GANDLF/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/metrics/segmentation.py` & `GANDLF-0.0.16.dev20230508/GANDLF/metrics/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/MSDNet.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/MSDNet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/__init__.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/brain_age.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/brain_age.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/deep_unet.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/deep_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/densenet.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/densenet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/efficientnet.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/fcn.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/fcn.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/imagenet_unet.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/imagenet_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/imagenet_vgg.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/imagenet_vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/light_unet.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/light_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/light_unet_multilayer.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/light_unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/modelBase.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/modelBase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/resnet.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/resnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/sdnet.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/sdnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/DecodingModule.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/DecodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/DownsamplingModule.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/DownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/EncodingModule.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/EncodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/FCNUpsamplingModule.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/FCNUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/IncConv.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/IncConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/IncDownsamplingModule.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/IncDownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/IncDropout.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/IncDropout.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/IncUpsamplingModule.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/IncUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/InceptionModule.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/InceptionModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/InitialConv.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/InitialConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/Interpolate.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/Interpolate.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/ResNetModule.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/ResNetModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/UpsamplingModule.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/UpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/add_conv_block.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/add_conv_block.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/average_pool.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/average_pool.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/seg_modules/out_conv.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/seg_modules/out_conv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/transunet.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/transunet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/uinc.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/uinc.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/unet.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/unet_multilayer.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/unetr.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/unetr.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/models/vgg.py` & `GANDLF-0.0.16.dev20230508/GANDLF/models/vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/optimizers/__init__.py` & `GANDLF-0.0.16.dev20230508/GANDLF/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/optimizers/wrap_torch.py` & `GANDLF-0.0.16.dev20230508/GANDLF/optimizers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/parseConfig.py` & `GANDLF-0.0.16.dev20230508/GANDLF/parseConfig.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/schedulers/__init__.py` & `GANDLF-0.0.16.dev20230508/GANDLF/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/schedulers/wrap_torch.py` & `GANDLF-0.0.16.dev20230508/GANDLF/schedulers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/training_manager.py` & `GANDLF-0.0.16.dev20230508/GANDLF/training_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/utils/__init__.py` & `GANDLF-0.0.16.dev20230508/GANDLF/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/utils/generic.py` & `GANDLF-0.0.16.dev20230508/GANDLF/utils/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/utils/handle_collisions.py` & `GANDLF-0.0.16.dev20230508/GANDLF/utils/handle_collisions.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/utils/imaging.py` & `GANDLF-0.0.16.dev20230508/GANDLF/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/utils/modelbase.py` & `GANDLF-0.0.16.dev20230508/GANDLF/utils/modelbase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/utils/modelio.py` & `GANDLF-0.0.16.dev20230508/GANDLF/utils/modelio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/utils/parameter_processing.py` & `GANDLF-0.0.16.dev20230508/GANDLF/utils/parameter_processing.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/utils/tensor.py` & `GANDLF-0.0.16.dev20230508/GANDLF/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF/utils/write_parse.py` & `GANDLF-0.0.16.dev20230508/GANDLF/utils/write_parse.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF.egg-info/PKG-INFO` & `GANDLF-0.0.16.dev20230508/GANDLF.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.16.dev20230507
+Version: 0.0.16.dev20230508
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.16.dev20230507 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.16.dev20230508 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.16.dev20230507/GANDLF.egg-info/SOURCES.txt` & `GANDLF-0.0.16.dev20230508/GANDLF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/HISTORY.md` & `GANDLF-0.0.16.dev20230508/HISTORY.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/LICENSE` & `GANDLF-0.0.16.dev20230508/LICENSE`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/PKG-INFO` & `GANDLF-0.0.16.dev20230508/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.16.dev20230507
+Version: 0.0.16.dev20230508
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.16.dev20230507 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.16.dev20230508 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.16.dev20230507/README.md` & `GANDLF-0.0.16.dev20230508/README.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/SECURITY.md` & `GANDLF-0.0.16.dev20230508/SECURITY.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/gandlf_anonymizer` & `GANDLF-0.0.16.dev20230508/gandlf_anonymizer`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/gandlf_collectStats` & `GANDLF-0.0.16.dev20230508/gandlf_collectStats`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/gandlf_configGenerator` & `GANDLF-0.0.16.dev20230508/gandlf_configGenerator`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/gandlf_constructCSV` & `GANDLF-0.0.16.dev20230508/gandlf_constructCSV`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/gandlf_deploy` & `GANDLF-0.0.16.dev20230508/gandlf_deploy`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/gandlf_optimizeModel` & `GANDLF-0.0.16.dev20230508/gandlf_optimizeModel`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/gandlf_patchMiner` & `GANDLF-0.0.16.dev20230508/gandlf_patchMiner`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/gandlf_preprocess` & `GANDLF-0.0.16.dev20230508/gandlf_preprocess`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/gandlf_recoverConfig` & `GANDLF-0.0.16.dev20230508/gandlf_recoverConfig`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/gandlf_run` & `GANDLF-0.0.16.dev20230508/gandlf_run`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/gandlf_verifyInstall` & `GANDLF-0.0.16.dev20230508/gandlf_verifyInstall`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230507/setup.py` & `GANDLF-0.0.16.dev20230508/setup.py`

 * *Files identical despite different names*

