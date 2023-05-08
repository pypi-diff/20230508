# Comparing `tmp/libertem-blobfinder-0.4.1.tar.gz` & `tmp/libertem-blobfinder-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libertem-blobfinder-0.4.1.tar", last modified: Tue Jun 16 10:37:18 2020, max compression
+gzip compressed data, was "libertem-blobfinder-0.5.0.tar", last modified: Mon May  8 12:58:12 2023, max compression
```

## Comparing `libertem-blobfinder-0.4.1.tar` & `libertem-blobfinder-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,39 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-16 10:37:18.000000 libertem-blobfinder-0.4.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)    35149 2020-06-16 10:37:06.000000 libertem-blobfinder-0.4.1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2020-06-16 10:37:06.000000 libertem-blobfinder-0.4.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2358 2020-06-16 10:37:18.000000 libertem-blobfinder-0.4.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      849 2020-06-16 10:37:06.000000 libertem-blobfinder-0.4.1/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-16 10:37:18.000000 libertem-blobfinder-0.4.1/libertem_blobfinder/
--rw-rw-r--   0 travis    (2000) travis    (2000)       53 2020-06-16 10:37:18.000000 libertem-blobfinder-0.4.1/libertem_blobfinder/_baked_revision.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      751 2020-06-16 10:37:18.000000 libertem-blobfinder-0.4.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     3996 2020-06-16 10:37:06.000000 libertem-blobfinder-0.4.1/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-16 10:37:18.000000 libertem-blobfinder-0.4.1/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-16 10:37:18.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder/
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2020-06-16 10:37:06.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2020-06-16 10:37:06.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder/__version__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-16 10:37:18.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-06-16 10:37:06.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16947 2020-06-16 10:37:06.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder/base/correlation.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-16 10:37:18.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder/common/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-06-16 10:37:06.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder/common/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7161 2020-06-16 10:37:06.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder/common/correlation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9998 2020-06-16 10:37:06.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder/common/patterns.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-16 10:37:18.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder/udf/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-06-16 10:37:06.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder/udf/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13229 2020-06-16 10:37:06.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder/udf/correlation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9758 2020-06-16 10:37:06.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder/udf/refinement.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2612 2020-06-16 10:37:06.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder/udf/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      351 2020-06-16 10:37:06.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder/versioning.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-16 10:37:18.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2358 2020-06-16 10:37:18.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      821 2020-06-16 10:37:18.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-16 10:37:18.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-16 10:37:18.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      131 2020-06-16 10:37:18.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       20 2020-06-16 10:37:18.000000 libertem-blobfinder-0.4.1/src/libertem_blobfinder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:12.790321 libertem-blobfinder-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-08 12:58:12.790321 libertem-blobfinder-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:12.778321 libertem-blobfinder-0.5.0/libertem_blobfinder/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-08 12:58:12.782321 libertem-blobfinder-0.5.0/libertem_blobfinder/_baked_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-08 12:58:12.790321 libertem-blobfinder-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:12.782321 libertem-blobfinder-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:12.786321 libertem-blobfinder-0.5.0/src/libertem_blobfinder/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:12.786321 libertem-blobfinder-0.5.0/src/libertem_blobfinder/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16944 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/base/correlation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:12.786321 libertem-blobfinder-0.5.0/src/libertem_blobfinder/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/common/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/common/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:12.786321 libertem-blobfinder-0.5.0/src/libertem_blobfinder/udf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/udf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/udf/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/udf/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/udf/refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/udf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:12.786321 libertem-blobfinder-0.5.0/src/libertem_blobfinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-08 12:58:12.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-08 12:58:12.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:58:12.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:58:12.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-08 12:58:12.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-08 12:58:12.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:12.790321 libertem-blobfinder-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20203 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/tests/test_udf.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `libertem-blobfinder-0.4.1/LICENSE` & `libertem-blobfinder-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libertem-blobfinder-0.4.1/PKG-INFO` & `libertem-blobfinder-0.5.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,73 @@
 Metadata-Version: 2.1
 Name: libertem-blobfinder
-Version: 0.4.1
+Version: 0.5.0
 Summary: LiberTEM correlation and refinement library
 Home-page: https://libertem.github.io/LiberTEM-blobfinder
 Author: the LiberTEM team
 Author-email: libertem-dev@googlegroups.com
 License: GPL v3
-Description: .. _`strain mapping`:
-        
-        LiberTEM-blobfinder is a package for correlation-based peak finding and strain
-        mapping. It is part of the `LiberTEM project
-        <https://libertem.github.io/LiberTEM/>`_.
-        
-        Usage
-        -----
-        
-        See `Usage documentation <https://libertem.github.io/LiberTEM-blobfinder/usage.html>`_!
-        
-        
-        Installation
-        ------------
-        
-        The quick version from PyPI:
-        
-        .. code-block:: shell
-        
-            $ pip install libertem-blobfinder[pyfftw]
-        
-        See `full installation instructions
-        <https://libertem.github.io/LiberTEM-blobfinder/install.html>`_ for more
-        details!
-        
-        .. rubric:: Reference
-        
-        See `blobfinder API reference
-        <https://libertem.github.io/LiberTEM-blobfinder/reference.html>`_ for details!
-        
-        .. rubric:: Examples
-        
-        See `example applications
-        <https://libertem.github.io/LiberTEM-blobfinder/examples.html>`_!
-        
-        License
-        -------
-        
-        LiberTEM-blobfinder is licensed under GPLv3.
-        
 Keywords: electron microscopy
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: pyfftw
-Provides-Extra: udf
 Provides-Extra: common
