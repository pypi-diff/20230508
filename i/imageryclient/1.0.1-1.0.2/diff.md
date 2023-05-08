# Comparing `tmp/imageryclient-1.0.1.tar.gz` & `tmp/imageryclient-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imageryclient-1.0.1.tar", last modified: Tue Nov 29 00:38:58 2022, max compression
+gzip compressed data, was "imageryclient-1.0.2.tar", last modified: Mon May  8 17:55:09 2023, max compression
```

## Comparing `imageryclient-1.0.1.tar` & `imageryclient-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2022-11-29 00:38:58.160841 imageryclient-1.0.1/
--rw-r--r--   0 caseysm    (501) staff       (20)     1079 2022-11-16 18:21:56.000000 imageryclient-1.0.1/LICENSE
--rw-r--r--   0 caseysm    (501) staff       (20)       49 2022-11-16 18:21:56.000000 imageryclient-1.0.1/MANIFEST.in
--rw-r--r--   0 caseysm    (501) staff       (20)     1554 2022-11-29 00:38:58.160727 imageryclient-1.0.1/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)    15075 2022-11-28 07:21:09.000000 imageryclient-1.0.1/README.md
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2022-11-29 00:38:58.159694 imageryclient-1.0.1/imageryclient/
--rw-r--r--   0 caseysm    (501) staff       (20)      133 2022-11-29 00:38:47.000000 imageryclient-1.0.1/imageryclient/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    11005 2022-11-16 18:21:56.000000 imageryclient-1.0.1/imageryclient/composite.py
--rw-r--r--   0 caseysm    (501) staff       (20)    40154 2022-11-29 00:37:22.000000 imageryclient-1.0.1/imageryclient/imagery.py
--rw-r--r--   0 caseysm    (501) staff       (20)     5547 2022-11-29 00:20:08.000000 imageryclient-1.0.1/imageryclient/utils.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2022-11-29 00:38:58.160557 imageryclient-1.0.1/imageryclient.egg-info/
--rw-r--r--   0 caseysm    (501) staff       (20)     1554 2022-11-29 00:38:58.000000 imageryclient-1.0.1/imageryclient.egg-info/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)      356 2022-11-29 00:38:58.000000 imageryclient-1.0.1/imageryclient.egg-info/SOURCES.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        1 2022-11-29 00:38:58.000000 imageryclient-1.0.1/imageryclient.egg-info/dependency_links.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       81 2022-11-29 00:38:58.000000 imageryclient-1.0.1/imageryclient.egg-info/requires.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       14 2022-11-29 00:38:58.000000 imageryclient-1.0.1/imageryclient.egg-info/top_level.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       82 2022-11-28 07:21:09.000000 imageryclient-1.0.1/requirements.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       38 2022-11-29 00:38:58.160883 imageryclient-1.0.1/setup.cfg
--rw-r--r--   0 caseysm    (501) staff       (20)     1166 2022-11-16 18:21:56.000000 imageryclient-1.0.1/setup.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1254 2022-11-16 18:21:56.000000 imageryclient-1.0.1/short_readme.md
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-08 17:55:09.570518 imageryclient-1.0.2/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1079 2022-11-16 18:21:56.000000 imageryclient-1.0.2/LICENSE
+-rw-r--r--   0 caseysm    (501) staff       (20)       49 2022-11-16 18:21:56.000000 imageryclient-1.0.2/MANIFEST.in
+-rw-r--r--   0 caseysm    (501) staff       (20)     1554 2023-05-08 17:55:09.570395 imageryclient-1.0.2/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)    16014 2023-05-08 17:45:33.000000 imageryclient-1.0.2/README.md
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-08 17:55:09.569291 imageryclient-1.0.2/imageryclient/
+-rw-r--r--   0 caseysm    (501) staff       (20)      133 2023-05-08 17:54:59.000000 imageryclient-1.0.2/imageryclient/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    11089 2022-11-29 01:10:22.000000 imageryclient-1.0.2/imageryclient/composite.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    39350 2023-05-08 17:39:36.000000 imageryclient-1.0.2/imageryclient/imagery.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     6359 2022-11-29 01:07:39.000000 imageryclient-1.0.2/imageryclient/utils.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-08 17:55:09.570226 imageryclient-1.0.2/imageryclient.egg-info/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1554 2023-05-08 17:55:09.000000 imageryclient-1.0.2/imageryclient.egg-info/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)      356 2023-05-08 17:55:09.000000 imageryclient-1.0.2/imageryclient.egg-info/SOURCES.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-05-08 17:55:09.000000 imageryclient-1.0.2/imageryclient.egg-info/dependency_links.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       81 2023-05-08 17:55:09.000000 imageryclient-1.0.2/imageryclient.egg-info/requires.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       14 2023-05-08 17:55:09.000000 imageryclient-1.0.2/imageryclient.egg-info/top_level.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       82 2022-11-28 07:21:09.000000 imageryclient-1.0.2/requirements.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-05-08 17:55:09.570563 imageryclient-1.0.2/setup.cfg
+-rw-r--r--   0 caseysm    (501) staff       (20)     1166 2022-11-16 18:21:56.000000 imageryclient-1.0.2/setup.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     1254 2022-11-16 18:21:56.000000 imageryclient-1.0.2/short_readme.md
```

### Comparing `imageryclient-1.0.1/LICENSE` & `imageryclient-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `imageryclient-1.0.1/PKG-INFO` & `imageryclient-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imageryclient
-Version: 1.0.1
+Version: 1.0.2
 Summary: Front end tools for composite images for EM connectomics
 Home-page: https://github.com/ceesem/ImageryClient
 Author: Casey Schneider-Mizell
 Author-email: caseysm@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `imageryclient-1.0.1/README.md` & `imageryclient-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,22 @@
 Moreover, imagery and segmentation have data that means intrensically different things.
 Values in imagery indicate pixel intensity in order to produce a picture, while values in segmentation indicate the object id at a given location.
 ImageryClient acts as a front end for making aligned cutouts from multiple cloudvolume sources, splitting segmentations into masks for each object, and more.
 
 We make use of [Numpy arrays](https://numpy.org/doc/stable/) and [Pillow Images](https://pillow.readthedocs.io/) to represent data.
 Both are extremely rich tools, and to learn more about them please see the appropriate documentation for information about saving data to image files and more. 
 
+## Installation
+
+The standard installation:
+
+`pip install imageryclient`
+
+If you have installation issues due to Cloudvolume, which has a fairly complex set of requirements, we recommend looking at their github [issues page](https://github.com/seung-lab/cloud-volume/issues) for help.
+
 ## How to use ImageryClient
 
 Here, we will use the ImageryClient to get some data from the [Kasthuri et al. 2014 dataset](https://neuroglancer-demo.appspot.com/fafb.html#!gs://fafb-ffn1/main_ng.json) hosted by Google.
 In its simplest form, we just intialize an ImageryClient object with an image cloudpath and a segmentation cloudpath.
 Values are taken from the layers in the linked neuroglancer state.
 
 ```python
@@ -72,14 +80,18 @@
 
 ```python
 img_client = ic.ImageryClient(..., resolution=[8,8,30])
 ```
 You can also explicitly set the resolution to `"image"` or `"segmentation"` to use the highest available resolution available for either.
 Resolution can also be specified in each of the functions for image or segmentation cutouts, but will default to the client values.
 
+Note that the volumetric data itself is not necessarily at the resolution specified, but rather this parameter determines how to interpret the _coordinates_.
+The resolution is set by the image and segmentation mip levels, which can be added either when creating the ImageryClient instance or when doing any cutout download.
+By default, ImageryClient will use the highest resolution mip level that is not labeled as a `"placeholder"` in CloudVolume.
+
 #### Specifying image size instead of field of view
 
 When upper and lower bounds are specified or a `bbox_size` is used, the resolution will change with mip level but the field of view that is downloaded will remain the same.
 Alternatively, one might want to download an image with a specific size in pixels and a specific mip level without having to calculate what bounding box would get you that..
 This can be done in `image_cutout` by specifying the center point in the place of bounds and also specify `image_size` as a 2- or 3-element array.
 In this case, the center point will be adjusted according to the resolutions specified, while the field of view will change with image size.
 
@@ -99,14 +111,15 @@
 img_size=(400, 400)
 image = img_client.image_cutout(ctr, mip=3, image_size=img_size)
 Image.fromarray(image.T)
 ```
 
 ![imagery exact](example_images/exact_mip_3.png)
 
+You can also use the `scale_to_bounds=True` argument to upscale an image to the size specified in the bounding box, equivalent to having one pixel for each voxel as measured by the resolution parameter.
 
 ### Segmentations
 
 An aligned segmentation cutout is retrieved similarly.
 Note that segmentations show segment ids, and are not directly visualizable.
 However, in this case we can convert to a uint8 greyscale and see the gist, although there are many better approaches to coloring segmentations that will be shown later.
 Note that for dynamic segmentations, you can use the timestamp parameter to (optionally) set the time at which segmentation will e looked up.
```

### Comparing `imageryclient-1.0.1/imageryclient/composite.py` & `imageryclient-1.0.2/imageryclient/composite.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,14 +255,17 @@
 
     Returns
     -------
     list or PIL.Image.Image
         Image or list of composite overlay images, optionally overlaid over provided imagery. List or single image
         is determined based on segmentation arrays being 2 or 3 dimensional.
     """
+    if isinstance(segs, np.ndarray):
+        segs = utils.segmentation_masks(segs)
+
     if colors is None:
         colors = discrete_colors(segs, palette, h, l, s)
 
     n_dim = len(utils.get_first(segs).shape)
     if n_dim > 2:
         n_frames = utils.get_first(segs).shape[dim]
     else:
```

### Comparing `imageryclient-1.0.1/imageryclient/imagery.py` & `imageryclient-1.0.2/imageryclient/imagery.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,37 +30,14 @@
         2x3 array of lower and upper bounds (in that order).
     """
     xl = ctr - np.array([width // 2, height // 2, depth // 2])
     xh = xl + np.array([width, height, depth])
     return np.array([xl, xh])
 
 
-def segmentation_masks(seg_img, include_null_root=False):
-    """Convert a segmentation array into a dict of binary masks for each root id.
-
-    Parameters
-    ----------
-    seg_img : numpy.ndarray
-        Array with voxel values corresponding to the object id at that voxel
-    include_null_root : bool, optional
-        Create a mask for 0 id, which usually denotes no object, by default False
-
-    Returns
-    -------
-    dict
-        Dict of binary masks. Keys are root ids, values are boolean n-d arrays with a 1 where that object is.
-    """
-    split_segmentation = {}
-    for root_id in np.unique(seg_img):
-        if include_null_root is False:
-            if root_id == 0:
-                continue
-        split_segmentation[root_id] = (seg_img == root_id).astype(int)
-    return split_segmentation
-
 
 def save_image_slices(
     filename_prefix,
     filename_suffix,
     img,
     slice_axis,
     image_type,
@@ -581,15 +558,15 @@
             mip=mip,
             bbox_size=bbox_size,
             image_size=image_size,
             resolution=resolution,
             timestamp=timestamp,
             scale_to_bounds=scale_to_bounds,
         )
-        return segmentation_masks(seg_img, include_null_root)
+        return utils.segmentation_masks(seg_img, include_null_root)
 
     def image_and_segmentation_cutout(
         self,
         bounds,
         image_mip=None,
         segmentation_mip=None,
         root_ids="all",
@@ -726,15 +703,15 @@
         precomputed_image=None,
         slice_axis=2,
         bbox_size=None,
         image_size=None,
         resolution=None,
         scale_to_bounds=None,
         verbose=False,
-        *kwargs,
+        **kwargs,
     ):
         """Save queried or precomputed imagery to png files.
 
         Parameters
         ----------
         filename_prefix : str
             Prefix for the imagery filename. The full filename will be {filename_prefix}_imagery.png
```

### Comparing `imageryclient-1.0.1/imageryclient/utils.py` & `imageryclient-1.0.2/imageryclient/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -198,7 +198,31 @@
 
 
 def get_first(masks):
     if isinstance(masks, dict):
         return list(masks.values())[0]
     else:
         return masks[0]
+
+
+def segmentation_masks(seg_img, include_null_root=False):
+    """Convert a segmentation array into a dict of binary masks for each root id.
+
+    Parameters
+    ----------
+    seg_img : numpy.ndarray
+        Array with voxel values corresponding to the object id at that voxel
+    include_null_root : bool, optional
+        Create a mask for 0 id, which usually denotes no object, by default False
+
+    Returns
+    -------
+    dict
+        Dict of binary masks. Keys are root ids, values are boolean n-d arrays with a 1 where that object is.
+    """
+    split_segmentation = {}
+    for root_id in np.unique(seg_img):
+        if include_null_root is False:
+            if root_id == 0:
+                continue
+        split_segmentation[root_id] = (seg_img == root_id).astype(int)
+    return split_segmentation
```

### Comparing `imageryclient-1.0.1/imageryclient.egg-info/PKG-INFO` & `imageryclient-1.0.2/imageryclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imageryclient
-Version: 1.0.1
+Version: 1.0.2
 Summary: Front end tools for composite images for EM connectomics
 Home-page: https://github.com/ceesem/ImageryClient
 Author: Casey Schneider-Mizell
 Author-email: caseysm@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `imageryclient-1.0.1/setup.py` & `imageryclient-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `imageryclient-1.0.1/short_readme.md` & `imageryclient-1.0.2/short_readme.md`

 * *Files identical despite different names*

