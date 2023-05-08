# Comparing `tmp/liom-toolkit-0.3.8.tar.gz` & `tmp/liom-toolkit-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liom-toolkit-0.3.8.tar", last modified: Thu Mar 30 18:13:48 2023, max compression
+gzip compressed data, was "liom-toolkit-0.3.9.tar", last modified: Fri May  5 21:14:23 2023, max compression
```

## Comparing `liom-toolkit-0.3.8.tar` & `liom-toolkit-0.3.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:13:48.622763 liom-toolkit-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-03-30 18:13:33.000000 liom-toolkit-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-03-30 18:13:48.622763 liom-toolkit-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-03-30 18:13:33.000000 liom-toolkit-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:13:48.614763 liom-toolkit-0.3.8/liom_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-30 18:13:33.000000 liom-toolkit-0.3.8/liom_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:13:48.618763 liom-toolkit-0.3.8/liom_toolkit/registration/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-30 18:13:33.000000 liom-toolkit-0.3.8/liom_toolkit/registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-03-30 18:13:33.000000 liom-toolkit-0.3.8/liom_toolkit/registration/templating.py
--rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-03-30 18:13:33.000000 liom-toolkit-0.3.8/liom_toolkit/registration/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:13:48.618763 liom-toolkit-0.3.8/liom_toolkit/segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-30 18:13:33.000000 liom-toolkit-0.3.8/liom_toolkit/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-03-30 18:13:33.000000 liom-toolkit-0.3.8/liom_toolkit/segmentation/plane_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-03-30 18:13:33.000000 liom-toolkit-0.3.8/liom_toolkit/segmentation/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:13:48.622763 liom-toolkit-0.3.8/liom_toolkit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-30 18:13:33.000000 liom-toolkit-0.3.8/liom_toolkit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-03-30 18:13:33.000000 liom-toolkit-0.3.8/liom_toolkit/utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-30 18:13:33.000000 liom-toolkit-0.3.8/liom_toolkit/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:13:48.614763 liom-toolkit-0.3.8/liom_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-03-30 18:13:48.000000 liom-toolkit-0.3.8/liom_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-30 18:13:48.000000 liom-toolkit-0.3.8/liom_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 18:13:48.000000 liom-toolkit-0.3.8/liom_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-30 18:13:48.000000 liom-toolkit-0.3.8/liom_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-30 18:13:48.000000 liom-toolkit-0.3.8/liom_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 18:13:48.622763 liom-toolkit-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-30 18:13:33.000000 liom-toolkit-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:14:23.522673 liom-toolkit-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-05-05 21:14:14.000000 liom-toolkit-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-05 21:14:23.522673 liom-toolkit-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-05 21:14:14.000000 liom-toolkit-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:14:23.522673 liom-toolkit-0.3.9/liom_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 21:14:14.000000 liom-toolkit-0.3.9/liom_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:14:23.522673 liom-toolkit-0.3.9/liom_toolkit/registration/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 21:14:14.000000 liom-toolkit-0.3.9/liom_toolkit/registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-05 21:14:14.000000 liom-toolkit-0.3.9/liom_toolkit/registration/templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-05-05 21:14:14.000000 liom-toolkit-0.3.9/liom_toolkit/registration/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:14:23.522673 liom-toolkit-0.3.9/liom_toolkit/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-05 21:14:14.000000 liom-toolkit-0.3.9/liom_toolkit/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-05 21:14:14.000000 liom-toolkit-0.3.9/liom_toolkit/segmentation/plane_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-05-05 21:14:14.000000 liom-toolkit-0.3.9/liom_toolkit/segmentation/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:14:23.522673 liom-toolkit-0.3.9/liom_toolkit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 21:14:14.000000 liom-toolkit-0.3.9/liom_toolkit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-05-05 21:14:14.000000 liom-toolkit-0.3.9/liom_toolkit/utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-05 21:14:14.000000 liom-toolkit-0.3.9/liom_toolkit/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:14:23.522673 liom-toolkit-0.3.9/liom_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-05 21:14:23.000000 liom-toolkit-0.3.9/liom_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-05 21:14:23.000000 liom-toolkit-0.3.9/liom_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:14:23.000000 liom-toolkit-0.3.9/liom_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-05 21:14:23.000000 liom-toolkit-0.3.9/liom_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 21:14:23.000000 liom-toolkit-0.3.9/liom_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 21:14:23.522673 liom-toolkit-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-05 21:14:14.000000 liom-toolkit-0.3.9/setup.py
```

### Comparing `liom-toolkit-0.3.8/LICENSE` & `liom-toolkit-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.3.8/PKG-INFO` & `liom-toolkit-0.3.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liom-toolkit
-Version: 0.3.8
+Version: 0.3.9
 Summary: Package to support the research of LIOM.
 Home-page: https://github.com/LIOMLab/liom-toolkit
 Author: Laboratoire d’Imagerie Optique et Moléculaire
 Author-email: frederic.lesage@polymtl.ca
 License: GPLv3+
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `liom-toolkit-0.3.8/README.md` & `liom-toolkit-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.3.8/liom_toolkit/registration/templating.py` & `liom-toolkit-0.3.9/liom_toolkit/registration/templating.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.3.8/liom_toolkit/registration/utils.py` & `liom-toolkit-0.3.9/liom_toolkit/registration/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import numpy as np
 import zarr
 from ome_zarr.io import parse_url
 from ome_zarr.reader import Reader, Node
 from ome_zarr.writer import write_image
 from scipy.ndimage import binary_fill_holes
 
+from liom_toolkit.segmentation import remove_small_structures
 from liom_toolkit.utils import generate_axes_dict, create_transformation_dict, CustomScaler
 
 """
     Utility functions aiding in the registration process.
 """
 
 
@@ -39,15 +40,14 @@
     :return: The ANTs image.
     """
     volume = np.array(node.data[resolution_level])
     volume = np.transpose(volume, (2, 1, 0)).astype("uint32")
     volume = ants.from_numpy(volume)
     volume.set_spacing(scale)
     volume.set_direction([[1., 0., 0.], [0., 0., -1.], [0., -1., 0.]])
-    volume = ants.reorient_image2(volume, "RAS")
     return volume
 
 
 def load_mask(node: Node, resolution_level: int = 0) -> ants.ANTsImage:
     """
     Load a mask from a zarr file.
 
@@ -58,15 +58,14 @@
     volume = np.array(node.data[resolution_level])
     volume = volume.astype("ubyte")
     mask = ants.from_numpy(volume)
 
     transform = load_zarr_transform_from_node(node, resolution_level=resolution_level)
     mask.set_spacing(transform)
     mask.set_direction([[1., 0., 0.], [0., 0., -1.], [0., -1., 0.]])
-    mask = ants.reorient_image2(mask, "RAS")
     return mask
 
 
 def load_allen_template(atlas_file: str, resolution: int, padding: bool) -> ants.ANTsImage:
     """
     Load the allen template and set the resolution and direction (PIR).
 
@@ -81,15 +80,14 @@
         # Pad the atlas to avoid edge effects, the padding is 15% of the atlas size
         pad_size = int(atlas_data.shape[0] * 0.15)
         npad = ((pad_size, pad_size), (0, 0), (0, 0))
         atlas_data = np.pad(atlas_data, pad_width=npad, mode="constant", constant_values=0)
     atlas_volume = ants.from_numpy(atlas_data)
     atlas_volume.set_spacing([resolution, resolution, resolution])
     atlas_volume.set_direction([[0., 0., 1.], [1., 0., 0.], [0., -1., 0.]])
-    atlas_volume = ants.reorient_image2(atlas_volume, "RAS")
     return atlas_volume
 
 
 def load_zarr_transform_from_node(node: Node, resolution_level: int = 1) -> dict:
     """
     Load a zarr file to an ANTs image.
 
@@ -173,30 +171,34 @@
     ws = sitk.MorphologicalWatershedFromMarkers(img, marker_img)
 
     # Separating into foreground / background
     seg = sitk.ConnectedComponent(ws != ws[0, 0, 0])
 
     # Filling holes and returning the mask
     mask = fill_holes_2d_3d(sitk.GetArrayFromImage(seg))
+
+    # Remove small objects
+    mask = remove_small_structures(vol_p, mask)
+
     return mask
 
 
-def create_and_write_mask(zarr_file: str):
+def create_and_write_mask(zarr_file: str, overwrite: bool = False):
     """
     Create a mask for a zarr file and write it to disk.
 
     :param zarr_file: The zarr file to create a mask for
     """
     node = load_zarr(zarr_file)[0]
     image = load_ants_image_from_zarr(node, resolution_level=0)
     mask = segment_3d_brain(image)
 
     file = parse_url(zarr_file, mode="w").store
     root = zarr.group(store=file)
-    labels_grp = root.create_group("labels")
+    labels_grp = root.create_group("labels", overwrite=overwrite)
     label_name = "mask"
     labels_grp.attrs["labels"] = [label_name]
-    label_grp = labels_grp.create_group(label_name)
+    label_grp = labels_grp.create_group(label_name, overwrite=overwrite)
 
     write_image(image=mask, group=label_grp, axes=generate_axes_dict(),
                 coordinate_transformations=create_transformation_dict((6.5, 6.5, 6.5), 5),
                 storage_options=dict(chunks=(512, 512, 512)), scaler=CustomScaler(downscale=2, method="nearest"))
```

