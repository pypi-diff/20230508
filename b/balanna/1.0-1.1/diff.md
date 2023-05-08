# Comparing `tmp/balanna-1.0.tar.gz` & `tmp/balanna-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balanna-1.0.tar", last modified: Thu Apr 27 13:23:12 2023, max compression
+gzip compressed data, was "balanna-1.1.tar", last modified: Mon May  8 08:49:05 2023, max compression
```

## Comparing `balanna-1.0.tar` & `balanna-1.1.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 sele       (501) staff       (20)        0 2023-04-27 13:23:12.097470 balanna-1.0/
--rw-r--r--   0 sele       (501) staff       (20)     1070 2023-04-27 11:14:03.000000 balanna-1.0/LICENSE
--rw-r--r--   0 sele       (501) staff       (20)      245 2023-04-27 13:23:12.097623 balanna-1.0/PKG-INFO
--rw-r--r--   0 sele       (501) staff       (20)      517 2023-04-27 11:17:40.000000 balanna-1.0/README.md
-drwxr-xr-x   0 sele       (501) staff       (20)        0 2023-04-27 13:23:12.092117 balanna-1.0/balanna/
--rw-r--r--   0 sele       (501) staff       (20)      540 2023-04-27 13:14:38.000000 balanna-1.0/balanna/__init__.py
--rw-r--r--   0 sele       (501) staff       (20)     1095 2023-04-27 13:14:38.000000 balanna-1.0/balanna/__main__.py
--rw-r--r--   0 sele       (501) staff       (20)     1581 2023-04-27 11:14:03.000000 balanna-1.0/balanna/camera_trajectories.py
--rw-r--r--   0 sele       (501) staff       (20)    10078 2023-04-27 11:14:03.000000 balanna-1.0/balanna/trimesh.py
-drwxr-xr-x   0 sele       (501) staff       (20)        0 2023-04-27 13:23:12.096621 balanna-1.0/balanna/utils/
--rw-r--r--   0 sele       (501) staff       (20)       30 2023-04-27 11:14:03.000000 balanna-1.0/balanna/utils/__init__.py
--rw-r--r--   0 sele       (501) staff       (20)      559 2023-04-27 11:14:03.000000 balanna-1.0/balanna/utils/geometry.py
--rw-r--r--   0 sele       (501) staff       (20)    15330 2023-04-27 12:54:01.000000 balanna-1.0/balanna/window_base.py
--rw-r--r--   0 sele       (501) staff       (20)     4645 2023-04-27 13:16:24.000000 balanna-1.0/balanna/window_dataset.py
--rw-r--r--   0 sele       (501) staff       (20)     4593 2023-04-27 12:57:38.000000 balanna-1.0/balanna/window_generator.py
--rw-r--r--   0 sele       (501) staff       (20)     7265 2023-04-27 12:58:33.000000 balanna-1.0/balanna/window_real_time.py
-drwxr-xr-x   0 sele       (501) staff       (20)        0 2023-04-27 13:23:12.094874 balanna-1.0/balanna.egg-info/
--rw-r--r--   0 sele       (501) staff       (20)      245 2023-04-27 13:23:12.000000 balanna-1.0/balanna.egg-info/PKG-INFO
--rw-r--r--   0 sele       (501) staff       (20)      437 2023-04-27 13:23:12.000000 balanna-1.0/balanna.egg-info/SOURCES.txt
--rw-r--r--   0 sele       (501) staff       (20)        1 2023-04-27 13:23:12.000000 balanna-1.0/balanna.egg-info/dependency_links.txt
--rw-r--r--   0 sele       (501) staff       (20)       56 2023-04-27 13:23:12.000000 balanna-1.0/balanna.egg-info/requires.txt
--rw-r--r--   0 sele       (501) staff       (20)        8 2023-04-27 13:23:12.000000 balanna-1.0/balanna.egg-info/top_level.txt
--rw-r--r--   0 sele       (501) staff       (20)      103 2023-04-27 13:23:12.098296 balanna-1.0/setup.cfg
--rw-r--r--   0 sele       (501) staff       (20)      493 2023-04-27 13:17:06.000000 balanna-1.0/setup.py
+drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-08 08:49:05.015508 balanna-1.1/
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     1070 2023-05-08 07:14:59.000000 balanna-1.1/LICENSE
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      245 2023-05-08 08:49:05.015508 balanna-1.1/PKG-INFO
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      517 2023-05-08 07:14:59.000000 balanna-1.1/README.md
+drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-08 08:49:04.999507 balanna-1.1/balanna/
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      613 2023-05-08 08:42:52.000000 balanna-1.1/balanna/__init__.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     1095 2023-05-08 07:14:59.000000 balanna-1.1/balanna/__main__.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     1581 2023-05-08 07:14:59.000000 balanna-1.1/balanna/camera_trajectories.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     2013 2023-05-08 08:42:52.000000 balanna-1.1/balanna/rendering_dataset.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)    10078 2023-05-08 07:14:59.000000 balanna-1.1/balanna/trimesh.py
+drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-08 08:49:05.011508 balanna-1.1/balanna/utils/
+-rw-r--r--   0 sas      (23222) tumuser  (20909)       30 2023-05-08 07:14:59.000000 balanna-1.1/balanna/utils/__init__.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      559 2023-05-08 07:14:59.000000 balanna-1.1/balanna/utils/geometry.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     4463 2023-05-08 08:42:52.000000 balanna-1.1/balanna/utils/vedo_utils.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)    10610 2023-05-08 08:42:52.000000 balanna-1.1/balanna/window_base.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     4645 2023-05-08 07:14:59.000000 balanna-1.1/balanna/window_dataset.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     4593 2023-05-08 07:14:59.000000 balanna-1.1/balanna/window_generator.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     7265 2023-05-08 07:14:59.000000 balanna-1.1/balanna/window_real_time.py
+drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-08 08:49:05.007508 balanna-1.1/balanna.egg-info/
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      245 2023-05-08 08:49:04.000000 balanna-1.1/balanna.egg-info/PKG-INFO
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      494 2023-05-08 08:49:04.000000 balanna-1.1/balanna.egg-info/SOURCES.txt
+-rw-r--r--   0 sas      (23222) tumuser  (20909)        1 2023-05-08 08:49:04.000000 balanna-1.1/balanna.egg-info/dependency_links.txt
+-rw-r--r--   0 sas      (23222) tumuser  (20909)       56 2023-05-08 08:49:04.000000 balanna-1.1/balanna.egg-info/requires.txt
+-rw-r--r--   0 sas      (23222) tumuser  (20909)        8 2023-05-08 08:49:04.000000 balanna-1.1/balanna.egg-info/top_level.txt
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      103 2023-05-08 08:49:05.015508 balanna-1.1/setup.cfg
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      493 2023-05-08 08:43:23.000000 balanna-1.1/setup.py
```

### Comparing `balanna-1.0/LICENSE` & `balanna-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `balanna-1.0/README.md` & `balanna-1.1/README.md`

 * *Files identical despite different names*

