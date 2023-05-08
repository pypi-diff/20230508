# Comparing `tmp/hordelib-0.9.2.tar.gz` & `tmp/hordelib-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hordelib-0.9.2.tar", last modified: Mon Apr 17 22:29:42 2023, max compression
+gzip compressed data, was "hordelib-0.9.5.tar", last modified: Thu Apr 20 22:16:34 2023, max compression
```

## Comparing `hordelib-0.9.2.tar` & `hordelib-0.9.5.tar`

### file list

```diff
@@ -1,892 +1,892 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.016430 hordelib-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-17 22:29:24.000000 hordelib-0.9.2/.changelog
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-17 22:29:24.000000 hordelib-0.9.2/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.892428 hordelib-0.9.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.908428 hordelib-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-17 22:29:24.000000 hordelib-0.9.2/.github/workflows/maintests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-17 22:29:24.000000 hordelib-0.9.2/.github/workflows/prtests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-17 22:29:24.000000 hordelib-0.9.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-17 22:29:24.000000 hordelib-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    22583 2023-04-17 22:29:32.000000 hordelib-0.9.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-17 22:29:24.000000 hordelib-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-17 22:29:24.000000 hordelib-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    50204 2023-04-17 22:29:42.016430 hordelib-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-04-17 22:29:24.000000 hordelib-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-17 22:29:24.000000 hordelib-0.9.2/build_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.908428 hordelib-0.9.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-17 22:29:24.000000 hordelib-0.9.2/examples/run_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-17 22:29:24.000000 hordelib-0.9.2/examples/run_controlnet_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-17 22:29:24.000000 hordelib-0.9.2/examples/run_facefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-17 22:29:24.000000 hordelib-0.9.2/examples/run_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-17 22:29:24.000000 hordelib-0.9.2/examples/run_img2img_hires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-17 22:29:24.000000 hordelib-0.9.2/examples/run_img2img_inpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-17 22:29:24.000000 hordelib-0.9.2/examples/run_img2img_inpaint_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-17 22:29:24.000000 hordelib-0.9.2/examples/run_img2img_outpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-17 22:29:24.000000 hordelib-0.9.2/examples/run_inpainting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-17 22:29:24.000000 hordelib-0.9.2/examples/run_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-17 22:29:24.000000 hordelib-0.9.2/examples/run_stress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-17 22:29:24.000000 hordelib-0.9.2/examples/run_txt2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-17 22:29:24.000000 hordelib-0.9.2/examples/run_txt2img_hires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-17 22:29:24.000000 hordelib-0.9.2/examples/run_upscale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.912428 hordelib-0.9.2/hordelib/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.912428 hordelib-0.9.2/hordelib/_comfyui/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.916428 hordelib-0.9.2/hordelib/_comfyui/comfy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.916428 hordelib-0.9.2/hordelib/_comfyui/comfy/cldm/
--rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/cldm/cldm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/cli_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/clip_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/clip_vision_config_h.json
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/clip_vision_config_vitl.json
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/diffusers_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.916428 hordelib-0.9.2/hordelib/_comfyui/comfy/extra_samplers/
--rw-r--r--   0 runner    (1001) docker     (123)    38450 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.916428 hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/external.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/gns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.916428 hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/models/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    26723 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.916428 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.916428 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/data/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.916428 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/models/autoencoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.920428 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/models/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/models/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21367 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py
--rw-r--r--   0 runner    (1001) docker     (123)    89269 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.920428 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66501 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.920428 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/
--rw-r--r--   0 runner    (1001) docker     (123)    21572 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.920428 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37813 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31860 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.920428 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/ema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.920428 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.920428 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    22341 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.920428 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/
--rw-r--r--   0 runner    (1001) docker     (123)   441072 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png
--rw-r--r--   0 runner    (1001) docker     (123)    29024 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.924428 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.924428 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/tomesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/model_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    23539 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)    38722 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/sd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13673 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/sd1_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/sd1_clip_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.924428 hordelib-0.9.2/hordelib/_comfyui/comfy/sd1_tokenizer/
--rw-r--r--   0 runner    (1001) docker     (123)   524619 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/sd1_tokenizer/special_tokens_map.json
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json
--rw-r--r--   0 runner    (1001) docker     (123)  1059962 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/sd2_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/sd2_clip_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.924428 hordelib-0.9.2/hordelib/_comfyui/comfy/t2i_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/t2i_adapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.928429 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.928429 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.928429 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)    44849 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama
--rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat
--rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py
--rw-r--r--   0 runner    (1001) docker     (123)    52744 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py
--rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py
--rw-r--r--   0 runner    (1001) docker     (123)    51124 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py
--rw-r--r--   0 runner    (1001) docker     (123)    42740 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13485 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.932428 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/
--rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN
--rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    26761 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24279 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.932428 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/
--rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.932428 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/nodes_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/nodes_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   118577 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/comfyui_screenshot.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.932428 hordelib-0.9.2/hordelib/_comfyui/custom_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/custom_nodes/example_node.py.example
--rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/extra_model_paths.yaml.example
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/folder_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.932428 hordelib-0.9.2/hordelib/_comfyui/input/
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/input/example.png
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.896428 hordelib-0.9.2/hordelib/_comfyui/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.932428 hordelib-0.9.2/hordelib/_comfyui/models/checkpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/checkpoints/put_checkpoints_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.932428 hordelib-0.9.2/hordelib/_comfyui/models/clip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/clip/put_clip_or_text_encoder_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.932428 hordelib-0.9.2/hordelib/_comfyui/models/clip_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/clip_vision/put_clip_vision_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.936428 hordelib-0.9.2/hordelib/_comfyui/models/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/configs/anything_v3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/configs/v1-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/configs/v2-inference-v.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/configs/v2-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.936428 hordelib-0.9.2/hordelib/_comfyui/models/controlnet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/controlnet/put_controlnets_and_t2i_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.936428 hordelib-0.9.2/hordelib/_comfyui/models/diffusers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/diffusers/put_diffusers_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.936428 hordelib-0.9.2/hordelib/_comfyui/models/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/embeddings/put_embeddings_or_textual_inversion_concepts_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.936428 hordelib-0.9.2/hordelib/_comfyui/models/loras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/loras/put_loras_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.936428 hordelib-0.9.2/hordelib/_comfyui/models/style_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/style_models/put_t2i_style_model_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.936428 hordelib-0.9.2/hordelib/_comfyui/models/upscale_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/upscale_models/put_esrgan_and_other_upscale_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.936428 hordelib-0.9.2/hordelib/_comfyui/models/vae/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/models/vae/put_vae_here
--rw-r--r--   0 runner    (1001) docker     (123)    43898 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.936428 hordelib-0.9.2/hordelib/_comfyui/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/notebooks/comfyui_colab.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.936428 hordelib-0.9.2/hordelib/_comfyui/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/output/_output_images_will_be_put_here
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.936428 hordelib-0.9.2/hordelib/_comfyui/script_examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/script_examples/basic_api_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.936428 hordelib-0.9.2/hordelib/_comfyui/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.936428 hordelib-0.9.2/hordelib/_comfyui/web/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.940429 hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/colorPalette.js
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/keybinds.js
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/nodeTemplates.js
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/noteNode.js
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/rerouteNode.js
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/slotDefaults.js
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/snapToGrid.js
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/uploadImage.js
--rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/widgetInputs.js
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/extensions/logging.js.example
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/jsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.940429 hordelib-0.9.2/hordelib/_comfyui/web/lib/
--rw-r--r--   0 runner    (1001) docker     (123)   482237 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/lib/litegraph.core.js
--rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/lib/litegraph.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.940429 hordelib-0.9.2/hordelib/_comfyui/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/scripts/api.js
--rw-r--r--   0 runner    (1001) docker     (123)    31674 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/scripts/app.js
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/scripts/defaultGraph.js
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/scripts/pnginfo.js
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/scripts/ui.js
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/scripts/widgets.js
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.940429 hordelib-0.9.2/hordelib/_comfyui/web/types/
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/types/comfy.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)    52898 2023-04-17 22:29:34.000000 hordelib-0.9.2/hordelib/_comfyui/web/types/litegraph.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-17 22:29:41.000000 hordelib-0.9.2/hordelib/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.940429 hordelib-0.9.2/hordelib/blip/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/blip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/blip/caption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.940429 hordelib-0.9.2/hordelib/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/cache/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.940429 hordelib-0.9.2/hordelib/clip/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/clip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/clip/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/clip/coca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/clip/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/clip/interrogate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.944429 hordelib-0.9.2/hordelib/clip/ranking_lists/
--rw-r--r--   0 runner    (1001) docker     (123)    80572 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/clip/ranking_lists/artists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/clip/ranking_lists/flavors.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/clip/ranking_lists/mediums.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/clip/ranking_lists/movements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/clip/ranking_lists/sites.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22260 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/clip/ranking_lists/tags.txt
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/clip/ranking_lists/techniques.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/clip/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    17606 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/comfy_horde.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/config_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13522 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/horde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/initialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20247 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/install_comfy.patch
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/install_comfy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.944429 hordelib-0.9.2/hordelib/model_database/
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_database/aitemplate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_database/blip.json
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_database/clip.json
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_database/codeformer.json
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_database/controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)   218801 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_database/db.json
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_database/db_dep.json
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_database/db_embeds.json
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_database/diffusers.json
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_database/esrgan.json
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_database/gfpgan.json
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_database/med_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_database/safety_checker.json
--rw-r--r--   0 runner    (1001) docker     (123)   243306 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_database/stable_diffusion.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.948429 hordelib-0.9.2/hordelib/model_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31554 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_manager/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_manager/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_manager/codeformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_manager/compvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_manager/controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_manager/diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_manager/esrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_manager/gfpgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    14322 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_manager/hyper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_manager/safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/model_manager/torch_hijack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.948429 hordelib-0.9.2/hordelib/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.948429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.948429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/binary/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.948429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/canny/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/canny/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.948429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/color/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.948429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/hed/
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/install.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.948429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.952429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.952429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.952429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py
--rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.952429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.952429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.952429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.956429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.956429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.956429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.956429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.956429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.956429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.956429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.956429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.900428 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.956429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.956429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.960429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.964429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_160k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_20k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_40k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_80k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.900428 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.964429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.964429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.964429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.964429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.968429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/swish.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.968429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.968429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.968429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41996 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.968429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.972429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.972429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.976429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.980429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.980429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.984429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/closure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/iter_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.984429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.984429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.984429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.984429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.988429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.988429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.904428 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.988429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.988429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.988429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.988429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.988429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.988429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.992429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.992429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.992429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.992429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py
--rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.996429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.000429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.000429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.000429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.000429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.000429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.000429 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.000429 hordelib-0.9.2/hordelib/nodes/facerestore/
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.000429 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.000429 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/align_trans.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.004429 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/retinaface/
--rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.004429 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.004429 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.004429 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/autoanchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/extract_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.004429 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/parsing/bisenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/parsing/parsenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/parsing/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.004429 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/utils/face_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/facerestore/facelib/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/node_clip_similarities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/node_controlnet_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/node_image_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/node_image_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/node_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/nodes/node_upscale_model_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.008429 hordelib-0.9.2/hordelib/pipeline_designs/
--rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/pipeline_designs/pipeline_controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/pipeline_designs/pipeline_controlnet_annotator.json
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/pipeline_designs/pipeline_image_facefix.json
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/pipeline_designs/pipeline_image_upscale.json
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/pipeline_designs/pipeline_stable_diffusion.json
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.008429 hordelib-0.9.2/hordelib/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/pipelines/pipeline_controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/pipelines/pipeline_controlnet_annotator.json
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/pipelines/pipeline_image_facefix.json
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/pipelines/pipeline_image_upscale.json
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/pipelines/pipeline_stable_diffusion.json
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/pipelines/pipeline_stable_diffusion_paint.json
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/run_comfyui.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/shared_model_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.008429 hordelib-0.9.2/hordelib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.008429 hordelib-0.9.2/hordelib/utils/blip/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/utils/blip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/utils/blip/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)    41379 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/utils/blip/med.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/utils/blip/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/utils/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/utils/ioredirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-17 22:29:24.000000 hordelib-0.9.2/hordelib/utils/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:41.912428 hordelib-0.9.2/hordelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50204 2023-04-17 22:29:41.000000 hordelib-0.9.2/hordelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    49507 2023-04-17 22:29:41.000000 hordelib-0.9.2/hordelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 22:29:41.000000 hordelib-0.9.2/hordelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-17 22:29:41.000000 hordelib-0.9.2/hordelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 22:29:41.000000 hordelib-0.9.2/hordelib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.012429 hordelib-0.9.2/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71522 2023-04-17 22:29:24.000000 hordelib-0.9.2/images/test_annotator.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-04-17 22:29:24.000000 hordelib-0.9.2/images/test_db0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   538159 2023-04-17 22:29:24.000000 hordelib-0.9.2/images/test_facefix.png
--rw-r--r--   0 runner    (1001) docker     (123)  1474994 2023-04-17 22:29:24.000000 hordelib-0.9.2/images/test_inpaint.png
--rw-r--r--   0 runner    (1001) docker     (123)   411844 2023-04-17 22:29:24.000000 hordelib-0.9.2/images/test_inpaint_alpha.png
--rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-04-17 22:29:24.000000 hordelib-0.9.2/images/test_inpaint_mask.png
--rw-r--r--   0 runner    (1001) docker     (123)   407128 2023-04-17 22:29:24.000000 hordelib-0.9.2/images/test_inpaint_original.png
--rw-r--r--   0 runner    (1001) docker     (123)  1467500 2023-04-17 22:29:24.000000 hordelib-0.9.2/images/test_outpaint.png
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-17 22:29:34.000000 hordelib-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 22:29:24.000000 hordelib-0.9.2/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-17 22:29:34.000000 hordelib-0.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 22:29:42.016430 hordelib-0.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.016430 hordelib-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-17 22:29:24.000000 hordelib-0.9.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-17 22:29:24.000000 hordelib-0.9.2/tests/make_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:29:42.016430 hordelib-0.9.2/tests/model_managers/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-17 22:29:24.000000 hordelib-0.9.2/tests/model_managers/test_comvis.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-17 22:29:24.000000 hordelib-0.9.2/tests/model_managers/test_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-17 22:29:24.000000 hordelib-0.9.2/tests/model_managers/test_safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-17 22:29:24.000000 hordelib-0.9.2/tests/test_blip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-17 22:29:24.000000 hordelib-0.9.2/tests/test_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-04-17 22:29:24.000000 hordelib-0.9.2/tests/test_comfy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-17 22:29:24.000000 hordelib-0.9.2/tests/test_horde_controlnet_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-17 22:29:24.000000 hordelib-0.9.2/tests/test_horde_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-17 22:29:24.000000 hordelib-0.9.2/tests/test_horde_inference_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-04-17 22:29:24.000000 hordelib-0.9.2/tests/test_horde_inference_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-17 22:29:24.000000 hordelib-0.9.2/tests/test_horde_inference_painting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-17 22:29:24.000000 hordelib-0.9.2/tests/test_horde_pp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-17 22:29:24.000000 hordelib-0.9.2/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-17 22:29:24.000000 hordelib-0.9.2/tests/test_initialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-17 22:29:24.000000 hordelib-0.9.2/tests/test_safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-17 22:29:24.000000 hordelib-0.9.2/tests/test_shared_model_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-17 22:29:24.000000 hordelib-0.9.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-17 22:29:24.000000 hordelib-0.9.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.031641 hordelib-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-20 22:16:18.000000 hordelib-0.9.5/.changelog
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-20 22:16:18.000000 hordelib-0.9.5/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.911638 hordelib-0.9.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.927638 hordelib-0.9.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-20 22:16:18.000000 hordelib-0.9.5/.github/workflows/maintests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-20 22:16:18.000000 hordelib-0.9.5/.github/workflows/prtests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-20 22:16:18.000000 hordelib-0.9.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-20 22:16:18.000000 hordelib-0.9.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-04-20 22:16:23.000000 hordelib-0.9.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-20 22:16:18.000000 hordelib-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-20 22:16:18.000000 hordelib-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    50204 2023-04-20 22:16:34.031641 hordelib-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-04-20 22:16:18.000000 hordelib-0.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-20 22:16:18.000000 hordelib-0.9.5/build_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.927638 hordelib-0.9.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_controlnet_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_facefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_img2img_hires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_img2img_inpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_img2img_inpaint_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_img2img_outpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_inpainting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_stress_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_txt2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_txt2img_hires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_upscale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.927638 hordelib-0.9.5/hordelib/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.931638 hordelib-0.9.5/hordelib/_comfyui/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.931638 hordelib-0.9.5/hordelib/_comfyui/comfy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.931638 hordelib-0.9.5/hordelib/_comfyui/comfy/cldm/
+-rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/cldm/cldm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/cli_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/clip_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/clip_vision_config_h.json
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/clip_vision_config_vitl.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/diffusers_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.931638 hordelib-0.9.5/hordelib/_comfyui/comfy/extra_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)    38450 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.931638 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/gns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.935639 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26723 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.939638 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.939638 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/data/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.939638 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/autoencoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.939638 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21367 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89269 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.943639 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66501 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.943639 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    21572 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.943639 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37813 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31860 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.943639 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/ema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.943639 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.947639 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22341 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.947639 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)   441072 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29024 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.947639 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.947639 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/tomesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13187 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/model_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23539 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/sd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13673 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_clip_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.947639 hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (123)   524619 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_tokenizer/special_tokens_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1059962 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/sd2_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/sd2_clip_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.951639 hordelib-0.9.5/hordelib/_comfyui/comfy/t2i_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/t2i_adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.951639 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.951639 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.955639 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)    44849 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama
+-rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat
+-rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52744 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51124 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42740 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13485 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.955639 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/
+-rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26761 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24279 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.955639 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.955639 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/nodes_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/nodes_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118577 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfyui_screenshot.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.955639 hordelib-0.9.5/hordelib/_comfyui/custom_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/custom_nodes/example_node.py.example
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/extra_model_paths.yaml.example
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/folder_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.955639 hordelib-0.9.5/hordelib/_comfyui/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/input/example.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.915638 hordelib-0.9.5/hordelib/_comfyui/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.955639 hordelib-0.9.5/hordelib/_comfyui/models/checkpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/checkpoints/put_checkpoints_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.955639 hordelib-0.9.5/hordelib/_comfyui/models/clip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/clip/put_clip_or_text_encoder_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.955639 hordelib-0.9.5/hordelib/_comfyui/models/clip_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/clip_vision/put_clip_vision_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/models/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/anything_v3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/v1-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/v2-inference-v.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/v2-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/models/controlnet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/controlnet/put_controlnets_and_t2i_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/models/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/diffusers/put_diffusers_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/models/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/embeddings/put_embeddings_or_textual_inversion_concepts_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/models/loras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/loras/put_loras_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/models/style_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/style_models/put_t2i_style_model_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/models/upscale_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/upscale_models/put_esrgan_and_other_upscale_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/models/vae/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/vae/put_vae_here
+-rw-r--r--   0 runner    (1001) docker     (123)    43981 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/notebooks/comfyui_colab.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/output/_output_images_will_be_put_here
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/script_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/script_examples/basic_api_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/web/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/colorPalette.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/keybinds.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/nodeTemplates.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/noteNode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/rerouteNode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/slotDefaults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/snapToGrid.js
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/uploadImage.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/widgetInputs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/logging.js.example
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/jsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.963639 hordelib-0.9.5/hordelib/_comfyui/web/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)   482237 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/lib/litegraph.core.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/lib/litegraph.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.963639 hordelib-0.9.5/hordelib/_comfyui/web/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/scripts/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31674 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/scripts/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/scripts/defaultGraph.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/scripts/pnginfo.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/scripts/ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/scripts/widgets.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.963639 hordelib-0.9.5/hordelib/_comfyui/web/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/types/comfy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    52898 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/types/litegraph.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-20 22:16:33.000000 hordelib-0.9.5/hordelib/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.963639 hordelib-0.9.5/hordelib/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/blip/caption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.963639 hordelib-0.9.5/hordelib/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/cache/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.963639 hordelib-0.9.5/hordelib/clip/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/coca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/interrogate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.963639 hordelib-0.9.5/hordelib/clip/ranking_lists/
+-rw-r--r--   0 runner    (1001) docker     (123)    80572 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/ranking_lists/artists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/ranking_lists/flavors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/ranking_lists/mediums.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/ranking_lists/movements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/ranking_lists/sites.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22260 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/ranking_lists/tags.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/ranking_lists/techniques.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19562 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/comfy_horde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/config_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/horde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22045 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/install_comfy.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/install_comfy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.967639 hordelib-0.9.5/hordelib/model_database/
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/aitemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/blip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/clip.json
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/codeformer.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)   218801 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/db.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/db_dep.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/db_embeds.json
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/diffusers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/esrgan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/gfpgan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/med_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/safety_checker.json
+-rw-r--r--   0 runner    (1001) docker     (123)   243306 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/stable_diffusion.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.967639 hordelib-0.9.5/hordelib/model_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32017 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/codeformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/compvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/esrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/gfpgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14356 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/hyper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/safety_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.967639 hordelib-0.9.5/hordelib/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.971639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.971639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.971639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/canny/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/canny/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.971639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/color/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.971639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/hed/
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/install.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.971639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.971639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.971639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.971639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.971639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.919638 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.979640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.983640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.983640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_160k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_40k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_80k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.919638 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.983640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.983640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.983640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.983640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.987640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/swish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.987640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.987640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.987640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41996 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.987640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.991640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.991640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/deprecated.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.995640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.995640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.999640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.999640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/closure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/iter_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.999640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.003640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.003640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.003640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.003640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.003640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.923638 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.003640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.007640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.007640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.007640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.007640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.007640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.007640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.007640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.007640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.011640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.015641 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.015641 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.015641 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.015641 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.015641 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.015641 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.015641 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.019641 hordelib-0.9.5/hordelib/nodes/facerestore/
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.019641 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.019641 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/align_trans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.019641 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/retinaface/
+-rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.019641 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.019641 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.019641 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/autoanchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/extract_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.019641 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/parsing/bisenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/parsing/parsenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/parsing/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.019641 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/utils/face_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/node_clip_similarities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/node_controlnet_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/node_image_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/node_image_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/node_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/node_upscale_model_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.023641 hordelib-0.9.5/hordelib/pipeline_designs/
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipeline_designs/pipeline_controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipeline_designs/pipeline_controlnet_annotator.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipeline_designs/pipeline_image_facefix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipeline_designs/pipeline_image_upscale.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipeline_designs/pipeline_stable_diffusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.023641 hordelib-0.9.5/hordelib/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipelines/pipeline_controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipelines/pipeline_controlnet_annotator.json
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipelines/pipeline_image_facefix.json
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipelines/pipeline_image_upscale.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipelines/pipeline_stable_diffusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipelines/pipeline_stable_diffusion_paint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/run_comfyui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/shared_model_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.023641 hordelib-0.9.5/hordelib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.023641 hordelib-0.9.5/hordelib/utils/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/utils/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/utils/blip/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41378 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/utils/blip/med.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/utils/blip/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/utils/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/utils/ioredirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/utils/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.927638 hordelib-0.9.5/hordelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50204 2023-04-20 22:16:33.000000 hordelib-0.9.5/hordelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    49489 2023-04-20 22:16:33.000000 hordelib-0.9.5/hordelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 22:16:33.000000 hordelib-0.9.5/hordelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-20 22:16:33.000000 hordelib-0.9.5/hordelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-20 22:16:33.000000 hordelib-0.9.5/hordelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.027641 hordelib-0.9.5/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71522 2023-04-20 22:16:18.000000 hordelib-0.9.5/images/test_annotator.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-04-20 22:16:18.000000 hordelib-0.9.5/images/test_db0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   538159 2023-04-20 22:16:18.000000 hordelib-0.9.5/images/test_facefix.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1474994 2023-04-20 22:16:18.000000 hordelib-0.9.5/images/test_inpaint.png
+-rw-r--r--   0 runner    (1001) docker     (123)   411844 2023-04-20 22:16:18.000000 hordelib-0.9.5/images/test_inpaint_alpha.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-04-20 22:16:18.000000 hordelib-0.9.5/images/test_inpaint_mask.png
+-rw-r--r--   0 runner    (1001) docker     (123)   407128 2023-04-20 22:16:18.000000 hordelib-0.9.5/images/test_inpaint_original.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1467500 2023-04-20 22:16:18.000000 hordelib-0.9.5/images/test_outpaint.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-20 22:16:26.000000 hordelib-0.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-20 22:16:18.000000 hordelib-0.9.5/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-20 22:16:26.000000 hordelib-0.9.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 22:16:34.031641 hordelib-0.9.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.031641 hordelib-0.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/make_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.031641 hordelib-0.9.5/tests/model_managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/model_managers/test_comvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/model_managers/test_diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/model_managers/test_safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_comfy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_horde_controlnet_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_horde_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_horde_inference_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_horde_inference_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_horde_inference_painting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_horde_pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_shared_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-20 22:16:18.000000 hordelib-0.9.5/tox.ini
```

### Comparing `hordelib-0.9.2/.changelog` & `hordelib-0.9.5/.changelog`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/.github/workflows/maintests.yml` & `hordelib-0.9.5/.github/workflows/prtests.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,37 @@
-name: Tests
+name: Unstable Tests
 
 on:
-  push:
+  pull_request_target:
     branches:
       - main
+    types:
+      - opened
+      - synchronize
     paths:
       - '**.py'
       - '**.json'
+      - 'tox.ini'
+      - '.github/workflows/maintests.yml'
+      - '.github/workflows/prtests.yml'
+      - '.github/workflows/release.yml' 
 jobs:
   build:
 
     runs-on: self-hosted
     env:
       HORDELIB_TESTING: "no-cuda"
     strategy:
       matrix:
         python: ["3.10"]
 
     steps:
       - uses: actions/checkout@v3
+        with:
+          ref: ${{ github.event.pull_request.head.sha }}
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
       - name: Install tox and any other packages
         run: pip install --upgrade -r requirements.dev.txt
       - name: Run lint/format check
@@ -37,8 +46,8 @@
         uses: shallwefootball/s3-upload-action@master
         id: S3
         with:
           aws_key_id: ${{secrets.S3_BUILD_ARTIFACTS_ACCESS_KEY_ID}}
           aws_secret_access_key: ${{secrets.S3_BUILD_ARTIFACTS_SECRET_ACCESS_KEY}}
           aws_bucket: hordelib
           source_dir: images/
-          destination_dir: ''
+          destination_dir: 'unstable/'
```

