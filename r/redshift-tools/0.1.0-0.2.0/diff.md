# Comparing `tmp/redshift_tools-0.1.0.tar.gz` & `tmp/redshift_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redshift_tools-0.1.0.tar", last modified: Sat Apr 22 16:00:47 2023, max compression
+gzip compressed data, was "redshift_tools-0.2.0.tar", last modified: Mon May  8 12:22:31 2023, max compression
```

## Comparing `redshift_tools-0.1.0.tar` & `redshift_tools-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-22 16:00:47.203040 redshift_tools-0.1.0/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      148 2023-04-22 15:30:55.000000 redshift_tools-0.1.0/AUTHORS.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1581 2023-04-22 15:42:05.000000 redshift_tools-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)       99 2023-04-22 15:57:52.000000 redshift_tools-0.1.0/HISTORY.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1116 2023-04-14 15:03:33.000000 redshift_tools-0.1.0/LICENSE
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      100 2023-04-14 15:03:33.000000 redshift_tools-0.1.0/MANIFEST.in
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1880 2023-04-22 16:00:47.203112 redshift_tools-0.1.0/PKG-INFO
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1012 2023-04-22 15:39:07.000000 redshift_tools-0.1.0/README.md
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      735 2023-04-14 15:03:33.000000 redshift_tools-0.1.0/pyproject.toml
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1418 2023-04-22 16:00:47.203461 redshift_tools-0.1.0/setup.cfg
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-22 16:00:47.199510 redshift_tools-0.1.0/src/
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-22 16:00:47.201701 redshift_tools-0.1.0/src/redshift_tools/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      320 2023-04-14 15:03:33.000000 redshift_tools-0.1.0/src/redshift_tools/__init__.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2497 2023-04-14 15:34:04.000000 redshift_tools-0.1.0/src/redshift_tools/base.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     5440 2023-04-16 12:01:45.000000 redshift_tools-0.1.0/src/redshift_tools/create.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     4703 2023-04-16 12:01:45.000000 redshift_tools-0.1.0/src/redshift_tools/manipulate.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     5774 2023-04-16 12:01:45.000000 redshift_tools-0.1.0/src/redshift_tools/plot.py
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-22 16:00:47.202649 redshift_tools-0.1.0/src/redshift_tools.egg-info/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1880 2023-04-22 16:00:46.000000 redshift_tools-0.1.0/src/redshift_tools.egg-info/PKG-INFO
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      521 2023-04-22 16:00:47.000000 redshift_tools-0.1.0/src/redshift_tools.egg-info/SOURCES.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-04-22 16:00:46.000000 redshift_tools-0.1.0/src/redshift_tools.egg-info/dependency_links.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-04-16 09:01:24.000000 redshift_tools-0.1.0/src/redshift_tools.egg-info/not-zip-safe
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      326 2023-04-22 16:00:47.000000 redshift_tools-0.1.0/src/redshift_tools.egg-info/requires.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)       15 2023-04-22 16:00:47.000000 redshift_tools-0.1.0/src/redshift_tools.egg-info/top_level.txt
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-22 16:00:47.202790 redshift_tools-0.1.0/tests/
--rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)     1505 2023-04-16 12:01:45.000000 redshift_tools-0.1.0/tests/test_redshift_tools.py
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-05-08 12:22:31.064015 redshift_tools-0.2.0/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      148 2023-04-22 15:30:55.000000 redshift_tools-0.2.0/AUTHORS.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1581 2023-04-22 15:42:05.000000 redshift_tools-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      186 2023-05-08 12:21:50.000000 redshift_tools-0.2.0/HISTORY.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1116 2023-04-14 15:03:33.000000 redshift_tools-0.2.0/LICENSE
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      100 2023-04-14 15:03:33.000000 redshift_tools-0.2.0/MANIFEST.in
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1860 2023-05-08 12:22:31.064095 redshift_tools-0.2.0/PKG-INFO
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1012 2023-04-22 15:39:07.000000 redshift_tools-0.2.0/README.md
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      735 2023-04-14 15:03:33.000000 redshift_tools-0.2.0/pyproject.toml
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1351 2023-05-08 12:22:31.064444 redshift_tools-0.2.0/setup.cfg
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-05-08 12:22:31.059676 redshift_tools-0.2.0/src/
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-05-08 12:22:31.062156 redshift_tools-0.2.0/src/redshift_tools/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      320 2023-05-08 12:21:57.000000 redshift_tools-0.2.0/src/redshift_tools/__init__.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2497 2023-04-14 15:34:04.000000 redshift_tools-0.2.0/src/redshift_tools/base.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     6469 2023-05-08 12:17:28.000000 redshift_tools-0.2.0/src/redshift_tools/create.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     4703 2023-04-16 12:01:45.000000 redshift_tools-0.2.0/src/redshift_tools/manipulate.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     5774 2023-04-16 12:01:45.000000 redshift_tools-0.2.0/src/redshift_tools/plot.py
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-05-08 12:22:31.063547 redshift_tools-0.2.0/src/redshift_tools.egg-info/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1860 2023-05-08 12:22:31.000000 redshift_tools-0.2.0/src/redshift_tools.egg-info/PKG-INFO
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      521 2023-05-08 12:22:31.000000 redshift_tools-0.2.0/src/redshift_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-05-08 12:22:31.000000 redshift_tools-0.2.0/src/redshift_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-04-16 09:01:24.000000 redshift_tools-0.2.0/src/redshift_tools.egg-info/not-zip-safe
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      260 2023-05-08 12:22:31.000000 redshift_tools-0.2.0/src/redshift_tools.egg-info/requires.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)       15 2023-05-08 12:22:31.000000 redshift_tools-0.2.0/src/redshift_tools.egg-info/top_level.txt
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-05-08 12:22:31.063750 redshift_tools-0.2.0/tests/
+-rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)     1855 2023-05-08 12:17:28.000000 redshift_tools-0.2.0/tests/test_redshift_tools.py
```

### Comparing `redshift_tools-0.1.0/CONTRIBUTING.rst` & `redshift_tools-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `redshift_tools-0.1.0/LICENSE` & `redshift_tools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redshift_tools-0.1.0/PKG-INFO` & `redshift_tools-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: redshift_tools
-Version: 0.1.0
+Version: 0.2.0
 Summary: Package to create and mmanipulate redshift distributions for cosmic shear forecasts or analyses
 Author: Silvan Fischbacher
 Author-email: silvanf@phys.ethz.ch
 License: MIT License
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/redshift_tools
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -47,9 +46,7 @@
 -------
 
 The package was created by Silvan Fischbacher
 in the Cosmology Research Group at ETH Zurich.
 
 The package is maintained by Silvan Fischbacher:
 silvanf@phys.ethz.ch
-
-
```

