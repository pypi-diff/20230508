# Comparing `tmp/navalmartin_mir_vision_utils-0.0.8.tar.gz` & `tmp/navalmartin_mir_vision_utils-0.0.9.tar.gz`

## Comparing `navalmartin_mir_vision_utils-0.0.8.tar` & `navalmartin_mir_vision_utils-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/distribute.sh
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/requirements.txt
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/setup.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/.idea/.gitignore
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/.idea/misc.xml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/.idea/modules.xml
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/.idea/src.iml
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/.idea/vcs.xml
--rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/.idea/workspace.xml
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/__init__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/exceptions.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/image_enums.py
--rw-r--r--   0        0        0     5877 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/image_loaders.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/image_transformers.py
--rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/image_utils.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/plot_images.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/examples/__init__.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/examples/image_transformations_examples.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/examples/image_utils_examples.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/image_quality/__init__.py
--rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/image_quality/brisque.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/image_quality/models/__init__.py
--rw-r--r--   0        0        0   351414 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/image_quality/models/brisque_svm.txt
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/image_quality/models/normalize.pickle
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/io/__init__.py
--rw-r--r--   0        0        0     7870 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/io/file_utils.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/io/tempfile.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/statistics/__init__.py
--rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/statistics/image_statistics.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/statistics/statistics_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/statistics/distributions/__init__.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/statistics/distributions/asymmetric_generalized_gaussian.py
--rw-r--r--   0        0        0   142798 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/test_data/corrosion_4.png
--rw-r--r--   0        0        0    18154 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/test_data/img_18_3.jpg
--rw-r--r--   0        0        0    15826 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/test_data/img_2_6.jpg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/tests/test_brisque_image_quality.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/tests/test_image_statistics.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/tests/test_image_utils.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/LICENSE
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/README.md
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/distribute.sh
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/setup.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/.idea/.gitignore
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/.idea/misc.xml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/.idea/modules.xml
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/.idea/src.iml
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/.idea/vcs.xml
+-rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/.idea/workspace.xml
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/exceptions.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/image_enums.py
+-rw-r--r--   0        0        0     5877 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/image_loaders.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/image_transformers.py
+-rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/image_utils.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/plot_images.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/examples/__init__.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/examples/image_transformations_examples.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/examples/image_utils_examples.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/image_quality/__init__.py
+-rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/image_quality/brisque.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/image_quality/models/__init__.py
+-rw-r--r--   0        0        0   351414 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/image_quality/models/brisque_svm.txt
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/image_quality/models/normalize.pickle
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/mir_vison_io/__init__.py
+-rw-r--r--   0        0        0     7870 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/mir_vison_io/file_utils.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/mir_vison_io/tempfile.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/statistics/__init__.py
+-rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/statistics/image_statistics.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/statistics/statistics_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/statistics/distributions/__init__.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/statistics/distributions/asymmetric_generalized_gaussian.py
+-rw-r--r--   0        0        0   142798 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/test_data/corrosion_4.png
+-rw-r--r--   0        0        0    18154 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/test_data/img_18_3.jpg
+-rw-r--r--   0        0        0    15826 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/test_data/img_2_6.jpg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/tests/test_brisque_image_quality.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/tests/test_image_statistics.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/tests/test_image_utils.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/README.md
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 navalmartin_mir_vision_utils-0.0.9/PKG-INFO
```

### Comparing `navalmartin_mir_vision_utils-0.0.8/setup.py` & `navalmartin_mir_vision_utils-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/src/.idea/src.iml` & `navalmartin_mir_vision_utils-0.0.9/src/.idea/src.iml`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/src/.idea/workspace.xml` & `navalmartin_mir_vision_utils-0.0.9/src/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/__init__.py` & `navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Various utilities for working with images in the _mir_ project.
 """
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 from typing import TypeVar
 
 from .image_utils import (is_valid_pil_image_from_bytes_string,
                           is_valid_pil_image_file,
                           show_pil_image,
                           get_img_files, 
                           get_pil_image_size)
```