+Provides-Extra: udf
+License-File: LICENSE
+
+.. _`strain mapping`:
+
+LiberTEM-blobfinder is a package for correlation-based peak finding and strain
+mapping. It is part of the `LiberTEM project
+<https://libertem.github.io/LiberTEM/>`_.
+
+Usage
+-----
+
+See `Usage documentation <https://libertem.github.io/LiberTEM-blobfinder/usage.html>`_!
+
+
+Installation
+------------
+
+The quick version from PyPI:
+
+.. code-block:: shell
+
+    $ pip install libertem-blobfinder[pyfftw]
+
+See `full installation instructions
+<https://libertem.github.io/LiberTEM-blobfinder/install.html>`_ for more
+details!
+
+.. rubric:: Reference
+
+See `blobfinder API reference
+<https://libertem.github.io/LiberTEM-blobfinder/reference.html>`_ for details!
+
+.. rubric:: Examples
+
+See `example applications
+<https://libertem.github.io/LiberTEM-blobfinder/examples.html>`_!
+
+License
+-------
+
+LiberTEM-blobfinder is licensed under GPLv3.
```

### Comparing `libertem-blobfinder-0.4.1/README.rst` & `libertem-blobfinder-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `libertem-blobfinder-0.4.1/setup.py` & `libertem-blobfinder-0.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -72,24 +72,24 @@
 
 setup(
     name="libertem-blobfinder",
     version=find_version("src", "libertem_blobfinder", "__version__.py"),
     license='GPL v3',
     include_package_data=True,
     zip_safe=False,
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     install_requires=[
         "numpy",
         # Moved numba.unsafe.ndarray -> numba.np.unsafe.ndarray
         "numba>=0.49",
     ],
     extras_require={
         'pyfftw': 'pyfftw',
-        'common': ['libertem>=0.4.0.dev0', 'scikit-image'],
-        'udf': ['libertem>=0.4.0.dev0', 'scikit-image', 'matplotlib'],
+        'common': ['libertem>=0.4.0,<1', 'scikit-image'],
+        'udf': ['libertem>=0.5.0,<1', 'scikit-image', 'matplotlib'],
     },
     package_dir={"": "src"},
     # FIXME find_namespace_packages doesn't seem to be supported in Python 3.6
     packages=find_packages(where='src'),
     cmdclass={
         'sdist': BakedRevisionBuilderSdist,
         'build_py': BakedRevisionBuilderBuildPy,
@@ -99,16 +99,19 @@
     long_description=remove_rst_roles(read("README.rst")),
     long_description_content_type="text/x-rst",
     url="https://libertem.github.io/LiberTEM-blobfinder",
     author_email="libertem-dev@googlegroups.com",
     author="the LiberTEM team",
     classifiers=[
         'Development Status :: 4 - Beta',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: POSIX :: Linux',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
         'Intended Audience :: End Users/Desktop',
```

