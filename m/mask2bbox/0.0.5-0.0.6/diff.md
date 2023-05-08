# Comparing `tmp/mask2bbox-0.0.5.tar.gz` & `tmp/mask2bbox-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mask2bbox-0.0.5.tar", last modified: Wed May  3 13:29:02 2023, max compression
+gzip compressed data, was "mask2bbox-0.0.6.tar", last modified: Mon May  8 12:59:22 2023, max compression
```

## Comparing `mask2bbox-0.0.5.tar` & `mask2bbox-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:02.296460 mask2bbox-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-03 13:28:45.000000 mask2bbox-0.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 13:28:45.000000 mask2bbox-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-03 13:29:02.292460 mask2bbox-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-03 13:28:45.000000 mask2bbox-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 13:29:02.296460 mask2bbox-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-03 13:28:45.000000 mask2bbox-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:02.292460 mask2bbox-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:02.292460 mask2bbox-0.0.5/src/mask2bbox/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-03 13:28:45.000000 mask2bbox-0.0.5/src/mask2bbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-05-03 13:28:45.000000 mask2bbox-0.0.5/src/mask2bbox/_bboxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-03 13:28:45.000000 mask2bbox-0.0.5/src/mask2bbox/mask2bbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:02.292460 mask2bbox-0.0.5/src/mask2bbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-03 13:29:02.000000 mask2bbox-0.0.5/src/mask2bbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-03 13:29:02.000000 mask2bbox-0.0.5/src/mask2bbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:29:02.000000 mask2bbox-0.0.5/src/mask2bbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-03 13:29:02.000000 mask2bbox-0.0.5/src/mask2bbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 13:29:02.000000 mask2bbox-0.0.5/src/mask2bbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:02.292460 mask2bbox-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:28:45.000000 mask2bbox-0.0.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:02.292460 mask2bbox-0.0.5/tests/test_mask2bbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:28:45.000000 mask2bbox-0.0.5/tests/test_mask2bbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-03 13:28:45.000000 mask2bbox-0.0.5/tests/test_mask2bbox/test_mask2bbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:22.098933 mask2bbox-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 12:59:11.000000 mask2bbox-0.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 12:59:11.000000 mask2bbox-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-08 12:59:22.098933 mask2bbox-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-08 12:59:11.000000 mask2bbox-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 12:59:22.098933 mask2bbox-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-08 12:59:11.000000 mask2bbox-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:22.094933 mask2bbox-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:22.094933 mask2bbox-0.0.6/src/mask2bbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 12:59:11.000000 mask2bbox-0.0.6/src/mask2bbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-05-08 12:59:11.000000 mask2bbox-0.0.6/src/mask2bbox/_bboxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-08 12:59:11.000000 mask2bbox-0.0.6/src/mask2bbox/mask2bbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:22.098933 mask2bbox-0.0.6/src/mask2bbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-08 12:59:22.000000 mask2bbox-0.0.6/src/mask2bbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 12:59:22.000000 mask2bbox-0.0.6/src/mask2bbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:59:22.000000 mask2bbox-0.0.6/src/mask2bbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-08 12:59:22.000000 mask2bbox-0.0.6/src/mask2bbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 12:59:22.000000 mask2bbox-0.0.6/src/mask2bbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:22.098933 mask2bbox-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:11.000000 mask2bbox-0.0.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:22.098933 mask2bbox-0.0.6/tests/test_mask2bbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:11.000000 mask2bbox-0.0.6/tests/test_mask2bbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-08 12:59:11.000000 mask2bbox-0.0.6/tests/test_mask2bbox/test_mask2bbox.py
```

### Comparing `mask2bbox-0.0.5/LICENSE.txt` & `mask2bbox-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mask2bbox-0.0.5/PKG-INFO` & `mask2bbox-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mask2bbox
-Version: 0.0.5
+Version: 0.0.6
 Summary: Gets the bounding boxes from a mask file.
 Home-page: https://github.com/SchapiroLabor/mask2bbox
 Author: Miguel Ibarra
 Author-email: c180l058j@mozmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # mask2bbox
