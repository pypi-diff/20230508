# Comparing `tmp/cameramodels-0.2.8.tar.gz` & `tmp/cameramodels-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cameramodels-0.2.8.tar", last modified: Tue Sep  6 08:31:27 2022, max compression
+gzip compressed data, was "cameramodels-0.2.9.tar", last modified: Fri Sep  9 16:15:31 2022, max compression
```

## Comparing `cameramodels-0.2.8.tar` & `cameramodels-0.2.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 08:31:27.426450 cameramodels-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-09-06 08:31:17.000000 cameramodels-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-06 08:31:17.000000 cameramodels-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1334 2022-09-06 08:31:27.426450 cameramodels-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-09-06 08:31:17.000000 cameramodels-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 08:31:27.422450 cameramodels-0.2.8/cameramodels/
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-09-06 08:31:17.000000 cameramodels-0.2.8/cameramodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1634 2022-09-06 08:31:17.000000 cameramodels-0.2.8/cameramodels/align.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 08:31:27.422450 cameramodels-0.2.8/cameramodels/data/
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-09-06 08:31:17.000000 cameramodels-0.2.8/cameramodels/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 08:31:27.422450 cameramodels-0.2.8/cameramodels/data/kinect_v2/
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-09-06 08:31:17.000000 cameramodels-0.2.8/cameramodels/data/kinect_v2/camera_info.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   291867 2022-09-06 08:31:17.000000 cameramodels-0.2.8/cameramodels/data/kinect_v2/hd.jpg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 08:31:27.422450 cameramodels-0.2.8/cameramodels/io/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-09-06 08:31:17.000000 cameramodels-0.2.8/cameramodels/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-09-06 08:31:17.000000 cameramodels-0.2.8/cameramodels/io/honnotate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 08:31:27.422450 cameramodels-0.2.8/cameramodels/models/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-06 08:31:17.000000 cameramodels-0.2.8/cameramodels/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4058 2022-09-06 08:31:17.000000 cameramodels-0.2.8/cameramodels/models/azure_kinect.py
--rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-09-06 08:31:17.000000 cameramodels-0.2.8/cameramodels/models/d415.py
--rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-09-06 08:31:17.000000 cameramodels-0.2.8/cameramodels/models/d435.py
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-09-06 08:31:17.000000 cameramodels-0.2.8/cameramodels/models/kinect_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-09-06 08:31:17.000000 cameramodels-0.2.8/cameramodels/models/xtion.py
--rw-r--r--   0 runner    (1001) docker     (121)    52807 2022-09-06 08:31:17.000000 cameramodels-0.2.8/cameramodels/pinhole_camera.py
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-09-06 08:31:17.000000 cameramodels-0.2.8/cameramodels/rgbd_camera.py
--rw-r--r--   0 runner    (1001) docker     (121)     6307 2022-09-06 08:31:17.000000 cameramodels-0.2.8/cameramodels/stereo_camera.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 08:31:27.422450 cameramodels-0.2.8/cameramodels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1334 2022-09-06 08:31:27.000000 cameramodels-0.2.8/cameramodels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-09-06 08:31:27.000000 cameramodels-0.2.8/cameramodels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 08:31:27.000000 cameramodels-0.2.8/cameramodels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 08:31:27.000000 cameramodels-0.2.8/cameramodels.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-09-06 08:31:27.000000 cameramodels-0.2.8/cameramodels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-09-06 08:31:27.000000 cameramodels-0.2.8/cameramodels.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-09-06 08:31:27.426450 cameramodels-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2080 2022-09-06 08:31:17.000000 cameramodels-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 08:31:27.426450 cameramodels-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-06 08:31:17.000000 cameramodels-0.2.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 08:31:27.426450 cameramodels-0.2.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-06 08:31:17.000000 cameramodels-0.2.8/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-09-06 08:31:17.000000 cameramodels-0.2.8/tests/data/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 08:31:27.426450 cameramodels-0.2.8/tests/io/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-06 08:31:17.000000 cameramodels-0.2.8/tests/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-09-06 08:31:17.000000 cameramodels-0.2.8/tests/io/test_honnotate.py
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-09-06 08:31:17.000000 cameramodels-0.2.8/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-09-06 08:31:17.000000 cameramodels-0.2.8/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)    10348 2022-09-06 08:31:17.000000 cameramodels-0.2.8/tests/test_pinhole_camera.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 16:15:31.745903 cameramodels-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-09-09 16:15:23.000000 cameramodels-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-09 16:15:23.000000 cameramodels-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1334 2022-09-09 16:15:31.745903 cameramodels-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      539 2022-09-09 16:15:23.000000 cameramodels-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 16:15:31.745903 cameramodels-0.2.9/cameramodels/
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-09-09 16:15:23.000000 cameramodels-0.2.9/cameramodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1634 2022-09-09 16:15:23.000000 cameramodels-0.2.9/cameramodels/align.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 16:15:31.745903 cameramodels-0.2.9/cameramodels/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-09-09 16:15:23.000000 cameramodels-0.2.9/cameramodels/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 16:15:31.745903 cameramodels-0.2.9/cameramodels/data/kinect_v2/
+-rw-r--r--   0 runner    (1001) docker     (121)      683 2022-09-09 16:15:23.000000 cameramodels-0.2.9/cameramodels/data/kinect_v2/camera_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)   291867 2022-09-09 16:15:23.000000 cameramodels-0.2.9/cameramodels/data/kinect_v2/hd.jpg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 16:15:31.745903 cameramodels-0.2.9/cameramodels/io/
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-09-09 16:15:23.000000 cameramodels-0.2.9/cameramodels/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-09-09 16:15:23.000000 cameramodels-0.2.9/cameramodels/io/honnotate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 16:15:31.745903 cameramodels-0.2.9/cameramodels/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-09 16:15:23.000000 cameramodels-0.2.9/cameramodels/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4058 2022-09-09 16:15:23.000000 cameramodels-0.2.9/cameramodels/models/azure_kinect.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-09-09 16:15:23.000000 cameramodels-0.2.9/cameramodels/models/d415.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-09-09 16:15:23.000000 cameramodels-0.2.9/cameramodels/models/d435.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-09-09 16:15:23.000000 cameramodels-0.2.9/cameramodels/models/kinect_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      841 2022-09-09 16:15:23.000000 cameramodels-0.2.9/cameramodels/models/xtion.py
+-rw-r--r--   0 runner    (1001) docker     (121)    53556 2022-09-09 16:15:23.000000 cameramodels-0.2.9/cameramodels/pinhole_camera.py
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-09-09 16:15:23.000000 cameramodels-0.2.9/cameramodels/rgbd_camera.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6307 2022-09-09 16:15:23.000000 cameramodels-0.2.9/cameramodels/stereo_camera.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 16:15:31.745903 cameramodels-0.2.9/cameramodels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1334 2022-09-09 16:15:31.000000 cameramodels-0.2.9/cameramodels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      934 2022-09-09 16:15:31.000000 cameramodels-0.2.9/cameramodels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-09 16:15:31.000000 cameramodels-0.2.9/cameramodels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-09 16:15:31.000000 cameramodels-0.2.9/cameramodels.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2022-09-09 16:15:31.000000 cameramodels-0.2.9/cameramodels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-09-09 16:15:31.000000 cameramodels-0.2.9/cameramodels.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2022-09-09 16:15:31.749903 cameramodels-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2080 2022-09-09 16:15:23.000000 cameramodels-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 16:15:31.745903 cameramodels-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 16:15:23.000000 cameramodels-0.2.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 16:15:31.745903 cameramodels-0.2.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 16:15:23.000000 cameramodels-0.2.9/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2022-09-09 16:15:23.000000 cameramodels-0.2.9/tests/data/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 16:15:31.745903 cameramodels-0.2.9/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 16:15:23.000000 cameramodels-0.2.9/tests/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      327 2022-09-09 16:15:23.000000 cameramodels-0.2.9/tests/io/test_honnotate.py
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2022-09-09 16:15:23.000000 cameramodels-0.2.9/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (121)      822 2022-09-09 16:15:23.000000 cameramodels-0.2.9/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10348 2022-09-09 16:15:23.000000 cameramodels-0.2.9/tests/test_pinhole_camera.py
```

### Comparing `cameramodels-0.2.8/LICENSE` & `cameramodels-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cameramodels-0.2.8/PKG-INFO` & `cameramodels-0.2.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cameramodels
-Version: 0.2.8
+Version: 0.2.9
 Summary: A python library for cameramodels
 Home-page: https://github.com/iory/cameramodels
 Author: iory
 Author-email: ab.ioryz@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cameramodels Version: 0.2.8 Summary: A python