### Comparing `liom-toolkit-0.3.8/liom_toolkit/segmentation/plane_segmentation.py` & `liom-toolkit-0.3.9/liom_toolkit/segmentation/plane_segmentation.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,29 +68,40 @@
 
     # Apply threshold
     mask = img > threshold_tissue
 
     # Filter out noisy segmentation
     mask = median_filter(mask, 5)
 
+    mask = remove_small_structures(img, mask)
+
+    return mask
+
+
+def remove_small_structures(img, mask):
+    """
+    Remove small structures from a mask
+
+    :param img: The image with which the mask was generated
+    :param mask: The mask to remove small structures from
+    :return: The mask with small structures removed
+    """
     # Filter out small structures
     img_labels = label(mask)
     props = regionprops(img_labels)
 
     # Area threshold
     img_size = img.size
     tissue_labels = []
     for this_region in props:
         if this_region.area / img_size >= 0.05:
             tissue_labels.append(this_region.label)
-
     mask = np.zeros_like(mask)
     for this_label in tissue_labels:
         mask[img_labels == this_label] = 1
-
     return mask
 
 
 def erode_mask(mask, disk_size=30):
     """
     Erode the outer edge of a mask
     :param mask: The mask to erode
```

### Comparing `liom-toolkit-0.3.8/liom_toolkit/segmentation/stats.py` & `liom-toolkit-0.3.9/liom_toolkit/segmentation/stats.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.3.8/liom_toolkit/utils/conversion.py` & `liom-toolkit-0.3.9/liom_toolkit/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.3.8/liom_toolkit.egg-info/PKG-INFO` & `liom-toolkit-0.3.9/liom_toolkit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liom-toolkit
-Version: 0.3.8
+Version: 0.3.9
 Summary: Package to support the research of LIOM.
 Home-page: https://github.com/LIOMLab/liom-toolkit
 Author: Laboratoire d’Imagerie Optique et Moléculaire
 Author-email: frederic.lesage@polymtl.ca
 License: GPLv3+
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `liom-toolkit-0.3.8/liom_toolkit.egg-info/SOURCES.txt` & `liom-toolkit-0.3.9/liom_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.3.8/setup.py` & `liom-toolkit-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 setup(
     name="liom-toolkit",
-     version="0.3.8",
+     version="0.3.9",
     author="Laboratoire d’Imagerie Optique et Moléculaire",
     author_email="frederic.lesage@polymtl.ca",
     packages=find_packages(),
     description="Package to support the research of LIOM.",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/LIOMLab/liom-toolkit",
```