### Comparing `redshift_tools-0.1.0/README.md` & `redshift_tools-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `redshift_tools-0.1.0/pyproject.toml` & `redshift_tools-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `redshift_tools-0.1.0/setup.cfg` & `redshift_tools-0.2.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 install_requires = 
 	numpy
 	matplotlib
 	cycler
 	scipy
 	PyCosmo
 	astropy
-	cosmic_toolbox @ git+https://cosmo-gitlab.phys.ethz.ch/silvanf/cosmic_toolbox.git
+	cosmic_toolbox
 packages = find:
 package_dir = 
 	=src
 zip_safe = False
 python_requires = >=3.7
 
 [options.packages.find]
```

### Comparing `redshift_tools-0.1.0/src/redshift_tools/base.py` & `redshift_tools-0.2.0/src/redshift_tools/base.py`

 * *Files identical despite different names*

### Comparing `redshift_tools-0.1.0/src/redshift_tools/create.py` & `redshift_tools-0.2.0/src/redshift_tools/create.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,14 +23,34 @@
     :param z0: parameter of the Smail-type distribution
     :param normalization: normalization of the Smail-type distribution
     :return: Smail-type redshift distribution
     """
     return z**alpha * np.exp(-((z / z0) ** beta)) * normalization
 
 
+def fu(z, a=0.612, b=8.125, c=0.620, A=None):
+    """
+    Fu-type function for the overall redshift distribution.
+    (z**a + a**(a*b)) / (z**b + c) * A
+    Default values are taken from Fu et al. arXiv:0712.0884
+
+    :param z: redshift
+    :param a: parameter of the Fu-type distribution
+    :param b: parameter of the Fu-type distribution
+    :param c: parameter of the Fu-type distribution
+    :param A: normalization of the Fu-type distribution
+    :return: Fu-type redshift distribution
+    """
+    nz = (z**a + z ** (a * b)) / (z**b + c)
+    if A is None:
+        return normalize(nz, z)
+    else:
+        return nz * A
+
+
 def normalize(y, x):
     """
     Normalize a function to 1
 
     :param y: function values
     :param x: x values
     :return: normalized function
@@ -47,15 +67,14 @@
     :param n_bins: number of bins in which the overall redshift distribution is cut
     :param z_max: maximum redshift
     :param num_z: number of points used for the interpolation
     :param dist_params: parameters of the distribution
     :return: list with the threshold values starting including
         start value (0) and final value (z_max)
     """
-
     z = np.linspace(0, z_max, num_z)
     nz = normalize(distribution(z, **dist_params), z)
     n_per_bin = 1 / n_bins
     z_threshold = [0]
     i_last_threshold = 0
     for i in range(num_z):
         current_fraction = np.trapz(nz[i_last_threshold:i], z[i_last_threshold:i])
@@ -71,41 +90,53 @@
     sigma_z,
     max_z=5,
     min_z=0,
     num_z=1000,
     redshift_dep=False,
     z_t=None,
     normalize_bins=True,
-    **smail_parameters,
+    distribution="smail",
+    **distribution_parameters,
 ):
     """
     Creates redshift bins following an overall Smail-type distribution
 
     :param bins: number of bins
     :param sigma_z: array with the photometric_scatter per bin
     :param max_z: maximum redshift
     :param min_z: minimum redshift
     :param num_z: size of the returned redshift array
     :param redshift_dep: boolean if the photometric scatter has a
