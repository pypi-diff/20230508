# Comparing `tmp/daemonflux-0.6.0.tar.gz` & `tmp/daemonflux-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daemonflux-0.6.0.tar", last modified: Fri Apr  7 04:18:30 2023, max compression
+gzip compressed data, was "daemonflux-0.6.1.tar", last modified: Mon May  8 08:50:04 2023, max compression
```

## Comparing `daemonflux-0.6.0.tar` & `daemonflux-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:18:30.103651 daemonflux-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-07 04:18:03.000000 daemonflux-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-07 04:18:30.103651 daemonflux-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-07 04:18:03.000000 daemonflux-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-07 04:18:03.000000 daemonflux-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-07 04:18:30.103651 daemonflux-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:18:30.099651 daemonflux-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:18:30.099651 daemonflux-0.6.0/src/daemonflux/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-07 04:18:03.000000 daemonflux-0.6.0/src/daemonflux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21621 2023-04-07 04:18:03.000000 daemonflux-0.6.0/src/daemonflux/flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-04-07 04:18:03.000000 daemonflux-0.6.0/src/daemonflux/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:18:30.103651 daemonflux-0.6.0/src/daemonflux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-07 04:18:30.000000 daemonflux-0.6.0/src/daemonflux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-07 04:18:30.000000 daemonflux-0.6.0/src/daemonflux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 04:18:30.000000 daemonflux-0.6.0/src/daemonflux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-07 04:18:30.000000 daemonflux-0.6.0/src/daemonflux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-07 04:18:30.000000 daemonflux-0.6.0/src/daemonflux.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:18:30.103651 daemonflux-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13462 2023-04-07 04:18:03.000000 daemonflux-0.6.0/tests/test_daemonflux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:50:04.333390 daemonflux-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-08 08:49:33.000000 daemonflux-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-08 08:50:04.333390 daemonflux-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-05-08 08:49:33.000000 daemonflux-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-08 08:49:33.000000 daemonflux-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-08 08:50:04.333390 daemonflux-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:50:04.329390 daemonflux-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:50:04.333390 daemonflux-0.6.1/src/daemonflux/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-08 08:49:33.000000 daemonflux-0.6.1/src/daemonflux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21769 2023-05-08 08:49:33.000000 daemonflux-0.6.1/src/daemonflux/flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-08 08:49:33.000000 daemonflux-0.6.1/src/daemonflux/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:50:04.333390 daemonflux-0.6.1/src/daemonflux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-08 08:50:04.000000 daemonflux-0.6.1/src/daemonflux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-08 08:50:04.000000 daemonflux-0.6.1/src/daemonflux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:50:04.000000 daemonflux-0.6.1/src/daemonflux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 08:50:04.000000 daemonflux-0.6.1/src/daemonflux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 08:50:04.000000 daemonflux-0.6.1/src/daemonflux.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:50:04.333390 daemonflux-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-08 08:49:34.000000 daemonflux-0.6.1/tests/test_daemonflux.py
```

### Comparing `daemonflux-0.6.0/LICENSE` & `daemonflux-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `daemonflux-0.6.0/PKG-INFO` & `daemonflux-0.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daemonflux
-Version: 0.6.0
+Version: 0.6.1
 Summary: Tabulated representation of a muon-calibrated muon and neutrino flux model
 Home-page: https://github.com/mceq-project/daemonflux
 Download-URL: https://pypi.python.org/pypi/daemonflux
 Author: Anatoli Fedynitch
 Maintainer-email: afedynitch@gmail.com
 License: BSD 3-Clause License
 Classifier: Development Status :: 4 - Beta
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: examples
 License-File: LICENSE
 
 # daemonflux: DAta-drivEn and MuOn-calibrated Neutrino flux
 
@@ -76,15 +76,15 @@
 Resulting in the following figure:
 
 ![Muon Neutrino Flux plot](flux_example.png "Muon neutrino flux scaled by $E^3$ for clarity.")
 
 
 ## Explanation of quantities and units
 
-For **neutrinos**, the methods `Flux.flux` and `Flux.error` return values in the units of $(E/\text{GeV})^3/(\text{GeV}~\text{cm}^2~\text{s}~\text{sr})$, i.e. multiplied by $E^3$. For **muon quantities** are reported as a function of total momentum instead of energy, i.e. the units are  $(p/\text{(GeV/c)})^3/(\text{(GeV/c)}~\text{cm}^2~\text{s}~\text{sr})$. Natural units $\hbar=c=1$ are used everywhere.
+For **neutrinos**, the methods `Flux.flux` and `Flux.error` return values in the units of $(E/\text{GeV})^3/(\text{GeV }\text{s }\text{sr }\text{cm}^2)$, i.e. multiplied by $E^3$. For **muon quantities** are reported as a function of total momentum instead of energy, i.e. the units are  $(p/\text{(GeV/c)})^3/(\text{(GeV/c) } \text{s }\text{sr }\text{cm}^2)$. Natural units $\hbar=c=1$ are used everywhere.
 
 The quantities are: 
 
 - muons: `muflux`, `muratio`, `mu+`, `mu-`,
 - muon neutrinos: `numuflux`, `numuratio`, `numu`, `antinumu`, `flavorratio`
 - electron neutrinos: `nueflux`, `nueratio`, `nue`, `antinue`, `flavorratio`
```

