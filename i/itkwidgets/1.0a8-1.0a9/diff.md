# Comparing `tmp/itkwidgets-1.0a8.tar.gz` & `tmp/itkwidgets-1.0a9.tar.gz`

## Comparing `itkwidgets-1.0a8.tar` & `itkwidgets-1.0a9.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/.idea/workspace.xml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/Makefile
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/conf.py
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/deployments.md
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/development.md
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/index.md
--rw-r--r--   0        0        0     8924 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/integrations.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/make.bat
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/quick_start_guide.md
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/requirements.txt
--rw-r--r--   0        0        0  3051499 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/images/Hello3DWorld.gif
--rw-r--r--   0        0        0    40756 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/images/colab.png
--rw-r--r--   0        0        0   249408 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/images/dask.png
--rw-r--r--   0        0        0    21365 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/images/dask_stack.png
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/images/imjoy-lab.png
--rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/images/imjoy-notebook.png
--rw-r--r--   0        0        0   254991 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/images/itkimage.png
--rw-r--r--   0        0        0   588862 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/images/monai_pytorch.png
--rw-r--r--   0        0        0   255498 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/images/numpy.png
--rw-r--r--   0        0        0   475593 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/images/pyimagej.png
--rw-r--r--   0        0        0   348039 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/images/pyvista.png
--rw-r--r--   0        0        0   165233 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/images/vtkpolydata.png
--rw-r--r--   0        0        0   395283 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/images/xarray.png
--rw-r--r--   0        0        0   416221 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/images/xarray2.png
--rw-r--r--   0        0        0   467117 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/images/zarr.png
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/jupyterlite/jupyterlite_config.json
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/docs/jupyterlite/files/Hello3DWorld.ipynb
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/__init__.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/_initialization_params.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/_type_aliases.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/imjoy.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/render_types.py
--rw-r--r--   0        0        0    14533 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/viewer.py
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/integrations/__init__.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/integrations/dask.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/integrations/imageio.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/integrations/itk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/integrations/meshio.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/integrations/monai.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/integrations/numpy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/integrations/pyimagej.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/integrations/pytorch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/integrations/pyvista.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/integrations/skan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/integrations/vedo.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/integrations/vtk.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/integrations/xarray.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/itkwidgets/integrations/zarr.py
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/utilities/release-notes.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/LICENSE
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/README.md
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/pyproject.toml
--rw-r--r--   0        0        0    15044 2020-02-02 00:00:00.000000 itkwidgets-1.0a8/PKG-INFO
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/ReleaseNotes.txt
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/.idea/workspace.xml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/Makefile
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/conf.py
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/deployments.md
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/development.md
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/index.md
+-rw-r--r--   0        0        0     8924 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/integrations.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/make.bat
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/quick_start_guide.md
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/requirements.txt
+-rw-r--r--   0        0        0  3051499 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/images/Hello3DWorld.gif
+-rw-r--r--   0        0        0    40756 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/images/colab.png
+-rw-r--r--   0        0        0   249408 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/images/dask.png
+-rw-r--r--   0        0        0    21365 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/images/dask_stack.png
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/images/imjoy-lab.png
+-rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/images/imjoy-notebook.png
+-rw-r--r--   0        0        0   254991 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/images/itkimage.png
+-rw-r--r--   0        0        0   588862 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/images/monai_pytorch.png
+-rw-r--r--   0        0        0   255498 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/images/numpy.png
+-rw-r--r--   0        0        0   475593 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/images/pyimagej.png
+-rw-r--r--   0        0        0   348039 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/images/pyvista.png
+-rw-r--r--   0        0        0   165233 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/images/vtkpolydata.png
+-rw-r--r--   0        0        0   395283 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/images/xarray.png
+-rw-r--r--   0        0        0   416221 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/images/xarray2.png
+-rw-r--r--   0        0        0   467117 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/images/zarr.png
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/jupyterlite/jupyterlite_config.json
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/docs/jupyterlite/files/Hello3DWorld.ipynb
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/__init__.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/_initialization_params.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/_type_aliases.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/imjoy.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/render_types.py
+-rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/viewer.py
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/integrations/__init__.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/integrations/dask.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/integrations/imageio.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/integrations/itk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/integrations/meshio.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/integrations/monai.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/integrations/numpy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/integrations/pyimagej.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/integrations/pytorch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/integrations/pyvista.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/integrations/skan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/integrations/vedo.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/integrations/vtk.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/integrations/xarray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/itkwidgets/integrations/zarr.py
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/utilities/release-notes.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/LICENSE
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/README.md
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/pyproject.toml
+-rw-r--r--   0        0        0    16305 2020-02-02 00:00:00.000000 itkwidgets-1.0a9/PKG-INFO
```

### Comparing `itkwidgets-1.0a8/.github/workflows/publish.yml` & `itkwidgets-1.0a9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/.idea/workspace.xml` & `itkwidgets-1.0a9/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/Makefile` & `itkwidgets-1.0a9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/conf.py` & `itkwidgets-1.0a9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/deployments.md` & `itkwidgets-1.0a9/docs/deployments.md`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/index.md` & `itkwidgets-1.0a9/docs/index.md`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/integrations.md` & `itkwidgets-1.0a9/docs/integrations.md`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/make.bat` & `itkwidgets-1.0a9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/quick_start_guide.md` & `itkwidgets-1.0a9/docs/quick_start_guide.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,39 +3,39 @@
 ## Installation
 
 ### Jupyter Notebook
 
 To install the widgets for the Jupyter Notebook with pip:
 
 ```bash