+[![PyPI](https://img.shields.io/pypi/v/mask2bbox?style=flat-square)](https://pypi.org/project/mask2bbox/)
 
 For a given mask, gets the coordinates of bounding box of each element of the mask. It will also allow for more operations in the future.
 
 ## Instalation
 
 `pip install mask2bbox`
 
@@ -38,23 +39,23 @@
 all_boxes.remove_edge_boxes()
 
 # Get the area of all the bounding boxes
 araa = all_boxes.get_bbox_areas()
 
 # Get the dimensions on x and y of all the bounding boxes
 dims = all_boxes.get_bbox_dims()
- 
+
 # Get the center of all the bounding boxes
 centers = all_boxes.get_bbox_centers()
 
 # Get the ratio x/y of all the bounding boxes
 ratios = all_boxes.get_bbox_ratios()
 
 # Get the IoU matrix of all the bounding boxes
-iou = all_boxes.get_iou_matrix()
+iou = all_boxes.iou_matrix()
 
 # Save the IoU matrix to a csv file
 all_boxes.save_iou("path/to/save/iou.csv")
 
 # Plot the bounding boxes on the mask image
 all_boxes.plot_to_mask("path/to/save/image.png")
 
@@ -71,16 +72,16 @@
   - `boxes.are_overlaping()` - Returns identities where the IoU is greater than 0
   - `boxes.overlaping_pais()` - Returns the pairs of bounding boxes that are overlaping.
   - `boxes.save_iou()` - Saves the IoU matrix to a csv file.
 
 - Plots
   - `boxes.plot_to_mask()` Plots the bounding boxes on the mask image.
 
-#### Example of `boxes.plot_to_mask()` where only the overlaping masks are highlighted.
-![Plot](plot.png) 
+Example of `boxes.plot_to_mask()` where only the overlapping bounding boxes are highlighted.
+![](tests/plot.png)
 
 ### 0.0.4 - Added functionality
 Now is possible to extract:
 - Bounding boxes dimensions `BBoxes.get_bbox_dims()`
 - Bounding boxes area `BBoxes.get_bbox_areas()`
 - Bounding boxes center `BBoxes.get_bbox_centers()`
 - Bounding boxes ratios `BBoxes.get_bbox_ratios()`
```

### Comparing `mask2bbox-0.0.5/README.md` & `mask2bbox-0.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # mask2bbox
+[![PyPI](https://img.shields.io/pypi/v/mask2bbox?style=flat-square)](https://pypi.org/project/mask2bbox/)
 
 For a given mask, gets the coordinates of bounding box of each element of the mask. It will also allow for more operations in the future.
 
 ## Instalation
 
 `pip install mask2bbox`
 
@@ -21,23 +22,23 @@
 all_boxes.remove_edge_boxes()
 
 # Get the area of all the bounding boxes
 araa = all_boxes.get_bbox_areas()
 
 # Get the dimensions on x and y of all the bounding boxes
 dims = all_boxes.get_bbox_dims()
- 
+
 # Get the center of all the bounding boxes
 centers = all_boxes.get_bbox_centers()
 
 # Get the ratio x/y of all the bounding boxes
 ratios = all_boxes.get_bbox_ratios()
 
 # Get the IoU matrix of all the bounding boxes
-iou = all_boxes.get_iou_matrix()
+iou = all_boxes.iou_matrix()
 
 # Save the IoU matrix to a csv file
 all_boxes.save_iou("path/to/save/iou.csv")
 
 # Plot the bounding boxes on the mask image
 all_boxes.plot_to_mask("path/to/save/image.png")
 
@@ -54,16 +55,16 @@
   - `boxes.are_overlaping()` - Returns identities where the IoU is greater than 0
   - `boxes.overlaping_pais()` - Returns the pairs of bounding boxes that are overlaping.
   - `boxes.save_iou()` - Saves the IoU matrix to a csv file.
 
 - Plots
   - `boxes.plot_to_mask()` Plots the bounding boxes on the mask image.
 
-#### Example of `boxes.plot_to_mask()` where only the overlaping masks are highlighted.
-![Plot](plot.png) 
+Example of `boxes.plot_to_mask()` where only the overlapping bounding boxes are highlighted.
+![](tests/plot.png)
 
 ### 0.0.4 - Added functionality
 Now is possible to extract:
 - Bounding boxes dimensions `BBoxes.get_bbox_dims()`
 - Bounding boxes area `BBoxes.get_bbox_areas()`
 - Bounding boxes center `BBoxes.get_bbox_centers()`
 - Bounding boxes ratios `BBoxes.get_bbox_ratios()`
```

### Comparing `mask2bbox-0.0.5/setup.py` & `mask2bbox-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mask2bbox",
-    version="0.0.5",
+    version="0.0.6",
     description="Gets the bounding boxes from a mask file.",
     url="https://github.com/SchapiroLabor/mask2bbox",
     author="Miguel Ibarra",
     author_email="c180l058j@mozmail.com",
     license="MIT",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `mask2bbox-0.0.5/src/mask2bbox/_bboxes.py` & `mask2bbox-0.0.6/src/mask2bbox/_bboxes.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,17 +18,19 @@
         self.mask = io.imread(mask_file)
 
         # Get the shape of the mask image
         self.mask_shape = self.mask.shape
 
         # Get the bounding boxes
         self.bboxes = self._get_bboxes()
-        self.n = self.bboxes.shape[0]
 
-    def _get_bboxes(self):
+    def __len__(self) -> int:
+        return self.bboxes.shape[0]
+
+    def _get_bboxes(self) -> np.ndarray:
         """
         Calculates the bounding boxes from the mask file.
         :return: A numpy array with the bounding boxes.
         """
         # Get indexes of nonzero elements
         nonzero = np.array(np.nonzero(self.mask)).T
 
@@ -50,96 +52,94 @@
 
         # Since the bounding boxes are calculated from the group identities we can add column with the identities
         bboxes = np.column_stack((np.unique(stacked[:, 0]), bboxes))
 
         # Return the bounding boxes
         return bboxes
 
-    def expand(self, n):
+    def expand(self, n) -> None:
         # Expand the bounding boxes by n pixels, but not beyond the image size.
         self.bboxes = np.array(list(map(lambda x: np.array([x[0],
                                                             max(x[1] - n, 0),
                                                             min(x[2] + n, self.mask_shape[0]),
                                                             max(x[3] - n, 0),
                                                             min(x[4] + n, self.mask_shape[1])]), self.bboxes)))
 
-    def remove_edge_boxes(self):
+    def remove_edge_boxes(self) -> None:
         # Removes the bonds that are on the edge of the image
         self.bboxes = self.bboxes[np.where((self.bboxes[:, 1] > 0) &
                                            (self.bboxes[:, 2] < self.mask_shape[0]) &
                                            (self.bboxes[:, 3] > 0) &
                                            (self.bboxes[:, 4] < self.mask_shape[1]))]
-        self.n = self.bboxes.shape[0]
 
-    def get_bbox_dims(self):
+    def get_bbox_dims(self) -> np.ndarray:
         # Get the sides of the bounding boxes
         return np.array([self.bboxes[:, 0],
                          self.bboxes[:, 2] - self.bboxes[:, 1],
                          self.bboxes[:, 4] - self.bboxes[:, 3]]).T
 
-    def get_bbox_areas(self):
+    def get_bbox_areas(self) -> np.ndarray:
         # Get the areas of the bounding boxes
         return np.array([self.bboxes[:, 0],
                          (self.bboxes[:, 2] - self.bboxes[:, 1]) *
                          (self.bboxes[:, 4] - self.bboxes[:, 3])]).T
 
-    def get_bbox_ratios(self):
+    def get_bbox_ratios(self) -> np.ndarray:
         # Get the aspect ratios of the bounding boxes
         ratios = np.array((self.bboxes[:, 2] - self.bboxes[:, 1]) / (self.bboxes[:, 4] - self.bboxes[:, 3]))
 
         return np.array(([self.bboxes[:, 0], ratios]))
 
-    def get_bbox_centers(self):
+    def get_bbox_centers(self) -> np.ndarray:
         # Get the centers of the bounding boxes
         return np.array([self.bboxes[:, 0],
                          (self.bboxes[:, 2] + self.bboxes[:, 1]) // 2,
                          (self.bboxes[:, 4] + self.bboxes[:, 3]) // 2]).T
 
-    def is_area_smaller_than(self, area):
+    def is_area_smaller_than(self, area) -> ndarray:
         # Get areas of the bounding boxes
         areas = self.get_bbox_areas()
 
         # Get the identities of the bounding boxes that have an area smaller than the area parameter
         identities = areas[np.where(areas[:, 1] < area)[0], 0]
 
         return identities
 
-    def is_area_larger_than(self, area):
+    def is_area_larger_than(self, area) -> ndarray:
         # Get areas of the bounding boxes
         areas = self.get_bbox_areas()
 
         # Get the identities of the bounding boxes that have an area bigger than the area parameter
         identities = areas[np.where(areas[:, 1] >= area)[0], 0]
 
         return identities
 
-    def are_dims_smaller_than(self, dims):
+    def are_dims_smaller_than(self, dims) -> ndarray:
         # Get dimensions of the bounding boxes
         dimensions = self.get_bbox_dims()
 
         # Get the identities of the bounding boxes that have a dimension smaller than the dims parameter
         identities = dimensions[np.where((dimensions[:, 1] < dims[0]) & (dimensions[:, 2] < dims[1]))[0], 0]
 
         return identities
 
-    def are_dims_larger_than(self, dims):
+    def are_dims_larger_than(self, dims) -> np.ndarray:
         # Get dimensions of the bounding boxes
         dimensions = self.get_bbox_dims()
 
         # Get the identities of the bounding boxes that have a dimension bigger than the dims parameter
         identities = dimensions[np.where((dimensions[:, 1] >= dims[0]) & (dimensions[:, 2] > dims[1]))[0], 0]
 
         return identities
 
-    def filter_identities(self, identities):
+    def filter_identities(self, identities) -> None:
         # Get only the bounding boxes of the specific identity
         self.bboxes = self.bboxes[np.where(np.isin(self.bboxes[:, 0], identities))]
-        self.n = self.bboxes.shape[0]
 
-    def plot_to_mask(self, output_file=None):
+    def plot_to_mask(self, output_file=None) -> None:
         # Get the ratio of the mask
         mask_ratio = self.mask_shape[0] / self.mask_shape[1]
 
         # Draw the bounding boxes on the mask
         fig, ax = plt.subplots(1, 1, figsize=(10, mask_ratio * 10))
         ax.imshow(self.mask, cmap="gray")
 
@@ -155,15 +155,15 @@
         # If not path is given, show the plot
         if output_file is not None:
             plt.savefig(output_file)
         else:
             plt.show()
 
     @staticmethod
-    def iou(box1, box2):
+    def iou(box1, box2) -> float:
         # Calculate the intersection box
         x1 = max(box1[1], box2[1])
         x2 = min(box1[2], box2[2])
         y1 = max(box1[3], box2[3])
         y2 = min(box1[4], box2[4])
 
         # Calculate intersection area
@@ -173,51 +173,57 @@
         area1 = (box1[3] - box1[1]) * (box1[4] - box1[2])
         area2 = (box2[3] - box2[1]) * (box2[4] - box2[2])
         union = area1 + area2 - intersection
 
         # Calculate and return IoU
         return intersection / union
 
-    def get_iou_matrix(self) -> ndarray:
+    @property
+    def iou_matrix(self) -> ndarray:
+        n = self.__len__()
         # compute the size of the matrix based on the length of the array
-        size = self.n * (self.n - 1) // 2
+        size = n * (n - 1) // 2
 
         # create a 1D array of zeros to hold the upper triangular matrix
         triangular = np.zeros(size)
 
         # fill the upper triangular matrix with elements from the original array
         k = 0
-        for i in range(self.n):
-            for j in range(i + 1, self.n):
+        for i in range(n):
+            for j in range(i + 1, n):
                 triangular[k] = self.iou(self.bboxes[i], self.bboxes[j])
                 k += 1
 
         # convert the 1D array to a 2D matrix
-        matrix: ndarray = np.zeros((self.n, self.n))
-        matrix[np.triu_indices(self.n, k=1)] = triangular
+        matrix: ndarray = np.zeros((n, n))
+        matrix[np.triu_indices(n, k=1)] = triangular
 
         return matrix
 
-    def are_overlapping(self):
+    def are_overlapping(self) -> ndarray:
         # Get the IoU matrix
-        overlapping = np.where(self.get_iou_matrix() > 0)
+        overlapping = np.where(self.iou_matrix > 0)
 
         # Get the identities from the overlapping indexes
         identities = self.bboxes[np.unique(overlapping), 0]
 
         return identities
 
-    def overlapping_pairs(self):
+    def overlapping_pairs(self) -> (ndarray, ndarray):
         # Get the IoU matrix
-        x, y = np.where(self.get_iou_matrix() > 0)
+        iou_matrix = self.iou_matrix
+
+        # Get elements that are not zero
+        x, y = np.where(iou_matrix > 0)
+        v = iou_matrix[x, y]
         x = self.bboxes[x, 0]
         y = self.bboxes[y, 0]
 
-        return np.array([x, y]).T
+        return np.array([x, y]).T, v
 
-    def save_iou(self, output_file):
+    def save_iou(self, output_file: str) -> None:
         # Save the IoU matrix to a csv file
-        np.savetxt(output_file, self.get_iou_matrix(), delimiter=",")
+        np.savetxt(output_file, self.iou_matrix, delimiter=",")
 
-    def save_csv(self, output_file):
+    def save_csv(self, output_file: str) -> None:
         # Save the bounding boxes to a csv file
         np.savetxt(output_file, self.bboxes, delimiter=",", fmt="%d")
```

### Comparing `mask2bbox-0.0.5/src/mask2bbox/mask2bbox.py` & `mask2bbox-0.0.6/src/mask2bbox/mask2bbox.py`

 * *Files identical despite different names*

### Comparing `mask2bbox-0.0.5/src/mask2bbox.egg-info/PKG-INFO` & `mask2bbox-0.0.6/src/mask2bbox.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mask2bbox
-Version: 0.0.5
+Version: 0.0.6
 Summary: Gets the bounding boxes from a mask file.
 Home-page: https://github.com/SchapiroLabor/mask2bbox
 Author: Miguel Ibarra
 Author-email: c180l058j@mozmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # mask2bbox
+[![PyPI](https://img.shields.io/pypi/v/mask2bbox?style=flat-square)](https://pypi.org/project/mask2bbox/)
 
 For a given mask, gets the coordinates of bounding box of each element of the mask. It will also allow for more operations in the future.
 
 ## Instalation
 
 `pip install mask2bbox`
 
@@ -38,23 +39,23 @@
 all_boxes.remove_edge_boxes()
 
 # Get the area of all the bounding boxes
 araa = all_boxes.get_bbox_areas()
 
 # Get the dimensions on x and y of all the bounding boxes
 dims = all_boxes.get_bbox_dims()
- 
+
 # Get the center of all the bounding boxes
 centers = all_boxes.get_bbox_centers()
 
 # Get the ratio x/y of all the bounding boxes
 ratios = all_boxes.get_bbox_ratios()
 
 # Get the IoU matrix of all the bounding boxes
-iou = all_boxes.get_iou_matrix()
+iou = all_boxes.iou_matrix()
 
 # Save the IoU matrix to a csv file
 all_boxes.save_iou("path/to/save/iou.csv")
 
 # Plot the bounding boxes on the mask image
 all_boxes.plot_to_mask("path/to/save/image.png")
 
@@ -71,16 +72,16 @@
   - `boxes.are_overlaping()` - Returns identities where the IoU is greater than 0
   - `boxes.overlaping_pais()` - Returns the pairs of bounding boxes that are overlaping.
   - `boxes.save_iou()` - Saves the IoU matrix to a csv file.
 
 - Plots
   - `boxes.plot_to_mask()` Plots the bounding boxes on the mask image.
 
-#### Example of `boxes.plot_to_mask()` where only the overlaping masks are highlighted.
-![Plot](plot.png) 
+Example of `boxes.plot_to_mask()` where only the overlapping bounding boxes are highlighted.
+![](tests/plot.png)
 
 ### 0.0.4 - Added functionality
 Now is possible to extract:
 - Bounding boxes dimensions `BBoxes.get_bbox_dims()`
 - Bounding boxes area `BBoxes.get_bbox_areas()`
 - Bounding boxes center `BBoxes.get_bbox_centers()`
 - Bounding boxes ratios `BBoxes.get_bbox_ratios()`
```

