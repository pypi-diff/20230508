# Comparing `tmp/flatnet-0.1.4.tar.gz` & `tmp/flatnet-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatnet-0.1.4.tar", last modified: Fri May  5 22:51:32 2023, max compression
+gzip compressed data, was "flatnet-0.2.0.tar", last modified: Mon May  8 10:12:02 2023, max compression
```

## Comparing `flatnet-0.1.4.tar` & `flatnet-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 05:02:27.266479 flatnet-0.1.4/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      299 2023-05-06 05:02:27.257483 flatnet-0.1.4/PKG-INFO
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 05:02:26.692868 flatnet-0.1.4/flatnet/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       24 2023-05-06 03:00:44.000000 flatnet-0.1.4/flatnet/__init__.py
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 05:02:27.174946 flatnet-0.1.4/flatnet/modules/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2022-04-06 05:54:15.000000 flatnet-0.1.4/flatnet/modules/__init__.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     3564 2023-05-05 20:51:08.000000 flatnet-0.1.4/flatnet/modules/flatnet_nn.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)    14367 2023-05-06 05:00:43.000000 flatnet-0.1.4/flatnet/train.py
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 05:02:27.005877 flatnet-0.1.4/flatnet.egg-info/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      299 2023-05-06 05:02:26.000000 flatnet-0.1.4/flatnet.egg-info/PKG-INFO
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      257 2023-05-06 05:02:26.000000 flatnet-0.1.4/flatnet.egg-info/SOURCES.txt
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        1 2023-05-06 05:02:26.000000 flatnet-0.1.4/flatnet.egg-info/dependency_links.txt
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      556 2023-05-06 05:02:26.000000 flatnet-0.1.4/flatnet.egg-info/requires.txt
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        8 2023-05-06 05:02:26.000000 flatnet-0.1.4/flatnet.egg-info/top_level.txt
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       38 2023-05-06 05:02:27.269479 flatnet-0.1.4/setup.cfg
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     1202 2023-05-06 04:40:41.000000 flatnet-0.1.4/setup.py
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-08 20:34:24.043226 flatnet-0.2.0/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     5804 2023-05-08 20:34:24.043226 flatnet-0.2.0/PKG-INFO
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     3562 2023-05-06 15:23:53.000000 flatnet-0.2.0/README.md
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-08 20:34:23.543223 flatnet-0.2.0/flatnet/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       24 2023-05-06 03:00:44.000000 flatnet-0.2.0/flatnet/__init__.py
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-08 20:34:23.965098 flatnet-0.2.0/flatnet/modules/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2022-04-06 05:54:15.000000 flatnet-0.2.0/flatnet/modules/__init__.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     3564 2023-05-05 20:51:08.000000 flatnet-0.2.0/flatnet/modules/flatnet_nn.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)    16415 2023-05-08 04:24:36.000000 flatnet-0.2.0/flatnet/train.py
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-08 20:34:23.824508 flatnet-0.2.0/flatnet.egg-info/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     5804 2023-05-08 20:34:22.000000 flatnet-0.2.0/flatnet.egg-info/PKG-INFO
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      267 2023-05-08 20:34:23.000000 flatnet-0.2.0/flatnet.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        1 2023-05-08 20:34:22.000000 flatnet-0.2.0/flatnet.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      572 2023-05-08 20:34:22.000000 flatnet-0.2.0/flatnet.egg-info/requires.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        8 2023-05-08 20:34:22.000000 flatnet-0.2.0/flatnet.egg-info/top_level.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       38 2023-05-08 20:34:24.043226 flatnet-0.2.0/setup.cfg
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     2213 2023-05-08 04:12:54.000000 flatnet-0.2.0/setup.py
```

### Comparing `flatnet-0.1.4/flatnet/modules/flatnet_nn.py` & `flatnet-0.2.0/flatnet/modules/flatnet_nn.py`

 * *Files identical despite different names*

### Comparing `flatnet-0.1.4/flatnet/train.py` & `flatnet-0.2.0/flatnet/train.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 # used for optimizing over Stiefel
 import geoopt
 
 from .modules import flatnet_nn
 
 from tqdm import trange
 
+# for saving gifs
+import matplotlib.pyplot as plt
+import imageio
+import os
 
 # ****************************i*************************************************
 # This is the primary script for the curvature compression algorithm.
 # Input: data matrix X of shape (n,D), where D is the embedding dimension and
 # n is the number of data points;
 # d_desired is the desired dimension to flatten X onto
 