### Comparing `libertem-blobfinder-0.4.1/src/libertem_blobfinder/base/correlation.py` & `libertem-blobfinder-0.5.0/src/libertem_blobfinder/base/correlation.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         refined_y = y + ry - r
         refined_x = x + rx - r
         # print(y, x, refined_y, refined_x, "\n", cutout)
         return (np.float32(refined_y), np.float32(refined_x))
 
 
 @numba.njit
-def peak_elevation(center, corrmap, height, r_min=1.5, r_max=np.float('inf')):
+def peak_elevation(center, corrmap, height, r_min=1.5, r_max=float('inf')):
     '''
     Return the slope of the tightest cone around :code:`center` with height :code:`height`
     that touches :code:`corrmap` between :code:`r_min` and :code:`r_max`.
 
     The correlation of two disks -- mask and perfect diffraction spot -- has the shape of a cone.
     The function's return value correlates with the quality of a correlation. Higher slope
     means a strong peak and
```

### Comparing `libertem-blobfinder-0.4.1/src/libertem_blobfinder/common/correlation.py` & `libertem-blobfinder-0.5.0/src/libertem_blobfinder/common/correlation.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     '''
     Find peaks of the correlation between :code:`sum_result` and :code:`match_pattern`.
 
     The result  can then be used as input to
     :meth:`~libertem.analysis.fullmatch.FullMatcher.full_match`
     to extract grid parameters, :meth:`~libertem_blobfinder.correlation.run_fastcorrelation`
     to find the position in each frame or to construct a mask to extract feature vectors with
-    :meth:`~libertem_blobfinder.utils.feature_vector`.
+    :meth:`~libertem_blobfinder.common.patterns.feature_vector`.
 
     Parameters
     ----------
 
     sum_result: numpy.ndarray
         2D result frame as correlation input
     match_pattern : MatchPattern
```

### Comparing `libertem-blobfinder-0.4.1/src/libertem_blobfinder/common/patterns.py` & `libertem-blobfinder-0.5.0/src/libertem_blobfinder/common/patterns.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 class Circular(MatchPattern):
     '''
     Circular pattern with radius :code:`radius`.
 
     This pattern is useful for constructing feature vectors using
-    :meth:`~libertem_blobfinder.feature_vector`.
+    :meth:`~libertem_blobfinder.common.patterns.feature_vector`.
 
     .. versionadded:: 0.3.0
     '''
     def __init__(self, radius, search=None):
         '''
         Parameters
         ----------
```

### Comparing `libertem-blobfinder-0.4.1/src/libertem_blobfinder/udf/correlation.py` & `libertem-blobfinder-0.5.0/src/libertem_blobfinder/udf/correlation.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,25 +9,28 @@
 from libertem_blobfinder.common.patterns import MatchPattern
 import libertem_blobfinder.base.correlation as ltbc
 from libertem_blobfinder.common.correlation import get_peaks
 
 
 class CorrelationUDF(UDF):
     '''
-    Abstract base class for peak correlation implementations
+    Base class for peak correlation implementations
     '''
-    def __init__(self, peaks, *args, **kwargs):
+    def __init__(self, peaks, zero_shift=None, *args, **kwargs):
         '''
         Parameters
         ----------
 
         peaks : numpy.ndarray
             Numpy array of (y, x) coordinates with peak positions in px to correlate
+        zero_shift : Union[AUXBufferWrapper, numpy.ndarray, None], optional
+            Zero shift, for example descan error. Can be :code:`None`, :code:`numpy.array((y, x))`
+            or AUX data with :code:`(y, x)` for each frame.
         '''
-        super().__init__(peaks=np.round(peaks).astype(int), *args, **kwargs)
+        super().__init__(peaks=np.round(peaks).astype(int), zero_shift=zero_shift, *args, **kwargs)
 
     def get_result_buffers(self):
         '''
         The common buffers for all correlation methods.
 
         :code:`centers`:
             (y, x) integer positions.