### Comparing `hordelib-0.9.2/.github/workflows/release.yml` & `hordelib-0.9.5/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
       with:
         python-version: "3.10"
 
     # Install build deps
     - name: "🛠 Install pypa/build"
       if: ${{ steps.release.outputs.version != '' }}
       run: >-
-        python -m pip install build loguru --user
+        python -m pip install build typing-extensions loguru --user
 
     - name: "✏️ Install changelog dependencies"
       if: ${{ steps.release.outputs.version != '' }}
       uses: actions/setup-node@v3
 
     - name: "✏️ Generate release changelog"
       if: ${{ steps.release.outputs.version != '' }}
```

### Comparing `hordelib-0.9.2/.gitignore` & `hordelib-0.9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/CHANGELOG.md` & `hordelib-0.9.5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,32 @@
 ## hordelib Changelog
 
+## [v0.9.5](https://github.com/jug-dev/hordelib/compare/v0.9.4...v0.9.5)
+
+20 April 2023
+
+- build: fix missing dependency in pypi build [`01169be`](https://github.com/jug-dev/hordelib/commit/01169beb575c0a0577eebc00210ca98d14eeff42)  (Jug)
+
+## [v0.9.4](https://github.com/jug-dev/hordelib/compare/v0.9.3...v0.9.4)
+
+20 April 2023
+
+- fix: add missing dependency [`1dc5127`](https://github.com/jug-dev/hordelib/commit/1dc51270a15981aa6eb08aafe2ae8fba7a1e7d57)  (Jug)
+
+## [v0.9.3](https://github.com/jug-dev/hordelib/compare/v0.9.2...v0.9.3)
+
+20 April 2023
+
+- CI: trigger CI with certain other critical files [`#152`](https://github.com/jug-dev/hordelib/pull/152) (tazlin)
+- fix: stability fixes [`#150`](https://github.com/jug-dev/hordelib/pull/150) (Jug)
+- fix: Tox lint/style environments now build (more) correctly [`#151`](https://github.com/jug-dev/hordelib/pull/151) (tazlin)
+- Revert "Merge branch 'releases' into main" [`27987a0`](https://github.com/jug-dev/hordelib/commit/27987a0884b0ce48cad9d458c9fbdfa9b423b4a2)  (Jug)
+- refactor: Housekeeping, preparing for full lint ruleset in CI [`06155d2`](https://github.com/jug-dev/hordelib/commit/06155d26eb0b81ba704466adfefe34fd7347e42f)  (tazlin)
+- refactor: Control net model manager housekeeping [`37b6cac`](https://github.com/jug-dev/hordelib/commit/37b6cac2c1ebf79479996aecec1c4414d9c8b243)  (tazlin)
+
 ## [v0.9.2](https://github.com/jug-dev/hordelib/compare/v0.9.1...v0.9.2)
 
 17 April 2023
 
 - fix: don't mix up controlnets and run out of vram [`#147`](https://github.com/jug-dev/hordelib/pull/147) (Jug)
 
 ## [v0.9.1](https://github.com/jug-dev/hordelib/compare/v0.9.0...v0.9.1)
```

### Comparing `hordelib-0.9.2/LICENSE` & `hordelib-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/PKG-INFO` & `hordelib-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 0.9.2
+Version: 0.9.5
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
 Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hordelib-0.9.2/README.md` & `hordelib-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/build_helper.py` & `hordelib-0.9.5/build_helper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/examples/run_controlnet.py` & `hordelib-0.9.5/examples/run_controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/examples/run_controlnet_annotator.py` & `hordelib-0.9.5/examples/run_controlnet_annotator.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/examples/run_facefix.py` & `hordelib-0.9.5/examples/run_facefix.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/examples/run_img2img.py` & `hordelib-0.9.5/examples/run_img2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/examples/run_img2img_hires.py` & `hordelib-0.9.5/examples/run_img2img_hires.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/examples/run_img2img_inpaint.py` & `hordelib-0.9.5/examples/run_img2img_inpaint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/examples/run_img2img_inpaint_mask.py` & `hordelib-0.9.5/examples/run_img2img_inpaint_mask.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/examples/run_img2img_outpaint.py` & `hordelib-0.9.5/examples/run_img2img_outpaint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/examples/run_inpainting.py` & `hordelib-0.9.5/examples/run_inpainting.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/examples/run_memory_test.py` & `hordelib-0.9.5/examples/run_memory_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 def main():
     hordelib.initialise(setup_logging=False)
 
     from hordelib.horde import HordeLib
     from hordelib.shared_model_manager import SharedModelManager
 
-    generate = HordeLib()
+    HordeLib()
     SharedModelManager.loadModelManagers(compvis=True)
 
     load_and_free()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `hordelib-0.9.2/examples/run_stress_test.py` & `hordelib-0.9.5/examples/run_stress_test.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/examples/run_txt2img.py` & `hordelib-0.9.5/examples/run_txt2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/examples/run_txt2img_hires.py` & `hordelib-0.9.5/examples/run_txt2img_hires.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/examples/run_upscale.py` & `hordelib-0.9.5/examples/run_upscale.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/LICENSE` & `hordelib-0.9.5/hordelib/_comfyui/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/README.md` & `hordelib-0.9.5/hordelib/_comfyui/README.md`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/cldm/cldm.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/cldm/cldm.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/cli_args.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/cli_args.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/clip_vision.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/clip_vision.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/diffusers_convert.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/diffusers_convert.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/augmentation.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/augmentation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/config.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/evaluation.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/evaluation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/external.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/external.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/gns.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/gns.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/layers.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/layers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/sampling.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/sampling.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/k_diffusion/utils.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/data/util.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/data/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/models/autoencoder.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/attention.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/ema.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/ema.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/api.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/api.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/modules/tomesd.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/tomesd.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/ldm/util.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/model_management.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/model_management.py`

 * *Files 3% similar despite different names*

```diff
@@ -233,14 +233,29 @@
                 return
 
             device = get_torch_device()
             for m in models:
                 if m not in self.current_gpu_controlnets:
                     self.current_gpu_controlnets.append(m.to(device))
 
+    def unload_controlnet_gpu(self, models):        
+        global vram_state
+        with self._mutex:
+            if vram_state == VRAMState.CPU:
+                return
+
+            if vram_state == VRAMState.LOW_VRAM or vram_state == VRAMState.NO_VRAM:
+                #don't load controlnets like this if low vram because they will be loaded right before running and unloaded right after
+                return
+
+            for m in models:
+                if m in self.current_gpu_controlnets:
+                    m.cpu()
+                    self.current_gpu_controlnets.remove(m)
+                    del m
 
 model_manager = ModelManager()
 
 
 def load_if_low_vram(model):
     global vram_state
     if vram_state == VRAMState.LOW_VRAM or vram_state == VRAMState.NO_VRAM:
```

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/samplers.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/samplers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/sd.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/sd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import torch
 import contextlib
 import copy
+import threading
 
 import sd1_clip
 import sd2_clip
 from comfy import model_management
 from .ldm.util import instantiate_from_config
 from .ldm.models.autoencoder import AutoencoderKL
 import yaml
@@ -560,16 +561,25 @@
     def get_control_models(self):
         out = []
         if self.previous_controlnet is not None:
             out += self.previous_controlnet.get_control_models()
         out.append(self.control_model)
         return out
 
+_controlnet_models = {}
+_mutex = threading.Lock()
+
 def load_controlnet(ckpt_path, model=None):
-    controlnet_data = utils.load_torch_file(ckpt_path)
+    with _mutex:
+        if ckpt_path in _controlnet_models:
+            controlnet_data = copy.deepcopy(_controlnet_models.get(ckpt_path))
+        else:
+            controlnet_data = utils.load_torch_file(ckpt_path)
+            _controlnet_models[ckpt_path] = copy.deepcopy(controlnet_data)
+
     pth_key = 'control_model.input_blocks.1.1.transformer_blocks.0.attn2.to_k.weight'
     pth = False
     sd2 = False
     key = 'input_blocks.1.1.transformer_blocks.0.attn2.to_k.weight'
     if pth_key in controlnet_data:
         pth = True
         key = pth_key
```

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/sd1_clip.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/sd1_clip_config.json` & `hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_clip_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt` & `hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json` & `hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json` & `hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/sd2_clip.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/sd2_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/sd2_clip_config.json` & `hordelib-0.9.5/hordelib/_comfyui/comfy/sd2_clip_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/t2i_adapter/adapter.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/t2i_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy/utils.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/chainner_models/types.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/types.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/nodes_mask.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/nodes_mask.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/nodes_post_processing.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/nodes_post_processing.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py` & `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/comfyui_screenshot.png` & `hordelib-0.9.5/hordelib/_comfyui/comfyui_screenshot.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/custom_nodes/example_node.py.example` & `hordelib-0.9.5/hordelib/_comfyui/custom_nodes/example_node.py.example`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/execution.py` & `hordelib-0.9.5/hordelib/_comfyui/execution.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/extra_model_paths.yaml.example` & `hordelib-0.9.5/hordelib/_comfyui/extra_model_paths.yaml.example`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/folder_paths.py` & `hordelib-0.9.5/hordelib/_comfyui/folder_paths.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/input/example.png` & `hordelib-0.9.5/hordelib/_comfyui/input/example.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/main.py` & `hordelib-0.9.5/hordelib/_comfyui/main.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/models/configs/anything_v3.yaml` & `hordelib-0.9.5/hordelib/_comfyui/models/configs/anything_v3.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/models/configs/v1-inference.yaml` & `hordelib-0.9.5/hordelib/_comfyui/models/configs/v1-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml` & `hordelib-0.9.5/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml` & `hordelib-0.9.5/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml` & `hordelib-0.9.5/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml` & `hordelib-0.9.5/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/models/configs/v2-inference-v.yaml` & `hordelib-0.9.5/hordelib/_comfyui/models/configs/v2-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml` & `hordelib-0.9.5/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/models/configs/v2-inference.yaml` & `hordelib-0.9.5/hordelib/_comfyui/models/configs/v2-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml` & `hordelib-0.9.5/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml` & `hordelib-0.9.5/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/nodes.py` & `hordelib-0.9.5/hordelib/_comfyui/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -733,14 +733,15 @@
         sampler = comfy.samplers.KSampler(real_model, steps=steps, device=device, sampler=sampler_name, scheduler=scheduler, denoise=denoise, model_options=model.model_options)
     else:
         #other samplers
         pass
 
     samples = sampler.sample(noise, positive_copy, negative_copy, cfg=cfg, latent_image=latent_image, start_step=start_step, last_step=last_step, force_full_denoise=force_full_denoise, denoise_mask=noise_mask)
     samples = samples.cpu()
+    comfy.model_management.model_manager.unload_controlnet_gpu(control_net_models)
     for c in control_nets:
         c.cleanup()
 
     out = latent.copy()
     out["samples"] = samples
     comfy.model_management.model_manager.done_with_model(model)
     return (out, )
```

### Comparing `hordelib-0.9.2/hordelib/_comfyui/notebooks/comfyui_colab.ipynb` & `hordelib-0.9.5/hordelib/_comfyui/notebooks/comfyui_colab.ipynb`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/script_examples/basic_api_example.py` & `hordelib-0.9.5/hordelib/_comfyui/script_examples/basic_api_example.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/server.py` & `hordelib-0.9.5/hordelib/_comfyui/server.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/colorPalette.js` & `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/colorPalette.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js` & `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js` & `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js` & `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/keybinds.js` & `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/keybinds.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/nodeTemplates.js` & `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/nodeTemplates.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/noteNode.js` & `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/noteNode.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/rerouteNode.js` & `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/rerouteNode.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js` & `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/snapToGrid.js` & `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/snapToGrid.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/extensions/core/widgetInputs.js` & `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/widgetInputs.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/extensions/logging.js.example` & `hordelib-0.9.5/hordelib/_comfyui/web/extensions/logging.js.example`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/index.html` & `hordelib-0.9.5/hordelib/_comfyui/web/index.html`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/lib/litegraph.core.js` & `hordelib-0.9.5/hordelib/_comfyui/web/lib/litegraph.core.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/lib/litegraph.css` & `hordelib-0.9.5/hordelib/_comfyui/web/lib/litegraph.css`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/scripts/api.js` & `hordelib-0.9.5/hordelib/_comfyui/web/scripts/api.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/scripts/app.js` & `hordelib-0.9.5/hordelib/_comfyui/web/scripts/app.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/scripts/defaultGraph.js` & `hordelib-0.9.5/hordelib/_comfyui/web/scripts/defaultGraph.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/scripts/pnginfo.js` & `hordelib-0.9.5/hordelib/_comfyui/web/scripts/pnginfo.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/scripts/ui.js` & `hordelib-0.9.5/hordelib/_comfyui/web/scripts/ui.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/scripts/widgets.js` & `hordelib-0.9.5/hordelib/_comfyui/web/scripts/widgets.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/style.css` & `hordelib-0.9.5/hordelib/_comfyui/web/style.css`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/types/comfy.d.ts` & `hordelib-0.9.5/hordelib/_comfyui/web/types/comfy.d.ts`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/_comfyui/web/types/litegraph.d.ts` & `hordelib-0.9.5/hordelib/_comfyui/web/types/litegraph.d.ts`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/blip/caption.py` & `hordelib-0.9.5/hordelib/blip/caption.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/cache/cache.py` & `hordelib-0.9.5/hordelib/cache/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 import hashlib
+import importlib.resources as importlib_resources
 import os
 import sqlite3
 import sys
 from pathlib import Path
 
 from loguru import logger
 from PIL import Image
 from tqdm import tqdm
 
 from hordelib.settings import UserSettings
 
-if sys.version_info < (3, 9):  # XXX is <3.9 support going to be a thing?
-    import importlib_resources
-else:
-    import importlib.resources as importlib_resources
-
 
 def get_package():
     return importlib_resources.files("annotator")
     # XXX this predates me (@tazlin), doesn't look right
 
 
 def get_cache_directory():
```

### Comparing `hordelib-0.9.2/hordelib/clip/bulk.py` & `hordelib-0.9.5/hordelib/clip/bulk.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,10 +58,10 @@
         logger.info(f"Reading from {input_directory}")
         directory_list = self.cache_image.list_dir(input_directory)
         logger.info(f"Found {len(directory_list)} files. Filtering...")
         filtered_list = self.cache_image.filter_list(directory_list)
         logger.info(f"Found {len(filtered_list)} files to embed.")
         for image in tqdm(
             filtered_list,
-            disable=UserSettings.disable_progress.active,
+            disable=UserSettings.disable_download_progress.active,
         ):
             self.insert(image, input_directory)
```

### Comparing `hordelib-0.9.2/hordelib/clip/coca.py` & `hordelib-0.9.5/hordelib/clip/coca.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class CoCa:
     def __init__(self, model, transform, device="cuda", half_precision=True):
         self.model = model
         self.transform = transform
         self.device = device
         self.half_precision = half_precision
 
-    def __call__(self, input_image: Union[str, Image.Image]):
+    def __call__(self, input_image: str | Image.Image):
         if isinstance(input_image, str):
             if not os.path.exists(input_image):
                 raise ValueError(f"Image path {input_image} does not exist")
             try:
                 input_image = Image.open(input_image)
             except Exception as e:
                 raise ValueError(f"Could not open image {input_image}: {e}")
```

### Comparing `hordelib-0.9.2/hordelib/clip/image.py` & `hordelib-0.9.5/hordelib/clip/image.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/clip/interrogate.py` & `hordelib-0.9.5/hordelib/clip/interrogate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import hashlib
 import os
-from typing import Dict, List, Union
 
 import numpy as np
 import torch
 from loguru import logger
 from PIL import Image
 
 from hordelib.cache import Cache
@@ -32,15 +31,15 @@
             cache_subname="image",
         )
         self.embed_lists = {}
 
     def load(
         self,
         key: str,
-        text_array: List[str],
+        text_array: list[str],
         individual: bool = True,
         device: str = "cuda",
     ):
         """
         :param key: Key to use for embed_lists
         :param text_array: List of text to embed
         :param individual: Whether to store each text embed individually or as a concatenated tensor
@@ -193,22 +192,22 @@
         top = [
             {
                 "text": text_array[top_labels[0][i].numpy()],
                 "confidence": (top_probs[0][i].numpy() * 100),
             }
             for i in range(top_count)
         ]
-        return top  # noqa: RET504
+        return top
 
     def __call__(
         self,
-        image: Image.Image = None,
-        filename: str = None,
-        directory: str = None,
-        text_array: Union[List[str], Dict[str, List[str]], None] = None,
+        image: Image.Image | None = None,
+        filename: str | None = None,
+        directory: str | None = None,
+        text_array: list[str] | dict[str, list[str]] | None = None,
         similarity=False,
         rank=False,
         top_count=2,
     ):
         """
         :param input_image: PIL image
         :param text_array: List of text to compare to image, or dict of lists of text to compare to image
@@ -238,15 +237,15 @@
             text_array = {"default": text_array}
         elif isinstance(text_array, dict):
             pass
         image_embed = ImageEmbed(self.model_info, self.cache_image)
         image_hash = image_embed(image, filename, directory)
         image_embed_array = np.load(f"{self.cache_image.cache_dir}/{image_hash}.npy")
         image_features = torch.from_numpy(image_embed_array).float().to(self.model_info["device"])
-        if similarity and not rank:
+        if similarity and not rank:  # XXX # TODO: Refactor this
             results = {}
             for k in text_array:
                 results[k] = self.similarity(
                     image_features,
                     text_array[k],
                     k,
                     self.model_info["device"],
@@ -261,15 +260,15 @@
                     text_array[k],
                     k,
                     self.model_info["device"],
                     top_count,
                 )
                 logger.debug(f"{k}: {results[k]}")
             return results
-        else:  # noqa: RET505
+        else:
             similarity = {}
             for k in text_array:
                 similarity[k] = self.similarity(
                     image_features,
                     text_array[k],
                     k,
                     self.model_info["device"],
```

### Comparing `hordelib-0.9.2/hordelib/clip/ranking_lists/artists.txt` & `hordelib-0.9.5/hordelib/clip/ranking_lists/artists.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/clip/ranking_lists/flavors.txt` & `hordelib-0.9.5/hordelib/clip/ranking_lists/flavors.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/clip/ranking_lists/mediums.txt` & `hordelib-0.9.5/hordelib/clip/ranking_lists/mediums.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/clip/ranking_lists/movements.txt` & `hordelib-0.9.5/hordelib/clip/ranking_lists/movements.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/clip/ranking_lists/tags.txt` & `hordelib-0.9.5/hordelib/clip/ranking_lists/tags.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/clip/ranking_lists/techniques.txt` & `hordelib-0.9.5/hordelib/clip/ranking_lists/techniques.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/clip/text.py` & `hordelib-0.9.5/hordelib/clip/text.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/comfy_horde.py` & `hordelib-0.9.5/hordelib/comfy_horde.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import json
 import os
 import re
 import time
 import sys
 import typing
 import random
+import threading
 from pprint import pformat
 
 import torch
 from loguru import logger
 
 from hordelib.settings import UserSettings
 from hordelib.utils.ioredirect import OutputCollector
@@ -26,31 +27,74 @@
 # isort: off
 from execution import nodes as _comfy_nodes
 from execution import PromptExecutor as _comfy_PromptExecutor
 from folder_paths import folder_names_and_paths as _comfy_folder_paths
 from comfy.sd import load_checkpoint_guess_config as __comfy_load_checkpoint_guess_config
 from comfy.sd import load_controlnet as __comfy_load_controlnet
 from comfy.model_management import model_manager as _comfy_model_manager
+from comfy.model_management import get_torch_device as __comfy_get_torch_device
 from comfy.utils import load_torch_file as __comfy_load_torch_file
 from comfy_extras.chainner_models import model_loading as _comfy_model_loading
 
 # isort: on
 
+__models_to_release = {}
+_controlnet_mutex = threading.Lock()
+_facefix_mutex = threading.Lock()
+
+
+def cleanup():
+    with _comfy_model_manager.sampler_mutex:
+        # Do we have any models waiting to be released?
+        if not __models_to_release:
+            return
+
+        # Can we release any of them?
+        for model_name, model_data in __models_to_release.copy().items():
+            if is_model_in_use(model_data["model"]):
+                # We're in the middle of using it, nothing we can do
+                continue
+            # Unload the model from the GPU
+            unload_model_from_gpu(model_data["model"])
+            # Free ram
+            if "model" in model_data:
+                del model_data["model"]
+            if "clip" in model_data:
+                del model_data["clip"]
+            if "vae" in model_data:
+                del model_data["vae"]
+            if "clipVisionModel" in model_data:
+                del model_data["clipVisionModel"]
+            del model_data
+            del __models_to_release[model_name]
+            gc.collect()
+
+
+def remove_model_from_memory(model_name, model_data):
+    with _comfy_model_manager.sampler_mutex:
+        if model_name not in __models_to_release:
+            __models_to_release[model_name] = model_data
+
 
 def get_models_on_gpu():
     return _comfy_model_manager.get_models_on_gpu()
 
 
+def get_torch_device():
+    return __comfy_get_torch_device()
+
+
 def unload_model_from_gpu(model):
     _comfy_model_manager.unload_model(model)
     gc.collect()
-    if torch.cuda.is_available():
-        if torch.version.cuda:  # This seems to make things worse on ROCm so I only do it for cuda
-            torch.cuda.empty_cache()
-            torch.cuda.ipc_collect()
+    if not torch.cuda.is_available():
+        return None
+    if torch.version.cuda:
+        torch.cuda.empty_cache()
+        torch.cuda.ipc_collect()
 
 
 def is_model_in_use(model):
     return _comfy_model_manager.model_in_use(model)
 
 
 def load_torch_file(filename):
@@ -170,15 +214,18 @@
         return executor
 
     def _fix_pipeline_types(self, data: dict) -> dict:
         # We have a list of nodes and each node has a class type, which we may want to change
         for nodename, node in data.items():
             if ("class_type" in node) and (node["class_type"] in Comfy_Horde.NODE_REPLACEMENTS):
                 logger.debug(
-                    f"Changed type {data[nodename]['class_type']} to {Comfy_Horde.NODE_REPLACEMENTS[node['class_type']]}",
+                    (
+                        f"Changed type {data[nodename]['class_type']} to "
+                        f"{Comfy_Horde.NODE_REPLACEMENTS[node['class_type']]}"
+                    ),
                 )
                 data[nodename]["class_type"] = Comfy_Horde.NODE_REPLACEMENTS[node["class_type"]]
         # Now we've fixed up node types, check for any node input parameter rename needed
         for nodename, node in data.items():
             if ("class_type" in node) and (node["class_type"] in Comfy_Horde.NODE_PARAMETER_REPLACEMENTS):
                 for oldname, newname in Comfy_Horde.NODE_PARAMETER_REPLACEMENTS[node["class_type"]].items():
                     if "inputs" in node and oldname in node["inputs"]:
@@ -268,14 +315,15 @@
                         designdata = json.loads(designfile.read())
                     data = self._patch_pipeline(data, designdata)
                 self.pipelines[pipeline_name] = data
                 logger.debug(f"Loaded inference pipeline: {pipeline_name}")
                 return True
         except (OSError, ValueError):
             logger.error(f"Invalid inference pipeline file: {filename}")
+            return None
 
     def _load_pipelines(self) -> int:
         files = glob.glob(self._this_dir("pipeline_*.json", subdir="pipelines"))
         loaded_count = 0
         for file in files:
             if self._load_pipeline(file):
                 loaded_count += 1
@@ -365,15 +413,18 @@
         # XXX This probably shouldn't be here. But for the moment, it works.
         if "image_loader.image" in params:
             self.reconnect_input(pipeline, "sampler.latent_image", "vae_encode")
 
         # XXX This shouldn't be here either, but it's not clear to me yet where the
         # XXX correct place for dynamic connection of nodes is. Need to do a few more
         # XXX pipelines to see.
+        mutex = None
         if "control_type" in params:
+            # FIXME Only allow one controlnet job at a time
+            mutex = _controlnet_mutex
             # Inject control net model manager
             if "controlnet_model_loader.model_manager" not in params:
                 logger.debug("Injecting controlnet model manager")
                 params["controlnet_model_loader.model_manager"] = SharedModelManager
             # Connect to the correct pre-processor node
             if params.get("return_control_map", False):
                 # Connect annotator to output image directly
@@ -402,22 +453,33 @@
         # This is useful for dumping the entire pipeline to the terminal when
         # developing and debugging new pipelines. A badly structured pipeline
         # file just results in a cryptic error from comfy
         pretty_pipeline = pformat(pipeline)
         if False:  # This isn't here Tazlin :)
             logger.error(pretty_pipeline)
 
+        # Last minute mutex setup
+        if pipeline_name == "image_facefix":
+            mutex = _facefix_mutex
+
         # The client_id parameter here is just so we receive comfy callbacks for debugging.
         # We pretend we are a web client and want async callbacks.
         stdio = OutputCollector()
-        with contextlib.redirect_stdout(stdio):
-            with contextlib.redirect_stderr(stdio):
+        with contextlib.redirect_stdout(stdio), contextlib.redirect_stderr(stdio):
+            if mutex:
+                with mutex:
+                    inference.execute(pipeline, extra_data={"client_id": random.randint(0, sys.maxsize)})
+            else:
                 inference.execute(pipeline, extra_data={"client_id": random.randint(0, sys.maxsize)})
+
         stdio.replay()
 
+        # Check if there are any resource to clean up
+        cleanup()
+
         return inference.outputs
 
     # Run a pipeline that returns an image in pixel space
     def run_image_pipeline(self, pipeline_name: str, params: dict) -> list[dict] | None:
         # From the horde point of view, let us assume the output we are interested in
         # is always in a HordeImageOutput node named "output_image". This is an array of
         # dicts of the form:
```

### Comparing `hordelib-0.9.2/hordelib/config_path.py` & `hordelib-0.9.5/hordelib/config_path.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/consts.py` & `hordelib-0.9.5/hordelib/consts.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/horde.py` & `hordelib-0.9.5/hordelib/horde.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,15 +85,14 @@
         if cls._instance is None:
             cls._instance = super().__new__(cls)
         return cls._instance
 
     # We initialise only ever once (in the lifetime of the singleton)
     def __init__(self):
         if not self._initialised:
-            self.generator = Comfy_Horde()
             self.__class__._initialised = True
 
     def _parameter_remap(self, payload: dict[str, str | None]) -> dict[str, str | None]:
         params = {}
         # Extract from the payload things we understand
         for key, value in payload.items():
             newkey = HordeLib.BASIC_INFERENCE_PARAMS.get(key, None)
@@ -133,15 +132,18 @@
             params["prompt.text"] = promptsSplit[0]
             params["negative_prompt.text"] = ""
         elif len(promptsSplit) == 2:
             params["prompt.text"] = promptsSplit[0]
             params["negative_prompt.text"] = promptsSplit[1]
 
         # Sampler remap
-        sampler = HordeLib.SAMPLERS_MAP.get(params["sampler.sampler_name"], "euler")
+        sampler = HordeLib.SAMPLERS_MAP.get(params["sampler.sampler_name"], "unknown")
+        if sampler == "unknown":
+            logger.error(f"Unknown sampler {params['sampler.sampler_name']} defaulting to euler")
+            sampler = "euler"
         params["sampler.sampler_name"] = sampler
 
         # Clip skip inversion, comfy uses -1, -2, etc
         clip_skip_key = "clip_skip.stop_at_clip_layer"
         if params.get(clip_skip_key, 0) > 0:
             params[clip_skip_key] = -params[clip_skip_key]
 
@@ -170,17 +172,20 @@
                 # Finally mark that we are using hires fix
                 params["hires_fix"] = True
 
         # ControlNet?
         if cnet := payload.get("control_type"):
             # Determine the pre-processor that was requested
             pre_processor = HordeLib.CONTROLNET_IMAGE_PREPROCESSOR_MAP.get(cnet)
+            if not pre_processor:
+                logger.error("Unknown controlnet pre-processor type {cnet} defaulting to canny")
+                pre_processor = "canny"
 
             # The controlnet type becomes a direct parameter to the pipeline
-            # It is tranlated to its model as required my ComfyUI from the CN ModelManager
+            # It is translated to its model as required my ComfyUI from the CN ModelManager
             params["controlnet_model_loader.control_net_name"] = cnet
 
             # For the pre-processor we dynamically reroute nodes in the pipeline later
             params["control_type"] = pre_processor
 
             # Remove the source_processing settings in case they conflict later
             if "source_processing" in params:
@@ -231,18 +236,15 @@
         elif source_proc == "inpainting":
             pipeline = "stable_diffusion_paint"
         elif source_proc == "outpainting":
             pipeline = "stable_diffusion_paint"
 
         # ControlNet
         if params.get("control_type"):
-            if params.get("return_control_map", False):
-                pipeline = "controlnet_annotator"
-            else:
-                pipeline = "controlnet"
+            pipeline = "controlnet_annotator" if params.get("return_control_map", False) else "controlnet"
 
         return pipeline
 
     def _add_image_alpha_channel(self, source_image, alpha_image):
         # Convert images to RGBA mode
         source_image = source_image.convert("RGBA")
         # Convert alpha image to greyscale
@@ -297,36 +299,39 @@
         self._validate_BASIC_INFERENCE_PARAMS(payload)
         self._resize_sources_to_request(payload)
         # Determine our parameters
         params = self._parameter_remap_basic_inference(payload)
         # Determine the correct pipeline
         pipeline = self._get_appropriate_pipeline(params)
         # Run the pipeline
-        images = self.generator.run_image_pipeline(pipeline, params)
+        generator = Comfy_Horde()
+        images = generator.run_image_pipeline(pipeline, params)
         if images is None:
             return None  # XXX Log error and/or raise Exception here
         # XXX Assumes the horde only asks for and wants 1 image
         return Image.open(images[0]["imagedata"])
 
     def image_upscale(self, payload: dict[str, str | None]) -> Image.Image | None:
         # Determine our parameters
         params = self._parameter_remap(payload)
         # Determine the correct pipeline
         pipeline = "image_upscale"
         # Run the pipeline
-        images = self.generator.run_image_pipeline(pipeline, params)
+        generator = Comfy_Horde()
+        images = generator.run_image_pipeline(pipeline, params)
         if images is None:
             return None  # XXX Log error and/or raise Exception here
         # XXX Assumes the horde only asks for and wants 1 image
         return Image.open(images[0]["imagedata"])
 
     def image_facefix(self, payload: dict[str, str | None]) -> Image.Image | None:
         # Determine our parameters
         params = self._parameter_remap(payload)
         # Determine the correct pipeline
         pipeline = "image_facefix"
         # Run the pipeline
-        images = self.generator.run_image_pipeline(pipeline, params)
+        generator = Comfy_Horde()
+        images = generator.run_image_pipeline(pipeline, params)
         if images is None:
             return None  # XXX Log error and/or raise Exception here
         # XXX Assumes the horde only asks for and wants 1 image
         return Image.open(images[0]["imagedata"])
```

### Comparing `hordelib-0.9.2/hordelib/initialisation.py` & `hordelib-0.9.5/hordelib/initialisation.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 def initialise(
     model_managers_to_load: dict[MODEL_CATEGORY_NAMES, bool] = DEFAULT_MODEL_MANAGERS,
     setup_logging=True,
 ):
     # Setup logging if requested
     HordeLog.initialise(setup_logging)
 
-    logger.level("DEBUG")  # XXX # FIXME
-
     # If developer mode, don't permit some things
     if not RELEASE_VERSION and " " in get_hordelib_path():
         # Our runtime patching can't handle this
         raise Exception(
             "Do not run this project in developer mode from a path that " "contains spaces in directory names.",
         )
```

### Comparing `hordelib-0.9.2/hordelib/install_comfy.patch` & `hordelib-0.9.5/hordelib/install_comfy.patch`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ﻿diff --git a/comfy/model_management.py b/comfy/model_management.py
-index 76455e4..12eaa4c 100644
+index 76455e4..5f4daf8 100644
 --- a/comfy/model_management.py
 +++ b/comfy/model_management.py
 @@ -1,6 +1,8 @@
  import psutil
  from enum import Enum
  from cli_args import args
 +import threading
 +from loguru import logger
  
  class VRAMState(Enum):
      CPU = 0
-@@ -113,87 +115,130 @@ if args.cpu:
+@@ -113,87 +115,145 @@ if args.cpu:
  print(f"Set vram state to: {vram_state.name}")
  
  
 -current_loaded_model = None
 -current_gpu_controlnets = []
 -
 -model_accelerated = False
@@ -214,14 +214,29 @@
 +                return
 +
 +            device = get_torch_device()
 +            for m in models:
 +                if m not in self.current_gpu_controlnets:
 +                    self.current_gpu_controlnets.append(m.to(device))
 +
++    def unload_controlnet_gpu(self, models):        
++        global vram_state
++        with self._mutex:
++            if vram_state == VRAMState.CPU:
++                return
++
++            if vram_state == VRAMState.LOW_VRAM or vram_state == VRAMState.NO_VRAM:
++                #don't load controlnets like this if low vram because they will be loaded right before running and unloaded right after
++                return
++
++            for m in models:
++                if m in self.current_gpu_controlnets:
++                    m.cpu()
++                    self.current_gpu_controlnets.remove(m)
++                    del m
 +
 +model_manager = ModelManager()
  
  
  def load_if_low_vram(model):
 diff --git a/comfy/samplers.py b/comfy/samplers.py
 index ed36442..6b10249 100644
@@ -321,48 +336,75 @@
 +                    elif self.sampler == "dpm_adaptive":
 +                        samples = k_diffusion_sampling.sample_dpm_adaptive(self.model_k, noise, sigma_min, sigmas[0], extra_args=extra_args)
 +                    else:
 +                        samples = getattr(k_diffusion_sampling, "sample_{}".format(self.sampler))(self.model_k, noise, sigmas, extra_args=extra_args)
  
          return samples.to(torch.float32)
 diff --git a/comfy/sd.py b/comfy/sd.py
-index 9c632e2..3ec8e7a 100644
+index 9c632e2..5b82f11 100644
 --- a/comfy/sd.py
 +++ b/comfy/sd.py
-@@ -415,7 +415,6 @@ class VAE:
+@@ -1,6 +1,7 @@
+ import torch
+ import contextlib
+ import copy
++import threading
+ 
+ import sd1_clip
+ import sd2_clip
+@@ -415,7 +416,6 @@ class VAE:
          return output
  
      def decode(self, samples_in):
 -        model_management.unload_model()
          self.first_stage_model = self.first_stage_model.to(self.device)
          try:
              free_memory = model_management.get_free_memory(self.device)
-@@ -435,14 +434,12 @@ class VAE:
+@@ -435,14 +435,12 @@ class VAE:
          return pixel_samples
  
      def decode_tiled(self, samples, tile_x=64, tile_y=64, overlap = 16):
 -        model_management.unload_model()
          self.first_stage_model = self.first_stage_model.to(self.device)
          output = self.decode_tiled_(samples, tile_x, tile_y, overlap)
          self.first_stage_model = self.first_stage_model.cpu()
          return output.movedim(1,-1)
  
      def encode(self, pixel_samples):
 -        model_management.unload_model()
          self.first_stage_model = self.first_stage_model.to(self.device)
          pixel_samples = pixel_samples.movedim(-1,1).to(self.device)
          samples = self.first_stage_model.encode(2. * pixel_samples - 1.).sample() * self.scale_factor
-@@ -451,7 +448,6 @@ class VAE:
+@@ -451,7 +449,6 @@ class VAE:
          return samples
  
      def encode_tiled(self, pixel_samples, tile_x=512, tile_y=512, overlap = 64):
 -        model_management.unload_model()
          self.first_stage_model = self.first_stage_model.to(self.device)
          pixel_samples = pixel_samples.movedim(-1,1).to(self.device)
          samples = utils.tiled_scale(pixel_samples, lambda a: self.first_stage_model.encode(2. * a - 1.).sample() * self.scale_factor, tile_x, tile_y, overlap, upscale_amount = (1/8), out_channels=4)
+@@ -568,8 +565,17 @@ class ControlNet:
+         out.append(self.control_model)
+         return out
+ 
++_controlnet_models = {}
++_mutex = threading.Lock()
++
+ def load_controlnet(ckpt_path, model=None):
+-    controlnet_data = utils.load_torch_file(ckpt_path)
++    with _mutex:
++        if ckpt_path in _controlnet_models:
++            controlnet_data = copy.deepcopy(_controlnet_models.get(ckpt_path))
++        else:
++            controlnet_data = utils.load_torch_file(ckpt_path)
++            _controlnet_models[ckpt_path] = copy.deepcopy(controlnet_data)
++
+     pth_key = 'control_model.input_blocks.1.1.transformer_blocks.0.attn2.to_k.weight'
+     pth = False
+     sd2 = False
 diff --git a/execution.py b/execution.py
 index 73be6db..b637eb9 100644
 --- a/execution.py
 +++ b/execution.py
 @@ -7,6 +7,7 @@ import heapq
  import traceback
  import gc
@@ -416,15 +458,15 @@
  
      init_custom_nodes()
 +    load_custom_nodes(os.getenv("AIWORKER_CUSTOM_NODES"))
      server.add_routes()
      hijack_progress(server)
  
 diff --git a/nodes.py b/nodes.py
-index c775da0..75abed0 100644
+index c775da0..013db3d 100644
 --- a/nodes.py
 +++ b/nodes.py
 @@ -696,7 +696,8 @@ def common_ksampler(model, seed, steps, cfg, sampler_name, scheduler, positive,
          noise_mask = noise_mask.to(device)
  
      real_model = None
 -    comfy.model_management.load_model_gpu(model)
@@ -438,15 +480,21 @@
      for x in control_nets:
          control_net_models += x.get_control_models()
 -    comfy.model_management.load_controlnet_gpu(control_net_models)
 +    comfy.model_management.model_manager.load_controlnet_gpu(control_net_models)
  
      if sampler_name in comfy.samplers.KSampler.SAMPLERS:
          sampler = comfy.samplers.KSampler(real_model, steps=steps, device=device, sampler=sampler_name, scheduler=scheduler, denoise=denoise, model_options=model.model_options)
-@@ -741,6 +742,7 @@ def common_ksampler(model, seed, steps, cfg, sampler_name, scheduler, positive,
+@@ -736,11 +737,13 @@ def common_ksampler(model, seed, steps, cfg, sampler_name, scheduler, positive,
+ 
+     samples = sampler.sample(noise, positive_copy, negative_copy, cfg=cfg, latent_image=latent_image, start_step=start_step, last_step=last_step, force_full_denoise=force_full_denoise, denoise_mask=noise_mask)
+     samples = samples.cpu()
++    comfy.model_management.model_manager.unload_controlnet_gpu(control_net_models)
+     for c in control_nets:
+         c.cleanup()
  
      out = latent.copy()
      out["samples"] = samples
 +    comfy.model_management.model_manager.done_with_model(model)
      return (out, )
  
  class KSampler:
```

### Comparing `hordelib-0.9.2/hordelib/install_comfy.py` & `hordelib-0.9.5/hordelib/install_comfy.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             cwd=directory,
         )
 
     @classmethod
     def _run(cls, command, directory=get_hordelib_path()) -> tuple[bool, str] | None:
         # Don't if we're a release version
         if RELEASE_VERSION:
-            return
+            return None
         try:
             result = cls._run_get_result(command, directory)
         except Exception as Ex:
             logger.error(Ex)
             return None
         if result.returncode:
             logger.error(result.stderr)
```

### Comparing `hordelib-0.9.2/hordelib/model_database/aitemplate.json` & `hordelib-0.9.5/hordelib/model_database/aitemplate.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/model_database/blip.json` & `hordelib-0.9.5/hordelib/model_database/blip.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/model_database/clip.json` & `hordelib-0.9.5/hordelib/model_database/clip.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/model_database/controlnet.json` & `hordelib-0.9.5/hordelib/model_database/controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/model_database/db.json` & `hordelib-0.9.5/hordelib/model_database/db.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/model_database/db_dep.json` & `hordelib-0.9.5/hordelib/model_database/db_dep.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/model_database/db_embeds.json` & `hordelib-0.9.5/hordelib/model_database/db_embeds.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/model_database/diffusers.json` & `hordelib-0.9.5/hordelib/model_database/diffusers.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/model_database/esrgan.json` & `hordelib-0.9.5/hordelib/model_database/esrgan.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/model_database/gfpgan.json` & `hordelib-0.9.5/hordelib/model_database/gfpgan.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/model_database/safety_checker.json` & `hordelib-0.9.5/hordelib/model_database/safety_checker.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/model_database/stable_diffusion.json` & `hordelib-0.9.5/hordelib/model_database/stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/model_manager/base.py` & `hordelib-0.9.5/hordelib/model_manager/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import gc
 import hashlib
 import importlib.resources as importlib_resources
 import json
 import os
 import shutil
+import threading
 import time
 import typing
 import zipfile
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Any
 from uuid import uuid4
@@ -17,37 +18,54 @@
 import requests
 import torch
 from loguru import logger
 from tqdm import tqdm
 from transformers import logging
 
 from hordelib.cache import get_cache_directory
-from hordelib.comfy_horde import get_models_on_gpu, is_model_in_use, unload_model_from_gpu
+from hordelib.comfy_horde import get_models_on_gpu, remove_model_from_memory
+from hordelib.comfy_horde import get_torch_device as _get_torch_device
 from hordelib.config_path import get_hordelib_path
 from hordelib.consts import REMOTE_MODEL_DB
 from hordelib.settings import UserSettings
 
 logging.set_verbosity_error()
 
 
 class BaseModelManager(ABC):
     modelFolderPath: str  # XXX # TODO Convert to `Path`
     """The path to the directory to store this model type."""
     model_reference: dict  # XXX is this even wanted/used/useful?
     available_models: list[str]  # XXX rework as a property?
-    loaded_models: dict[str, dict]
+    _loaded_models: dict[str, dict]
     """The models available for immediate use."""
     tainted_models: list
     models_db_name: str
     models_db_path: Path
     cuda_available: bool
     cuda_devices: list
     recommended_gpu: list
     download_reference: bool
     remote_db: str
+    _mutex = threading.RLock()
+
+    def get_torch_device(self):
+        return _get_torch_device()
+
+    def get_loaded_models(self):
+        return self._loaded_models.copy()
+
+    def add_loaded_model(self, model_name, model_data):
+        with self._mutex:
+            self._loaded_models[model_name] = model_data
+
+    def remove_loaded_model(self, model_name):
+        with self._mutex:
+            if model_name in self._loaded_models:
+                del self._loaded_models[model_name]
 
     def __init__(
         self,
         *,
         models_db_name: str,  # XXX Remove default
         modelFolder: str | None = None,
         download_reference: bool = False,
@@ -64,15 +82,15 @@
                 f"{models_db_name}",
             )
         else:  # XXX # FIXME The only exception to this right now is compvis
             self.modelFolderPath = os.path.join(get_cache_directory(), f"{modelFolder}")
 
         self.model_reference = {}
         self.available_models = []
-        self.loaded_models = {}
+        self._loaded_models = {}
         self.tainted_models = []
         self.pkg = importlib_resources.files("hordelib")  # XXX Remove
         self.models_db_name = models_db_name
         self.models_db_path = Path(get_hordelib_path()).joinpath(
             "model_database/",
             f"{self.models_db_name}.json",
         )
@@ -82,15 +100,18 @@
         self.remote_db = f"{REMOTE_MODEL_DB}{self.models_db_name}.json"
         self.download_reference = download_reference
         self.loadModelDatabase()
 
     def loadModelDatabase(self, list_models=False):
         if self.model_reference:
             logger.info(
-                f"Model reference was already loaded. Got {len(self.model_reference)} models for {self.models_db_name}.",
+                (
+                    "Model reference was already loaded."
+                    f" Got {len(self.model_reference)} models for {self.models_db_name}."
+                ),
             )
             logger.info("Reloading model reference...")
 
         if self.download_reference:
             self.model_reference = self.download_model_reference()
             logger.info(
                 " ".join(
@@ -137,50 +158,53 @@
                 "Model Reference",
                 status=f"Download failed: {e}",
             )
             logger.init_warn("Model Reference", status="Local")
             return json.loads((self.models_db_path).read_text())
 
     def _modelref_to_name(self, modelref):
-        for name, data in self.loaded_models.items():
-            if modelref and data["model"] is modelref:
-                return name
-        return None
+        with self._mutex:
+            for name, data in self.get_loaded_models().items():
+                if modelref and data["model"] is modelref:
+                    return name
+            return None
 
     def ensure_memory_available(self):
         # Can this type of model be cached?
         if not self.can_cache_on_disk():
             return
-        # If we have less than the minimum RAM free, free some up
-        freemem = round(psutil.virtual_memory().available / (1024 * 1024))
-        logger.debug(f"Free RAM is: {freemem} MB, ({len(self.loaded_models)} models loaded in RAM)")
-        if freemem > UserSettings.ram_to_leave_free_mb + 4096:
-            return
-        logger.debug(f"Not enough free RAM attempting to free some")
-        # Grab a list of models (ModelPatcher) that are loaded on the gpu
-        # These are actually returned with the least important at the bottom of the list
-        busy_models = get_models_on_gpu()
-        # Try to find one we have in ram that isn't on the gpu
-        idle_model = None
-        for ram_model_name, ram_model_data in self.loaded_models.items():
-            if type(ram_model_data["model"]) is not str and ram_model_data["model"] not in busy_models:
-                idle_model = ram_model_name
-                break
-        # If we didn't have one hanging around in ram not on the gpu
-        # pick the least used gpu model
-        if not idle_model and busy_models:
-            idle_model = self._modelref_to_name(busy_models[-1])
-
-        if idle_model:
-            logger.debug(f"Moving model {idle_model} to disk to free up RAM")
-            self.move_to_disk_cache(idle_model)
-        else:
-            # Nothing else to release
-            logger.debug(f"Could not find a model to free RAM")
+        with self._mutex:
+            # If we have less than the minimum RAM free, free some up
+            freemem = round(psutil.virtual_memory().available / (1024 * 1024))
+            logger.debug(f"Free RAM is: {freemem} MB, ({len(self.get_loaded_models())} models loaded in RAM)")
+            if freemem > UserSettings.ram_to_leave_free_mb + 4096:
+                return
+            logger.debug("Not enough free RAM attempting to free some")
+            # Grab a list of models (ModelPatcher) that are loaded on the gpu
+            # These are actually returned with the least important at the bottom of the list
+            busy_models = get_models_on_gpu()
+            # Try to find one we have in ram that isn't on the gpu
+            idle_model = None
+            for ram_model_name, ram_model_data in self.get_loaded_models().items():
+                if type(ram_model_data["model"]) is not str and ram_model_data["model"] not in busy_models:
+                    idle_model = ram_model_name
+                    break
+            # If we didn't have one hanging around in ram not on the gpu
+            # pick the least used gpu model
+            if not idle_model and busy_models:
+                idle_model = self._modelref_to_name(busy_models[-1])
+
+            if idle_model:
+                logger.debug(f"Moving model {idle_model} to disk to free up RAM")
+                self.move_to_disk_cache(idle_model)
+            else:
+                # Nothing else to release
+                logger.debug("Could not find a model to free RAM")
 
+    # @abstractmethod # TODO
     def move_to_disk_cache(self, model_name):
         pass
 
     def can_cache_on_disk(self):
         """Can this of type model be cached on disk?"""
         return False
 
@@ -189,53 +213,57 @@
         model_name: str,
         *,
         half_precision: bool = True,
         gpu_id: int | None = 0,
         cpu_only: bool = False,
         **kwargs,
     ):  # XXX # FIXME
-        self.ensure_memory_available()
-        if model_name not in self.model_reference:
-            logger.error(f"{model_name} not found")
-            return False
-        if model_name not in self.available_models:
-            logger.error(f"{model_name} not available")
-            download_succeeded = self.download_model(model_name)
-            if not download_succeeded:
-                logger.init_err(f"{model_name} failed to download", status="Error")
-                return False
-            logger.init_ok(f"{model_name}", status="Downloaded")
-        if model_name not in self.loaded_models:
-            model_validated = self.validate_model(model_name)
-            if not model_validated:
+        with self._mutex:
+            self.ensure_memory_available()
+            if model_name not in self.model_reference:
+                logger.error(f"{model_name} not found")
                 return False
-            logger.init(f"{model_name}", status="Loading")
-
-            tic = time.time()
-            logger.init(f"{model_name}", status="Loading")
-
-            try:
-                self.loaded_models[model_name] = self.modelToRam(
-                    model_name=model_name,
-                    half_precision=half_precision,
-                    gpu_id=gpu_id,
-                    cpu_only=cpu_only,
-                    **kwargs,
-                )
-
-            except RuntimeError:
-                # It failed, it happens.
-                logger.error(f"Failed to load model {model_name}")
-                return None
+            if model_name not in self.available_models:
+                logger.error(f"{model_name} not available")
+                download_succeeded = self.download_model(model_name)
+                if not download_succeeded:
+                    logger.init_err(f"{model_name} failed to download", status="Error")
+                    return False
+                logger.init_ok(f"{model_name}", status="Downloaded")
+            if model_name not in self.get_loaded_models():
+                model_validated = self.validate_model(model_name)
+                if not model_validated:
+                    return False
+                logger.init(f"{model_name}", status="Loading")
 
-            toc = time.time()
+                tic = time.time()
+                logger.init(f"{model_name}", status="Loading")
 
-            logger.init_ok(f"{model_name}: {round(toc-tic,2)} seconds", status="Loaded")
-            return True
-        return None
+                try:
+                    self.add_loaded_model(
+                        model_name,
+                        self.modelToRam(
+                            model_name=model_name,
+                            half_precision=half_precision,
+                            gpu_id=gpu_id,
+                            cpu_only=cpu_only,
+                            **kwargs,
+                        ),
+                    )
+
+                except RuntimeError:
+                    # It failed, it happens.
+                    logger.error(f"Failed to load model {model_name}")
+                    return None
+
+                toc = time.time()
+
+                logger.init_ok(f"{model_name}: {round(toc-tic,2)} seconds", status="Loaded")
+                return True
+            return None
 
     def getFullModelPath(self, model_name: str):
         """Returns the fully qualified filename for the specified model."""
         ckpt_path = self.get_model_files(model_name)[0]["path"]  # XXX Rework?
         return f"{self.modelFolderPath}/{ckpt_path}"
 
     @abstractmethod
@@ -294,95 +322,73 @@
             ):
                 models_available.append(model)
         return models_available
 
     def count_available_models_by_types(self, model_types: list[str] | None = None):
         return len(self.get_available_models_by_types(model_types))
 
-    def get_loaded_models(self):
-        """
-        Returns the loaded models
-        """
-        return self.loaded_models[:]
-
     def get_loaded_model(self, model_name: str):
         """
         :param model_name: Name of the model
         Returns the loaded model
         """
-        return self.loaded_models[model_name]
+        return self.get_loaded_models()[model_name]
 
     def get_loaded_models_names(self, string=False) -> list[str] | str:  # XXX Rework 'string' param
         """Return a list of loaded model names.
 
         Args:
             string (bool, optional): Return as a comma separated string. Defaults to False.
 
         Returns:
             list[str] | str: The list of models, as a `list` or a comma separated string.
         """
         # return ["Deliberate"]
-        if string:
-            return ", ".join(self.loaded_models.keys())
-        return list(self.loaded_models.keys())
+        with self._mutex:
+            if string:
+                return ", ".join(self.get_loaded_models().keys())
+            return list(self.get_loaded_models().keys())
 
     def is_model_loaded(self, model_name: str) -> bool:
         """Returns True if the model is loaded, False otherwise.
 
         Args:
             model_name (str): The name of the model to check.
 
         Returns:
             _type_: _description_
         """
-        return model_name in self.loaded_models
-
-    def remove_model_from_ram(self, model_name):
-        if model_name not in self.loaded_models:
-            return
-        # Remove the model from ram. Just removing from the dictionary
-        # wasn't actually releasing the RAM
-        model = self.loaded_models[model_name]
-        del self.loaded_models[model_name]
-        if "model" in model:
-            del model["model"]
-        if "clip" in model:
-            del model["clip"]
-        if "vae" in model:
-            del model["vae"]
-        if "clipVisionModel" in model:
-            del model["clipVisionModel"]
-        del model
-        gc.collect()
+        with self._mutex:
+            return model_name in self.get_loaded_models()
 
     def unload_model(self, model_name: str):
         """
         :param model_name: Name of the model
-        Unloads a model. Completely remove it, free all resources, forget it exists.
-        """
-        if model_name in self.loaded_models:
-            if not is_model_in_use(self.loaded_models[model_name]["model"]):
-                # Unload it from the GPU if it has been loaded there
-                try:
-                    unload_model_from_gpu(self.loaded_models[model_name]["model"])
-                    # Free it's ram
-                    self.remove_model_from_ram(model_name)
-                    return True
-                except Exception as e:
-                    logger.warning(f"Failed to unload model {model_name}: {e}")
-                    return False
-        return None
+        Issue a request to unload a model, completely remove it, free all resources, forget it exists.
+        This may not be possible right now, as it may be being used, so we actually issue a request for it to
+        be unloaded at the earliest opportunity.
+        """
+        with self._mutex:
+            if model_name in self._loaded_models:
+                self.free_model_resources(model_name)
+                self.remove_loaded_model(model_name)
+                return True
+
+    def free_model_resources(self, model_name: str):
+        with self._mutex:
+            remove_model_from_memory(model_name, self.get_loaded_model(model_name))
 
     def unload_all_models(self):
         """
         Unloads all models
         """
-        for model in self.loaded_models:
-            self.unload_model(model)
-        return True
+        with self._mutex:
+            for model in self.get_loaded_models():
+                self.unload_model(model)
+            return True
 
     def taint_model(self, model_name: str):
         """Marks a model as not valid by removing it from available_models"""
         if model_name in self.available_models:
             self.available_models.remove(model_name)
             self.tainted_models.append(model_name)
```

### Comparing `hordelib-0.9.2/hordelib/model_manager/blip.py` & `hordelib-0.9.5/hordelib/model_manager/blip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/model_manager/clip.py` & `hordelib-0.9.5/hordelib/model_manager/clip.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,31 +131,31 @@
         if self.model_reference[model_name]["type"] == "open_clip":
             loaded_model_info = self.load_open_clip(
                 model_name,
                 half_precision,
                 gpu_id,
                 cpu_only,
             )
-            self.loaded_models[model_name] = loaded_model_info
+            self.add_loaded_model(model_name, loaded_model_info)
         elif self.model_reference[model_name]["type"] == "clip":
             loaded_model_info = self.load_clip(
                 model_name,
                 half_precision,
                 gpu_id,
                 cpu_only,
             )
-            self.loaded_models[model_name] = loaded_model_info
+            self.add_loaded_model(model_name, loaded_model_info)
         elif self.model_reference[model_name]["type"] == "coca":
             loaded_model_info = self.load_coca(
                 model_name,
                 half_precision,
                 gpu_id,
                 cpu_only,
             )
-            self.loaded_models[model_name] = loaded_model_info
+            self.add_loaded_models(model_name, loaded_model_info)
         else:
             logger.error(
                 f"Unknown model type: {self.model_reference[model_name]['type']}",
             )
             return {}  # XXX # FIXME
         if not loaded_model_info:
             logger.init_error(f"Failed to load {model_name}", status="Error")
@@ -167,10 +167,9 @@
             f"Loading {model_name}: Took {toc-tic} seconds",
             status="Success",
         )  # logger.init_ok
         return loaded_model_info
 
 
 def load_list(filename):
-    with open(filename, "r", encoding="utf-8", errors="replace") as f:
-        items = [line.strip() for line in f.readlines()]
-        return items
+    with open(filename, encoding="utf-8", errors="replace") as f:
+        return [line.strip() for line in f.readlines()]
```

### Comparing `hordelib-0.9.2/hordelib/model_manager/codeformer.py` & `hordelib-0.9.5/hordelib/model_manager/gfpgan.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-import time
 import typing
 
-from loguru import logger
 from typing_extensions import override
 
 from hordelib import comfy_horde
 from hordelib.consts import MODEL_CATEGORY_NAMES, MODEL_DB_NAMES
 from hordelib.model_manager.base import BaseModelManager
 
 
-class CodeFormerModelManager(BaseModelManager):
+class GfpganModelManager(BaseModelManager):
     def __init__(self, download_reference=False):
         super().__init__(
-            models_db_name=MODEL_DB_NAMES[MODEL_CATEGORY_NAMES.codeformer],
+            models_db_name=MODEL_DB_NAMES[MODEL_CATEGORY_NAMES.gfpgan],
             download_reference=download_reference,
         )
 
     @override
     def modelToRam(
         self,
         model_name: str,
```

### Comparing `hordelib-0.9.2/hordelib/model_manager/compvis.py` & `hordelib-0.9.5/hordelib/model_manager/compvis.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,21 +56,26 @@
             model_timestamp = os.path.getmtime(model_filename)
             cache_timestamp = os.path.getmtime(cache_file)
             if model_timestamp <= cache_timestamp:
                 return True
         return False
 
     def move_to_disk_cache(self, model_name):
-        cache_file = self.get_model_cache_filename(model_name)
-        # Serialise our objects
-        model_data = copy.copy(self.loaded_models[model_name])
-        components = ["model", "vae", "clip"]
-        if not self.have_model_cache(model_name):
-            with open(cache_file, "wb") as cache:
-                for component in components:
-                    pickle.dump(self.loaded_models[model_name][component], cache, protocol=pickle.HIGHEST_PROTOCOL)
-        for component in components:
-            model_data[component] = cache_file
-        # Remove from ram
-        self.remove_model_from_ram(model_name)
-        # Point the model to the cache
-        self.loaded_models[model_name] = model_data
+        with self._mutex:
+            cache_file = self.get_model_cache_filename(model_name)
+            # Serialise our objects
+            model_data = copy.copy(self.get_loaded_model(model_name))
+            components = ["model", "vae", "clip"]
+            if not self.have_model_cache(model_name):
+                with open(cache_file, "wb") as cache:
+                    for component in components:
+                        pickle.dump(
+                            self.get_loaded_model(model_name)[component],
+                            cache,
+                            protocol=pickle.HIGHEST_PROTOCOL,
+                        )
+            for component in components:
+                model_data[component] = cache_file
+            # Remove from vram/ram
+            self.free_model_resources(model_name)
+            # Point the model to the cache
+            self.add_loaded_model(model_name, model_data)
```

### Comparing `hordelib-0.9.2/hordelib/model_manager/diffusers.py` & `hordelib-0.9.5/hordelib/model_manager/diffusers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/model_manager/esrgan.py` & `hordelib-0.9.5/hordelib/model_manager/esrgan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing
 
-from typing_extensions import override  # noqa: I001
+from typing_extensions import override
 
 from hordelib import comfy_horde
 from hordelib.consts import MODEL_CATEGORY_NAMES, MODEL_DB_NAMES
 from hordelib.model_manager.base import BaseModelManager
 
 
 class EsrganModelManager(BaseModelManager):
```

### Comparing `hordelib-0.9.2/hordelib/model_manager/hyper.py` & `hordelib-0.9.5/hordelib/model_manager/hyper.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from hordelib.model_manager.esrgan import EsrganModelManager
 from hordelib.model_manager.gfpgan import GfpganModelManager
 from hordelib.model_manager.safety_checker import SafetyCheckerModelManager
 
 # from worker.util.voodoo import initialise_voodoo
 
 
-MODEL_MANAGERS_TYPE_LOOKUP: dict[MODEL_CATEGORY_NAMES, type] = {
+MODEL_MANAGERS_TYPE_LOOKUP: dict[MODEL_CATEGORY_NAMES, type[BaseModelManager]] = {
     # ModelCategoryNames.aitemplate: AITemplateModelManager,
     MODEL_CATEGORY_NAMES.blip: BlipModelManager,
     MODEL_CATEGORY_NAMES.clip: ClipModelManager,
     MODEL_CATEGORY_NAMES.codeformer: CodeFormerModelManager,
     MODEL_CATEGORY_NAMES.compvis: CompVisModelManager,
     MODEL_CATEGORY_NAMES.controlnet: ControlNetModelManager,
     MODEL_CATEGORY_NAMES.diffusers: DiffusersModelManager,
@@ -48,15 +48,15 @@
     gfpgan: GfpganModelManager | None = None
     safety_checker: SafetyCheckerModelManager | None = None
     # XXX I think this can be reworked into an array of BaseModelManager instances
 
     @property
     def models(self) -> dict:
         """All model manager's internal dictionaries of models, loaded from model database JSON files."""
-        _models = {}
+        _models: dict = {}
         for model_manager in self.active_model_managers:
             model_manager.model_reference
             _models.update(model_manager.model_reference)
         return _models
 
     @property
     def available_models(self) -> list[str]:
@@ -67,19 +67,19 @@
         return all_available_models
 
     @property
     def loaded_models(self) -> dict[str, dict]:
         """All models for which have successfully loaded across all `BaseModelManager` types."""
         all_loaded_models: dict[str, dict] = {}
         for model_manager in self.active_model_managers:
-            all_loaded_models.update(model_manager.loaded_models)
+            all_loaded_models.update(model_manager.get_loaded_models())
         return all_loaded_models
 
     @property
-    def active_model_managers(self) -> list[BaseModelManager] | None:
+    def active_model_managers(self) -> list[BaseModelManager]:
         """All loaded model managers."""
         all_model_managers = [
             # self.aitemplate, # XXX TODO
             self.blip,
             self.clip,
             self.compvis,
             self.diffusers,
@@ -124,17 +124,16 @@
         args_passed.pop("self")  # XXX This is temporary
 
         allModelMangerTypeKeys = MODEL_MANAGERS_TYPE_LOOKUP.keys()
         # e.g. `MODEL_MANAGERS_TYPE_LOOKUP["compvis"]`` returns type `CompVisModelManager`
 
         for argName, argValue in args_passed.items():
             if not (argName in allModelMangerTypeKeys and hasattr(self, argName)):
-                raise Exception(
-                    f"{argName} is not a valid model manager type!",
-                )  # XXX better guarantees need to be made
+                raise Exception(f"{argName} is not a valid model manager type!")
+                # XXX better guarantees need to be made
             if not argValue:
                 continue
             if getattr(self, argName) is not None:
                 continue
 
             modelmanager = MODEL_MANAGERS_TYPE_LOOKUP[argName]
 
@@ -288,24 +287,24 @@
         """Returns a list of all available models.
 
         Returns:
             list: All available models.
         """
         return self.available_models
 
-    def ensure_memory_available(self, specific_type=None):
+    def ensure_memory_available(self, specific_type: type[BaseModelManager] | None = None) -> None:
         """Asserts minimum amount of RAM is available. Unloads models if necessary."""
         for model_manager_type in MODEL_MANAGERS_TYPE_LOOKUP:
             if specific_type and specific_type != model_manager_type:
                 continue
             model_manager: BaseModelManager = getattr(self, model_manager_type)
             if model_manager is None:
                 continue
             model_manager.ensure_memory_available()
-        return None
+        return
 
     def load(
         self,
         model_name: str,
         half_precision: bool = True,
         gpu_id: int = 0,
         cpu_only: bool = False,
```

### Comparing `hordelib-0.9.2/hordelib/model_manager/safety_checker.py` & `hordelib-0.9.5/hordelib/model_manager/safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/README.md` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/README.md`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/install.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/install.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/comfy_controlnet_preprocessors/util.py` & `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/__init__.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import comfy.utils
 import numpy as np
 import cv2
 import math
 from facerestore.facelib.utils.face_restoration_helper import FaceRestoreHelper
 from facerestore.facelib.detection.retinaface import retinaface
 from torchvision.transforms.functional import normalize
+import threading
+from loguru import logger
 
 
 def img2tensor(imgs, bgr2rgb=True, float32=True):
     """Numpy array to tensor.
 
     Args:
         imgs (list[ndarray] | ndarray): Input images.
@@ -103,14 +105,15 @@
         result.append(img_np)
     if len(result) == 1:
         result = result[0]
     return result
 
 
 class FaceRestoreWithModel:
+    _mutex = threading.Lock()
     @classmethod
     def INPUT_TYPES(s):
         return {
             "required": {
                 "upscale_model": ("UPSCALE_MODEL",),
                 "image": ("IMAGE",),
                 "facedetection": (
@@ -126,91 +129,88 @@
 
     RETURN_TYPES = ("IMAGE",)
 
     FUNCTION = "restore_face"
 
     CATEGORY = "facerestore"
 
-    def __init__(self):
-        self.face_helper = None
-
     def restore_face(self, upscale_model, image, facedetection):
-        device = model_management.get_torch_device()
-        upscale_model.to(device)
-        if self.face_helper is None:
-            self.face_helper = FaceRestoreHelper(
+        with FaceRestoreWithModel._mutex:
+            device = model_management.get_torch_device()
+            upscale_model.to(device)
+            face_helper = FaceRestoreHelper(
                 1,
                 face_size=512,
                 crop_ratio=(1, 1),
                 det_model=facedetection,
                 save_ext="png",
                 use_parse=True,
                 device=device,
             )
 
-        image_np = 255.0 * image.cpu().numpy().squeeze()
+            image_np = 255.0 * image.cpu().numpy().squeeze()
 
-        image_np = image_np[:, :, ::-1]
+            image_np = image_np[:, :, ::-1]
 
-        original_resolution = image_np.shape[0:2]
+            original_resolution = image_np.shape[0:2]
 
-        if upscale_model is None or self.face_helper is None:
-            return image
+            if upscale_model is None or face_helper is None:
+                return image
 
-        self.face_helper.clean_all()
-        self.face_helper.read_image(image_np)
-        self.face_helper.get_face_landmarks_5(
-            only_center_face=False, resize=640, eye_dist_threshold=5
-        )
-        self.face_helper.align_warp_face()
-
-        restored_face = None
-        for idx, cropped_face in enumerate(self.face_helper.cropped_faces):
-            cropped_face_t = img2tensor(
-                cropped_face / 255.0, bgr2rgb=True, float32=True
+            face_helper.clean_all()
+            face_helper.read_image(image_np)
+            face_helper.get_face_landmarks_5(
+                only_center_face=False, resize=640, eye_dist_threshold=5
             )
-            normalize(cropped_face_t, (0.5, 0.5, 0.5), (0.5, 0.5, 0.5), inplace=True)
-            cropped_face_t = cropped_face_t.unsqueeze(0).to(device)
+            face_helper.align_warp_face()
 
-            try:
-                with torch.no_grad():
-                    # output = upscale_model(cropped_face_t, w=strength, adain=True)[0]
-                    output = upscale_model(cropped_face_t)[0]
-                    restored_face = tensor2img(output, rgb2bgr=True, min_max=(-1, 1))
-                del output
-                torch.cuda.empty_cache()
-            except Exception as error:
-                print(f"\tFailed inference for CodeFormer: {error}", file=sys.stderr)
-                restored_face = tensor2img(
-                    cropped_face_t, rgb2bgr=True, min_max=(-1, 1)
+            restored_face = None
+            for idx, cropped_face in enumerate(face_helper.cropped_faces):
+                cropped_face_t = img2tensor(
+                    cropped_face / 255.0, bgr2rgb=True, float32=True
                 )
+                normalize(cropped_face_t, (0.5, 0.5, 0.5), (0.5, 0.5, 0.5), inplace=True)
+                cropped_face_t = cropped_face_t.unsqueeze(0).to(device)
 
-            restored_face = restored_face.astype("uint8")
-            self.face_helper.add_restored_face(restored_face)
-
-        self.face_helper.get_inverse_affine(None)
-
-        restored_img = self.face_helper.paste_faces_to_input_image()
-        restored_img = restored_img[:, :, ::-1]
-
-        if original_resolution != restored_img.shape[0:2]:
-            restored_img = cv2.resize(
-                restored_img,
-                (0, 0),
-                fx=original_resolution[1] / restored_img.shape[1],
-                fy=original_resolution[0] / restored_img.shape[0],
-                interpolation=cv2.INTER_LINEAR,
-            )
+                try:
+                    with torch.no_grad():
+                        # output = upscale_model(cropped_face_t, w=strength, adain=True)[0]
+                        output = upscale_model(cropped_face_t)[0]
+                        restored_face = tensor2img(output, rgb2bgr=True, min_max=(-1, 1))
+                    del output
+                    # torch.cuda.empty_cache()
+                except Exception as error:
+                    logger.error(f"Failed inference for CodeFormer: {error}")
+                    restored_face = tensor2img(
+                        cropped_face_t, rgb2bgr=True, min_max=(-1, 1)
+                    )
+
+                restored_face = restored_face.astype("uint8")
+                face_helper.add_restored_face(restored_face)
+
+            face_helper.get_inverse_affine(None)
+
+            restored_img = face_helper.paste_faces_to_input_image()
+            restored_img = restored_img[:, :, ::-1]
+
+            if original_resolution != restored_img.shape[0:2]:
+                restored_img = cv2.resize(
+                    restored_img,
+                    (0, 0),
+                    fx=original_resolution[1] / restored_img.shape[1],
+                    fy=original_resolution[0] / restored_img.shape[0],
+                    interpolation=cv2.INTER_LINEAR,
+                )
 
-        self.face_helper.clean_all()
+            face_helper.clean_all()
 
-        # restored_img = cv2.cvtColor(restored_face, cv2.COLOR_BGR2RGB)
+            # restored_img = cv2.cvtColor(restored_face, cv2.COLOR_BGR2RGB)
 
-        restored_img_np = np.array(restored_img).astype(np.float32) / 255.0
-        restored_img_tensor = torch.from_numpy(restored_img_np).unsqueeze(0)
+            restored_img_np = np.array(restored_img).astype(np.float32) / 255.0
+            restored_img_tensor = torch.from_numpy(restored_img_np).unsqueeze(0)
 
-        return (restored_img_tensor,)
+            return (restored_img_tensor,)
 
 
 NODE_CLASS_MAPPINGS = {
     "FaceRestoreWithModel": FaceRestoreWithModel,
 }
```

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/__init__.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/align_trans.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/align_trans.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/parsing/__init__.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/parsing/bisenet.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/parsing/bisenet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/parsing/parsenet.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/parsing/parsenet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/parsing/resnet.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/parsing/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/utils/face_utils.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/utils/face_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/facerestore/facelib/utils/misc.py` & `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/node_clip_similarities.py` & `hordelib-0.9.5/hordelib/nodes/node_clip_similarities.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/node_controlnet_model_loader.py` & `hordelib-0.9.5/hordelib/nodes/node_controlnet_model_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
         with HordeDiffControlNetLoader._mutex:
             merged_model = model_manager.manager.controlnet.merge_controlnet(
                 control_net_name,
                 model,
             )
 
-            return merged_model  # noqa: RET504
+            return merged_model
 
 
 NODE_CLASS_MAPPINGS = {"HordeDiffControlNetLoader": HordeDiffControlNetLoader}
 
 logger.debug("Loaded HordeDiffControlNetLoader")
```

### Comparing `hordelib-0.9.2/hordelib/nodes/node_image_loader.py` & `hordelib-0.9.5/hordelib/nodes/node_image_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/node_image_output.py` & `hordelib-0.9.5/hordelib/nodes/node_image_output.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/nodes/node_model_loader.py` & `hordelib-0.9.5/hordelib/nodes/node_model_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # node_model_loader.py
 # Simple proof of concept custom node to load models.
 
+import contextlib
 import os
 import pickle
 
 from loguru import logger
 
 
 class HordeCheckpointLoader:
@@ -29,37 +30,37 @@
     ):
         logger.debug(f"Loading model {model_name} through our custom node")
 
         if model_manager.manager is None:
             logger.error("horde_model_manager appears to be missing!")
             raise RuntimeError  # XXX better guarantees need to be made
 
-        if model_name not in model_manager.manager.loaded_models:
+        loaded_models = model_manager.manager.loaded_models
+        if model_name not in loaded_models:
             logger.error(f"Model {model_name} is not loaded")
             raise RuntimeError  # XXX better guarantees need to be made
 
-        model = model_manager.manager.loaded_models[model_name]["model"]
-        clip = model_manager.manager.loaded_models[model_name]["clip"]
-        vae = model_manager.manager.loaded_models[model_name]["vae"]
+        model = loaded_models[model_name]["model"]
+        clip = loaded_models[model_name]["clip"]
+        vae = loaded_models[model_name]["vae"]
 
         # If we got strings, not objects, it's a cache reference, load the cache
         if type(model) is str:
             logger.info("Loading model data from disk cache")
             model_cache = model
             try:
                 with open(model, "rb") as cache:
                     model = pickle.load(cache)
                     vae = pickle.load(cache)
                     clip = pickle.load(cache)
             except (pickle.PickleError, EOFError):
                 # Most likely corrupt cache file, remove the file
-                try:
-                    os.remove(model)
-                except OSError:
-                    pass  # we tried
+                with contextlib.suppress(OSError):
+                    os.remove(model)  # ... at least try to remove it
+
                 raise Exception(f"Model cache file {model_cache} was corrupt. It has been removed.")
 
         # XXX # TODO I would like to revisit this dict->tuple conversion at some point soon
         return (model, clip, vae)
 
 
 NODE_CLASS_MAPPINGS = {"HordeCheckpointLoader": HordeCheckpointLoader}
```

### Comparing `hordelib-0.9.2/hordelib/nodes/node_upscale_model_loader.py` & `hordelib-0.9.5/hordelib/nodes/node_upscale_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/pipeline_designs/pipeline_controlnet.json` & `hordelib-0.9.5/hordelib/pipeline_designs/pipeline_controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/pipeline_designs/pipeline_controlnet_annotator.json` & `hordelib-0.9.5/hordelib/pipeline_designs/pipeline_controlnet_annotator.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/pipeline_designs/pipeline_image_facefix.json` & `hordelib-0.9.5/hordelib/pipeline_designs/pipeline_image_facefix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/pipeline_designs/pipeline_image_upscale.json` & `hordelib-0.9.5/hordelib/pipeline_designs/pipeline_image_upscale.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/pipeline_designs/pipeline_stable_diffusion.json` & `hordelib-0.9.5/hordelib/pipeline_designs/pipeline_stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json` & `hordelib-0.9.5/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json` & `hordelib-0.9.5/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/pipelines/pipeline_controlnet.json` & `hordelib-0.9.5/hordelib/pipelines/pipeline_controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/pipelines/pipeline_controlnet_annotator.json` & `hordelib-0.9.5/hordelib/pipelines/pipeline_controlnet_annotator.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/pipelines/pipeline_image_facefix.json` & `hordelib-0.9.5/hordelib/pipelines/pipeline_image_facefix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/pipelines/pipeline_image_upscale.json` & `hordelib-0.9.5/hordelib/pipelines/pipeline_image_upscale.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/pipelines/pipeline_stable_diffusion.json` & `hordelib-0.9.5/hordelib/pipelines/pipeline_stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json` & `hordelib-0.9.5/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/pipelines/pipeline_stable_diffusion_paint.json` & `hordelib-0.9.5/hordelib/pipelines/pipeline_stable_diffusion_paint.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/run_comfyui.py` & `hordelib-0.9.5/hordelib/run_comfyui.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/safety_checker.py` & `hordelib-0.9.5/hordelib/safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/shared_model_manager.py` & `hordelib-0.9.5/hordelib/shared_model_manager.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/utils/blip/blip.py` & `hordelib-0.9.5/hordelib/utils/blip/blip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/utils/blip/med.py` & `hordelib-0.9.5/hordelib/utils/blip/med.py`

 * *Files 0% similar despite different names*

```diff
@@ -540,15 +540,15 @@
 
     config_class = BertConfig
     base_model_prefix = "bert"
     _keys_to_ignore_on_load_missing = [r"position_ids"]
 
     def _init_weights(self, module):
         """Initialize the weights"""
-        if isinstance(module, (nn.Linear, nn.Embedding)):
+        if isinstance(module, nn.Linear | nn.Embedding):
             # Slightly different from the TF version which uses truncated_normal for initialization
             # cf https://github.com/pytorch/pytorch/pull/5617
             module.weight.data.normal_(mean=0.0, std=self.config.initializer_range)
         elif isinstance(module, nn.LayerNorm):
             module.bias.data.zero_()
             module.weight.data.fill_(1.0)
         if isinstance(module, nn.Linear) and module.bias is not None:
@@ -590,15 +590,15 @@
         """
         for layer, heads in heads_to_prune.items():
             self.encoder.layer[layer].attention.prune_heads(heads)
 
     def get_extended_attention_mask(
         self,
         attention_mask: Tensor,
-        input_shape: Tuple[int],
+        input_shape: tuple[int],
         device: device,
         is_decoder: bool,
     ) -> Tensor:
         """
         Makes broadcastable attention and causal masks so that future and masked tokens are ignored.
 
         Arguments:
```

### Comparing `hordelib-0.9.2/hordelib/utils/blip/vit.py` & `hordelib-0.9.5/hordelib/utils/blip/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/utils/cast.py` & `hordelib-0.9.5/hordelib/utils/cast.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/hordelib/utils/ioredirect.py` & `hordelib-0.9.5/hordelib/utils/ioredirect.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import io
 from collections import deque
 
 from loguru import logger
 
 
-class OutputCollector:
+class OutputCollector(io.TextIOWrapper):
     def __init__(self):
         logger.disable("tqdm")  # just.. no
         self.deque = deque()
 
     def write(self, s):
         if s != "\n":
             self.deque.append(s.strip())
```

### Comparing `hordelib-0.9.2/hordelib/utils/logger.py` & `hordelib-0.9.5/hordelib/utils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import sys
 from functools import partialmethod
 
 from loguru import logger
 
 
 class HordeLog:
@@ -159,19 +160,18 @@
         logger.__class__.message = partialmethod(logger.__class__.log, "MESSAGE")
         logger.__class__.stats = partialmethod(logger.__class__.log, "STATS")
 
     @classmethod
     def set_sinks(cls):
         # Remove any existing sinks that we added
         for sink in cls.sinks:
-            try:
+            with contextlib.suppress(ValueError):
+                # Suppress if someone else beat us to it
                 logger.remove(sink)
-            except ValueError:
-                # Someone else beat us to it
-                pass
+
         cls.sinks = []
 
         config = {
             "handlers": [
                 {
                     "sink": sys.stderr,
                     "format": cls.logfmt,
```

### Comparing `hordelib-0.9.2/hordelib.egg-info/PKG-INFO` & `hordelib-0.9.5/hordelib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 0.9.2
+Version: 0.9.5
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
 Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hordelib-0.9.2/hordelib.egg-info/SOURCES.txt` & `hordelib-0.9.5/hordelib.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 pyproject.toml
 requirements.dev.txt
 requirements.txt
 tox.ini
 .github/workflows/maintests.yml
 .github/workflows/prtests.yml
 .github/workflows/release.yml
+examples/run_clip.py
 examples/run_controlnet.py
 examples/run_controlnet_annotator.py
 examples/run_facefix.py
 examples/run_img2img.py
 examples/run_img2img_hires.py
 examples/run_img2img_inpaint.py
 examples/run_img2img_inpaint_mask.py
@@ -266,15 +267,14 @@
 hordelib/model_manager/compvis.py
 hordelib/model_manager/controlnet.py
 hordelib/model_manager/diffusers.py
 hordelib/model_manager/esrgan.py
 hordelib/model_manager/gfpgan.py
 hordelib/model_manager/hyper.py
 hordelib/model_manager/safety_checker.py
-hordelib/model_manager/torch_hijack.py
 hordelib/nodes/__init__.py
 hordelib/nodes/node_clip_similarities.py
 hordelib/nodes/node_controlnet_model_loader.py
 hordelib/nodes/node_image_loader.py
 hordelib/nodes/node_image_output.py
 hordelib/nodes/node_model_loader.py
 hordelib/nodes/node_upscale_model_loader.py
```

### Comparing `hordelib-0.9.2/images/test_annotator.jpg` & `hordelib-0.9.5/images/test_annotator.jpg`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/images/test_db0.jpg` & `hordelib-0.9.5/images/test_db0.jpg`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/images/test_facefix.png` & `hordelib-0.9.5/images/test_facefix.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/images/test_inpaint.png` & `hordelib-0.9.5/images/test_inpaint.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/images/test_inpaint_alpha.png` & `hordelib-0.9.5/images/test_inpaint_alpha.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/images/test_inpaint_mask.png` & `hordelib-0.9.5/images/test_inpaint_mask.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/images/test_inpaint_original.png` & `hordelib-0.9.5/images/test_inpaint_original.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/images/test_outpaint.png` & `hordelib-0.9.5/images/test_outpaint.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/pyproject.toml` & `hordelib-0.9.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -64,17 +64,18 @@
 [tool.black]
 line-length = 119
 # Exclude ComfyUI and any packages we have installed in nodes/
 exclude = '''
 /(
     ComfyUI
   | \.tox
-  | nodes[\\/].*
+  | comfy_controlnet_preprocessors
+  | facerestore
 )/
-'''
+''' # If you change this, you probably need to also change [tool.mypy] below
 
 [tool.ruff] # XXX this isn't part of CI yet
 line-length=119
 exclude=["comfy_controlnet_preprocessors", "facerestore"]
 ignore=[
     "F401", # imported but unused
     "E402", # Module level import not at top of file
@@ -98,17 +99,30 @@
     "C4",   # flake8-comprehensions
     # "G",    # flake8-logging-format
     "INP",  # flake8-no-pep420
     "PIE",  # flake8-pie
     # "T20",  # flake8-print
     # "UP",   # pyupgrade
     "RSE",  # flake8-raise
-    "RET",  # flake8-return
+    # "RET",  # flake8-return
     # "SLF",  # flake8-self
     # "SIM",  # flake8-simplify
     # "ARG",  # flake8-unused-arguments
     # "TRY",  # tryceratops
     "RUF100"
 ]
 
 [tool.ruff.per-file-ignores]
-"comfy_horde.py" = ["I001", "F401"]
+"comfy_horde.py" = ["I001", "F401"] # I001 is isort, F401 is imported but unused
+"make_index.py" = ["E501"] # E501 is line too long
+"med.py" = ["E501", "UP035"]
+"vit.py" = ["E501", "UP035", "F821"] # F821 looks like a real bug, suppressed only for dev CI purposes
+"run_stress_test.py" = ["F841"]
+
+
+[tool.mypy]
+exclude = '''(?x)(
+    ComfyUI
+  | \.tox
+  | comfy_controlnet_preprocessors
+  | facerestore
+)''' # If you change this, you probably need to also change [tool.black] above
```

### Comparing `hordelib-0.9.2/requirements.txt` & `hordelib-0.9.5/requirements.txt`

 * *Files 20% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 pillow
 loguru
 GitPython
 clip-anytorch
 diffusers
 omegaconf
 psutil
+typing-extensions
 # face fixer custom nodes
 opencv-python
 # controlnet custom nodes
 opencv-contrib-python
 opencv-python
 timm==0.6.12
 torchvision
```

### Comparing `hordelib-0.9.2/tests/make_index.py` & `hordelib-0.9.5/tests/make_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,13 +94,13 @@
     indexhtml = indexhtml.replace("[input_images]", "".join(in_refs))
     indexhtml = indexhtml.replace(
         "[timestamp]",
         datetime.datetime.utcnow().strftime("%Y-%m-%d %H:%M:%S"),
     )
 
     # Output results
-    with open("images/index.html", "wt") as outfile:
+    with open("images/index.html", "w") as outfile:
         outfile.write(indexhtml)
 
 
 if __name__ == "__main__":
     create_index()
```

### Comparing `hordelib-0.9.2/tests/model_managers/test_comvis.py` & `hordelib-0.9.5/tests/model_managers/test_comvis.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/tests/model_managers/test_diffusers.py` & `hordelib-0.9.5/tests/model_managers/test_diffusers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/tests/model_managers/test_safety_checker.py` & `hordelib-0.9.5/tests/model_managers/test_safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/tests/test_blip.py` & `hordelib-0.9.5/tests/test_blip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/tests/test_clip.py` & `hordelib-0.9.5/tests/test_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/tests/test_comfy.py` & `hordelib-0.9.5/tests/test_comfy.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/tests/test_horde_controlnet_annotator.py` & `hordelib-0.9.5/tests/test_horde_controlnet_annotator.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/tests/test_horde_inference.py` & `hordelib-0.9.5/tests/test_horde_inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/tests/test_horde_inference_controlnet.py` & `hordelib-0.9.5/tests/test_horde_inference_controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/tests/test_horde_inference_img2img.py` & `hordelib-0.9.5/tests/test_horde_inference_img2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/tests/test_horde_inference_painting.py` & `hordelib-0.9.5/tests/test_horde_inference_painting.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/tests/test_horde_pp.py` & `hordelib-0.9.5/tests/test_horde_pp.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/tests/test_inference.py` & `hordelib-0.9.5/tests/test_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,17 @@
             "sampler.steps": 20,
             "prompt.text": (
                 "photograph of medusa, reverence princesss, cinematic, realistic, "
                 "hyperrealistic, very realistic, extremely detailed, detailed, sharp focus, "
                 "establishing shot, 8k resolution, dramatic lighting, award winning "
                 "photograph, masterpiece, very detailed, sharp focus, very realistic lighting"
             ),
-            "negative_prompt.text": "render, cg, drawing, painting, artist, graphics, deformed, black and white, deformed eyes",
+            "negative_prompt.text": (
+                "render, cg, drawing, painting, artist, graphics, deformed, black and white, deformed eyes"
+            ),
             "model_loader.model_name": "Deliberate",
             "empty_latent_image.width": 256,
             "empty_latent_image.height": 256,
             "latent_upscale.width": 512,
             "latent_upscale.height": 512,
             "latent_upscale.crop": "disabled",
             "latent_upscale.upscale_method": "nearest-exact",
@@ -114,15 +116,17 @@
             "sampler.steps": 20,
             "prompt.text": (
                 "photograph of medusa, reverence princesss, cinematic, realistic, "
                 "hyperrealistic, very realistic, extremely detailed, detailed, sharp focus, "
                 "establishing shot, 8k resolution, dramatic lighting, award winning "
                 "photograph, masterpiece, very detailed, sharp focus, very realistic lighting"
             ),
-            "negative_prompt.text": "render, cg, drawing, painting, artist, graphics, deformed, black and white, deformed eyes",
+            "negative_prompt.text": (
+                "render, cg, drawing, painting, artist, graphics, deformed, black and white, deformed eyes"
+            ),
             "model_loader.model_name": "Deliberate",
             "empty_latent_image.width": 256,
             "empty_latent_image.height": 256,
             "latent_upscale.width": 512,
             "latent_upscale.height": 512,
             "latent_upscale.crop": "disabled",
             "latent_upscale.upscale_method": "nearest-exact",
```

### Comparing `hordelib-0.9.2/tests/test_safety_checker.py` & `hordelib-0.9.5/tests/test_safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.2/tests/test_shared_model_manager.py` & `hordelib-0.9.5/tests/test_shared_model_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,15 @@
         for model_manager in SharedModelManager.manager.active_model_managers:
             for model in model_manager.available_models:
                 model_file_details = model_manager.get_model_files(model)
                 for file in model_file_details:
                     path = file.get("path")
                     if not (".pt" in path or ".ckpt" in path or ".safetensors" in path):
                         continue
-                    hash = model_manager.get_file_sha256_hash(f"{model_manager.modelFolderPath}/{path}")
-                    # print(f"{path}: {hash}")
+                    model_manager.get_file_sha256_hash(f"{model_manager.modelFolderPath}/{path}")
         pass
 
     def test_check_validate_all_available_models(self):
         assert SharedModelManager.manager is not None
         for model_manager in SharedModelManager.manager.active_model_managers:
             for model in model_manager.available_models:
                 assert model_manager.validate_model(model)
```

### Comparing `hordelib-0.9.2/tox.ini` & `hordelib-0.9.5/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -34,51 +34,73 @@
     pytest-sugar
     pytest-cov
     requests
     -r requirements.txt
 
 [testenv:format]
 description = check formatting rules
+skip_install = true
+install_command = pip install
 deps =
     black==22.3.0
-skip_install = true
 commands = black --check .
 
 [testenv:lint]
-description = check linting rules
+description = check all linting rules
+skip_install = true
+install_command = pip install
 deps =
     ruff==0.0.261
-skip_install = true
 commands = ruff .
 
+[testenv:lint-fix]
+description = fix all linting rules
+skip_install = true
+install_command = pip install
+deps =
+    ruff==0.0.261
+    black==22.3.0
+commands = 
+    black .
+    ruff --fix .
+    black .
+    ruff --fix .
+
 [testenv:lint-weak-check]
 description = check only certain few linting rules
+skip_install = true
+install_command = pip install
 deps =
     ruff==0.0.261
-skip_install = true
-commands = ruff --select COM,I .
+commands = 
+    ruff --select COM,I .    
+    python -c "print('*'*80 + '\n' + 'DEPRECATED: Favor using `tox -e lint` for checking for linting issues.\n' + '*'*80)"
 
 [testenv:lint-weak-fix]
 description = fixes only certain few linting rules
+skip_install = true
+install_command = pip install
 deps =
     black==22.3.0
     ruff==0.0.261
-skip_install = true
 commands = 
     black .
     ruff --fix --select COM,I .
     black .
     ruff --fix --select COM,I .
+    python -c "print('*'*80 + '\n' + 'DEPRECATED: Favor using `tox -e lint-fix` for fixing linting issues.\n' + '*'*80)"
     
 [testenv:comfyui]
 description = run comfyui
 skip_install = true
 commands =
     {envpython} -m hordelib.run_comfyui
 
 [testenv:tests]
 description = install pytest in a virtual environment and invoke it on the tests folder
+skip_install = false
+install_command = pip install {opts} {packages}
 passenv =
     HORDELIB_TESTING
     AIWORKER_CACHE_HOME
 commands =
     pytest tests {posargs} --cov
```

