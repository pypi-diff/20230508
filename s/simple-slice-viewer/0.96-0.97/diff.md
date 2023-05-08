# Comparing `tmp/simple-slice-viewer-0.96.tar.gz` & `tmp/simple-slice-viewer-0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-slice-viewer-0.96.tar", last modified: Tue Jan  3 14:23:22 2023, max compression
+gzip compressed data, was "simple-slice-viewer-0.97.tar", last modified: Mon May  8 08:52:21 2023, max compression
```

## Comparing `simple-slice-viewer-0.96.tar` & `simple-slice-viewer-0.97.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-01-03 14:23:22.281205 simple-slice-viewer-0.96/
--rw-rw-rw-   0        0        0     2158 2023-01-03 14:23:22.281205 simple-slice-viewer-0.96/PKG-INFO
--rw-rw-rw-   0        0        0     1580 2022-12-13 15:46:57.000000 simple-slice-viewer-0.96/README.md
--rw-rw-rw-   0        0        0       42 2023-01-03 14:23:22.281205 simple-slice-viewer-0.96/setup.cfg
--rw-rw-rw-   0        0        0     1679 2023-01-03 14:21:39.000000 simple-slice-viewer-0.96/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-03 14:23:22.264799 simple-slice-viewer-0.96/simple_slice_viewer/
--rw-rw-rw-   0        0        0      582 2022-12-13 15:46:57.000000 simple-slice-viewer-0.96/simple_slice_viewer/__init__.py
--rw-rw-rw-   0        0        0      960 2023-01-03 14:09:51.000000 simple-slice-viewer-0.96/simple_slice_viewer/console.py
--rw-rw-rw-   0        0        0    23923 2023-01-03 14:09:51.000000 simple-slice-viewer-0.96/simple_slice_viewer/controller.py
--rw-rw-rw-   0        0        0     2365 2023-01-03 13:57:50.000000 simple-slice-viewer-0.96/simple_slice_viewer/controller_base.py
--rw-rw-rw-   0        0        0    18911 2023-01-03 14:16:41.000000 simple-slice-viewer-0.96/simple_slice_viewer/load_pet_view.py
--rw-rw-rw-   0        0        0     2271 2022-10-05 17:39:02.000000 simple-slice-viewer-0.96/simple_slice_viewer/logger.py
--rw-rw-rw-   0        0        0     6497 2023-01-03 14:16:41.000000 simple-slice-viewer-0.96/simple_slice_viewer/menus.py
--rw-rw-rw-   0        0        0    14939 2023-01-03 14:16:41.000000 simple-slice-viewer-0.96/simple_slice_viewer/model.py
--rw-rw-rw-   0        0        0     8103 2023-01-03 14:16:41.000000 simple-slice-viewer-0.96/simple_slice_viewer/movie_maker.py
--rw-rw-rw-   0        0        0    14024 2023-01-03 14:16:41.000000 simple-slice-viewer-0.96/simple_slice_viewer/preset_controllers.py
--rw-rw-rw-   0        0        0    15182 2023-01-03 14:06:41.000000 simple-slice-viewer-0.96/simple_slice_viewer/preset_model.py
--rw-rw-rw-   0        0        0    19472 2023-01-03 14:17:04.000000 simple-slice-viewer-0.96/simple_slice_viewer/preset_view.py
--rw-rw-rw-   0        0        0     2502 2023-01-02 11:49:06.000000 simple-slice-viewer-0.96/simple_slice_viewer/presets.yml
--rw-rw-rw-   0        0        0     2489 2022-12-27 13:32:47.000000 simple-slice-viewer-0.96/simple_slice_viewer/test.py
--rw-rw-rw-   0        0        0    23601 2023-01-03 14:16:41.000000 simple-slice-viewer-0.96/simple_slice_viewer/view.py
--rw-rw-rw-   0        0        0     2124 2023-01-03 14:01:08.000000 simple-slice-viewer-0.96/simple_slice_viewer/view_base.py
-drwxrwxrwx   0        0        0        0 2023-01-03 14:23:22.275198 simple-slice-viewer-0.96/simple_slice_viewer.egg-info/
--rw-rw-rw-   0        0        0     2158 2023-01-03 14:23:22.000000 simple-slice-viewer-0.96/simple_slice_viewer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      963 2023-01-03 14:23:22.000000 simple-slice-viewer-0.96/simple_slice_viewer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-03 14:23:22.000000 simple-slice-viewer-0.96/simple_slice_viewer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      128 2023-01-03 14:23:22.000000 simple-slice-viewer-0.96/simple_slice_viewer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-01-03 14:23:22.000000 simple-slice-viewer-0.96/simple_slice_viewer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      121 2023-01-03 14:23:22.000000 simple-slice-viewer-0.96/simple_slice_viewer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-01-03 14:23:22.000000 simple-slice-viewer-0.96/simple_slice_viewer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-03 14:23:22.280203 simple-slice-viewer-0.96/sitk_tools/
--rw-rw-rw-   0        0        0      138 2022-12-02 13:19:02.000000 simple-slice-viewer-0.96/sitk_tools/__init__.py
--rw-rw-rw-   0        0        0     9882 2022-12-02 13:19:02.000000 simple-slice-viewer-0.96/sitk_tools/dicom_reader.py
--rw-rw-rw-   0        0        0    27788 2022-12-05 14:40:18.000000 simple-slice-viewer-0.96/sitk_tools/image.py
--rw-rw-rw-   0        0        0     4059 2022-12-02 13:19:02.000000 simple-slice-viewer-0.96/sitk_tools/statistics.py
--rw-rw-rw-   0        0        0     6302 2022-12-05 14:39:25.000000 simple-slice-viewer-0.96/sitk_tools/suv.py
+drwxrwxrwx   0        0        0        0 2023-05-08 08:52:21.912249 simple-slice-viewer-0.97/
+-rw-rw-rw-   0        0        0     2158 2023-05-08 08:52:21.912249 simple-slice-viewer-0.97/PKG-INFO
+-rw-rw-rw-   0        0        0     1580 2023-05-03 09:29:12.000000 simple-slice-viewer-0.97/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 08:52:21.912249 simple-slice-viewer-0.97/setup.cfg
+-rw-rw-rw-   0        0        0     1679 2023-05-08 08:51:26.000000 simple-slice-viewer-0.97/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 08:52:21.865391 simple-slice-viewer-0.97/simple_slice_viewer/
+-rw-rw-rw-   0        0        0      582 2023-05-03 09:29:12.000000 simple-slice-viewer-0.97/simple_slice_viewer/__init__.py
+-rw-rw-rw-   0        0        0      960 2023-05-03 09:29:12.000000 simple-slice-viewer-0.97/simple_slice_viewer/console.py
+-rw-rw-rw-   0        0        0    24819 2023-05-08 08:50:41.000000 simple-slice-viewer-0.97/simple_slice_viewer/controller.py
+-rw-rw-rw-   0        0        0     2365 2023-05-03 09:29:12.000000 simple-slice-viewer-0.97/simple_slice_viewer/controller_base.py
+-rw-rw-rw-   0        0        0    18911 2023-05-03 09:29:12.000000 simple-slice-viewer-0.97/simple_slice_viewer/load_pet_view.py
+-rw-rw-rw-   0        0        0     2271 2022-10-25 12:03:22.000000 simple-slice-viewer-0.97/simple_slice_viewer/logger.py
+-rw-rw-rw-   0        0        0     6592 2023-05-03 09:31:44.000000 simple-slice-viewer-0.97/simple_slice_viewer/menus.py
+-rw-rw-rw-   0        0        0    14969 2023-05-04 09:18:20.000000 simple-slice-viewer-0.97/simple_slice_viewer/model.py
+-rw-rw-rw-   0        0        0     8103 2023-05-03 09:29:12.000000 simple-slice-viewer-0.97/simple_slice_viewer/movie_maker.py
+-rw-rw-rw-   0        0        0    14024 2023-05-03 09:29:12.000000 simple-slice-viewer-0.97/simple_slice_viewer/preset_controllers.py
+-rw-rw-rw-   0        0        0    15182 2023-05-03 09:29:12.000000 simple-slice-viewer-0.97/simple_slice_viewer/preset_model.py
+-rw-rw-rw-   0        0        0    19472 2023-05-03 09:29:12.000000 simple-slice-viewer-0.97/simple_slice_viewer/preset_view.py
+-rw-rw-rw-   0        0        0     2502 2023-05-03 16:01:17.000000 simple-slice-viewer-0.97/simple_slice_viewer/presets.yml
+-rw-rw-rw-   0        0        0    23599 2023-05-04 08:56:29.000000 simple-slice-viewer-0.97/simple_slice_viewer/view.py
+-rw-rw-rw-   0        0        0     2124 2023-05-03 09:29:12.000000 simple-slice-viewer-0.97/simple_slice_viewer/view_base.py
+drwxrwxrwx   0        0        0        0 2023-05-08 08:52:21.881018 simple-slice-viewer-0.97/simple_slice_viewer.egg-info/
+-rw-rw-rw-   0        0        0     2158 2023-05-08 08:52:21.000000 simple-slice-viewer-0.97/simple_slice_viewer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      935 2023-05-08 08:52:21.000000 simple-slice-viewer-0.97/simple_slice_viewer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 08:52:21.000000 simple-slice-viewer-0.97/simple_slice_viewer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      128 2023-05-08 08:52:21.000000 simple-slice-viewer-0.97/simple_slice_viewer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-10-25 12:03:42.000000 simple-slice-viewer-0.97/simple_slice_viewer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      121 2023-05-08 08:52:21.000000 simple-slice-viewer-0.97/simple_slice_viewer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-05-08 08:52:21.000000 simple-slice-viewer-0.97/simple_slice_viewer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 08:52:21.912249 simple-slice-viewer-0.97/sitk_tools/
+-rw-rw-rw-   0        0        0      138 2023-05-03 09:29:12.000000 simple-slice-viewer-0.97/sitk_tools/__init__.py
+-rw-rw-rw-   0        0        0     9882 2023-05-03 09:29:12.000000 simple-slice-viewer-0.97/sitk_tools/dicom_reader.py
+-rw-rw-rw-   0        0        0    27788 2023-05-03 09:29:12.000000 simple-slice-viewer-0.97/sitk_tools/image.py
+-rw-rw-rw-   0        0        0     4059 2023-05-03 09:29:12.000000 simple-slice-viewer-0.97/sitk_tools/statistics.py
+-rw-rw-rw-   0        0        0     6302 2023-05-03 09:29:12.000000 simple-slice-viewer-0.97/sitk_tools/suv.py
```

### Comparing `simple-slice-viewer-0.96/PKG-INFO` & `simple-slice-viewer-0.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-slice-viewer
-Version: 0.96
+Version: 0.97
 Summary: Simple slice viewer for Simple ITK images
 Author: M. Segbers
 Author-email: m.segbers@gmail.com
 License: MIT
 Keywords: ImageViewer DICOM,SimpleITK
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `simple-slice-viewer-0.96/README.md` & `simple-slice-viewer-0.97/README.md`

 * *Files identical despite different names*