@@ -67,35 +70,54 @@
         '''
         r = self.results
         return (r.centers, r.refineds, r.peak_values, r.peak_elevations)
 
     def postprocess(self):
         pass
 
+    def get_peaks(self):
+        return self.params.peaks
+
+    def get_zero_shift(self, index=None):
+        if self.params.zero_shift is None:
+            result = np.array((0, 0))
+        elif index is None:
+            # Called when masked with view
+            result = self.params.zero_shift
+        else:
+            # Called when not masked, in postprocess() etc.
+            result = self.params.zero_shift[index]
+        return result
+
 
 class FastCorrelationUDF(CorrelationUDF):
     '''
     Fourier-based fast correlation-based refinement of peak positions within a search frame
     for each peak.
     '''
-    def __init__(self, *args, **kwargs):
+    def __init__(self, peaks, match_pattern, zero_shift=None, *args, **kwargs):
         '''
         Parameters
         ----------
 
         peaks : numpy.ndarray
             Numpy array of (y, x) coordinates with peak positions in px to correlate
         match_pattern : MatchPattern
             Instance of :class:`~libertem_blobfinder.MatchPattern`
+        zero_shift : Union[AUXBufferWrapper, numpy.ndarray, None], optional
+            Zero shift, for example descan error. Can be :code:`None`, :code:`numpy.array((y, x))`
+            or AUX data with :code:`(y, x)` for each frame.
         '''
         # For testing purposes, allow to inject a different limit via
         # an internal kwarg
         # It has to come through kwarg because of how UDFs are run
         self.limit = kwargs.get('__limit', 2**19)  # 1/2 MB
-        super().__init__(*args, **kwargs)
+        super().__init__(
+            peaks=peaks, match_pattern=match_pattern, zero_shift=zero_shift, *args, **kwargs
+        )
 
     def get_task_data(self):
         ""
         n_peaks = len(self.get_peaks())
         mask = self.get_pattern()
         crop_size = mask.get_crop_size()
         template = mask.get_template(sig_shape=(2 * crop_size, 2 * crop_size))
@@ -103,29 +125,26 @@
         crop_bufs = ltbc.allocate_crop_bufs(crop_size, n_peaks, dtype=dtype, limit=self.limit)
         kwargs = {
             'crop_bufs': crop_bufs,
             'template': template,
         }
         return kwargs
 
-    def get_peaks(self):
-        return self.params.peaks
-
     def get_pattern(self):
         return self.params.match_pattern
 
     def get_template(self):
         return self.task_data.template
 
     def process_frame(self, frame):
         match_pattern = self.get_pattern()
         (centers, refineds, peak_values, peak_elevations) = self.output_buffers()
         ltbc.process_frame_fast(
             template=self.get_template(), crop_size=match_pattern.get_crop_size(),
-            frame=frame, peaks=self.get_peaks(),
+            frame=frame, peaks=self.get_peaks() + np.round(self.get_zero_shift()).astype(int),
             out_centers=centers, out_refineds=refineds,
             out_heights=peak_values, out_elevations=peak_elevations,
             crop_bufs=self.task_data.crop_bufs
         )
 
 
 class FullFrameCorrelationUDF(CorrelationUDF):
@@ -134,30 +153,35 @@
     frame for each peak using a single correlation step. This can be faster for
     correlating a large number of peaks in small frames in comparison to
     :class:`FastCorrelationUDF`. However, it is more sensitive to interference
     from strong peaks next to the peak of interest.
 
     .. versionadded:: 0.3.0
     '''
