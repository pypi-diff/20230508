# Comparing `tmp/dicom_numpy-0.6.3.tar.gz` & `tmp/dicom_numpy-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicom_numpy-0.6.3.tar", last modified: Thu Oct  6 19:50:36 2022, max compression
+gzip compressed data, was "dicom_numpy-0.6.4.tar", last modified: Mon May  8 18:53:36 2023, max compression
```

## Comparing `dicom_numpy-0.6.3.tar` & `dicom_numpy-0.6.4.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 19:50:36.497659 dicom_numpy-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-10-06 19:50:24.000000 dicom_numpy-0.6.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-10-06 19:50:36.497659 dicom_numpy-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-10-06 19:50:24.000000 dicom_numpy-0.6.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 19:50:36.497659 dicom_numpy-0.6.3/dicom_numpy/
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-10-06 19:50:24.000000 dicom_numpy-0.6.3/dicom_numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13256 2022-10-06 19:50:24.000000 dicom_numpy-0.6.3/dicom_numpy/combine_slices.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-06 19:50:24.000000 dicom_numpy-0.6.3/dicom_numpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-06 19:50:24.000000 dicom_numpy-0.6.3/dicom_numpy/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-10-06 19:50:24.000000 dicom_numpy-0.6.3/dicom_numpy/zip_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 19:50:36.497659 dicom_numpy-0.6.3/dicom_numpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-10-06 19:50:36.000000 dicom_numpy-0.6.3/dicom_numpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-10-06 19:50:36.000000 dicom_numpy-0.6.3/dicom_numpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-06 19:50:36.000000 dicom_numpy-0.6.3/dicom_numpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-10-06 19:50:36.000000 dicom_numpy-0.6.3/dicom_numpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-06 19:50:36.000000 dicom_numpy-0.6.3/dicom_numpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-10-06 19:50:36.497659 dicom_numpy-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-10-06 19:50:24.000000 dicom_numpy-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:53:36.545419 dicom_numpy-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-08 18:53:26.000000 dicom_numpy-0.6.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-08 18:53:36.545419 dicom_numpy-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-08 18:53:26.000000 dicom_numpy-0.6.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:53:36.545419 dicom_numpy-0.6.4/dicom_numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-08 18:53:26.000000 dicom_numpy-0.6.4/dicom_numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14272 2023-05-08 18:53:26.000000 dicom_numpy-0.6.4/dicom_numpy/combine_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-08 18:53:26.000000 dicom_numpy-0.6.4/dicom_numpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 18:53:26.000000 dicom_numpy-0.6.4/dicom_numpy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-08 18:53:26.000000 dicom_numpy-0.6.4/dicom_numpy/zip_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:53:36.545419 dicom_numpy-0.6.4/dicom_numpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-08 18:53:36.000000 dicom_numpy-0.6.4/dicom_numpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-08 18:53:36.000000 dicom_numpy-0.6.4/dicom_numpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:53:36.000000 dicom_numpy-0.6.4/dicom_numpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-08 18:53:36.000000 dicom_numpy-0.6.4/dicom_numpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 18:53:36.000000 dicom_numpy-0.6.4/dicom_numpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 18:53:36.545419 dicom_numpy-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-08 18:53:26.000000 dicom_numpy-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:53:36.545419 dicom_numpy-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-08 18:53:26.000000 dicom_numpy-0.6.4/tests/test_combine_from_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-05-08 18:53:26.000000 dicom_numpy-0.6.4/tests/test_combine_slices.py
```

### Comparing `dicom_numpy-0.6.3/LICENSE.txt` & `dicom_numpy-0.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dicom_numpy-0.6.3/PKG-INFO` & `dicom_numpy-0.6.4/dicom_numpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dicom_numpy
-Version: 0.6.3
+Name: dicom-numpy
+Version: 0.6.4
 Summary: Extract image data into a 3D numpy array from a set of DICOM files.
 Home-page: https://github.com/innolitics/dicom-numpy
 Author: Innolitics, LLC
 Author-email: info@innolitics.com
 License: MIT
 Keywords: dicom numpy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dicom_numpy-0.6.3/dicom_numpy/combine_slices.py` & `dicom_numpy-0.6.4/dicom_numpy/combine_slices.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,22 @@
 
 from .exceptions import DicomImportException, MissingInstanceNumberException
 
 
 logger = logging.getLogger(__name__)
 
 