+Metadata-Version: 2.1 Name: cameramodels Version: 0.2.9 Summary: A python
 library for cameramodels Home-page: https://github.com/iory/cameramodels
 Author: iory Author-email: ab.ioryz@gmail.com License: MIT Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 2.7 Classifier: Programming Language ::
 Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
```

### Comparing `cameramodels-0.2.8/README.md` & `cameramodels-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `cameramodels-0.2.8/cameramodels/align.py` & `cameramodels-0.2.9/cameramodels/align.py`

 * *Files identical despite different names*

### Comparing `cameramodels-0.2.8/cameramodels/data/kinect_v2/camera_info.yaml` & `cameramodels-0.2.9/cameramodels/data/kinect_v2/camera_info.yaml`

 * *Files identical despite different names*

### Comparing `cameramodels-0.2.8/cameramodels/data/kinect_v2/hd.jpg` & `cameramodels-0.2.9/cameramodels/data/kinect_v2/hd.jpg`

 * *Files identical despite different names*

### Comparing `cameramodels-0.2.8/cameramodels/io/honnotate.py` & `cameramodels-0.2.9/cameramodels/io/honnotate.py`

 * *Files identical despite different names*

### Comparing `cameramodels-0.2.8/cameramodels/models/azure_kinect.py` & `cameramodels-0.2.9/cameramodels/models/azure_kinect.py`

 * *Files identical despite different names*