-    def __init__(self, *args, **kwargs):
+    def __init__(self, peaks, match_pattern, zero_shift=None, *args, **kwargs):
         '''
         Parameters
         ----------
 
         peaks : numpy.ndarray
             Numpy array of (y, x) coordinates with peak positions in px to correlate
         match_pattern : MatchPattern
             Instance of :class:`~libertem_blobfinder.MatchPattern`
+        zero_shift : Union[AUXBufferWrapper, numpy.ndarray, None], optional
+            Zero shift, for example descan error. Can be :code:`None`, :code:`numpy.array((y, x))`
+            or AUX data with :code:`(y, x)` for each frame.
         '''
         # For testing purposes, allow to inject a different limit via
         # an internal kwarg
         # It has to come through kwarg because of how UDFs are run
         self.limit = kwargs.get('__limit', 2**19)  # 1/2 MB
 
-        super().__init__(*args, **kwargs)
+        super().__init__(
+            peaks=peaks, match_pattern=match_pattern, zero_shift=zero_shift, *args, **kwargs
+        )
 
     def get_task_data(self):
         ""
         mask = self.get_pattern()
         n_peaks = len(self.params.peaks)
         template = mask.get_template(sig_shape=self.meta.dataset_shape.sig)
         dtype = np.result_type(self.meta.input_dtype, np.float32)
@@ -166,31 +190,28 @@
         kwargs = {
             'template': template,
             'frame_buf': frame_buf,
             'buf_count': ltbc.get_buf_count(crop_size, n_peaks, dtype, self.limit),
         }
         return kwargs
 
-    def get_peaks(self):
-        return self.params.peaks
-
     def get_pattern(self):
         return self.params.match_pattern
 
     def get_template(self):
         return self.task_data.template
 
     def process_frame(self, frame):
         match_pattern = self.get_pattern()
         (centers, refineds, peak_values, peak_elevations) = self.output_buffers()
         ltbc.process_frame_full(
             template=self.get_template(),
             crop_size=match_pattern.get_crop_size(),
             frame=frame,
-            peaks=self.get_peaks(),
+            peaks=self.get_peaks() + np.round(self.get_zero_shift()).astype(int),
             out_centers=centers,
             out_refineds=refineds,
             out_heights=peak_values,
             out_elevations=peak_elevations,
             frame_buf=self.task_data.frame_buf,
             buf_count=self.task_data.buf_count,
         )
@@ -198,30 +219,34 @@
 
 class SparseCorrelationUDF(CorrelationUDF):
     '''
     Direct correlation using sparse matrices
 
     This method allows to adjust the number of correlation steps independent of the template size.
     '''
-    def __init__(self, *args, **kwargs):
+    def __init__(self, peaks, match_pattern, steps, *args, **kwargs):
         '''
         Parameters
         ----------
 
         peaks : numpy.ndarray
             Numpy array of (y, x) coordinates with peak positions in px to correlate
         match_pattern : MatchPattern
             Instance of :class:`~libertem_blobfinder.MatchPattern`
         steps : int
             The template is correlated with 2 * steps + 1 symmetrically around the peak position
             in x and y direction. This defines the maximum shift that can be
             detected. The number of calculations grows with the square of this value, that means
             keeping this as small as the data allows speeds up the calculation.
         '''
-        super().__init__(*args, **kwargs)
+        super().__init__(
+            peaks=peaks, match_pattern=match_pattern, steps=steps, *args, **kwargs
+        )
+        if self.params.zero_shift is not None:
+            raise ValueError("Parameter zero_shift not supported for SparseCorrelationUDF")
 
     def get_result_buffers(self):
         """
         This method adds the :code:`corr` buffer to the result of
         :meth:`CorrelationUDF.get_result_buffers`. See source code for the
         exact buffer declaration.
         """
@@ -301,52 +326,57 @@
             ltbc.evaluate_correlations(
                 corrs=corrmaps[f], peaks=peaks, crop_size=self.params.steps,
                 out_centers=centers[f], out_refineds=refineds[f],
                 out_heights=peak_values[f], out_elevations=peak_elevations[f]
             )
 
 
