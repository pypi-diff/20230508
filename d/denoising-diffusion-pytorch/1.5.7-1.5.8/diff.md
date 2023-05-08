# Comparing `tmp/denoising-diffusion-pytorch-1.5.7.tar.gz` & `tmp/denoising-diffusion-pytorch-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.5.7.tar", last modified: Mon May  8 02:31:14 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.5.8.tar", last modified: Mon May  8 05:12:44 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.5.7.tar` & `denoising-diffusion-pytorch-1.5.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 02:31:14.594257 denoising-diffusion-pytorch-1.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-08 02:31:02.000000 denoising-diffusion-pytorch-1.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-08 02:31:14.594257 denoising-diffusion-pytorch-1.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-05-08 02:31:02.000000 denoising-diffusion-pytorch-1.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 02:31:14.594257 denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-08 02:31:02.000000 denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-05-08 02:31:02.000000 denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-05-08 02:31:02.000000 denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36019 2023-05-08 02:31:02.000000 denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    30767 2023-05-08 02:31:02.000000 denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-05-08 02:31:02.000000 denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36748 2023-05-08 02:31:02.000000 denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-05-08 02:31:02.000000 denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-05-08 02:31:02.000000 denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-05-08 02:31:02.000000 denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 02:31:02.000000 denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-08 02:31:02.000000 denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 02:31:14.594257 denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-08 02:31:14.000000 denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-08 02:31:14.000000 denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 02:31:14.000000 denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-08 02:31:14.000000 denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 02:31:14.000000 denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 02:31:14.594257 denoising-diffusion-pytorch-1.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-08 02:31:02.000000 denoising-diffusion-pytorch-1.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:12:44.084786 denoising-diffusion-pytorch-1.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-08 05:12:44.084786 denoising-diffusion-pytorch-1.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:12:44.084786 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36018 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30767 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36748 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:12:44.084786 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-08 05:12:44.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-08 05:12:44.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 05:12:44.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-08 05:12:44.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 05:12:44.000000 denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 05:12:44.084786 denoising-diffusion-pytorch-1.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-08 05:12:32.000000 denoising-diffusion-pytorch-1.5.8/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.5.7/LICENSE` & `denoising-diffusion-pytorch-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.7/PKG-INFO` & `denoising-diffusion-pytorch-1.5.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.5.7
+Version: 1.5.8
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.5.7/README.md` & `denoising-diffusion-pytorch-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 from PIL import Image
 from tqdm.auto import tqdm
 from ema_pytorch import EMA
 
 from accelerate import Accelerator
 
+import numpy as np
 from pytorch_fid.inception import InceptionV3
 from pytorch_fid.fid_score import calculate_frechet_distance
 
 from denoising_diffusion_pytorch.version import __version__
 
 # constants
 
@@ -946,18 +947,18 @@
             self.accelerator.scaler.load_state_dict(data['scaler'])
 
     @torch.no_grad()
     def calculate_activation_statistics(self, samples):
         assert exists(self.inception_v3)
 
         features = self.inception_v3(samples)[0]
-        features = rearrange(features, '... 1 1 -> ...')
+        features = rearrange(features, '... 1 1 -> ...').cpu().numpy()
 
-        mu = torch.mean(features, dim = 0).cpu()
-        sigma = torch.cov(rearrange(features, '... i j -> ... j i')).cpu()
+        mu = np.mean(features, axis = 0)
+        sigma = np.cov(features, rowvar = False)
         return mu, sigma
 
     def fid_score(self, real_samples, fake_samples):
 
         if self.channels == 1:
             real_samples, fake_samples = map(lambda t: repeat(t, 'b 1 ... -> b c ...', c = 3), (real_samples, fake_samples))
```

### Comparing `denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.5.7
+Version: 1.5.8
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.5.7/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.5.8/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.7/setup.py` & `denoising-diffusion-pytorch-1.5.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     'artificial intelligence',
     'generative models'
   ],
   install_requires=[
     'accelerate',
     'einops',
     'ema-pytorch',
+    'numpy',
     'pillow',
     'pytorch-fid',
     'torch',
     'torchvision',
     'tqdm'
   ],
   classifiers=[
```