### Comparing `cameramodels-0.2.8/cameramodels/models/d415.py` & `cameramodels-0.2.9/cameramodels/models/d415.py`

 * *Files identical despite different names*

### Comparing `cameramodels-0.2.8/cameramodels/models/d435.py` & `cameramodels-0.2.9/cameramodels/models/d435.py`

 * *Files identical despite different names*

### Comparing `cameramodels-0.2.8/cameramodels/models/kinect_v2.py` & `cameramodels-0.2.9/cameramodels/models/kinect_v2.py`

 * *Files identical despite different names*

### Comparing `cameramodels-0.2.8/cameramodels/models/xtion.py` & `cameramodels-0.2.9/cameramodels/models/xtion.py`

 * *Files identical despite different names*

### Comparing `cameramodels-0.2.8/cameramodels/pinhole_camera.py` & `cameramodels-0.2.9/cameramodels/pinhole_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -1574,31 +1574,56 @@
                [100,   2]])
         """
         flat_pixel_locations = np.array(flat_pixel_locations, dtype=np.int64)
         return np.hstack([
             (flat_pixel_locations % self.width).reshape(-1, 1),
             (flat_pixel_locations.T // self.width).reshape(-1, 1)])
 
-    def dump(self, output_filepath):
+    def dump(self, output_filepath, save_original=True):
         """Dump this camera's parameter to yaml file.
 
         Parameters
         ----------
         output_filepath : str or pathlib.Path
             output path