-pip install 'itkwidgets[notebook]>=1.0a6'
+pip install 'itkwidgets[notebook]>=1.0a8'
 ```
 
 Then look for the ImJoy icon at the top in the Jupyter Notebook:
 
 ![ImJoy Icon in Jupyter Notebook](images/imjoy-notebook.png)
 
 ### Jupyter Lab
 
 For Jupyter Lab 3 run:
 
 ```bash
-pip install 'itkwidgets[lab]>=1.0a6'
+pip install 'itkwidgets[lab]>=1.0a8'
 ```
 
 Then look for the ImJoy icon at the top in the Jupyter Notebook:
 
 ![ImJoy Icon in Jupyter Lab](images/imjoy-lab.png)
 
 ### Google Colab
 
 For Google Colab run:
 
 ```bash
-pip install 'itkwidgets>=1.0a6'
+pip install 'itkwidgets>=1.0a8'
 ```
 
 ## Example Notebooks
 
 Example Notebooks can be accessed locally by cloning the repository:
 
 ```bash
```

### Comparing `itkwidgets-1.0a8/docs/images/Hello3DWorld.gif` & `itkwidgets-1.0a9/docs/images/Hello3DWorld.gif`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/images/colab.png` & `itkwidgets-1.0a9/docs/images/colab.png`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/images/dask.png` & `itkwidgets-1.0a9/docs/images/dask.png`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/images/dask_stack.png` & `itkwidgets-1.0a9/docs/images/dask_stack.png`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/images/imjoy-lab.png` & `itkwidgets-1.0a9/docs/images/imjoy-lab.png`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/images/imjoy-notebook.png` & `itkwidgets-1.0a9/docs/images/imjoy-notebook.png`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/images/itkimage.png` & `itkwidgets-1.0a9/docs/images/itkimage.png`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/images/monai_pytorch.png` & `itkwidgets-1.0a9/docs/images/monai_pytorch.png`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/images/numpy.png` & `itkwidgets-1.0a9/docs/images/numpy.png`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/images/pyimagej.png` & `itkwidgets-1.0a9/docs/images/pyimagej.png`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/images/pyvista.png` & `itkwidgets-1.0a9/docs/images/pyvista.png`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/images/vtkpolydata.png` & `itkwidgets-1.0a9/docs/images/vtkpolydata.png`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/images/xarray.png` & `itkwidgets-1.0a9/docs/images/xarray.png`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/images/xarray2.png` & `itkwidgets-1.0a9/docs/images/xarray2.png`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/images/zarr.png` & `itkwidgets-1.0a9/docs/images/zarr.png`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/jupyterlite/jupyterlite_config.json` & `itkwidgets-1.0a9/docs/jupyterlite/jupyterlite_config.json`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/docs/jupyterlite/files/Hello3DWorld.ipynb` & `itkwidgets-1.0a9/docs/jupyterlite/files/Hello3DWorld.ipynb`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/itkwidgets/_initialization_params.py` & `itkwidgets-1.0a9/itkwidgets/_initialization_params.py`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/itkwidgets/_type_aliases.py` & `itkwidgets-1.0a9/itkwidgets/_type_aliases.py`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/itkwidgets/imjoy.py` & `itkwidgets-1.0a9/itkwidgets/imjoy.py`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/itkwidgets/viewer.py` & `itkwidgets-1.0a9/itkwidgets/viewer.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,15 +80,15 @@
                 result = data
             self.init_data[key] = result
 
         itk_viewer = await api.createWindow(
             name=f"itkwidgets viewer {_viewer_count}",
             type="itk-vtk-viewer",
             src="https://kitware.github.io/itk-vtk-viewer/app",
-            fullscreen=False,
+            fullscreen=True,
             data=self.init_data,
             # config should be a python data dictionary and can't be a string e.g. 'pydata-sphinx',
             config=config,
         )
         _viewer_count += 1
 
         self.set_default_ui_values(itk_viewer)
