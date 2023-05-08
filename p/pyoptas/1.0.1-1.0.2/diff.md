# Comparing `tmp/pyoptas-1.0.1.tar.gz` & `tmp/pyoptas-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoptas-1.0.1.tar", last modified: Mon May  8 11:24:06 2023, max compression
+gzip compressed data, was "pyoptas-1.0.2.tar", last modified: Mon May  8 11:55:31 2023, max compression
```

## Comparing `pyoptas-1.0.1.tar` & `pyoptas-1.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-05-08 11:24:06.037500 pyoptas-1.0.1/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      583 2022-10-10 13:03:33.000000 pyoptas-1.0.1/LICENSE
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    10113 2023-05-08 11:24:06.037500 pyoptas-1.0.1/PKG-INFO
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     9214 2023-05-08 11:22:00.000000 pyoptas-1.0.1/README.md
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-05-08 11:24:06.033500 pyoptas-1.0.1/optas/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     1194 2023-04-10 19:50:52.000000 pyoptas-1.0.1/optas/__init__.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    21019 2023-04-10 19:50:52.000000 pyoptas-1.0.1/optas/builder.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    65452 2023-04-18 18:18:27.000000 pyoptas-1.0.1/optas/models.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    20074 2023-04-10 19:50:52.000000 pyoptas-1.0.1/optas/optimization.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    27057 2023-04-10 19:50:52.000000 pyoptas-1.0.1/optas/solver.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    11921 2023-04-18 18:18:27.000000 pyoptas-1.0.1/optas/spatialmath.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     4557 2023-04-10 19:50:52.000000 pyoptas-1.0.1/optas/sx_container.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    11538 2023-04-10 19:50:52.000000 pyoptas-1.0.1/optas/templates.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    42110 2023-04-10 19:50:52.000000 pyoptas-1.0.1/optas/visualize.py
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-05-08 11:24:06.037500 pyoptas-1.0.1/pyoptas.egg-info/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    10113 2023-05-08 11:24:06.000000 pyoptas-1.0.1/pyoptas.egg-info/PKG-INFO
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      586 2023-05-08 11:24:06.000000 pyoptas-1.0.1/pyoptas.egg-info/SOURCES.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)        1 2023-05-08 11:24:06.000000 pyoptas-1.0.1/pyoptas.egg-info/dependency_links.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      152 2023-05-08 11:24:06.000000 pyoptas-1.0.1/pyoptas.egg-info/requires.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)        6 2023-05-08 11:24:06.000000 pyoptas-1.0.1/pyoptas.egg-info/top_level.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      800 2023-05-08 11:23:24.000000 pyoptas-1.0.1/pyproject.toml
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       38 2023-05-08 11:24:06.037500 pyoptas-1.0.1/setup.cfg
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     1048 2023-05-08 11:23:20.000000 pyoptas-1.0.1/setup.py
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-05-08 11:24:06.037500 pyoptas-1.0.1/tests/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    16371 2023-03-07 17:13:56.000000 pyoptas-1.0.1/tests/test_builder.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     1999 2023-04-10 19:50:52.000000 pyoptas-1.0.1/tests/test_examples.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    38341 2023-04-18 18:18:27.000000 pyoptas-1.0.1/tests/test_models.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     5890 2023-03-07 17:13:56.000000 pyoptas-1.0.1/tests/test_optas_utils.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    12874 2023-04-10 19:50:52.000000 pyoptas-1.0.1/tests/test_optimization.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     3025 2023-03-07 17:13:56.000000 pyoptas-1.0.1/tests/test_solver.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    17271 2023-04-10 19:50:52.000000 pyoptas-1.0.1/tests/test_spatialmath.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     1773 2023-03-07 17:13:56.000000 pyoptas-1.0.1/tests/test_sx_container.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      874 2023-03-07 17:13:56.000000 pyoptas-1.0.1/tests/tester_robot_model.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-05-08 11:55:31.924827 pyoptas-1.0.2/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      583 2022-10-10 13:03:33.000000 pyoptas-1.0.2/LICENSE
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    10113 2023-05-08 11:55:31.924827 pyoptas-1.0.2/PKG-INFO
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     9214 2023-05-08 11:34:46.000000 pyoptas-1.0.2/README.md
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-05-08 11:55:31.920827 pyoptas-1.0.2/optas/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     1194 2023-04-10 19:50:52.000000 pyoptas-1.0.2/optas/__init__.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    21019 2023-04-10 19:50:52.000000 pyoptas-1.0.2/optas/builder.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    65452 2023-04-18 18:18:27.000000 pyoptas-1.0.2/optas/models.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    20074 2023-04-10 19:50:52.000000 pyoptas-1.0.2/optas/optimization.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    27057 2023-04-10 19:50:52.000000 pyoptas-1.0.2/optas/solver.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    11921 2023-04-18 18:18:27.000000 pyoptas-1.0.2/optas/spatialmath.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     4557 2023-04-10 19:50:52.000000 pyoptas-1.0.2/optas/sx_container.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    11538 2023-04-10 19:50:52.000000 pyoptas-1.0.2/optas/templates.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    43584 2023-05-08 11:55:21.000000 pyoptas-1.0.2/optas/visualize.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-05-08 11:55:31.920827 pyoptas-1.0.2/pyoptas.egg-info/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    10113 2023-05-08 11:55:31.000000 pyoptas-1.0.2/pyoptas.egg-info/PKG-INFO
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      586 2023-05-08 11:55:31.000000 pyoptas-1.0.2/pyoptas.egg-info/SOURCES.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)        1 2023-05-08 11:55:31.000000 pyoptas-1.0.2/pyoptas.egg-info/dependency_links.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      152 2023-05-08 11:55:31.000000 pyoptas-1.0.2/pyoptas.egg-info/requires.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)        6 2023-05-08 11:55:31.000000 pyoptas-1.0.2/pyoptas.egg-info/top_level.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      800 2023-05-08 11:55:21.000000 pyoptas-1.0.2/pyproject.toml
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       38 2023-05-08 11:55:31.924827 pyoptas-1.0.2/setup.cfg
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     1048 2023-05-08 11:55:21.000000 pyoptas-1.0.2/setup.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-05-08 11:55:31.924827 pyoptas-1.0.2/tests/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    16371 2023-03-07 17:13:56.000000 pyoptas-1.0.2/tests/test_builder.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     1999 2023-04-10 19:50:52.000000 pyoptas-1.0.2/tests/test_examples.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    38341 2023-04-18 18:18:27.000000 pyoptas-1.0.2/tests/test_models.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     5890 2023-03-07 17:13:56.000000 pyoptas-1.0.2/tests/test_optas_utils.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    12874 2023-04-10 19:50:52.000000 pyoptas-1.0.2/tests/test_optimization.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     3025 2023-03-07 17:13:56.000000 pyoptas-1.0.2/tests/test_solver.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    17271 2023-04-10 19:50:52.000000 pyoptas-1.0.2/tests/test_spatialmath.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     1773 2023-03-07 17:13:56.000000 pyoptas-1.0.2/tests/test_sx_container.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      874 2023-03-07 17:13:56.000000 pyoptas-1.0.2/tests/tester_robot_model.py
```

### Comparing `pyoptas-1.0.1/LICENSE` & `pyoptas-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.1/PKG-INFO` & `pyoptas-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoptas
-Version: 1.0.1
+Version: 1.0.2
 Summary: An optimization-based task specification library for task and motion planning (TAMP), trajectory optimization, and model predictive control.
 Home-page: https://github.com/cmower/optas
 Author: Christopher E. Mower
 Author-email: "Christopher E. Mower" <christopher.mower@kcl.ac.uk>
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://cmower.github.io/optas/
 Project-URL: Documentation, https://cmower.github.io/optas/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyoptas Version: 1.0.1 Summary: An optimization-