+        save_original : bool
+            If `False`, save resized camera info.
         """
+        if save_original is True:
+            width = self._full_width
+            height = self._full_height
+            K = self.full_K
+            P = self.full_P
+            binning_x = self._binning_x
+            binning_y = self._binning_y
+            x_offset = self.roi[1]
+            y_offset = self.roi[0]
+            roi_height = self.roi[2] - self.roi[0]
+            roi_width = self.roi[3] - self.roi[1]
+        else:
+            width = int(self._width / self._binning_x)
+            height = int(self._height / self._binning_y)
+            K = self.K
+            P = self.P
+            binning_x = 1
+            binning_y = 1
+            x_offset = 0
+            y_offset = 0
+            roi_height = 0
+            roi_width = 0
+
         camera_data = "\n".join([
-                "image_width: %d" % self._full_width,
-                "image_height: %d" % self._full_height,
+                "image_width: %d" % width,
+                "image_height: %d" % height,
                 "camera_name: " + self.name,
                 "camera_matrix:",
                 "  rows: 3",
                 "  cols: 3",
                 "  data: " + format_mat(
-                    np.array(self.full_K.reshape(-1), dtype=np.float64), 5),
+                    np.array(K.reshape(-1), dtype=np.float64), 5),
                 "distortion_model: " + self.distortion_model,
                 "distortion_coefficients:",
                 "  rows: 1",
                 "  cols: %d" % len(self.D),
                 "  data: [%s]" % ", ".join(
                     "%8f" % x
                     for x in self.D),
@@ -1607,22 +1632,22 @@
                 "  cols: 3",
                 "  data: " + format_mat(
                     np.array(self.R.reshape(-1), dtype=np.float64), 8),
                 "projection_matrix:",
                 "  rows: 3",
                 "  cols: 4",
                 "  data: " + format_mat(
-                    np.array(self.full_P.reshape(-1), dtype=np.float64), 5),
-                "binning_x: %f" % self._binning_x,
-                "binning_y: %f" % self._binning_y,
+                    np.array(P.reshape(-1), dtype=np.float64), 5),
+                "binning_x: %f" % binning_x,
+                "binning_y: %f" % binning_y,
                 "roi:",
-                "  x_offset: %d" % self.roi[1],
-                "  y_offset: %d" % self.roi[0],
-                "  height: %d" % (self.roi[2] - self.roi[0]),
-                "  width: %d" % (self.roi[3] - self.roi[1]),
+                "  x_offset: %d" % x_offset,
+                "  y_offset: %d" % y_offset,
+                "  height: %d" % roi_height,
+                "  width: %d" % roi_width,
                 ""
             ])
         with open(str(output_filepath), 'w') as f:
             f.write(camera_data)
 
     def draw_roi(self, bgr_img, color=(46, 204, 113),
                  box_width=None, copy=False):
```

### Comparing `cameramodels-0.2.8/cameramodels/stereo_camera.py` & `cameramodels-0.2.9/cameramodels/stereo_camera.py`

 * *Files identical despite different names*

### Comparing `cameramodels-0.2.8/cameramodels.egg-info/PKG-INFO` & `cameramodels-0.2.9/cameramodels.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cameramodels
-Version: 0.2.8
+Version: 0.2.9
 Summary: A python library for cameramodels
 Home-page: https://github.com/iory/cameramodels
 Author: iory
 Author-email: ab.ioryz@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cameramodels Version: 0.2.8 Summary: A python
+Metadata-Version: 2.1 Name: cameramodels Version: 0.2.9 Summary: A python
 library for cameramodels Home-page: https://github.com/iory/cameramodels
 Author: iory Author-email: ab.ioryz@gmail.com License: MIT Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 2.7 Classifier: Programming Language ::
 Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
```

### Comparing `cameramodels-0.2.8/cameramodels.egg-info/SOURCES.txt` & `cameramodels-0.2.9/cameramodels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cameramodels-0.2.8/setup.py` & `cameramodels-0.2.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess
 import sys
 
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = '0.2.8'
+version = '0.2.9'
 
 
 if sys.argv[-1] == 'release':
     # Release via github-actions.
     commands = [
         'git tag v{:s}'.format(version),
         'git push origin master --tag',
```

### Comparing `cameramodels-0.2.8/tests/test_align.py` & `cameramodels-0.2.9/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `cameramodels-0.2.8/tests/test_models.py` & `cameramodels-0.2.9/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `cameramodels-0.2.8/tests/test_pinhole_camera.py` & `cameramodels-0.2.9/tests/test_pinhole_camera.py`

 * *Files identical despite different names*

