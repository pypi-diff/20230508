# Comparing `tmp/napari-sam-0.4.6.tar.gz` & `tmp/napari-sam-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sam-0.4.6.tar", last modified: Fri May  5 12:35:57 2023, max compression
+gzip compressed data, was "napari-sam-0.4.7.tar", last modified: Mon May  8 12:07:19 2023, max compression
```

## Comparing `napari-sam-0.4.6.tar` & `napari-sam-0.4.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:35:57.075731 napari-sam-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-05 12:35:37.000000 napari-sam-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 12:35:37.000000 napari-sam-0.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-05 12:35:57.079731 napari-sam-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-05 12:35:37.000000 napari-sam-0.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 12:35:37.000000 napari-sam-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-05 12:35:57.079731 napari-sam-0.4.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:35:57.075731 napari-sam-0.4.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:35:57.075731 napari-sam-0.4.6/src/napari_sam/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-05 12:35:37.000000 napari-sam-0.4.6/src/napari_sam/QCollapsibleBox.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-05 12:35:37.000000 napari-sam-0.4.6/src/napari_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65134 2023-05-05 12:35:37.000000 napari-sam-0.4.6/src/napari_sam/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-05 12:35:37.000000 napari-sam-0.4.6/src/napari_sam/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-05 12:35:37.000000 napari-sam-0.4.6/src/napari_sam/slicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-05 12:35:37.000000 napari-sam-0.4.6/src/napari_sam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:35:57.075731 napari-sam-0.4.6/src/napari_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-05 12:35:57.000000 napari-sam-0.4.6/src/napari_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-05 12:35:57.000000 napari-sam-0.4.6/src/napari_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:35:57.000000 napari-sam-0.4.6/src/napari_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-05 12:35:57.000000 napari-sam-0.4.6/src/napari_sam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-05 12:35:57.000000 napari-sam-0.4.6/src/napari_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 12:35:57.000000 napari-sam-0.4.6/src/napari_sam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:07:19.217528 napari-sam-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-08 12:06:59.000000 napari-sam-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-08 12:06:59.000000 napari-sam-0.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-08 12:07:19.217528 napari-sam-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-08 12:06:59.000000 napari-sam-0.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-08 12:06:59.000000 napari-sam-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-08 12:07:19.217528 napari-sam-0.4.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:07:19.209528 napari-sam-0.4.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:07:19.213528 napari-sam-0.4.7/src/napari_sam/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-08 12:06:59.000000 napari-sam-0.4.7/src/napari_sam/QCollapsibleBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 12:06:59.000000 napari-sam-0.4.7/src/napari_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66801 2023-05-08 12:06:59.000000 napari-sam-0.4.7/src/napari_sam/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-08 12:06:59.000000 napari-sam-0.4.7/src/napari_sam/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-08 12:06:59.000000 napari-sam-0.4.7/src/napari_sam/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-08 12:06:59.000000 napari-sam-0.4.7/src/napari_sam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:07:19.217528 napari-sam-0.4.7/src/napari_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-08 12:07:19.000000 napari-sam-0.4.7/src/napari_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-08 12:07:19.000000 napari-sam-0.4.7/src/napari_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:07:19.000000 napari-sam-0.4.7/src/napari_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-08 12:07:19.000000 napari-sam-0.4.7/src/napari_sam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-08 12:07:19.000000 napari-sam-0.4.7/src/napari_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 12:07:19.000000 napari-sam-0.4.7/src/napari_sam.egg-info/top_level.txt
```

### Comparing `napari-sam-0.4.6/LICENSE` & `napari-sam-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.6/PKG-INFO` & `napari-sam-0.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.4.6
+Version: 0.4.7
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

### Comparing `napari-sam-0.4.6/README.md` & `napari-sam-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.6/setup.cfg` & `napari-sam-0.4.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.6/src/napari_sam/QCollapsibleBox.py` & `napari-sam-0.4.7/src/napari_sam/QCollapsibleBox.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.6/src/napari_sam/_widget.py` & `napari-sam-0.4.7/src/napari_sam/_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -577,14 +577,31 @@
     def _activate(self):
         self.btn_activate.setEnabled(False)
         if not self.is_active:
             self.image_name = self.cb_image_layers.currentText()
             self.image_layer = self.viewer.layers[self.cb_image_layers.currentText()]
             self.label_layer = self.viewer.layers[self.cb_label_layers.currentText()]
             self.label_layer_changes = None