@@ -115,23 +115,17 @@
     async def create_screenshot(self):
         base64_image = await self.itk_viewer.captureImage()
         self.update_screenshot(base64_image)
 
     def update_screenshot(self, base64_image):
         html = HTML(
             f'''
-                <img id=screenshot_{self.wid} src={base64_image}>
-                <script id="script_{self.wid}" type="text/javascript">
-                    var container = document.getElementById("script_{self.wid}").parentNode;
+                <img id="screenshot_{self.wid}" src={base64_image}>
+                <script type="text/javascript">
                     var image = document.getElementById("screenshot_{self.wid}");
-                    if (!image) {{
-                        image = document.createElement("img");
-                        image.id = "screenshot_{self.wid}";
-                        container.appendChild(image);
-                    }}
                     image.src = "{base64_image}";
                     var viewer = document.getElementById("{self.wid}");
                     // Hide the static image if the Viewer is visible
                     image.style.display = viewer ? "none" : "block";
                 </script>
             ''')
         self.img.display(html)
```

### Comparing `itkwidgets-1.0a8/itkwidgets/integrations/__init__.py` & `itkwidgets-1.0a9/itkwidgets/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/itkwidgets/integrations/itk.py` & `itkwidgets-1.0a9/itkwidgets/integrations/itk.py`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/utilities/release-notes.py` & `itkwidgets-1.0a9/utilities/release-notes.py`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/LICENSE` & `itkwidgets-1.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `itkwidgets-1.0a8/pyproject.toml` & `itkwidgets-1.0a9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "visualization",
     "webgl",
     "webgpu",
 ]
 
 requires-python = ">=3.7"
 dependencies = [
-    "itkwasm",
+    "itkwasm >= 1.0b1",
     "imjoy-rpc >= 0.5.13",
     "imjoy-utils >= 0.1.2",
     "numcodecs",
     "zarr",
 ]
 
 [tool.hatch.version]
```

### Comparing `itkwidgets-1.0a8/PKG-INFO` & `itkwidgets-1.0a9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkwidgets
-Version: 1.0a8
+Version: 1.0a9
 Project-URL: Home, https://itkwidgets.readthedocs.io/en/latest/
 Project-URL: Documentation, https://itkwidgets.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itkwidgets
 Author-email: Matt McCormick <matt.mccormick@kitware.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
@@ -211,23 +211,23 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Multimedia :: Graphics
 Requires-Python: >=3.7
 Requires-Dist: imjoy-rpc>=0.5.13
 Requires-Dist: imjoy-utils>=0.1.2
-Requires-Dist: itkwasm
+Requires-Dist: itkwasm>=1.0b1
 Requires-Dist: numcodecs
 Requires-Dist: zarr
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == 'doc'
 Provides-Extra: lab
 Requires-Dist: imjoy-elfinder[jupyter]; extra == 'lab'
 Requires-Dist: imjoy-jupyterlab-extension>=0.1.13; extra == 'lab'
@@ -240,8 +240,83 @@
 
 # itkwidgets
 
 [![Documentation Status](https://readthedocs.org/projects/itkwidgets/badge/?version=latest)](https://itkwidgets.readthedocs.io/en/latest/?badge=latest)
 
 Interactive widgets to visualize images, point sets, and 3D geometry on the web.
 
-Check out the [Quick Start Guide](https://itkwidgets.readthedocs.io/en/latest/quick_start_guide.html) if you're ready to get started or visit the [docs](https://itkwidgets.readthedocs.io/en/latest/) for more information.
+# Getting Started
+
+## Installation
+
+### Jupyter Notebook
+
+To install the widgets for the Jupyter Notebook with pip:
+
+```bash
+pip install 'itkwidgets[notebook]>=1.0a8'
+```
+
+Then look for the ImJoy icon at the top in the Jupyter Notebook:
+
+![ImJoy Icon in Jupyter Notebook](docs/images/imjoy-notebook.png)
+
+### Jupyter Lab
+
+For Jupyter Lab 3 run:
+
+```bash
+pip install 'itkwidgets[lab]>=1.0a8'
+```
+
+Then look for the ImJoy icon at the top in the Jupyter Notebook:
+
+![ImJoy Icon in Jupyter Lab](docs/images/imjoy-lab.png)
+
+### Google Colab
+
+For Google Colab run:
+
+```bash
+pip install 'itkwidgets>=1.0a8'
+```
+
+## Example Notebooks
+
+Example Notebooks can be accessed locally by cloning the repository:
+
+```bash
+git clone -b main https://github.com/InsightSoftwareConsortium/itkwidgets.git
+```
+
+Then navigate into the examples directory:
+
+```bash
+cd itkwidgets/examples
+```
+
+## Usage
+
+In Jupyter, import the view function:
+
+```python
+from itkwidgets import view
+```
+
+Then, call the view function at the end of a cell, passing in the image to examine:
+
+```python
+view(image)
+```
+
+For information on additional options, see the view function docstring:
+
+```python
+view?
+```
+
+See the [deployments](deployments.md) section for a more detailed overview of additional notebook
+options as well as other ways to run and interact with your notebooks.
+
+# Learn more
+
+Visit the [docs](https://itkwidgets.readthedocs.io/en/latest/) for more information on supported notebooks and integrations.
```

