# Comparing `tmp/vit-pytorch-1.2.0.tar.gz` & `tmp/vit-pytorch-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vit-pytorch-1.2.0.tar", last modified: Sat Mar 18 16:42:16 2023, max compression
+gzip compressed data, was "vit-pytorch-1.2.1.tar", last modified: Mon May  8 16:34:53 2023, max compression
```

## Comparing `vit-pytorch-1.2.0.tar` & `vit-pytorch-1.2.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 16:42:16.298650 vit-pytorch-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-03-18 16:42:16.298650 vit-pytorch-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    60828 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-18 16:42:16.298650 vit-pytorch-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 16:42:16.294650 vit-pytorch-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 16:42:16.298650 vit-pytorch-1.2.0/vit_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/ats_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/cait.py
--rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/cct.py
--rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/cct_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/cross_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/crossformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/cvt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/deepvit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/dino.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/distill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/efficient.py
--rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/es_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/learnable_memory_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/levit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/local_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/mae.py
--rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/max_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/mobile_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/mp3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/mpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/nest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/parallel_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/pit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/regionvit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/rvt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/scalable_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/sep_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/simmim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/simple_flash_attn_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/simple_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/simple_vit_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/simple_vit_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/simple_vit_with_patch_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/t2t.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/twins_svt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/vit_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/vit_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/vit_for_small_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/vit_with_patch_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/vit_with_patch_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-03-18 16:41:59.000000 vit-pytorch-1.2.0/vit_pytorch/vivit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 16:42:16.298650 vit-pytorch-1.2.0/vit_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-03-18 16:42:16.000000 vit-pytorch-1.2.0/vit_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-18 16:42:16.000000 vit-pytorch-1.2.0/vit_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 16:42:16.000000 vit-pytorch-1.2.0/vit_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-18 16:42:16.000000 vit-pytorch-1.2.0/vit_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-18 16:42:16.000000 vit-pytorch-1.2.0/vit_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:34:53.164325 vit-pytorch-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-08 16:34:53.164325 vit-pytorch-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    60828 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:34:53.164325 vit-pytorch-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:34:53.160325 vit-pytorch-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:34:53.164325 vit-pytorch-1.2.1/vit_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/ats_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/cait.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/cct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/cct_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/cross_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/crossformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/cvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/deepvit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/dino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/distill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/efficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/es_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/learnable_memory_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/levit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/local_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/mae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/max_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/mobile_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/mp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/mpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/nest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/parallel_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/pit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/regionvit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/rvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/scalable_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/sep_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/simmim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/simple_flash_attn_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/simple_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/simple_vit_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/simple_vit_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/simple_vit_with_patch_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/t2t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/twins_svt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/vit_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/vit_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/vit_for_small_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/vit_with_patch_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/vit_with_patch_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-05-08 16:34:39.000000 vit-pytorch-1.2.1/vit_pytorch/vivit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:34:53.164325 vit-pytorch-1.2.1/vit_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-08 16:34:53.000000 vit-pytorch-1.2.1/vit_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-08 16:34:53.000000 vit-pytorch-1.2.1/vit_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:34:53.000000 vit-pytorch-1.2.1/vit_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:34:53.000000 vit-pytorch-1.2.1/vit_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 16:34:53.000000 vit-pytorch-1.2.1/vit_pytorch.egg-info/top_level.txt
```

### Comparing `vit-pytorch-1.2.0/LICENSE` & `vit-pytorch-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/PKG-INFO` & `vit-pytorch-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-pytorch
-Version: 1.2.0
+Version: 1.2.1
 Summary: Vision Transformer (ViT) - Pytorch
 Home-page: https://github.com/lucidrains/vit-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vit-pytorch-1.2.0/README.md` & `vit-pytorch-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/setup.py` & `vit-pytorch-1.2.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vit-pytorch',
   packages = find_packages(exclude=['examples']),