+            # Fixes shape adjustment by napari
+            self.image_layer_affine_scale = self.image_layer.affine.scale
+            self.image_layer_scale = self.image_layer.scale
+            self.image_layer_scale_factor = self.image_layer.scale_factor
+            self.label_layer_affine_scale = self.label_layer.affine.scale
+            self.label_layer_scale = self.label_layer.scale
+            self.label_layer_scale_factor = self.label_layer.scale_factor
+            self.image_layer.affine.scale = np.array([1, 1, 1])
+            self.image_layer.scale = np.array([1, 1, 1])
+            self.image_layer.scale_factor = 1
+            self.label_layer.affine.scale = np.array([1, 1, 1])
+            self.label_layer.scale = np.array([1, 1, 1])
+            self.label_layer.scale_factor = 1
+            pos = self.viewer.dims.point
+            self.viewer.dims.set_point(0, 0)
+            self.viewer.dims.set_point(0, pos[0])
+            self.viewer.reset_view()
 
             if self.image_layer.ndim != 2 and self.image_layer.ndim != 3:
                 raise RuntimeError("Only 2D and 3D images are supported.")
 
             if self.image_layer.ndim == 2:
                 self.sam_logits = None
             else:
@@ -628,16 +645,19 @@
                 if self.viewer.layers.selection.active != self.points_layer:
                     selected_layer = self.viewer.layers.selection.active
                 self.bbox_layer = self.viewer.add_shapes(name=self.bbox_layer_name)
                 if selected_layer is not None:
                     self.viewer.layers.selection.active = selected_layer
                 if self.image_layer.ndim == 3:
                     self.check_auto_inc_bbox.setChecked(False)
-                    # This tries to fix the problem that the first drawn bbox is not visible. Fix does not really work though...
+                    # This "fixes" the problem that the first drawn bbox is not visible.
                     self.update_bbox_layer({}, bbox_tmp=[[self.viewer.dims.current_step[0], 0, 0], [self.viewer.dims.current_step[0], 0, 10], [self.viewer.dims.current_step[0], 10, 10], [self.viewer.dims.current_step[0], 10, 0]])
+                    self.update_bbox_layer({}, bbox_tmp=None)
+                    self.viewer.dims.set_point(0, 0)
+                    self.viewer.dims.set_point(0, pos[0])
                 self.bbox_layer.editable = False
                 self.bbox_first_coords = None
                 self.prev_segmentation_mode = SegmentationMode.SEMANTIC
 
                 if self.image_layer.ndim == 2:
                     self.point_size = int(np.min(self.image_layer.data.shape[:2]) / 100)
                     if self.point_size == 0:
@@ -707,14 +727,25 @@
         self.cb_label_layers.setEnabled(True)
         self.btn_mode_switch.setEnabled(False)
         self.btn_mode_switch.setText("Switch to BBox Mode")
         self.check_prev_mask.setEnabled(False)
         self.check_auto_inc_bbox.setEnabled(False)
         self.prev_segmentation_mode = SegmentationMode.SEMANTIC
         self.annotator_mode = AnnotatorMode.CLICK
+
+        # Undo: Fixes shape adjustment by napari  # TODO: Not working correctly atm
+        # self.image_layer.affine.scale = self.image_layer_affine_scale
+        # self.image_layer.scale = self.image_layer_scale
+        # self.image_layer.scale_factor = self.image_layer_scale_factor
+        # self.label_layer.affine.scale = self.label_layer_affine_scale
+        # self.label_layer.scale = self.label_layer_scale
+        # self.label_layer.scale_factor = self.label_layer_scale_factor
+        # self.image_layer.refresh()
+        # self.label_layer.refresh()
+
         self.remove_all_widget_callbacks(self.viewer)
         if self.label_layer is not None:
             self.remove_all_widget_callbacks(self.label_layer)
         if self.points_layer is not None and self.points_layer in self.viewer.layers:
             self.viewer.layers.remove(self.points_layer)
         if self.bbox_layer is not None and self.bbox_layer in self.viewer.layers:
             self.viewer.layers.remove(self.bbox_layer)
```

### Comparing `napari-sam-0.4.6/src/napari_sam/slicer.py` & `napari-sam-0.4.7/src/napari_sam/slicer.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.6/src/napari_sam/utils.py` & `napari-sam-0.4.7/src/napari_sam/utils.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.6/src/napari_sam.egg-info/PKG-INFO` & `napari-sam-0.4.7/src/napari_sam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.4.6
+Version: 0.4.7
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