-                         redshift dependence sigma_z*(1+z)
+        redshift dependence sigma_z*(1+z)
     :param z_t: thresholds for the different bins.
-                If None, the thresholds are computed
+        If None, the thresholds are computed
     :param normalize_bins: If returned bins should be normalized
-    :param smail_parameters: paramters that specify the
-                             Smail-type distribution
+    :param distribution: type of the overall redshift distribution,
+        options are "smail" or "fu"
+    :param distribution_parameters: paramters that specify the Smail-type or Fu-type
+        distribution
     :return nz: list with num_zx2 arrays with redshift on [:,0]
                 and n(z) on [:,1]
+    :raises ValueError: if distribution is not "smail" or "fu"
     """
     z = np.linspace(min_z, max_z, num_z)
-    n_tot = smail(z, **smail_parameters)
+    if distribution == "smail":
+        dist = smail
+    elif distribution == "fu":
+        dist = fu
+    else:
+        raise ValueError(f"Unknown distribution {distribution}. Use smail or fu.")
 
+    n_tot = dist(z, **distribution_parameters)
     if z_t is None:
-        z_t = find_z_threshold(smail, n_bins, max_z, num_z=num_z, **smail_parameters)
+        z_t = find_z_threshold(
+            dist, n_bins, max_z, num_z=num_z, **distribution_parameters
+        )
         LOGGER.info(
-            "No z thresholds given, bins are cut into equally"
+            "No z thresholds given, bins are cut into equally "
             f"populated bins at {z_t}"
         )
 
     if normalize_bins:
         norm = np.trapz(n_tot, z)
     else:
         norm = 1
```

### Comparing `redshift_tools-0.1.0/src/redshift_tools/manipulate.py` & `redshift_tools-0.2.0/src/redshift_tools/manipulate.py`

 * *Files identical despite different names*

### Comparing `redshift_tools-0.1.0/src/redshift_tools/plot.py` & `redshift_tools-0.2.0/src/redshift_tools/plot.py`

 * *Files identical despite different names*

### Comparing `redshift_tools-0.1.0/src/redshift_tools.egg-info/PKG-INFO` & `redshift_tools-0.2.0/src/redshift_tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: redshift-tools
-Version: 0.1.0
+Version: 0.2.0
 Summary: Package to create and mmanipulate redshift distributions for cosmic shear forecasts or analyses
 Author: Silvan Fischbacher
 Author-email: silvanf@phys.ethz.ch
 License: MIT License
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/redshift_tools
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -47,9 +46,7 @@
 -------
 
 The package was created by Silvan Fischbacher
 in the Cosmology Research Group at ETH Zurich.
 
 The package is maintained by Silvan Fischbacher:
 silvanf@phys.ethz.ch
-
-
```

### Comparing `redshift_tools-0.1.0/src/redshift_tools.egg-info/SOURCES.txt` & `redshift_tools-0.2.0/src/redshift_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redshift_tools-0.1.0/tests/test_redshift_tools.py` & `redshift_tools-0.2.0/tests/test_redshift_tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,20 +21,32 @@
     rt.plot_bins(nz)
     rt.plot_bins([nz, nz2])
     rt.plot_bins(nz, nz_tot)
     rt.plot_bins([nz, nz2], [nz_tot, nz_tot2])
     rt.plot_bins(_get_abspath("test_bins/example_bins"), nz_is_path=True)
 
 
-def test_create():
+def test_create_smail():
     nz, nz_tot = rt.create_bins(5, 0.1 * np.ones(5), redshift_dep=False)
     nz2, nz_tot = rt.create_bins(5, 0.1 * np.ones(5), redshift_dep=True)
     nz3, nz_tot = rt.create_bins(5, 0.1 * np.ones(5), alpha=3, beta=0.5, z0=0.5)
 
 
+def test_create_fu():
+    nz, nz_tot = rt.create_bins(
+        5, 0.1 * np.ones(5), redshift_dep=False, distribution="fu"
+    )
+    nz2, nz_tot = rt.create_bins(
+        5, 0.1 * np.ones(5), redshift_dep=True, distribution="fu"
+    )
+    nz3, nz_tot = rt.create_bins(
+        5, 0.1 * np.ones(5), distribution="fu", a=0.7, b=8.4, c=0.6
+    )
+
+
 def test_shift():
     nz, _ = rt.load_bins(_get_abspath("test_bins/example_bins"))
     rt.manipulate.shift(nz, np.array([0.1, -0.1, 0, 0.2, -0.2]))
     nz0 = rt.manipulate.shift(nz, np.zeros(5))
     for i in range(len(nz)):
         assert np.all(nz[i] == nz0[i])
```