### Comparing `simple-slice-viewer-0.96/setup.py` & `simple-slice-viewer-0.97/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 @author: M. Segbers
 """
 
 from setuptools import setup, find_packages
 
 README = 'README.md'
-VERSION = 0.96
+VERSION = 0.97
 DESCRIPTION = 'Simple slice viewer for Simple ITK images'
 NAME = 'simple-slice-viewer'
 
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
```

### Comparing `simple-slice-viewer-0.96/simple_slice_viewer/__init__.py` & `simple-slice-viewer-0.97/simple_slice_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `simple-slice-viewer-0.96/simple_slice_viewer/console.py` & `simple-slice-viewer-0.97/simple_slice_viewer/console.py`

 * *Files identical despite different names*

### Comparing `simple-slice-viewer-0.96/simple_slice_viewer/controller.py` & `simple-slice-viewer-0.97/simple_slice_viewer/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,22 +12,34 @@
 from simple_slice_viewer.preset_controllers import (StyleController,
                                                     ColorBarMenuController)
 from simple_slice_viewer.preset_model import PresetModel
 from simple_slice_viewer.preset_view import AvailableColorScaleDialog
 from simple_slice_viewer.controller_base import ControllerBase
 from simple_slice_viewer.load_pet_view import LoadPETController
 
-DEFAULT_PRESET = 'Min-Max'
-
+try:
+    import petmri_ac_composer 
+except ImportError:
+    petmri_ac_composer = None
+        
 
-SUPPORTED_FILES = ("Nifti Files (*.nii;*.nii.gz;*.nia;*.img;*.img.gz;*.hdr);;"
-                   "Nrrd (*.nrrd;*.nhdr);;"
-                   "Meta Image (*.mhd;*.mha);;"
-                   "All Files (*)")
+DEFAULT_PRESET = 'Min-Max'
 
+if petmri_ac_composer is not None:
+    SUPPORTED_FILES = ("Nifti Files (*.nii;*.nii.gz;*.nia;*.img;*.img.gz;*.hdr);;"
+                       "Nrrd (*.nrrd;*.nhdr);;"
+                       "Meta Image (*.mhd;*.mha);;"
+                       "HDF5 PIFA Files (*.hdf);;"
+                       "All Files (*)")
+else:
+    SUPPORTED_FILES = ("Nifti Files (*.nii;*.nii.gz;*.nia;*.img;*.img.gz;*.hdr);;"
+                       "Nrrd (*.nrrd;*.nhdr);;"
+                       "Meta Image (*.mhd;*.mha);;"                      
+                       "All Files (*)")
+        
 
 class FrameScrollController(ControllerBase):
     def __init__(self, *args, **kwargs):
 
         super().__init__(*args, **kwargs)
 
         self.update_scrollbar()
@@ -328,16 +340,19 @@
             return
 
         self.update_position(event[0])
 
         self.view.status_label.setText(self.mouse_text)
 
     def get_image_data(self, index):
-
+        
+        index = self.model[0].get_image_index(index)
         pos_phys = self.model[0].transform_index_to_physical_point(index)
+        
+        
         im_val = self.model[0].get_value_at_index(index)
         fusion_val = self.model[1].get_value_at_index(index)
         im_index = self.model[0].get_image_index(index)
 
         pos_phys = self.smart_round(pos_phys, 1)
         im_val = self.smart_round(im_val, 2)
         fusion_val = self.smart_round(fusion_val, 2)
@@ -392,14 +407,15 @@
 
     def image_menu_callback(self, menu_tree):
 
         if menu_tree[0] == MenuBar.OPEN_FILE:
             self.load_image_from_file()
         elif menu_tree[0] == MenuBar.LOAD_DICOM_FOLDER:
             self.load_image_from_dicom_folder()
+        
         elif menu_tree[0] == MenuBar.SAVE_FILE:
             self.save_image()
         elif menu_tree[0] == MenuBar.LOAD_PET:
             self.load_pet_as_image()
 
     def fusion_menu_callback(self, menu_tree):
         if menu_tree[0] == MenuBar.OPEN_FILE:
@@ -518,14 +534,15 @@
     def load_pet_as_image(self):
         dlg = LoadPETController(parent=self.view)
         dlg.view.exec_()
         if isinstance(dlg.image, sitk.Image):
 
             self.model.set_image(0, dlg.image)
         del dlg
+        
 
     def load_pet_as_fusion(self):
         dlg = LoadPETController()
         dlg.view.exec_()
         if isinstance(dlg.image, sitk.Image):
             self.model.set_image(1, dlg.image)
         del dlg
@@ -582,18 +599,25 @@
         folder_name = QFileDialog.getExistingDirectory(self.view, msg)
         return folder_name
 
     def read_image(self):
         file_name = self.get_open_file()
         image = None
         if file_name:
-            try:
-                image = sitk.ReadImage(file_name)
-            except:
-                self.show_warning(f'Could not open file {file_name}')
+            ext = os.path.splitext(file_name)[1]
+            if ext.lower() == '.hdf':
+                try:
+                    image = petmri_ac_composer.file_io.pifa_to_sitk(file_name)
+                except:
+                    self.show_warning(f'Could not open file {file_name}')
+            else:
+                try:
+                    image = sitk.ReadImage(file_name)
+                except:
+                    self.show_warning(f'Could not open file {file_name}')
         return image
 
     def load_image_from_dicom_folder(self):
         image = self.read_dicom()
         if image is not None:
             self.model.set_image(0, image)
```

### Comparing `simple-slice-viewer-0.96/simple_slice_viewer/controller_base.py` & `simple-slice-viewer-0.97/simple_slice_viewer/controller_base.py`

 * *Files identical despite different names*

### Comparing `simple-slice-viewer-0.96/simple_slice_viewer/load_pet_view.py` & `simple-slice-viewer-0.97/simple_slice_viewer/load_pet_view.py`

 * *Files identical despite different names*

### Comparing `simple-slice-viewer-0.96/simple_slice_viewer/logger.py` & `simple-slice-viewer-0.97/simple_slice_viewer/logger.py`

 * *Files identical despite different names*

### Comparing `simple-slice-viewer-0.96/simple_slice_viewer/menus.py` & `simple-slice-viewer-0.97/simple_slice_viewer/menus.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,16 @@
         
 
 class MenuBar(QWidget):
     IMAGE = 'Image'
     FUSION = 'Fusion'
     EXPORT = 'Export'
     
+    
+    LOAD_PIFA = 'Load Pifa'
     OPEN_FILE = 'Open File'
     SAVE_FILE = 'Save File'
     LOAD_DICOM_FOLDER = 'Load Dicom Folder'
     LOAD_PET = 'Load PET From Dicom'
     REMOVE_FUSION = 'Remove Fusion'
     MAKE_MOVIE = 'Export Movie of Slices'
     MAKE_MOVIE_OF_FRAMES = 'Export Movie of Frames'
@@ -110,21 +112,23 @@
     SHOW_CROSSHAIR = 'Show CrossHair'
     SAVE_PRESETS = 'Save Presets'
     RESET_PRESETS = 'Reset Presets to Defaults'
     
     IMAGE_MENU = [OPEN_FILE, 
                   SAVE_FILE,
                   LOAD_DICOM_FOLDER, 
-                  LOAD_PET]
+                  LOAD_PET,
+                  LOAD_PIFA]
                  
     
     FUSION_MENU = [OPEN_FILE, 
                   SAVE_FILE,
                   LOAD_DICOM_FOLDER, 
                   LOAD_PET,
+                  LOAD_PIFA,
                   REMOVE_FUSION]
                 
     
     SETTINGS_MENU = [COLORMAPS, SHOW_CROSSHAIR, SAVE_PRESETS, RESET_PRESETS]
     
     MOVIE_MENU = [MAKE_MOVIE, MAKE_MOVIE_OF_FRAMES]
```

### Comparing `simple-slice-viewer-0.96/simple_slice_viewer/model.py` & `simple-slice-viewer-0.97/simple_slice_viewer/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,16 +94,18 @@
             
             direction = self.get_view_direction()
         
             if direction == SAGGITAL:
                 index = [self.get_slice_index(), *index]
             elif direction == CORONAL:
                 index = [index[0], self.get_slice_index(), index[1]]
-            elif direction == AXIAL:               
-                index = [index[0], index[1], self.get_slice_index()]
+            elif direction == AXIAL:  
+                index[1] = self.get_image().GetSize()[1]-  index[1]
+                index = [*index, self.get_slice_index()]
+            
             if self.get_ndim() == 4:
                 return [*index, self.get_frame_index()]
             else:
                 return index
         else:
             raise RuntimeError()
     
@@ -114,15 +116,15 @@
         index = [math.floor(ii) for ii in index]
         
         for ii, value in enumerate(index):
             if value < 0:
                 index[ii] = 0
             if value >= self.get_image().GetSize()[ii]:
                 index[ii] = self.get_image().GetSize()[ii] - 1
-                    
+
         if len(index) == 2:
             image = self.get_sitk_slice()
         elif len(index) == 3:
             image = self.get_image()
         else:
             raise IndexError()
         
@@ -148,16 +150,16 @@
                 direction = self.get_view_direction()
                 if direction == SAGGITAL:
                     index = [self.get_slice_index(), *index]
                 elif direction == CORONAL:
                     index = [index[0], self.get_slice_index(), index[1]]
                 elif direction == AXIAL:
                     # account for y flip in viewing
-                    indexy = self.get_image().GetSize()[2]-  index[1]
-                    index = [index[0], indexy, self.get_slice_index()]
+                    index[1] = self.get_image().GetSize()[1]-  index[1]
+                    index = [*index, self.get_slice_index()]
                 else:
                     raise RuntimeError()
             else:
                 raise IndexError(f'Wrong number of values passed {len(index)}')
            
             phys = image.TransformContinuousIndexToPhysicalPoint(index)
```

### Comparing `simple-slice-viewer-0.96/simple_slice_viewer/movie_maker.py` & `simple-slice-viewer-0.97/simple_slice_viewer/movie_maker.py`

 * *Files identical despite different names*

### Comparing `simple-slice-viewer-0.96/simple_slice_viewer/preset_controllers.py` & `simple-slice-viewer-0.97/simple_slice_viewer/preset_controllers.py`

 * *Files identical despite different names*

### Comparing `simple-slice-viewer-0.96/simple_slice_viewer/preset_model.py` & `simple-slice-viewer-0.97/simple_slice_viewer/preset_model.py`

 * *Files identical despite different names*

### Comparing `simple-slice-viewer-0.96/simple_slice_viewer/preset_view.py` & `simple-slice-viewer-0.97/simple_slice_viewer/preset_view.py`

 * *Files identical despite different names*

### Comparing `simple-slice-viewer-0.96/simple_slice_viewer/presets.yml` & `simple-slice-viewer-0.97/simple_slice_viewer/presets.yml`

 * *Files identical despite different names*

### Comparing `simple-slice-viewer-0.96/simple_slice_viewer/view.py` & `simple-slice-viewer-0.97/simple_slice_viewer/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
         
     def set_position(self, pos):
         self.vertical_line.setValue(pos[0])
         self.horizontal_line.setValue(pos[1])
     
     def get_position(self):
         return Point(self.vertical_line.value(), 
-                       self.horizontal_line.value())
+                     self.horizontal_line.value())
     
     def position_changed(self, obj=None):
         self.positionChanged.emit(self.get_position())
         
 
         
 class ImageWidget(WidgetBase):
```

### Comparing `simple-slice-viewer-0.96/simple_slice_viewer/view_base.py` & `simple-slice-viewer-0.97/simple_slice_viewer/view_base.py`

 * *Files identical despite different names*

### Comparing `simple-slice-viewer-0.96/simple_slice_viewer.egg-info/PKG-INFO` & `simple-slice-viewer-0.97/simple_slice_viewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-slice-viewer
-Version: 0.96
+Version: 0.97
 Summary: Simple slice viewer for Simple ITK images
 Author: M. Segbers
 Author-email: m.segbers@gmail.com
 License: MIT
 Keywords: ImageViewer DICOM,SimpleITK
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `simple-slice-viewer-0.96/simple_slice_viewer.egg-info/SOURCES.txt` & `simple-slice-viewer-0.97/simple_slice_viewer.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 simple_slice_viewer/menus.py
 simple_slice_viewer/model.py
 simple_slice_viewer/movie_maker.py
 simple_slice_viewer/preset_controllers.py
 simple_slice_viewer/preset_model.py
 simple_slice_viewer/preset_view.py
 simple_slice_viewer/presets.yml
-simple_slice_viewer/test.py
 simple_slice_viewer/view.py
 simple_slice_viewer/view_base.py
 simple_slice_viewer.egg-info/PKG-INFO
 simple_slice_viewer.egg-info/SOURCES.txt
 simple_slice_viewer.egg-info/dependency_links.txt
 simple_slice_viewer.egg-info/entry_points.txt
 simple_slice_viewer.egg-info/not-zip-safe
```

### Comparing `simple-slice-viewer-0.96/sitk_tools/dicom_reader.py` & `simple-slice-viewer-0.97/sitk_tools/dicom_reader.py`

 * *Files identical despite different names*

### Comparing `simple-slice-viewer-0.96/sitk_tools/image.py` & `simple-slice-viewer-0.97/sitk_tools/image.py`

 * *Files identical despite different names*

### Comparing `simple-slice-viewer-0.96/sitk_tools/statistics.py` & `simple-slice-viewer-0.97/sitk_tools/statistics.py`

 * *Files identical despite different names*

### Comparing `simple-slice-viewer-0.96/sitk_tools/suv.py` & `simple-slice-viewer-0.97/sitk_tools/suv.py`

 * *Files identical despite different names*