### Comparing `daemonflux-0.6.0/README.md` & `daemonflux-0.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 Resulting in the following figure:
 
 ![Muon Neutrino Flux plot](flux_example.png "Muon neutrino flux scaled by $E^3$ for clarity.")
 
 
 ## Explanation of quantities and units
 
-For **neutrinos**, the methods `Flux.flux` and `Flux.error` return values in the units of $(E/\text{GeV})^3/(\text{GeV}~\text{cm}^2~\text{s}~\text{sr})$, i.e. multiplied by $E^3$. For **muon quantities** are reported as a function of total momentum instead of energy, i.e. the units are  $(p/\text{(GeV/c)})^3/(\text{(GeV/c)}~\text{cm}^2~\text{s}~\text{sr})$. Natural units $\hbar=c=1$ are used everywhere.
+For **neutrinos**, the methods `Flux.flux` and `Flux.error` return values in the units of $(E/\text{GeV})^3/(\text{GeV }\text{s }\text{sr }\text{cm}^2)$, i.e. multiplied by $E^3$. For **muon quantities** are reported as a function of total momentum instead of energy, i.e. the units are  $(p/\text{(GeV/c)})^3/(\text{(GeV/c) } \text{s }\text{sr }\text{cm}^2)$. Natural units $\hbar=c=1$ are used everywhere.
 
 The quantities are: 
 
 - muons: `muflux`, `muratio`, `mu+`, `mu-`,
 - muon neutrinos: `numuflux`, `numuratio`, `numu`, `antinumu`, `flavorratio`
 - electron neutrinos: `nueflux`, `nueratio`, `nue`, `antinue`, `flavorratio`
```

### Comparing `daemonflux-0.6.0/setup.cfg` & `daemonflux-0.6.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = daemonflux
-version = 0.6.0
+version = 0.6.1
 author = Anatoli Fedynitch
 maintainer_email = afedynitch@gmail.com
 description = Tabulated representation of a muon-calibrated muon and neutrino flux model
 license = BSD 3-Clause License
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mceq-project/daemonflux
@@ -22,18 +22,18 @@
 	License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 
 [options]
 packages = find:
 package_dir = 
 	= src
 include_package_data = True
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	numpy
-	scipy
+	scipy>=1.8.0
 	rich
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 test =
```

### Comparing `daemonflux-0.6.0/src/daemonflux/flux.py` & `daemonflux-0.6.1/src/daemonflux/flux.py`

 * *Files 2% similar despite different names*

```diff
@@ -534,15 +534,19 @@
                     format_angle(self._zenith_deg_arr[-1]),
                 )
             )
         if len(self._zenith_angles) < 2:
             raise ValueError("Zenith angle array must have at least two elements.")
 
         idxmin = np.digitize(np.min(zenith_angles_deg), self._zenith_deg_arr) - 1
-        idxmax = np.digitize(np.max(zenith_angles_deg), self._zenith_deg_arr)
+        idxmax = min(
+            len(self._zenith_deg_arr),
+            np.digitize(np.max(zenith_angles_deg), self._zenith_deg_arr) + 1,
+        )
+        assert self._zenith_deg_arr[idxmax - 1] >= np.max(zenith_angles_deg)
         if idxmax - idxmin < 2:
             idxmax += 1
             if idxmax > len(self._zenith_deg_arr):
                 idxmin -= 1
                 idxmax -= 1
         return idxmin, idxmax