+Metadata-Version: 2.1 Name: pyoptas Version: 1.0.2 Summary: An optimization-
 based task specification library for task and motion planning (TAMP),
 trajectory optimization, and model predictive control. Home-page: https://
 github.com/cmower/optas Author: Christopher E. Mower Author-email: "Christopher
 E. Mower"
 mower@kcl.ac.uk> License: Apache License, Version 2.0 Project-URL: Homepage,
 https://cmower.github.io/optas/ Project-URL: Documentation, https://
 cmower.github.io/optas/ Project-URL: Bug Tracker, https://github.com/cmower/
```

### Comparing `pyoptas-1.0.1/README.md` & `pyoptas-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.1/optas/__init__.py` & `pyoptas-1.0.2/optas/__init__.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.1/optas/builder.py` & `pyoptas-1.0.2/optas/builder.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.1/optas/models.py` & `pyoptas-1.0.2/optas/models.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.1/optas/optimization.py` & `pyoptas-1.0.2/optas/optimization.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.1/optas/solver.py` & `pyoptas-1.0.2/optas/solver.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.1/optas/spatialmath.py` & `pyoptas-1.0.2/optas/spatialmath.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.1/optas/sx_container.py` & `pyoptas-1.0.2/optas/sx_container.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.1/optas/templates.py` & `pyoptas-1.0.2/optas/templates.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.1/optas/visualize.py` & `pyoptas-1.0.2/optas/visualize.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,26 @@
     # def append_actors(self, *actors):
     #     for actor in actors:
     #         if isinstance(actor, list):
     #             self.actors += actor  # assume actor is a list of actors
     #         else:
     #             self.actors.append(actor)  # assume actor is a single actor
 