-  version = '1.2.0',
+  version = '1.2.1',
   license='MIT',
   description = 'Vision Transformer (ViT) - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vit-pytorch',
   keywords = [
     'artificial intelligence',
     'attention mechanism',
     'image recognition'
   ],
   install_requires=[
-    'einops>=0.6.0',
+    'einops>=0.6.1',
     'torch>=1.10',
     'torchvision'
   ],
   setup_requires=[
     'pytest-runner',
   ],
   tests_require=[
```

### Comparing `vit-pytorch-1.2.0/vit_pytorch/ats_vit.py` & `vit-pytorch-1.2.1/vit_pytorch/ats_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/cait.py` & `vit-pytorch-1.2.1/vit_pytorch/cait.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/cct.py` & `vit-pytorch-1.2.1/vit_pytorch/cct.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/cct_3d.py` & `vit-pytorch-1.2.1/vit_pytorch/cct_3d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/cross_vit.py` & `vit-pytorch-1.2.1/vit_pytorch/cross_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/crossformer.py` & `vit-pytorch-1.2.1/vit_pytorch/crossformer.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/cvt.py` & `vit-pytorch-1.2.1/vit_pytorch/cvt.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/deepvit.py` & `vit-pytorch-1.2.1/vit_pytorch/deepvit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/dino.py` & `vit-pytorch-1.2.1/vit_pytorch/dino.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/distill.py` & `vit-pytorch-1.2.1/vit_pytorch/distill.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/efficient.py` & `vit-pytorch-1.2.1/vit_pytorch/efficient.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/es_vit.py` & `vit-pytorch-1.2.1/vit_pytorch/es_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/extractor.py` & `vit-pytorch-1.2.1/vit_pytorch/extractor.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/learnable_memory_vit.py` & `vit-pytorch-1.2.1/vit_pytorch/learnable_memory_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/levit.py` & `vit-pytorch-1.2.1/vit_pytorch/levit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/local_vit.py` & `vit-pytorch-1.2.1/vit_pytorch/local_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/mae.py` & `vit-pytorch-1.2.1/vit_pytorch/mae.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/max_vit.py` & `vit-pytorch-1.2.1/vit_pytorch/max_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/mobile_vit.py` & `vit-pytorch-1.2.1/vit_pytorch/mobile_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/mp3.py` & `vit-pytorch-1.2.1/vit_pytorch/mp3.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/mpp.py` & `vit-pytorch-1.2.1/vit_pytorch/mpp.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/nest.py` & `vit-pytorch-1.2.1/vit_pytorch/nest.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/parallel_vit.py` & `vit-pytorch-1.2.1/vit_pytorch/parallel_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/pit.py` & `vit-pytorch-1.2.1/vit_pytorch/pit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/recorder.py` & `vit-pytorch-1.2.1/vit_pytorch/recorder.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/regionvit.py` & `vit-pytorch-1.2.1/vit_pytorch/regionvit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/rvt.py` & `vit-pytorch-1.2.1/vit_pytorch/rvt.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/scalable_vit.py` & `vit-pytorch-1.2.1/vit_pytorch/scalable_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/sep_vit.py` & `vit-pytorch-1.2.1/vit_pytorch/sep_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/simmim.py` & `vit-pytorch-1.2.1/vit_pytorch/simmim.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/simple_flash_attn_vit.py` & `vit-pytorch-1.2.1/vit_pytorch/simple_flash_attn_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/simple_vit.py` & `vit-pytorch-1.2.1/vit_pytorch/simple_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/simple_vit_1d.py` & `vit-pytorch-1.2.1/vit_pytorch/simple_vit_1d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/simple_vit_3d.py` & `vit-pytorch-1.2.1/vit_pytorch/simple_vit_3d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/simple_vit_with_patch_dropout.py` & `vit-pytorch-1.2.1/vit_pytorch/simple_vit_with_patch_dropout.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/t2t.py` & `vit-pytorch-1.2.1/vit_pytorch/t2t.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/twins_svt.py` & `vit-pytorch-1.2.1/vit_pytorch/twins_svt.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/vit.py` & `vit-pytorch-1.2.1/vit_pytorch/vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/vit_1d.py` & `vit-pytorch-1.2.1/vit_pytorch/vit_1d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/vit_3d.py` & `vit-pytorch-1.2.1/vit_pytorch/vit_3d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/vit_for_small_dataset.py` & `vit-pytorch-1.2.1/vit_pytorch/vit_for_small_dataset.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/vit_with_patch_dropout.py` & `vit-pytorch-1.2.1/vit_pytorch/vit_with_patch_dropout.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/vit_with_patch_merger.py` & `vit-pytorch-1.2.1/vit_pytorch/vit_with_patch_merger.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch/vivit.py` & `vit-pytorch-1.2.1/vit_pytorch/vivit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.0/vit_pytorch.egg-info/PKG-INFO` & `vit-pytorch-1.2.1/vit_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-pytorch
-Version: 1.2.0
+Version: 1.2.1
 Summary: Vision Transformer (ViT) - Pytorch
 Home-page: https://github.com/lucidrains/vit-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vit-pytorch-1.2.0/vit_pytorch.egg-info/SOURCES.txt` & `vit-pytorch-1.2.1/vit_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

