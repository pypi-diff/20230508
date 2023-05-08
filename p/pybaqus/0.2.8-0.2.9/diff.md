# Comparing `tmp/pybaqus-0.2.8.tar.gz` & `tmp/pybaqus-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybaqus-0.2.8.tar", max compression
+gzip compressed data, was "pybaqus-0.2.9.tar", max compression
```

## Comparing `pybaqus-0.2.8.tar` & `pybaqus-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1079 2020-09-09 17:36:39.254008 pybaqus-0.2.8/LICENSE
--rw-r--r--   0        0        0     2780 2022-09-14 11:47:54.941524 pybaqus-0.2.8/README.md
--rw-r--r--   0        0        0       52 2020-09-09 17:36:39.254008 pybaqus-0.2.8/pybaqus/__init__.py
--rw-r--r--   0        0        0    15108 2023-01-06 19:18:05.345302 pybaqus-0.2.8/pybaqus/elements.py
--rw-r--r--   0        0        0     5047 2022-11-10 16:40:59.636871 pybaqus-0.2.8/pybaqus/faces.py
--rw-r--r--   0        0        0   584978 2022-09-21 11:35:14.224726 pybaqus-0.2.8/pybaqus/fil_result.c
--rw-r--r--   0        0        0       78 2022-09-21 08:09:51.276745 pybaqus-0.2.8/pybaqus/fil_result.cpp
--rw-r--r--   0        0        0   453864 2022-09-21 11:35:14.280725 pybaqus-0.2.8/pybaqus/fil_result.html
--rw-r--r--   0        0        0    19016 2023-01-06 19:17:27.930170 pybaqus-0.2.8/pybaqus/fil_result.py
--rw-r--r--   0        0        0   876265 2022-09-21 10:43:53.920498 pybaqus-0.2.8/pybaqus/model.c
--rw-r--r--   0        0        0   805665 2022-09-21 10:43:54.028496 pybaqus-0.2.8/pybaqus/model.html
--rw-r--r--   0        0        0    24939 2023-01-06 19:08:51.034151 pybaqus-0.2.8/pybaqus/model.py
--rw-r--r--   0        0        0     2420 2023-01-06 15:23:59.626946 pybaqus-0.2.8/pybaqus/nodes.py
--rw-r--r--   0        0        0       38 2021-07-27 13:21:20.137074 pybaqus-0.2.8/pybaqus/plot_utils/mpl.py
--rw-r--r--   0        0        0       40 2021-07-27 13:21:29.892856 pybaqus-0.2.8/pybaqus/plot_utils/vtk.py
--rw-r--r--   0        0        0     1127 2022-11-10 16:45:40.057815 pybaqus-0.2.8/pybaqus/reader.py
--rw-r--r--   0        0        0     1315 2020-09-09 17:36:39.254008 pybaqus-0.2.8/pybaqus/step.py
--rw-r--r--   0        0        0       68 2021-07-27 13:24:15.933132 pybaqus-0.2.8/pybaqus/utils.py
--rw-r--r--   0        0        0      637 2023-01-06 19:21:20.900768 pybaqus-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     3675 1970-01-01 00:00:00.000000 pybaqus-0.2.8/setup.py
--rw-r--r--   0        0        0     3585 1970-01-01 00:00:00.000000 pybaqus-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1079 2020-09-09 17:36:39.254008 pybaqus-0.2.9/LICENSE
+-rw-r--r--   0        0        0     2780 2022-09-14 11:47:54.941524 pybaqus-0.2.9/README.md
+-rw-r--r--   0        0        0       52 2020-09-09 17:36:39.254008 pybaqus-0.2.9/pybaqus/__init__.py
+-rw-r--r--   0        0        0    15108 2023-01-06 19:18:05.345302 pybaqus-0.2.9/pybaqus/elements.py
+-rw-r--r--   0        0        0     5047 2022-11-10 16:40:59.636871 pybaqus-0.2.9/pybaqus/faces.py
+-rw-r--r--   0        0        0   584978 2022-09-21 11:35:14.224726 pybaqus-0.2.9/pybaqus/fil_result.c
+-rw-r--r--   0        0        0       78 2022-09-21 08:09:51.276745 pybaqus-0.2.9/pybaqus/fil_result.cpp
+-rw-r--r--   0        0        0   453864 2022-09-21 11:35:14.280725 pybaqus-0.2.9/pybaqus/fil_result.html
+-rw-r--r--   0        0        0    19016 2023-01-06 19:17:27.930170 pybaqus-0.2.9/pybaqus/fil_result.py
+-rw-r--r--   0        0        0   876265 2022-09-21 10:43:53.920498 pybaqus-0.2.9/pybaqus/model.c
+-rw-r--r--   0        0        0   805665 2022-09-21 10:43:54.028496 pybaqus-0.2.9/pybaqus/model.html
+-rw-r--r--   0        0        0    27189 2023-01-06 20:09:19.210113 pybaqus-0.2.9/pybaqus/model.py
+-rw-r--r--   0        0        0     2420 2023-01-06 15:23:59.626946 pybaqus-0.2.9/pybaqus/nodes.py
+-rw-r--r--   0        0        0       38 2021-07-27 13:21:20.137074 pybaqus-0.2.9/pybaqus/plot_utils/mpl.py
+-rw-r--r--   0        0        0       40 2021-07-27 13:21:29.892856 pybaqus-0.2.9/pybaqus/plot_utils/vtk.py
+-rw-r--r--   0        0        0     1127 2022-11-10 16:45:40.057815 pybaqus-0.2.9/pybaqus/reader.py
+-rw-r--r--   0        0        0     1315 2020-09-09 17:36:39.254008 pybaqus-0.2.9/pybaqus/step.py
+-rw-r--r--   0        0        0       68 2021-07-27 13:24:15.933132 pybaqus-0.2.9/pybaqus/utils.py
+-rw-r--r--   0        0        0      637 2023-01-06 20:11:23.515238 pybaqus-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     3675 1970-01-01 00:00:00.000000 pybaqus-0.2.9/setup.py
+-rw-r--r--   0        0        0     3585 1970-01-01 00:00:00.000000 pybaqus-0.2.9/PKG-INFO
```

### Comparing `pybaqus-0.2.8/LICENSE` & `pybaqus-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pybaqus-0.2.8/README.md` & `pybaqus-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pybaqus-0.2.8/pybaqus/elements.py` & `pybaqus-0.2.9/pybaqus/elements.py`

 * *Files identical despite different names*

### Comparing `pybaqus-0.2.8/pybaqus/faces.py` & `pybaqus-0.2.9/pybaqus/faces.py`

 * *Files identical despite different names*

### Comparing `pybaqus-0.2.8/pybaqus/fil_result.c` & `pybaqus-0.2.9/pybaqus/fil_result.c`

 * *Files identical despite different names*

### Comparing `pybaqus-0.2.8/pybaqus/fil_result.html` & `pybaqus-0.2.9/pybaqus/fil_result.html`

 * *Files identical despite different names*

### Comparing `pybaqus-0.2.8/pybaqus/fil_result.py` & `pybaqus-0.2.9/pybaqus/fil_result.py`

 * *Files identical despite different names*

### Comparing `pybaqus-0.2.8/pybaqus/model.c` & `pybaqus-0.2.9/pybaqus/model.c`

 * *Files identical despite different names*

### Comparing `pybaqus-0.2.8/pybaqus/model.html` & `pybaqus-0.2.9/pybaqus/model.html`

 * *Files identical despite different names*

### Comparing `pybaqus-0.2.8/pybaqus/model.py` & `pybaqus-0.2.9/pybaqus/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -152,15 +152,16 @@
 
         """
         if var not in self.elem_output[step][inc]:
             self.elem_output[step][inc][var] = dict()
 
         if elem not in self.elem_output[step][inc][var]:
             etype = self.elements[elem].elem_code
-            self.elem_output[step][inc][var][elem] = np.empty((N_INT_PNTS[etype], 1), dtype=float)
+            self.elem_output[step][inc][var][elem] = np.empty((N_INT_PNTS[etype], 1),
+                                                              dtype=float)
 
         self.elem_output[step][inc][var][elem][intpnt - 1] = data
 
     def add_nodal_output(self, node, var, data, step, inc):
         """Add nodal output results
 
         Parameters