@@ -32,18 +36,24 @@
        alpha_max=0.5,  # global parameter for kernel
        r_dimcheck_coeff=0.15,  # # radius for checking dimension.
        max_error_dimcheck_ratio=0.3,  # max l0 error with respect to r_dimcheck to stop dimension search
        r_min_coeff=0.15,  # minimum allowed radius for each flattening
        r_max_coeff=1.1,  # maximum allowed radius for each flattening
        r_step_min_coeff=1.0,  # max steps to take when finding biggest r
        n_iter_rsearch=1,  # max steps to take when finding biggest r
+       save_gif = False, # whether to save gif of flattening process. currently only works for 2D data
        ):
     N, D = X.shape
     # needed for dist-to-gamma conversion
     log2 = float(np.log(2))
+
+    # if save gif is set to true but data is not 2D, throw warning but continue running with save_gif = False
+    if save_gif and D != 2:
+        print("Warning: save_gif is set to True but data is not 2D. Setting save_gif to False")
+        save_gif = False
     #######	## HYPERPARAMETERS ####
     ##############################
 
     converge_counter = 0
 
     # used to define hyperparameters
     EDM_X = torch.cdist(X, X, p=2)
@@ -72,14 +82,27 @@
     ############# INIT GLOBAL VARIABLES##########
     # encoder network
     f = flatnet_nn.FlatteningNetwork()
     # decoder network
     g = flatnet_nn.FlatteningNetwork()
     Z = X.clone()
 
+    ################### ANIMATION SAVING #################
+
+    if save_gif:
+        # Ensure the 'flatnet_gif_frames' directory does not already exist
+        if os.path.exists('flatnet_gif_frames'):
+            raise Exception("The 'flatnet_gif_frames' directory already exists; to ensure this script does not damage your local files, please eiehter delete flatnet_gif_frames or move this script to a new directory and try again.")
+
+        # Create the 'flatnet_gif_frames' directory
+        os.makedirs('flatnet_gif_frames')
+
+        # create array to store frames
+        frames = []
+
     # ################ MAIN LOOP #########################
     with trange(n_iter, unit="iters") as pbar:
         for j in pbar:
             # if j % 20 == 0:
             # 	plt.scatter(Z[:,0].detach().numpy(), Z[:,1].detach().numpy())
             # 	plt.show()
 
@@ -169,19 +192,42 @@
                 converge_counter = 0
                 f.add_operation(f_layer)
                 g.add_operation(g_layer)
                 d_prev = U.shape[1]
                 # only update representation if we add the layer
                 Z = Z_new.clone()
 
+                # save gif frame
+                if save_gif:
+                    fig, ax = plt.subplots()
+                    ax.scatter(Z[:, 0].detach().numpy(), Z[:, 1].detach().numpy())
+                    ax.axis('off')
+                    for spine in ax.spines.values():
+                        spine.set_visible(False)
+                    plt.savefig(f"flatnet_gif_frames/frame_{j}.png")
+                    plt.close()
+                    # save frame
+                    frames.append(imageio.imread(f"flatnet_gif_frames/frame_{j}.png"))
+
             # with torch.no_grad():
             # 	recon_loss = 0.5*(g(Z) - X).pow(2).mean()
             pbar.set_postfix({"local_recon": loss_r.item(), \
                               "d": U.shape[1], "r_ratio": (r / r_max).item(), "alpha": alpha})
 
+    # final gif processing
+    if save_gif:
+        # save gif to be 6s long. note duration is duration
+        # of each frame in ms
+        imageio.mimsave('flatnet_flow.gif', frames, duration=6000 / len(frames))
+        
+        # delete auxillery files
+        for file_name in os.listdir('flatnet_gif_frames'):
+            os.remove(os.path.join('flatnet_gif_frames', file_name))
+        os.rmdir('flatnet_gif_frames')
+
     return f, g
 
 
 # ################## HELPER METHODS #####################
 
 def opt_UV(Z, z_c, U_0, n_iter_inner, r=-1, kernel=-1):
     D, d = U_0.shape
```

### Comparing `flatnet-0.1.4/flatnet.egg-info/requires.txt` & `flatnet-0.2.0/flatnet.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Jinja2>=3.1.2
 MarkupSafe>=2.1.2
 cmake>=3.26.3
 filelock>=3.12.0
 geoopt>=0.5.0
+imageio>=2.28.1
 lit>=16.0.2
 mpmath>=1.3.0
 networkx>=3.1
 numpy>=1.24.3
 nvidia-cublas-cu11>=11.10.3.66
 nvidia-cuda-cupti-cu11>=11.7.101
 nvidia-cuda-nvrtc-cu11>=11.7.99
```