-def combine_slices(datasets, rescale=None, enforce_slice_spacing=True, sort_by_instance=False, skip_sorting=False):
+def combine_slices(
+    datasets,
+    rescale=None,
+    enforce_slice_spacing=True,
+    sort_by_instance=False,
+    skip_sorting=False,
+    c_order_axes=False,
+):
     """
     Given a list of pydicom datasets for an image series, stitch them together into a
     three-dimensional numpy array.  Also calculate a 4x4 affine transformation
     matrix that converts the ijk-pixel-indices into the xyz-coordinates in the
     DICOM patient's coordinate system.
 
     Returns a two-tuple containing the 3D-ndarray and the affine matrix.
@@ -42,14 +49,23 @@
     is `True`, a `MissingInstanceNumberException` will be raised.
 
     If `skip_sorting` is set to `True`, `combine_slices` will not attempt to
     sort the slices. This can be useful if the volume must be ordered on other
     tags besides slice position or instance number. This overrides any value
     passed to `sort_by_instance`.
 
+    If `c_order_axes` is set to `True`, the returned array will have its axes
+    returned in the order of `(k, i, j)` rather than `(j, i, k)`. This is done
+    to optimize slice accesses by ensuring that each slice is contiguous in
+    memory. By default, this is done by keeping the axes `(j, i, k)` and storing
+    the array using Fortran ordering. This can cause issues with some serialization
+    libraries that require C-ordering, such as HDF5. In those cases, the axes may
+    be reordered such that slices remain contiguous in memory, but the array is
+    returned in C-ordering.
+
     The returned array has the column-major byte-order.
 
     Datasets produced by reading DICOMDIR files are ignored.
 
     This function requires that the datasets:
 
     - Be in same series (have the same
@@ -91,15 +107,15 @@
     elif sort_by_instance:
         sorted_datasets = sort_by_instance_number(slice_datasets)
     else:
         sorted_datasets = sort_by_slice_position(slice_datasets)
 
     _validate_slices_form_uniform_grid(sorted_datasets, enforce_slice_spacing=enforce_slice_spacing)
 
-    voxels = _merge_slice_pixel_arrays(sorted_datasets, rescale)
+    voxels = _merge_slice_pixel_arrays(sorted_datasets, rescale, c_order_axes=c_order_axes)
     transform = _ijk_to_patient_xyz_transform_matrix(sorted_datasets)
 
     return voxels, transform
 
 
 def sort_by_instance_number(slice_datasets):
     """
@@ -140,34 +156,42 @@
 
 
 def _is_dicomdir(dataset):
     media_sop_class = getattr(dataset, 'MediaStorageSOPClassUID', None)
     return media_sop_class == '1.2.840.10008.1.3.10'
 
 
-def _merge_slice_pixel_arrays(sorted_datasets, rescale=None):
+def _merge_slice_pixel_arrays(sorted_datasets, rescale=None, c_order_axes=False):
     if rescale is None:
         rescale = any(_requires_rescaling(d) for d in sorted_datasets)
 
     first_dataset = sorted_datasets[0]
     slice_dtype = first_dataset.pixel_array.dtype
-    slice_shape = first_dataset.pixel_array.T.shape
     num_slices = len(sorted_datasets)
-
-    voxels_shape = slice_shape + (num_slices,)
     voxels_dtype = np.float32 if rescale else slice_dtype
-    voxels = np.empty(voxels_shape, dtype=voxels_dtype, order='F')
+
+    if c_order_axes:
+        slice_shape = first_dataset.pixel_array.shape
+        voxels_shape = (num_slices,) + slice_shape
+        voxels = np.empty(voxels_shape, dtype=voxels_dtype)
+    else:
+        slice_shape = first_dataset.pixel_array.T.shape
+        voxels_shape = slice_shape + (num_slices,)
+        voxels = np.empty(voxels_shape, dtype=voxels_dtype, order='F')
 
     for k, dataset in enumerate(sorted_datasets):
-        pixel_array = dataset.pixel_array.T
+        pixel_array = dataset.pixel_array if c_order_axes else dataset.pixel_array.T
         if rescale:
             slope = float(getattr(dataset, 'RescaleSlope', 1))
             intercept = float(getattr(dataset, 'RescaleIntercept', 0))
             pixel_array = pixel_array.astype(np.float32) * slope + intercept
-        voxels[..., k] = pixel_array
+        if c_order_axes:
+            voxels[k, ...] = pixel_array
+        else:
+            voxels[..., k] = pixel_array
 
     return voxels
 
 
 def _requires_rescaling(dataset):
     return hasattr(dataset, 'RescaleSlope') or hasattr(dataset, 'RescaleIntercept')
```

### Comparing `dicom_numpy-0.6.3/dicom_numpy/zip_archive.py` & `dicom_numpy-0.6.4/dicom_numpy/zip_archive.py`

 * *Files identical despite different names*

### Comparing `dicom_numpy-0.6.3/dicom_numpy.egg-info/PKG-INFO` & `dicom_numpy-0.6.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dicom-numpy
-Version: 0.6.3
+Name: dicom_numpy
+Version: 0.6.4
 Summary: Extract image data into a 3D numpy array from a set of DICOM files.
 Home-page: https://github.com/innolitics/dicom-numpy
 Author: Innolitics, LLC
 Author-email: info@innolitics.com
 License: MIT
 Keywords: dicom numpy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dicom_numpy-0.6.3/setup.py` & `dicom_numpy-0.6.4/setup.py`

 * *Files identical despite different names*