```

### Comparing `daemonflux-0.6.0/src/daemonflux/utils.py` & `daemonflux-0.6.1/src/daemonflux/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-import urllib
+import urllib.request
 import zipfile
 import numpy as np
 from typing import Dict, Union
 
 
 # Quantities in daemonflux non-prefixed are conventional
 quantities = [
```

### Comparing `daemonflux-0.6.0/src/daemonflux.egg-info/PKG-INFO` & `daemonflux-0.6.1/src/daemonflux.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daemonflux
-Version: 0.6.0
+Version: 0.6.1
 Summary: Tabulated representation of a muon-calibrated muon and neutrino flux model
 Home-page: https://github.com/mceq-project/daemonflux
 Download-URL: https://pypi.python.org/pypi/daemonflux
 Author: Anatoli Fedynitch
 Maintainer-email: afedynitch@gmail.com
 License: BSD 3-Clause License
 Classifier: Development Status :: 4 - Beta
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: examples
 License-File: LICENSE
 
 # daemonflux: DAta-drivEn and MuOn-calibrated Neutrino flux
 
@@ -76,15 +76,15 @@
 Resulting in the following figure:
 
 ![Muon Neutrino Flux plot](flux_example.png "Muon neutrino flux scaled by $E^3$ for clarity.")
 
 
 ## Explanation of quantities and units
 
-For **neutrinos**, the methods `Flux.flux` and `Flux.error` return values in the units of $(E/\text{GeV})^3/(\text{GeV}~\text{cm}^2~\text{s}~\text{sr})$, i.e. multiplied by $E^3$. For **muon quantities** are reported as a function of total momentum instead of energy, i.e. the units are  $(p/\text{(GeV/c)})^3/(\text{(GeV/c)}~\text{cm}^2~\text{s}~\text{sr})$. Natural units $\hbar=c=1$ are used everywhere.
+For **neutrinos**, the methods `Flux.flux` and `Flux.error` return values in the units of $(E/\text{GeV})^3/(\text{GeV }\text{s }\text{sr }\text{cm}^2)$, i.e. multiplied by $E^3$. For **muon quantities** are reported as a function of total momentum instead of energy, i.e. the units are  $(p/\text{(GeV/c)})^3/(\text{(GeV/c) } \text{s }\text{sr }\text{cm}^2)$. Natural units $\hbar=c=1$ are used everywhere.
 
 The quantities are: 
 
 - muons: `muflux`, `muratio`, `mu+`, `mu-`,
 - muon neutrinos: `numuflux`, `numuratio`, `numu`, `antinumu`, `flavorratio`
 - electron neutrinos: `nueflux`, `nueratio`, `nue`, `antinue`, `flavorratio`
```

### Comparing `daemonflux-0.6.0/tests/test_daemonflux.py` & `daemonflux-0.6.1/tests/test_daemonflux.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,49 +87,48 @@
     cov = np.array([[1, 2, 3, 4], [2, 5, 6, 7], [3, 6, 8, 9], [4, 7, 9, 10]])
     expected = np.array([[10, 9, 7, 4], [9, 8, 6, 3], [7, 6, 5, 2], [4, 3, 2, 1]])
 
     assert np.allclose(rearrange_covariance(original_order, new_order, cov), expected)
 
 
 def test_interpolation_domain():
-    zenith_test_dataset = np.array([0, 10, 20, 30, 40, 50, 60, 70, 80, 90], dtype=float)
+    zenith_test_dataset = np.array([0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100], dtype=float)
     mock_spl = dict(
         [(format_angle(z), {"numuflux": [], "muflux": []}) for z in zenith_test_dataset]
     )
     known_parameters = ["p1", "p2"]
     values = np.array([1, 2])
     cov = np.array([[1.0, 0.5], [0.5, 1.0]])
     params = Parameters(known_parameters, values, cov)
     entry = _FluxEntry(
         "mock", fl_spl=mock_spl, jac_spl=mock_spl, params=params, debug=0
     )
-    # entry._zenith_deg_arr = np.array([0, 10, 20, 30, 40, 50, 60, 70, 80, 90])
 
     # Test for a single angle within the range
     assert entry._interpolation_domain(45) == (4, 6)
 
     # Test for multiple angles within the range
-    assert np.all(entry._interpolation_domain(np.array([45.0, 51.0])) == (4, 6))
+    assert np.all(entry._interpolation_domain(np.array([45.0, 51.0])) == (4, 7))
 
     # Test for an angle outside the range
     try:
         entry._interpolation_domain(-5)
     except ValueError as e:
         assert (
             str(e)
-            == "Requested zenith angles must be within the range 0.0000 - 90.0000"
+            == "Requested zenith angles must be within the range 0.0000 - 100.0000"
         )
 
     # Test for multiple angles outside the range
     try:
-        entry._interpolation_domain(np.array([-5.0, 95.0]))
+        entry._interpolation_domain(np.array([-5.0, 105.0]))
     except ValueError as e:
         assert (
             str(e)
-            == "Requested zenith angles must be within the range 0.0000 - 90.0000"
+            == "Requested zenith angles must be within the range 0.0000 - 100.0000"
         )
 
     # Test for unsorted angles
     try:
         entry._interpolation_domain(np.array([50.0, 45.0]))
     except ValueError as e:
         assert str(e) == "Requested angles must be sorted in ascending order."
```