+    def reset_camera(self, position, view_dir, view_up):
+        """! Reset the camera pose.
+
+        @param position The position of the camera.
+        @param view_dir The direction that the camera should view.
+        @param view_up The up direction for the image.
+        """
+        focal_point = (np.asarray(position) + np.asarray(view_dir)).tolist()
+        self.camera.SetPosition(*position)
+        self.camera.SetFocalPoint(*focal_point)
+        self.camera.SetViewUp(*view_up)
+
     #
     # Set/convert helper methods
     #
 
     @staticmethod
     @arrayify_args
     def cvt_orientation_to_rotation_matrix(
@@ -1130,14 +1142,43 @@
             self.animate_callbacks.append(
                 AnimationCallback(robot_traj, duration, self.iren, self.ren)
             )
             self.actors.start_adding_actors()
 
         return actors
 
+    def save(self, file_name):
+        """! Save the visualizer window as png image. Note, saving animations is currently not supported."""
+        assert (
+            len(self.animate_callbacks) == 0
+        ), "saving animations is currently not supported"
+
+        if not file_name.endswith(".png"):
+            file_name += ".png"
+
+        for actor in self.actors.actors:
+            self.ren.AddActor(actor)
+        self.iren.Initialize()
+
+        self.renWin.Render()
+
+        # Capture the contents of the render window
+        window_to_image_filter = vtk.vtkWindowToImageFilter()
+        window_to_image_filter.SetInput(self.renWin)
+        window_to_image_filter.Update()
+
+        # Write the captured image to a PNG file
+        png_writer = vtk.vtkPNGWriter()
+        png_writer.SetFileName(file_name)
+        png_writer.SetInputConnection(window_to_image_filter.GetOutputPort())
+        png_writer.Write()
+        print(f"Saved {file_name}")
+
+        self.iren.Start()
+
     def start(self) -> None:
         """! Start the visualizer."""
         for actor in self.actors.actors:
             self.ren.AddActor(actor)
         self.iren.Initialize()
 
         for callback in self.animate_callbacks:
```

### Comparing `pyoptas-1.0.1/pyoptas.egg-info/PKG-INFO` & `pyoptas-1.0.2/pyoptas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoptas
-Version: 1.0.1
+Version: 1.0.2
 Summary: An optimization-based task specification library for task and motion planning (TAMP), trajectory optimization, and model predictive control.
 Home-page: https://github.com/cmower/optas
 Author: Christopher E. Mower
 Author-email: "Christopher E. Mower" <christopher.mower@kcl.ac.uk>
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://cmower.github.io/optas/
 Project-URL: Documentation, https://cmower.github.io/optas/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyoptas Version: 1.0.1 Summary: An optimization-
+Metadata-Version: 2.1 Name: pyoptas Version: 1.0.2 Summary: An optimization-
 based task specification library for task and motion planning (TAMP),
 trajectory optimization, and model predictive control. Home-page: https://
 github.com/cmower/optas Author: Christopher E. Mower Author-email: "Christopher
 E. Mower"
 mower@kcl.ac.uk> License: Apache License, Version 2.0 Project-URL: Homepage,
 https://cmower.github.io/optas/ Project-URL: Documentation, https://
 cmower.github.io/optas/ Project-URL: Bug Tracker, https://github.com/cmower/
```

### Comparing `pyoptas-1.0.1/pyoptas.egg-info/SOURCES.txt` & `pyoptas-1.0.2/pyoptas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.1/pyproject.toml` & `pyoptas-1.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyoptas"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Christopher E. Mower", email="christopher.mower@kcl.ac.uk" },
 ]
 description = "An optimization-based task specification library for task and motion planning (TAMP), trajectory optimization, and model predictive control."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyoptas-1.0.1/setup.py` & `pyoptas-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pyoptas",
     description="An optimization-based task specification library for task and motion planning (TAMP), trajectory optimization, and model predictive control.",
-    version="1.0.1",
+    version="1.0.2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cmower/optas",
     project_urls={
         "Bug Tracker": "https://github.com/cmower/optas/issues",
     },
     author="Christopher E. Mower",
```

### Comparing `pyoptas-1.0.1/tests/test_builder.py` & `pyoptas-1.0.2/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.1/tests/test_examples.py` & `pyoptas-1.0.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.1/tests/test_models.py` & `pyoptas-1.0.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.1/tests/test_optas_utils.py` & `pyoptas-1.0.2/tests/test_optas_utils.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.1/tests/test_optimization.py` & `pyoptas-1.0.2/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.1/tests/test_solver.py` & `pyoptas-1.0.2/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.1/tests/test_spatialmath.py` & `pyoptas-1.0.2/tests/test_spatialmath.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.1/tests/test_sx_container.py` & `pyoptas-1.0.2/tests/test_sx_container.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.1/tests/tester_robot_model.py` & `pyoptas-1.0.2/tests/tester_robot_model.py`

 * *Files identical despite different names*