### Comparing `navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/image_enums.py` & `navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/image_enums.py`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/image_loaders.py` & `navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/image_loaders.py`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/image_transformers.py` & `navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/image_transformers.py`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/image_utils.py` & `navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/plot_images.py` & `navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/plot_images.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 import matplotlib.pyplot as plt
-import torch
-import torchvision
 
-def plot_pytorch_tensor_images(images: torch.Tensor, title: str,
+from navalmartin_mir_vision_utils import WITH_TORCH, TorchTensor
+
+if WITH_TORCH:
+    import torch
+    import torchvision
+
+
+
+
+def plot_pytorch_tensor_images(images: TorchTensor, title: str,
                                images_per_row: int) -> None:
     """Plot the images represented as PyTorch.Tensor tensors
 
     Parameters
     ----------
     images: The images to plot. 4D mini-batch Tensor of shape (B x C x H x W)
     title: The title of the plot
     images_per_row: Number of images in each row of the grid
 
     Returns
     -------
     None
     """
 
+    if not WITH_TORCH:
+        
+
     plt.figure()
     plt.title(title)
     plt.imshow(torchvision.utils.make_grid(images, nrow=images_per_row).permute(1, 2, 0))
```

### Comparing `navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/examples/image_transformations_examples.py` & `navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/examples/image_transformations_examples.py`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/examples/image_utils_examples.py` & `navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/examples/image_utils_examples.py`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/image_quality/brisque.py` & `navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/image_quality/brisque.py`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/image_quality/models/brisque_svm.txt` & `navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/image_quality/models/brisque_svm.txt`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/image_quality/models/normalize.pickle` & `navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/image_quality/models/normalize.pickle`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/io/file_utils.py` & `navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/mir_vison_io/file_utils.py`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/statistics/image_statistics.py` & `navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/statistics/image_statistics.py`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/statistics/statistics_utils.py` & `navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/statistics/statistics_utils.py`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/src/navalmartin_mir_vision_utils/statistics/distributions/asymmetric_generalized_gaussian.py` & `navalmartin_mir_vision_utils-0.0.9/src/navalmartin_mir_vision_utils/statistics/distributions/asymmetric_generalized_gaussian.py`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/test_data/corrosion_4.png` & `navalmartin_mir_vision_utils-0.0.9/test_data/corrosion_4.png`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/test_data/img_18_3.jpg` & `navalmartin_mir_vision_utils-0.0.9/test_data/img_18_3.jpg`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/test_data/img_2_6.jpg` & `navalmartin_mir_vision_utils-0.0.9/test_data/img_2_6.jpg`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/tests/test_brisque_image_quality.py` & `navalmartin_mir_vision_utils-0.0.9/tests/test_brisque_image_quality.py`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/tests/test_image_statistics.py` & `navalmartin_mir_vision_utils-0.0.9/tests/test_image_statistics.py`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/tests/test_image_utils.py` & `navalmartin_mir_vision_utils-0.0.9/tests/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/.gitignore` & `navalmartin_mir_vision_utils-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/LICENSE` & `navalmartin_mir_vision_utils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/README.md` & `navalmartin_mir_vision_utils-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `navalmartin_mir_vision_utils-0.0.8/pyproject.toml` & `navalmartin_mir_vision_utils-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "torch", "torchvision", "numpy",
             "Pillow", "scipy", "scikit-image", "libsvm"]
 build-backend = "hatchling.build"
 [project]
 name = "navalmartin_mir_vision_utils"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Alexandros Giavaras", email="a.giavaras@gmail.com" },
 ]
 description = "Various utilities for working with images in Python 3. for the mir project"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `navalmartin_mir_vision_utils-0.0.8/PKG-INFO` & `navalmartin_mir_vision_utils-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: navalmartin_mir_vision_utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Various utilities for working with images in Python 3. for the mir project
 Project-URL: Homepage, https://github.com/Navalmartin/navalmartin_mir_vision_utils
 Project-URL: Bug Tracker, https://github.com/Navalmartin/navalmartin_mir_vision_utils/issues
 Author-email: Alexandros Giavaras <a.giavaras@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