@@ -272,15 +273,17 @@
             keys = sorted(node_ids)
         else:
             # FIXME: have this variable sorted globally
             keys = sorted(list(self.nodes.keys()))
             try:
                 elem_ids = self.elem_output[step][inc][var].keys()
             except KeyError:
-                print(f"Requested output variable {var} not present as element result of the model.")
+                print(
+                    f"Requested output variable {var} not present as element result of the model."
+                )
 
         if var in self.nodal_output[step][inc]:
             results = self.nodal_output[step][inc][var]
         elif var in self.elem_output[step][inc]:
             results = self._nodal_result_from_elements(var, step, inc, elem_ids)
         else:
             # FIXME: handle errors properly some day
@@ -330,14 +333,94 @@
         counter[counter == 0] = np.nan
 
         result = res_nodes / counter
 
         # FIXME: output correct size
         return result
 
+    def get_local_csys(self, direction, step, inc, elem_set=None):
+        """Get the local coordinate system of each element (if present).
+
+        Parameters
+        ----------
+        direction : str
+            Direction of the local coordinate system.
+        step : int
+            Step number.
+        inc : int
+            Increment number within the step.
+        elem_set : str, list, optional
+            Element set.
+
+        Returns
+        -------
+        arraylike :
+            Array (3xn) or (2xn) depending on the dimensionality of the model.
+
+        """
+        if direction == "x":
+            dim = 0
+        elif direction == "y":
+            dim = 1
+        else:
+            dim = 2
+
+        # FIXME: have this variable sorted globally
+        keys = sorted(list(self.elements.keys()))
+
+        # Elements for which the output variable exists
+        keys_out = set(self.local_csys[step][inc].keys())
+
+        # Consider "deleted" elements (i.e. elements that have a 100% of damage according
+        # to the used fracture model)
+        if self._status is not None:
+            status = self.elem_output[step][inc][f"SDV{self._status}"]
+            del_elem = [k for k, v in status.items() if v[0] == 0]
+            keys_out = [k for k in keys_out if k not in del_elem]
+            keys = [k for k in keys if k not in del_elem]
+
+        if elem_set is not None:
+            keys_out, keys = self._map_elem_set_ids_to_output(elem_set, keys, keys_out)
+
+        csys = self.local_csys[step][inc]
+
+        nan_vec = np.ones(self._dimension) * np.nan
+
+        list_res = [csys[k][dim, :] if k in keys_out else nan_vec for k in keys]
+
+        return np.vstack(list_res)
+
+    def _map_elem_set_ids_to_output(self, elem_set, id_elem, id_elem_out):
+        """Get the keys of the elements in the element set mapped to the output array.
+
+        Parameters
+        ----------
+        elem_set : TODO
+        id_elem : TODO
+        id_elem_out : TODO
+
+        Returns
+        -------
+        keys_out : list
+        keys : list
+
+        """
+        set_elements = self.get_elems_from_set(elem_set)
+
+        def filter_elements(elem):
+            if elem in set_elements:
+                return True
+            else:
+                return False
+
+        keys_out = filter(filter_elements, id_elem)
+        keys = filter(filter_elements, id_elem_out)
+
+        return keys_out, keys
+
     def get_time_history_result_from_node(self, var, node_id, steps="all"):
         """Get results for a node duiring the whole simulation.
 
         Parameters
         ----------
         var : TODO
         node_id : TODO
@@ -432,24 +515,15 @@
         if self._status is not None:
             status = self.elem_output[step][inc][f"SDV{self._status}"]
             del_elem = [k for k, v in status.items() if v[0] == 0]
             keys_out = [k for k in keys_out if k not in del_elem]
             keys = [k for k in keys if k not in del_elem]
 
         if elem_set is not None:
-            set_elements = self.get_elems_from_set(elem_set)
-
-            def filter_elements(elem):
-                if elem in set_elements:
-                    return True
-                else:
-                    return False
-
-            keys_out = filter(filter_elements, keys_out)
-            keys = filter(filter_elements, keys)
+            keys_out, keys = self._map_elem_set_ids_to_output(elem_set, keys, keys_out)
 
         elif elem_id is not None:
             set_elements = set(elem_id)
 
             def filter_elements(elem):
                 if elem in set_elements:
                     return True
```

### Comparing `pybaqus-0.2.8/pybaqus/nodes.py` & `pybaqus-0.2.9/pybaqus/nodes.py`

 * *Files identical despite different names*

### Comparing `pybaqus-0.2.8/pybaqus/reader.py` & `pybaqus-0.2.9/pybaqus/reader.py`

 * *Files identical despite different names*

### Comparing `pybaqus-0.2.8/pybaqus/step.py` & `pybaqus-0.2.9/pybaqus/step.py`

 * *Files identical despite different names*

### Comparing `pybaqus-0.2.8/pyproject.toml` & `pybaqus-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybaqus"
-version = "0.2.8"
+version = "0.2.9"
 description = ""
 authors = ["Cristóbal Tapia Camú <crtapia@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/cristobaltapia/pybaqus"
 
 [tool.poetry.dependencies]
 python = "^3.7.7"
```

### Comparing `pybaqus-0.2.8/setup.py` & `pybaqus-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'pyvista>=0.37.0,<0.38.0',
  'scipy>=1.4.1,<2.0.0',
  'tqdm>=4.62.3,<5.0.0',
  'vtk>=9.0.3,<10.0.0']
 
 setup_kwargs = {
     'name': 'pybaqus',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': '',
     'long_description': '# Pybaqus\n\nPybaqus is a python library to import the output files generated by [Abaqus][1] in the ASCII `*.fil` format, and create a [VTK][2] object from the data.\nThe results can then be analyzed in pure python (i.e. no Abaqus licence needed) with the great tools provided by [PyVista][3].\n\n# Features\n\nPybaqus is in a very early development stage.\nTherefore, there are still many unimplemented functionalities.\nHowever, basic operations like importing the mesh and the nodal and element results is implemented and can be used for some analysis.\n\nThe following features are either already implemented or planned:\n\n- [x] Import 2D meshes\n- [x] Import 3D meshes\n- [x] Import nodal results\n- [x] Import element results\n- [x] Element and node sets\n- [x] Extrapolate element results from Gaussian points to nodes _(implemented for some elements)_\n- [ ] Import history output\n- [x] Compute stresses along paths\n- [ ] Compute section forces and moments\n\n# Installation\n\n```\npip install pybaqus\n```\n\n# Quick-start\n\nThe first thing you need is to tell Abaqus that you want am ASCII `*.fil` result file.\nTo get that you need to write the following lines in your `*.inp` file, within the step definition (before the `*End Step` command) e.g.:\n\n```\n...\n*FILE FORMAT, ASCII\n*EL FILE, DIRECTIONS=YES\nS, E, COORD\n*NODE FILE\nCOORD, U\n\n*End Step\n...\n```\n\nYou can specify different output variables (as long as they are available for the elements you are using, of course).\nAfter submitting your model you will get a `*.fil` file.\nThis is the file you need to import it with Pybaqus.\n\nImport the `*.fil` file like this:\n\n```python\nfrom pybaqus import open_fil\n\nres = open_fil("your_result.fil")\n\n```\n\nGreat!\nThat was it. :)\n\nNow you have your results as a VTK object, wrapped by PyVista, and there\'s nothing that can get in your way to analyze your results with pure python.\n\n### Plot the mesh\n\n```python\nimport pyvista as pv\n\nmesh = res.get_mesh()\n\n\nplot = pv.Plotter()\nplot.add_mesh(mesh, show_edges=True, color="white")\nplot.view_xy()\nplot.show()\n```\n\n![Mesh](examples/mesh_hole.png)\n\nCool! But something\'s missing there. Colors!\nWe can plot some of our results like this:\n\n```python\nmesh = res.get_deformed_mesh(step=1, inc=1, scale=3)\ns2 = res.get_nodal_result(var="S2", step=1, inc=1)\nmesh.point_arrays["S2"] = s2\n\nplot = pv.Plotter()\nplot.add_mesh(mesh, show_edges=True, color="white",\n           scalars="S2", show_scalar_bar=True)\nplot.view_xy()\nplot.show()\n```\n\n![Mesh](examples/mesh_results.png)\n\nThat\'s it!\nSince the API is still under development, some of these functions might change.\n\nAnd now you can de whatever you want with your results in python.\nHave fun!\n\n[1]: https://www.3ds.com/products-services/simulia/products/abaqus/\n[2]: https://vtk.org/\n[3]: https://www.pyvista.org/\n',
     'author': 'Cristóbal Tapia Camú',
     'author_email': 'crtapia@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/cristobaltapia/pybaqus',
```

### Comparing `pybaqus-0.2.8/PKG-INFO` & `pybaqus-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybaqus
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Home-page: https://github.com/cristobaltapia/pybaqus
 Author: Cristóbal Tapia Camú
 Author-email: crtapia@gmail.com
 Requires-Python: >=3.7.7,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