### Comparing `balanna-1.0/balanna/__init__.py` & `balanna-1.1/balanna/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import balanna.camera_trajectories as camera_trajectories
 import balanna.utils as utils
 import balanna.trimesh as trimesh
 
+from balanna.rendering_dataset import render_dataset
 from balanna.window_dataset import display_dataset
 from balanna.window_generator import display_generated, display_scenes
 from balanna.window_real_time import display_real_time, RealTimeNode
 from balanna.window_base import SceneDictType
 
 
 __all__ = [
   "camera_trajectories", 
   "trimesh",
   "display_dataset",
   "display_scenes",
   "display_generated",
   "display_real_time", 
   "RealTimeNode",
+  "render_dataset",
   "SceneDictType",
 ]
```

### Comparing `balanna-1.0/balanna/__main__.py` & `balanna-1.1/balanna/__main__.py`

 * *Files identical despite different names*

### Comparing `balanna-1.0/balanna/camera_trajectories.py` & `balanna-1.1/balanna/camera_trajectories.py`

 * *Files identical despite different names*

### Comparing `balanna-1.0/balanna/trimesh.py` & `balanna-1.1/balanna/trimesh.py`

 * *Files identical despite different names*

### Comparing `balanna-1.0/balanna/utils/geometry.py` & `balanna-1.1/balanna/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `balanna-1.0/balanna/window_base.py` & `balanna-1.1/balanna/window_base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 import datetime
 import image_grid
 import importlib.metadata
 import numpy as np
 import packaging.version
 import pathlib
 import trimesh.path.entities
-import trimesh.visual
 import trimesh.viewer
 import time
 import vedo
-import vtk
 
 import matplotlib
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_qtagg import (
     FigureCanvasQTAgg as FigureCanvas, NavigationToolbar2QT as NavigationToolbar)
 
 from functools import partial
 from PIL import Image
 from PyQt5 import Qt
 from typing import Any, Dict, List, Optional, Union
 from vtk.qt.QVTKRenderWindowInteractor import QVTKRenderWindowInteractor
-from vtk.util.numpy_support import numpy_to_vtk
 
+from balanna.utils.vedo_utils import trimesh_scene_2_vedo
 
 SceneDictType = Dict[str, Any]
 
 
 class MainWindow(Qt.QMainWindow):
 
     def __init__(
@@ -123,97 +121,19 @@
 
     def render_(self, scene_dict: SceneDictType, resetcam: bool = False):
         start_time = time.perf_counter()
 
         for key, element in scene_dict.items():
             if isinstance(element, trimesh.Scene) and key in self.scene_key_dict:
                 at = self.scene_key_dict[key]
-                meshes_vedo = []
-                for m in element.geometry.values():
-                    if isinstance(m, trimesh.Trimesh):
-                        m_vedo = vedo.trimesh2vedo(m)
-                        if m.visual.kind == "vertex":
-                            face_colors = trimesh.visual.color.vertex_to_face_color(m.visual.vertex_colors, m.faces)
-                            m_vedo.cellIndividualColors(face_colors)
-                        meshes_vedo.append(m_vedo)
-
-                    elif isinstance(m, trimesh.PointCloud):
-                        vertices = m.vertices
-                        vertex_colors = m.visual.vertex_colors
-                        n, _ = vertices.shape
-
-                        # vedo.Points uses vtk.vtkPolyData() as backend data storage and thus converts
-                        # the input to this type. However, the vedo conversion is quite inefficient, therefore
-                        # we convert the trimesh.PointCloud before passing it to vedo.
-                        # partially from https://github.com/pyvista/utilities/helpers.py
-                        vtkpts = vtk.vtkPoints()
-                        vtk_arr = numpy_to_vtk(vertices, deep=True)
-                        vtkpts.SetData(vtk_arr)
-                        pd = vtk.vtkPolyData()
-                        pd.SetPoints(vtkpts)
-
-                        # For some reason, vedo requires each vtk.vtkPolyData object to set an internal
-                        # cell array, as it uses the vertices, not the points attribute. As a point cloud
-                        # is unconnected, the offset and connectivity is just the index of the respective point.
-                        carr = vtk.vtkCellArray()
-                        carr.SetData(vedo.numpy2vtk(np.arange(n + 1), dtype="int"),  # offset
-                                     vedo.numpy2vtk(np.arange(n), dtype="int"))  # connectivity
-                        pd.SetVerts(carr)
-
-                        # Set vertex color RGB/RGBA values as active scalar property of the vtk.vtkPolyData.
-                        if vertex_colors.shape[1] == 3:
-                            ucols = numpy_to_vtk(vertex_colors)
-                            ucols.SetName("Points_RGB")
-                            pd.GetPointData().AddArray(ucols)
-                            pd.GetPointData().SetActiveScalars("Points_RGB")
-                        elif vertex_colors.shape[1] == 4:
-                            ucols = numpy_to_vtk(vertex_colors)
-                            ucols.SetName("Points_RGBA")
-                            pd.GetPointData().AddArray(ucols)
-                            pd.GetPointData().SetActiveScalars("Points_RGBA")
-                        else:
-                            print("\033[93m" + f"Invalid point cloud colors, skipping ..." + "\033[0m")
-
-                        m_vedo = vedo.Points(pd)
-                        meshes_vedo.append(m_vedo)
-
-                    elif isinstance(m, trimesh.path.Path3D):
-                        # The trimesh path consists of entities and vertices. The vertices are the 3D points,
-                        # that are connected as described in the entities.
-                        if not all([isinstance(me, trimesh.path.entities.Line) for me in m.entities]):
-                            raise ValueError("Currently only trimesh.path.entities.Line entities are supported")
-                        if not all([len(me.points) == 2 for me in m.entities]):
-                            raise ValueError("Invalid line entities, should have point lists [start, end]")
-
-                        # Add each line segment individually as a vedo line to support multicolored lines
-                        # and different alpha values along the line.
-                        for ke, line_entity in enumerate(m.entities):
-                            i, j = line_entity.points
-                            c = m.colors[ke, :3]
-                            alpha = m.colors[ke, -1] / 255  # [0, 255] -> [0, 1]
-                            m_vedo = vedo.Lines(m.vertices[None, i], m.vertices[None, j], lw=2, c=c, alpha=alpha)
-                            meshes_vedo.append(m_vedo)
-
-                    else:
-                        meshes_vedo.append(m)
-
-                if self.show_labels:
-                    annotation = vedo.CornerAnnotation()
-                    annotation.text(key)
-                    meshes_vedo.append(annotation)
-
-                camera_dict = None
-                if self.use_scene_cam:
-                    focal_distance = 1.0
-                    T_W_C = element.camera_transform
-                    cam_0 = T_W_C[:3, 3]
-                    cam_1 = cam_0 + T_W_C[:3, :3] @ np.array([0, 0, focal_distance])  # along z of camera
-                    view_up = - T_W_C[:3, 1]  # camera convention -> y points down
-                    camera_dict = dict(pos=cam_0, focal_point=cam_1, viewup=view_up)
-
+                meshes_vedo, camera_dict = trimesh_scene_2_vedo(
+                    scene=element,
+                    label=key if self.show_labels else None,
+                    use_scene_cam=self.use_scene_cam
+                )
                 self.vps[at].clear()
                 self.vps[at].show(meshes_vedo, bg="white", resetcam=resetcam, camera=camera_dict)
 
             elif isinstance(element, np.ndarray) and key in self.image_widge_dict:
                 if len(element.shape) == 3:
                     if element.shape[0] == 3:
                         element = np.transpose(element, (1, 2, 0))  # (C, H, W) -> (H, W, C)
```

### Comparing `balanna-1.0/balanna/window_dataset.py` & `balanna-1.1/balanna/window_dataset.py`

 * *Files identical despite different names*

### Comparing `balanna-1.0/balanna/window_generator.py` & `balanna-1.1/balanna/window_generator.py`

 * *Files identical despite different names*

### Comparing `balanna-1.0/balanna/window_real_time.py` & `balanna-1.1/balanna/window_real_time.py`

 * *Files identical despite different names*