-def run_fastcorrelation(ctx, dataset, peaks, match_pattern: MatchPattern, roi=None):
+def run_fastcorrelation(
+        ctx, dataset, peaks, match_pattern: MatchPattern, zero_shift=None, **kwargs):
     """
     Wrapper function to construct and run a :class:`FastCorrelationUDF`
 
     Parameters
     ----------
     ctx : libertem.api.Context
     dataset : libertem.io.dataset.base.DataSet
     peaks : numpy.ndarray
         List of peaks with (y, x) coordinates
     match_pattern : libertem_blobfinder.patterns.MatchPattern
-    roi : numpy.ndarray, optional
-        Boolean mask of the navigation dimension to select region of interest (ROI)
+    zero_shift : Union[AUXBufferWrapper, numpy.ndarray, None], optional
+        Zero shift, for example descan error. Can be :code:`None`, :code:`numpy.array((y, x))`
+        or AUX data with :code:`(y, x)` for each frame.
+    kwargs : passed through to :meth:`~libertem.api.Context.run_udf`
 
     Returns
     -------
     buffers : Dict[libertem.common.buffers.BufferWrapper]
         See :meth:`CorrelationUDF.get_result_buffers` for details.
     """
-    peaks = peaks.astype(np.int)
-    udf = FastCorrelationUDF(peaks=peaks, match_pattern=match_pattern)
-    return ctx.run_udf(dataset=dataset, udf=udf, roi=roi)
+    peaks = peaks.astype(int)
+    udf = FastCorrelationUDF(peaks=peaks, match_pattern=match_pattern, zero_shift=zero_shift)
+    return ctx.run_udf(dataset=dataset, udf=udf, **kwargs)
 
 
-def run_blobfinder(ctx, dataset, match_pattern: MatchPattern, num_peaks, roi=None):
+def run_blobfinder(ctx, dataset, match_pattern: MatchPattern, num_peaks, roi=None, progress=False):
     """
     Wrapper function to find peaks in a dataset and refine their position using
     :class:`FastCorrelationUDF`
 
     Parameters
     ----------
     ctx : libertem.api.Context
     dataset : libertem.io.dataset.base.DataSet
     match_pattern : libertem_blobfinder.patterns.MatchPattern
     num_peaks : int
         Number of peaks to look for
     roi : numpy.ndarray, optional
         Boolean mask of the navigation dimension to select region of interest (ROI)
+    progress : bool, optional
+        Show progress bar
 
     Returns
     -------
     sum_result : numpy.ndarray
         Log-scaled sum frame of the dataset/ROI
     centers, refineds, peak_values, peak_elevations : libertem.common.buffers.BufferWrapper
         See :meth:`CorrelationUDF.get_result_buffers` for details.
@@ -364,13 +394,14 @@
     )
 
     pass_2_results = run_fastcorrelation(
         ctx=ctx,
         dataset=dataset,
         peaks=peaks,
         match_pattern=match_pattern,
-        roi=roi
+        roi=roi,
+        progress=progress
     )
 
     return (sum_result, pass_2_results['centers'],
         pass_2_results['refineds'], pass_2_results['peak_values'],
         pass_2_results['peak_elevations'], peaks)
```

### Comparing `libertem-blobfinder-0.4.1/src/libertem_blobfinder/udf/refinement.py` & `libertem-blobfinder-0.5.0/src/libertem_blobfinder/udf/refinement.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         r = self.results
         for index in range(len(self.results.centers)):
             match = p.matcher.fastmatch(
                 centers=r.centers[index],
                 refineds=r.refineds[index],
                 peak_values=r.peak_values[index],
                 peak_elevations=r.peak_elevations[index],
-                zero=p.start_zero,
+                zero=p.start_zero + self.get_zero_shift(index),
                 a=p.start_a,
                 b=p.start_b,
             )
             self.apply_match(index, match)
 
 
 class AffineMixin(RefinementMixin):
@@ -145,15 +145,15 @@
                 indices=p.indices,
             )
             self.apply_match(index, match)
 
 
 def run_refine(
         ctx, dataset, zero, a, b, match_pattern: MatchPattern, matcher: grm.Matcher,
-        correlation='fast', match='fast', indices=None, steps=5, roi=None):
+        correlation='fast', match='fast', indices=None, steps=5, zero_shift=None, **kwargs):
     '''
     Wrapper function to refine the given lattice for each frame by calculating
     approximate peak positions and refining them for each frame using a
     combination of :class:`libertem_blobfinder.CorrelationUDF` and
     :class:`libertem_blobfinder.RefinementMixin`.
 
     .. versionchanged:: 0.3.0
@@ -191,16 +191,19 @@
         numpy.mgrid[h:k, i:j] works directly to specify indices. This saves
         boilerplate code when using this function.
         Default: numpy.mgrid[-10:10, -10:10].
     steps : int, optional
         Only for correlation == 'sparse': Correlation steps. See
         :meth:`~SparseCorelationUDF.__init__` for
         details.
-    roi : numpy.ndarray, optional
-        ROI for :meth:`~libertem.api.Context.run_udf`
+    zero_shift : Union[AUXBufferWrapper, numpy.ndarray, None], optional
+        Zero shift, for example descan error. Can be :code:`None`, :code:`numpy.array((y, x))`
+        or AUX data with :code:`(y, x)` for each frame. Only supported for correlation methods
+        :code:`fast` and `fullframe`.
+    kwargs : passed through to :meth:`~libertem.api.Context.run_udf`
 
     Returns
     -------
     result : Dict[str, BufferWrapper]
         Result buffers of the UDF. See
         :meth:`libertem_blobfinder.correlation.CorrelationUDF.get_result_buffers` and
         :meth:`RefinementMixin.get_result_buffers` for details on the available
@@ -264,16 +267,17 @@
         peaks=peaks,
         indices=indices,
         start_zero=zero,
         start_a=a,
         start_b=b,
         match_pattern=match_pattern,
         matcher=matcher,
-        steps=steps
+        steps=steps,
+        zero_shift=zero_shift,
     )
 
     result = ctx.run_udf(
         dataset=dataset,
         udf=udf,
-        roi=roi,
+        **kwargs
     )
     return (result, indices)
```

### Comparing `libertem-blobfinder-0.4.1/src/libertem_blobfinder/udf/utils.py` & `libertem-blobfinder-0.5.0/src/libertem_blobfinder/udf/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,44 +8,49 @@
     '''
     Visualize the refinement of a specific frame in matplotlib axes
     '''
     # Get the frame from the dataset
     get_sample_frame = ctx.create_pick_analysis(dataset=ds, y=y, x=x)
     sample_frame = ctx.run(get_sample_frame)
 
+    if y is None:
+        select = (x, )
+    else:
+        select = (y, x)
+
     d = sample_frame[0].raw_data.astype(np.float32)
 
     pcm = axes.imshow(np.log(d - np.min(d) + 1))
 
-    refined = result['refineds'].data[y, x]
-    elevations = result['peak_elevations'].data[y, x]
-    selector = result['selector'].data[y, x]
+    refined = result['refineds'].data[select]
+    elevations = result['peak_elevations'].data[select]
+    selector = result['selector'].data[select]
 
     max_elevation = np.max(elevations)
 
     # Calclate the best fit positions to compare with the
     # individual peak positions.
     # A difference between best fit and individual peaks highlights outliers.
     calculated = grm.calc_coords(
-        zero=result['zero'].data[y, x],
-        a=result['a'].data[y, x],
-        b=result['b'].data[y, x],
+        zero=result['zero'].data[select],
+        a=result['a'].data[select],
+        b=result['b'].data[select],
         indices=indices
     )
 
     paint_markers(
         axes=axes,
         r=r,
         refined=refined,
         normalized_elevations=elevations/max_elevation,
         calculated=calculated,
         selector=selector,
-        zero=result['zero'].data[y, x],
-        a=result['a'].data[y, x],
-        b=result['b'].data[y, x],
+        zero=result['zero'].data[select],
+        a=result['a'].data[select],
+        b=result['b'].data[select],
         colors=colors,
         stretch=stretch,
     )
     return pcm
 
 
 def paint_markers(axes, r, refined, normalized_elevations, calculated, selector, zero, a, b,
```

### Comparing `libertem-blobfinder-0.4.1/src/libertem_blobfinder.egg-info/PKG-INFO` & `libertem-blobfinder-0.5.0/src/libertem_blobfinder.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,73 @@
 Metadata-Version: 2.1
 Name: libertem-blobfinder
-Version: 0.4.1
+Version: 0.5.0
 Summary: LiberTEM correlation and refinement library
 Home-page: https://libertem.github.io/LiberTEM-blobfinder
 Author: the LiberTEM team
 Author-email: libertem-dev@googlegroups.com
 License: GPL v3
-Description: .. _`strain mapping`:
-        
-        LiberTEM-blobfinder is a package for correlation-based peak finding and strain
-        mapping. It is part of the `LiberTEM project
-        <https://libertem.github.io/LiberTEM/>`_.
-        
-        Usage
-        -----
-        
-        See `Usage documentation <https://libertem.github.io/LiberTEM-blobfinder/usage.html>`_!
-        
-        
-        Installation
-        ------------
-        
-        The quick version from PyPI:
-        
-        .. code-block:: shell
-        
-            $ pip install libertem-blobfinder[pyfftw]
-        
-        See `full installation instructions
-        <https://libertem.github.io/LiberTEM-blobfinder/install.html>`_ for more
-        details!
-        
-        .. rubric:: Reference
-        
-        See `blobfinder API reference
-        <https://libertem.github.io/LiberTEM-blobfinder/reference.html>`_ for details!
-        
-        .. rubric:: Examples
-        
-        See `example applications
-        <https://libertem.github.io/LiberTEM-blobfinder/examples.html>`_!
-        
-        License
-        -------
-        
-        LiberTEM-blobfinder is licensed under GPLv3.
-        
 Keywords: electron microscopy
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: pyfftw
-Provides-Extra: udf
 Provides-Extra: common
+Provides-Extra: udf
+License-File: LICENSE
+
+.. _`strain mapping`:
+
+LiberTEM-blobfinder is a package for correlation-based peak finding and strain
+mapping. It is part of the `LiberTEM project
+<https://libertem.github.io/LiberTEM/>`_.
+
+Usage
+-----
+
+See `Usage documentation <https://libertem.github.io/LiberTEM-blobfinder/usage.html>`_!
+
+
+Installation
+------------
+
+The quick version from PyPI:
+
+.. code-block:: shell
+
+    $ pip install libertem-blobfinder[pyfftw]
+
+See `full installation instructions
+<https://libertem.github.io/LiberTEM-blobfinder/install.html>`_ for more
+details!
+
+.. rubric:: Reference
+
+See `blobfinder API reference
+<https://libertem.github.io/LiberTEM-blobfinder/reference.html>`_ for details!
+
+.. rubric:: Examples
+
+See `example applications
+<https://libertem.github.io/LiberTEM-blobfinder/examples.html>`_!
+
+License
+-------
+
+LiberTEM-blobfinder is licensed under GPLv3.
```

### Comparing `libertem-blobfinder-0.4.1/src/libertem_blobfinder.egg-info/SOURCES.txt` & `libertem-blobfinder-0.5.0/src/libertem_blobfinder.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 src/libertem_blobfinder/__init__.py
 src/libertem_blobfinder/__version__.py
 src/libertem_blobfinder/versioning.py
 src/libertem_blobfinder.egg-info/PKG-INFO
 src/libertem_blobfinder.egg-info/SOURCES.txt
@@ -15,9 +16,13 @@
 src/libertem_blobfinder/base/__init__.py
 src/libertem_blobfinder/base/correlation.py
 src/libertem_blobfinder/common/__init__.py
 src/libertem_blobfinder/common/correlation.py
 src/libertem_blobfinder/common/patterns.py
 src/libertem_blobfinder/udf/__init__.py
 src/libertem_blobfinder/udf/correlation.py
+src/libertem_blobfinder/udf/integration.py
 src/libertem_blobfinder/udf/refinement.py
-src/libertem_blobfinder/udf/utils.py
+src/libertem_blobfinder/udf/utils.py
+tests/test_base.py
+tests/test_common.py
+tests/test_udf.py
```

