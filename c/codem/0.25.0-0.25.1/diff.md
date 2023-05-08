# Comparing `tmp/codem-0.25.0.tar.gz` & `tmp/codem-0.25.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codem-0.25.0.tar", last modified: Wed Mar  1 16:16:16 2023, max compression
+gzip compressed data, was "codem-0.25.1.tar", last modified: Mon May  8 20:56:26 2023, max compression
```

## Comparing `codem-0.25.0.tar` & `codem-0.25.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 16:16:16.591636 codem-0.25.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-01 16:15:59.000000 codem-0.25.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-03-01 16:16:16.591636 codem-0.25.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-03-01 16:15:59.000000 codem-0.25.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-03-01 16:15:59.000000 codem-0.25.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 16:16:16.591636 codem-0.25.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 16:16:16.587636 codem-0.25.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 16:16:16.587636 codem-0.25.0/src/codem/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-01 16:15:59.000000 codem-0.25.0/src/codem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 16:16:16.587636 codem-0.25.0/src/codem/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 16:15:59.000000 codem-0.25.0/src/codem/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-01 16:15:59.000000 codem-0.25.0/src/codem/lib/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-01 16:15:59.000000 codem-0.25.0/src/codem/lib/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    15540 2023-03-01 16:15:59.000000 codem-0.25.0/src/codem/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 16:16:16.587636 codem-0.25.0/src/codem/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 16:15:59.000000 codem-0.25.0/src/codem/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23496 2023-03-01 16:15:59.000000 codem-0.25.0/src/codem/preprocessing/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 16:16:16.587636 codem-0.25.0/src/codem/registration/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-01 16:15:59.000000 codem-0.25.0/src/codem/registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17446 2023-03-01 16:15:59.000000 codem-0.25.0/src/codem/registration/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)    24421 2023-03-01 16:15:59.000000 codem-0.25.0/src/codem/registration/dsm.py
--rw-r--r--   0 runner    (1001) docker     (123)    17307 2023-03-01 16:15:59.000000 codem-0.25.0/src/codem/registration/icp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 16:16:16.587636 codem-0.25.0/src/codem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-03-01 16:16:16.000000 codem-0.25.0/src/codem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-01 16:16:16.000000 codem-0.25.0/src/codem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 16:16:16.000000 codem-0.25.0/src/codem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-01 16:16:16.000000 codem-0.25.0/src/codem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 16:16:16.000000 codem-0.25.0/src/codem.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-01 16:16:16.000000 codem-0.25.0/src/codem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-01 16:16:16.000000 codem-0.25.0/src/codem.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 16:16:16.587636 codem-0.25.0/src/vcd/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-01 16:15:59.000000 codem-0.25.0/src/vcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-03-01 16:15:59.000000 codem-0.25.0/src/vcd/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 16:16:16.587636 codem-0.25.0/src/vcd/meshing/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-01 16:15:59.000000 codem-0.25.0/src/vcd/meshing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-03-01 16:15:59.000000 codem-0.25.0/src/vcd/meshing/mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 16:16:16.591636 codem-0.25.0/src/vcd/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-01 16:15:59.000000 codem-0.25.0/src/vcd/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-03-01 16:15:59.000000 codem-0.25.0/src/vcd/preprocessing/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 16:16:16.591636 codem-0.25.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-03-01 16:15:59.000000 codem-0.25.0/tests/test_registration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.755257 codem-0.25.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 20:56:07.000000 codem-0.25.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-05-08 20:56:26.755257 codem-0.25.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-08 20:56:07.000000 codem-0.25.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-08 20:56:07.000000 codem-0.25.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:56:26.755257 codem-0.25.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.751257 codem-0.25.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.751257 codem-0.25.1/src/codem/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.755257 codem-0.25.1/src/codem/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/lib/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/lib/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16296 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.755257 codem-0.25.1/src/codem/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29467 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/preprocessing/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.755257 codem-0.25.1/src/codem/registration/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17758 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/registration/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24882 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/registration/dsm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17692 2023-05-08 20:56:07.000000 codem-0.25.1/src/codem/registration/icp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.755257 codem-0.25.1/src/codem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-05-08 20:56:26.000000 codem-0.25.1/src/codem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-08 20:56:26.000000 codem-0.25.1/src/codem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:56:26.000000 codem-0.25.1/src/codem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 20:56:26.000000 codem-0.25.1/src/codem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:56:26.000000 codem-0.25.1/src/codem.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 20:56:26.000000 codem-0.25.1/src/codem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 20:56:26.000000 codem-0.25.1/src/codem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.755257 codem-0.25.1/src/vcd/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-08 20:56:07.000000 codem-0.25.1/src/vcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-05-08 20:56:07.000000 codem-0.25.1/src/vcd/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.755257 codem-0.25.1/src/vcd/meshing/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 20:56:07.000000 codem-0.25.1/src/vcd/meshing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-08 20:56:07.000000 codem-0.25.1/src/vcd/meshing/mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.755257 codem-0.25.1/src/vcd/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-08 20:56:07.000000 codem-0.25.1/src/vcd/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11610 2023-05-08 20:56:07.000000 codem-0.25.1/src/vcd/preprocessing/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:56:26.755257 codem-0.25.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-05-08 20:56:08.000000 codem-0.25.1/tests/test_registration.py
```

### Comparing `codem-0.25.0/LICENSE` & `codem-0.25.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codem-0.25.0/PKG-INFO` & `codem-0.25.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: codem
-Version: 0.25.0
+Version: 0.25.1
 Summary: A package for co-registering geospatial data
 Author: Jesse Shanahan, Bahirah Adewunmi
 Author-email: Preston Hartzell <pjhartzell@uh.edu>
 Maintainer-email: Ognyan Moore <ogi@hobu.co>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/NCALM-UH/CODEM
 Project-URL: repository, https://github.com/NCALM-UH/CODEM
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CODEM: Multi-Modal Digital Elevation Model Registration
 
 ![Registered Mesh](./docs/img/reg_mesh.png)
```

### Comparing `codem-0.25.0/pyproject.toml` & `codem-0.25.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "codem"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 description = "A package for co-registering geospatial data"
 readme = "readme.md"
 license = { text = "Apache-2.0" }
 authors = [
   { name = "Preston Hartzell", email = "pjhartzell@uh.edu"},
   { name = "Jesse Shanahan" },
   { name = "Bahirah Adewunmi" }
@@ -62,39 +62,42 @@
     | build
     | dist
   )/
 )
 '''
 
 [tool.mypy]
-python_version = 3.7
+python_version = 3.9
 warn_return_any = true
 disallow_untyped_defs = true
 disallow_untyped_calls = true
 disallow_incomplete_defs = true
 
 [[tool.mypy.overrides]]
 module = [
   "cv2",
   "enlighten",
   "matplotlib",
+  "matplotlib.colors",
   "matplotlib.pyplot",
   "matplotlib.tri",
   "pandas",
   "pdal",
   "pyproj",
   "pyproj.aoi",
   "pyproj.crs",
   "pyproj.database",
   "pyproj.enums",
   "pyproj.transformer",
   "rasterio",
+  "rasterio.coords",
   "rasterio.crs",
   "rasterio.enums",
   "rasterio.fill",
+  "rasterio.transform",
   "rich",
   "rich.console",
   "rich.logging",
   "rich.progress",
   "scipy",
   "scipy.sparse",
   "scipy.spatial",
```

### Comparing `codem-0.25.0/readme.md` & `codem-0.25.1/readme.md`

 * *Files identical despite different names*

### Comparing `codem-0.25.0/src/codem/lib/log.py` & `codem-0.25.1/src/codem/lib/log.py`

 * *Files identical despite different names*

### Comparing `codem-0.25.0/src/codem/main.py` & `codem-0.25.1/src/codem/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import yaml
 from codem.lib.log import Log
+from codem.preprocessing.preprocess import clip_data
 from codem.preprocessing.preprocess import GeoData
 from codem.preprocessing.preprocess import instantiate
 from codem.registration import ApplyRegistration
 from codem.registration import DsmRegistration
 from codem.registration import IcpRegistration
 from distutils.util import strtobool
 
@@ -93,14 +94,15 @@
     ICP_MAX_ITER: int = 100
     ICP_RMSE_THRESHOLD: float = 0.0001
     ICP_ROBUST: bool = True
     ICP_SOLVE_SCALE: bool = True
     VERBOSE: bool = False
     ICP_SAVE_RESIDUALS: bool = False
     OUTPUT_DIR: Optional[str] = None
+    TIGHT_SEARCH: bool = False
 
     def __post_init__(self) -> None:
         # set output directory
         if self.OUTPUT_DIR is None:
             current_time = time.localtime(time.time())
             timestamp = "%d-%02d-%02d_%02d-%02d-%02d" % (
                 current_time.tm_year,
@@ -281,15 +283,29 @@
         "--icp_solve_scale",
         "-iss",
         type=str2bool,
         default=True,
         help="boolean to include or exclude scale from the solved registration",
     )
     ap.add_argument(
-        "--verbose", "-v", type=str2bool, default=False, help="turn on verbose logging"
+        "--icp-save-residuals",
+        action="store_true",
+        help="Write ICP residual information",
+    )
+    ap.add_argument(
+        "--verbose", "-v", action="store_true", help="turn on verbose logging"
+    )
+    ap.add_argument(
+        "--tight-search",
+        "-ts",
+        action="store_true",
+        help=(
+            "Limits the registration search to the region of overlap. Both datasets "
+            "must have the same CRS defined."
+        ),
     )
     return ap.parse_args()
 
 
 def create_config(args: argparse.Namespace) -> Dict[str, Any]:
     config = CodemRunConfig(
         os.fsdecode(os.path.abspath(args.foundation_file)),
@@ -305,15 +321,16 @@
         ICP_ANGLE_THRESHOLD=float(args.icp_angle_threshold),
         ICP_DISTANCE_THRESHOLD=float(args.icp_distance_threshold),
         ICP_MAX_ITER=int(args.icp_max_iter),
         ICP_RMSE_THRESHOLD=float(args.icp_rmse_threshold),
         ICP_ROBUST=args.icp_robust,
         ICP_SOLVE_SCALE=args.icp_solve_scale,
         VERBOSE=args.verbose,
-        ICP_SAVE_RESIDUALS=False,
+        ICP_SAVE_RESIDUALS=args.icp_save_residuals,
+        TIGHT_SEARCH=args.tight_search,
     )
     return dataclasses.asdict(config)
 
 
 def run_console(
     config: Dict[str, Any], logger: logging.Logger, console: Console
 ) -> None:
@@ -347,14 +364,15 @@
         for key in config:
             logger.info(f"{key} = {config[key]}")
         progress.advance(registration, 1)
 
         console.print("══════════PREPROCESSING DATA══════════", justify="center")
         # status.update(stage="Preprocessing Inputs", force=True)
         fnd_obj, aoi_obj = preprocess(config)
+        clip_data(fnd_obj, aoi_obj, config)
         progress.advance(registration, 7)
         fnd_obj.prep()
         progress.advance(registration, 45)
         aoi_obj.prep()
         progress.advance(registration, 4)
         logger.info(
             f"Registration resolution has been set to: {fnd_obj.resolution} meters"
@@ -388,14 +406,19 @@
                 "leaving the min_resolution parameter to default value.",
                 UserWarning,
                 stacklevel=2,
             )
     else:
         resolution = max(fnd_obj.native_resolution, aoi_obj.native_resolution)
     fnd_obj.resolution = aoi_obj.resolution = resolution
+
+    # create DSM, but if doing tight-search do not resample
+    resample = not config["TIGHT_SEARCH"]
+    fnd_obj._create_dsm(resample=resample)
+    aoi_obj._create_dsm(resample=resample)
     return fnd_obj, aoi_obj
 
 
 def coarse_registration(
     fnd_obj: GeoData, aoi_obj: GeoData, config: Dict[str, Any]
 ) -> DsmRegistration:
     dsm_reg = DsmRegistration(fnd_obj, aoi_obj, config)
```

### Comparing `codem-0.25.0/src/codem/preprocessing/preprocess.py` & `codem-0.25.1/src/codem/preprocessing/preprocess.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,24 +22,33 @@
 * DSM - class for Digital Surface Model data
 * PointCloud - class for Point Cloud data
 * Mesh - class for Mesh data
 * instantiate - method for auto-instantiating the appropriate class
 """
 import json
 import logging
+import math
 import os
 import tempfile
+from typing import Any
+from typing import Dict
 from typing import Optional
+from typing import Tuple
 
 import codem.lib.resources as r
 import cv2
 import numpy as np
 import pdal
+import pyproj
 import rasterio.fill
+import rasterio.transform
 import trimesh
+from rasterio import windows
+from rasterio.coords import BoundingBox
+from rasterio.coords import disjoint_bounds
 from rasterio.crs import CRS
 from rasterio.enums import Resampling
 from typing_extensions import TypedDict
 
 
 class RegistrationParameters(TypedDict):
     matrix: np.ndarray
@@ -98,14 +107,17 @@
         self.processed = False
         self._resolution = 0.0
         self.native_resolution = 0.0
         self.units_factor = 1.0
         self.units: Optional[str] = None
         self.weak_size = config["DSM_WEAK_FILTER"]
         self.strong_size = config["DSM_STRONG_FILTER"]
+        self.config = config
+        self.bound_slices: Optional[Tuple[slice, slice]] = None
+        self.window: Optional[windows.Window] = None
 
     @property
     def type(self) -> str:
         return self._type
 
     @type.setter
     def type(self, value: str) -> None:
@@ -118,32 +130,34 @@
     @resolution.setter
     def resolution(self, value: float) -> None:
         if value <= 0.0:
             raise ValueError("Resolution must be greater than 0")
         self._resolution = value
         return None
 
-    def _read_dsm(self, file_path: str) -> None:
+    def _read_dsm(self, file_path: str, force: bool = False) -> None:
         """
         Reads in DSM data from a given file path.
 
         Parameters
         ----------
         file_path: str
             Path to DSM data
         """
         tag = ["AOI", "Foundation"][int(self.fnd)]
 
-        if self.dsm.size == 0:
+        if self.dsm.size == 0 or force:
             with rasterio.open(file_path) as data:
-                self.dsm = data.read(1)
-                self.transform = data.transform
+                self.dsm = data.read(1, window=self.window)
+                if self.window is None:
+                    self.transform = data.transform
+                else:
+                    self.transform = data.window_transform(self.window)
                 self.nodata = data.nodata
                 self.crs = data.crs
-
                 tags = data.tags()
             if "AREA_OR_POINT" in tags and tags["AREA_OR_POINT"] == "Area":
                 self.area_or_point = "Area"
             elif "AREA_OR_POINT" in tags and tags["AREA_OR_POINT"] == "Point":
                 self.area_or_point = "Point"
             else:
                 self.area_or_point = "Area"
@@ -294,38 +308,40 @@
             (array["NormalX"], array["NormalY"], array["NormalZ"])
         ).T
         self.normal_vectors = filtered_normals
 
     def _calculate_resolution(self) -> None:
         raise NotImplementedError
 
-    def _create_dsm(self) -> None:
+    def _create_dsm(self, resample: bool = True) -> None:
         raise NotImplementedError
 
     def prep(self) -> None:
         """
         Prepares data for registration.
         """
         tag = ["AOI", "Foundation"][int(self.fnd)]
         self.logger.info(f"Preparing {tag}-{self.type.upper()} for registration.")
-        self._create_dsm()
         self._infill()
         self._normalize()
         self._dsm2pc()
 
         if self.fnd:
             self._generate_vectors()
 
         self.processed = True
 
     def _debug_plot(self, keypoints: Optional[np.ndarray] = None) -> None:
         """Use this to show the raster"""
         import matplotlib.pyplot as plt
 
-        plt.imshow(self.infilled, cmap="gray")
+        if hasattr(self, "infilled"):
+            plt.imshow(self.infilled, cmap="gray")
+        else:
+            plt.imshow(self.dsm, cmap="gray")
         if keypoints is not None:
             plt.scatter(
                 keypoints[:, 0], keypoints[:, 1], marker="s", color="orange", s=10.0
             )
         plt.show()
 
 
@@ -335,21 +351,24 @@
     """
 
     def __init__(self, config: dict, fnd: bool) -> None:
         super().__init__(config, fnd)
         self.type = "dsm"
         self._calculate_resolution()
 
-    def _create_dsm(self) -> None:
+    def _create_dsm(self, resample: bool = True) -> None:
         """
         Resamples the DSM to the registration pipeline resolution and applies
         a scale factor to convert to meters.
         """
+
         with rasterio.open(self.file) as data:
-            resample_factor = self.native_resolution / self.resolution
+            resample_factor = (
+                self.native_resolution / self.resolution if resample else 1.0
+            )
             tag = ["AOI", "Foundation"][int(self.fnd)]
             if resample_factor != 1:
                 self.logger.info(
                     f"Resampling {tag}-{self.type.upper()} to a pixel resolution of: {self.resolution} meters"
                 )
                 # data is read as float32 as int dtypes result in poor keypoint identification
                 self.dsm = data.read(
@@ -357,29 +376,39 @@
                     out_shape=(
                         data.count,
                         int(data.height * resample_factor),
                         int(data.width * resample_factor),
                     ),
                     resampling=Resampling.cubic,
                     out_dtype=np.float32,
+                    window=self.window,
                 )
                 # We post-multiply the transform by the resampling scale. This does
                 # not change the origin coordinates, only the pixel scale.
-                self.transform = data.transform * data.transform.scale(
-                    (data.width / self.dsm.shape[-1]),
-                    (data.height / self.dsm.shape[-2]),
-                )
+                if self.window is None:
+                    self.transform = data.transform * data.transform.scale(
+                        (data.width / self.dsm.shape[-1]),
+                        (data.height / self.dsm.shape[-2]),
+                    )
+                else:
+                    transform = data.window_transform(self.window)
+                    self.transform = transform * transform.scale(
+                        (data.width / self.dsm.shape[1]),
+                        (data.height / self.dsm.shape[0]),
+                    )
             else:
                 self.logger.info(
                     f"No resampling required for {tag}-{self.type.upper()}"
                 )
                 # data is read as float32 as int dtypes result in poor keypoint identification
-                self.dsm = data.read(1, out_dtype=np.float32)
-                self.transform = data.transform
-
+                self.dsm = data.read(1, out_dtype=np.float32, window=self.window)
+                if self.window is None:
+                    self.transform = data.transform
+                else:
+                    self.transform = data.window_transform(self.window)
             self.nodata = data.nodata
             self.crs = data.crs
 
             # Scale the elevation values into meters
             mask = (self._get_nodata_mask(self.dsm)).astype(bool)
             if np.can_cast(self.units_factor, self.dsm.dtype, casting="same_kind"):
                 self.dsm[mask] *= self.units_factor
@@ -413,15 +442,14 @@
             elif "AREA_OR_POINT" in tags and tags["AREA_OR_POINT"] == "Point":
                 self.area_or_point = "Point"
             else:
                 self.area_or_point = "Area"
                 self.logger.debug(
                     f"'AREA_OR_POINT' not supplied in {tag}-{self.type.upper()} - defaulting to 'Area'"
                 )
-
         if self.nodata is None:
             self.logger.info(f"{tag}-{self.type.upper()} does not have a nodata value.")
         if self.transform == rasterio.Affine.identity():
             self.logger.warning(f"{tag}-{self.type.upper()} has an identity transform.")
 
     def _calculate_resolution(self) -> None:
         """
@@ -473,15 +501,15 @@
     """
 
     def __init__(self, config: dict, fnd: bool) -> None:
         super().__init__(config, fnd)
         self.type = "pcloud"
         self._calculate_resolution()
 
-    def _create_dsm(self) -> None:
+    def _create_dsm(self, resample: bool = True) -> None:
         """
         Converts the point cloud to meters and rasters it to a DSM.
         """
         tag = ["AOI", "Foundation"][int(self.fnd)]
         self.logger.info(
             f"Extracting DSM from {tag}-{self.type.upper()} with resolution of: {self.resolution} meters"
         )
@@ -507,15 +535,15 @@
                 "filename": tmp_file,
             },
         ]
 
         p = pdal.Pipeline(json.dumps(pipe))
         p.execute()
 
-        self._read_dsm(tmp_file)
+        self._read_dsm(tmp_file, force=True)
         os.close(file_handle)
         os.remove(tmp_file)
 
     def _calculate_resolution(self) -> None:
         """
         Calculates point cloud average point spacing.
         """
@@ -559,15 +587,15 @@
     """
 
     def __init__(self, config: dict, fnd: bool) -> None:
         super().__init__(config, fnd)
         self.type = "mesh"
         self._calculate_resolution()
 
-    def _create_dsm(self) -> None:
+    def _create_dsm(self, resample: bool = True) -> None:
         """
         Converts mesh vertices to meters and rasters them to a DSM.
         """
         tag = ["AOI", "Foundation"][int(self.fnd)]
         self.logger.info(
             f"Extracting DSM from {tag}-{self.type.upper()} with resolution of: {self.resolution} meters"
         )
@@ -673,7 +701,120 @@
         return DSM(config, fnd)
     if os.path.splitext(file_path)[-1] in r.mesh_filetypes:
         return Mesh(config, fnd)
     if os.path.splitext(file_path)[-1] in r.pcloud_filetypes:
         return PointCloud(config, fnd)
     logger.warning(f"File {file_path} has an unsupported type.")
     raise NotImplementedError("File type not currently supported.")
+
+
+def clip_data(fnd_obj: GeoData, aoi_obj: GeoData, config: Dict[str, Any]) -> None:
+    # how much outside of the bounds to search for registration features
+    oversize_scale = 1.5
+
+    if not config["TIGHT_SEARCH"]:
+        return None
+
+    # is foundation CRS defined:
+    if any(crs is None for crs in (fnd_obj.crs, aoi_obj.crs)):
+        raise AttributeError(
+            "To perform this operation, the CRS of both datasets must be defined and equal"
+        )
+
+    foundation_crs = pyproj.CRS(fnd_obj.crs)
+    compliment_crs = pyproj.CRS(aoi_obj.crs)
+
+    if not foundation_crs.equals(compliment_crs):
+        raise ValueError(
+            "To perform this operation, the CRS of both datasets must be equal"
+        )
+
+    # create our original and scaled bounding boxes (only handles right/bottom)
+    original_bounding_boxes: Dict[str, BoundingBox] = {}
+    scaled_bounding_boxes: Dict[str, BoundingBox] = {}
+    for dataset in [fnd_obj, aoi_obj]:
+        for scaling in (1.0, oversize_scale):
+            if math.isclose(scaling, 1.0):
+                bounding_boxes = original_bounding_boxes
+            else:
+                bounding_boxes = scaled_bounding_boxes
+            key = "foundation" if dataset.fnd else "compliment"
+            if dataset.transform is None:
+                raise RuntimeError("Transform needs to be specified for the datasets")
+
+            transform = dataset.transform * dataset.transform.scale(scaling)
+            left, top = transform * (0, 0)
+            right, bottom = transform * dataset.dsm.shape
+            bounding_boxes[key] = BoundingBox(left, bottom, right, top)
+
+    # need to adjust scale on left and top due to transform scaling math
+    for dataset in [fnd_obj, aoi_obj]:
+        key = "foundation" if dataset.fnd else "compliment"
+        x_expanded = abs(
+            scaled_bounding_boxes[key].right - original_bounding_boxes[key].right
+        )
+        y_expanded = abs(
+            scaled_bounding_boxes[key].bottom - original_bounding_boxes[key].bottom
+        )
+        left_new = scaled_bounding_boxes[key].left - x_expanded
+        top_new = scaled_bounding_boxes[key].top + y_expanded
+
+        right_new = scaled_bounding_boxes[key].right
+        bottom_new = scaled_bounding_boxes[key].bottom
+        scaled_bounding_boxes[key] = BoundingBox(
+            left_new, bottom_new, right_new, top_new
+        )
+
+    if disjoint_bounds(bounding_boxes["foundation"], bounding_boxes["compliment"]):
+        raise ValueError("Bounding boxes for foundation and compliment are disjoint")
+
+    # get new bounding boxes
+    clipped_bounding_boxes = compute_clipped_bounds(
+        original_bounding_boxes, scaled_bounding_boxes
+    )
+
+    for key in ("foundation", "compliment"):
+        dataset_obj = fnd_obj if key == "foundation" else aoi_obj
+        transform = rasterio.transform.AffineTransformer(dataset_obj.transform)
+        xs, ys = transform.rowcol(
+            [clipped_bounding_boxes[key].left, clipped_bounding_boxes[key].right],
+            [clipped_bounding_boxes[key].top, clipped_bounding_boxes[key].bottom],
+        )
+        dataset_obj.window = windows.Window.from_slices(slice(*xs), slice(*ys))
+        # need that we know the window, create the DSM with resampling
+        dataset_obj._create_dsm(resample=True)
+    return None
+
+
+def compute_clipped_bounds(
+    original: Dict[str, BoundingBox], scaled: Dict[str, BoundingBox]
+) -> Dict[str, BoundingBox]:
+    foundation_original = original["foundation"]
+    foundation_scaled = scaled["foundation"]
+    compliment_original = original["compliment"]
+    compliment_scaled = scaled["compliment"]
+
+    trimmed_foundation: Dict[str, float] = {}
+    trimmed_compliment: Dict[str, float] = {}
+    sides = foundation_original._fields
+    for fixed in ("foundation", "compliment"):
+        if fixed == "foundation":
+            new_bounds = trimmed_foundation
+            scaled = compliment_scaled
+            edge = foundation_original
+        else:
+            new_bounds = trimmed_compliment
+            scaled = foundation_scaled
+            edge = compliment_original
+
+        for side in sides:
+            closer = max if side in ("left", "bottom") else min
+            new_bounds[side] = closer(getattr(edge, side), getattr(scaled, side))
+    clipped_bounds: Dict[str, BoundingBox] = {
+        "foundation": BoundingBox(
+            *[trimmed_foundation[side] for side in ("left", "bottom", "right", "top")]
+        )
+    }
+    clipped_bounds["compliment"] = BoundingBox(
+        *[trimmed_compliment[side] for side in ("left", "bottom", "right", "top")]
+    )
+    return clipped_bounds
```

### Comparing `codem-0.25.0/src/codem/registration/apply.py` & `codem-0.25.1/src/codem/registration/apply.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from typing import Union
 
 import codem.lib.resources as r
 import numpy as np
 import pdal
 import rasterio
 import trimesh
+from codem import __version__
 from codem.preprocessing.preprocess import GeoData
 from codem.preprocessing.preprocess import RegistrationParameters
 from matplotlib.tri import LinearTriInterpolator
 from matplotlib.tri import Triangulation
 from numpy.lib import recfunctions as rfn
 
 
@@ -78,15 +79,17 @@
         self.fnd_units_factor = fnd_obj.units_factor
         self.fnd_units = fnd_obj.units
         self.aoi_file = aoi_obj.file
         self.aoi_nodata = aoi_obj.nodata
         self.aoi_resolution = aoi_obj.native_resolution
         self.aoi_units_factor = aoi_obj.units_factor
         self.aoi_type = aoi_obj.type
+        self.aoi_area_or_point = aoi_obj.area_or_point
         self.registration_transform = registration_parameters["matrix"]
+        self.registration_rmse = registration_parameters["rmse_3d"]
         self.residual_vectors = residual_vectors
         self.residual_origins = residual_origins
         self.config = config
 
         in_name = os.path.basename(self.aoi_file)
         root, ext = os.path.splitext(in_name)
         if output_format is not None:
@@ -94,15 +97,15 @@
                 output_format if output_format.startswith(".") else f".{output_format}"
             )
         out_name = f"{root}_registered{ext}"
         self.out_name: str = os.path.join(self.config["OUTPUT_DIR"], out_name)
 
     def get_registration_transformation(
         self,
-    ) -> Union[np.ndarray, Dict[str, str]]:
+    ) -> Union[np.ndarray, pdal.Pipeline]:
         """
         Generates the transformation from the AOI to FND coordinate system.
         The transformation accommodates linear unit differences and the solved
         registration matrix, which is only valid for linear units of meters.
 
         Returns
         --------
@@ -123,24 +126,21 @@
             return aoi_to_fnd_array
         else:
             aoi_to_fnd_array = np.reshape(aoi_to_fnd_array, (1, 16))
             aoi_to_fnd_string = [
                 " ".join(item) for item in aoi_to_fnd_array.astype(str)
             ][0]
             if self.fnd_crs is not None:
-                registration_transformation = {
-                    "type": "filters.transformation",
-                    "matrix": aoi_to_fnd_string,
-                    "override_srs": self.fnd_crs.to_string(),
-                }
+                registration_transformation = pdal.Filter.transformation(
+                    matrix=aoi_to_fnd_string, override_srs=self.fnd_crs.to_string()
+                )
             else:
-                registration_transformation = {
-                    "type": "filters.transformation",
-                    "matrix": aoi_to_fnd_string,
-                }
+                registration_transformation = pdal.Filter.transforamtion(
+                    matrix=aoi_to_fnd_string
+                )
             return registration_transformation
 
     def apply(self) -> None:
         """
         Call the appropriate registration function depending on data type
         """
         if os.path.splitext(self.aoi_file)[-1] in r.dsm_filetypes:
@@ -155,51 +155,57 @@
         Applies the registration transformation to a dsm file.
         We do not simply edit the transform of the DSM file because that is
         generally used to express 2D information. Instead, we apply the solved
         3D transformation to the 2.5D data and "re-raster" it.
         """
         input_name = os.path.basename(self.aoi_file)
         root, ext = os.path.splitext(input_name)
-        output_name = root + "_registered" + ext
+        output_name = f"{root}_registered{ext}"
         output_path = os.path.join(self.config["OUTPUT_DIR"], output_name)
 
         # construct pdal pipeline
-        pipe = [{"type": "readers.gdal", "filename": self.aoi_file, "header": "Z"}]
+        pipeline = pdal.Reader.gdal(filename=self.aoi_file, header="Z")
 
         # no nodata is present, filter based on its limits
         if self.aoi_nodata is not None:
-            range_filter_task = {
-                "type": "filters.range",
-                "limits": "Z![{}:{}]".format(self.aoi_nodata, self.aoi_nodata),
-            }
-            pipe.append(range_filter_task)
+            pipeline |= pdal.Filter.range(
+                limits=f"Z![{self.aoi_nodata}:{self.aoi_nodata}]"
+            )
 
         # insert the transform filter to register the AOI
         registration_task = self.get_registration_transformation()
-        if isinstance(registration_task, dict):
-            pipe.append(registration_task)
+        if isinstance(registration_task, pdal.pipeline.Filter):
+            pipeline |= registration_task
         else:
             raise ValueError(
-                f"get_registration_transoformation returned {type(registration_task)} "
+                f"get_registration_transformation returned {type(registration_task)} "
                 "not a dictionary of strings as needed for the pdal pipeline."
             )
 
-        # pdal writing task
-        writer_task = {
-            "type": "writers.gdal",
+        writer_kwargs = {
             "resolution": self.aoi_resolution,
             "output_type": "idw",
             "filename": output_path,
+            "metadata": (
+                f"CODEM_VERSION={__version__},"
+                "CODEM_INFO=Data registered and adjusted to "
+                f"{os.path.basename(self.config['FND_FILE'])} by NCALM CODEM. "
+                f"Total registration mean square error {self.registration_rmse:.3f},"
+                "TIFFTAG_IMAGEDESCRIPTION=RegisteredCompliment"
+            ),
         }
-        # Add nodata argument only if nodata is actually present
+
+        if self.aoi_area_or_point in ("Area", "Point"):
+            writer_kwargs["metadata"] += f",AREA_OR_POINT={self.aoi_area_or_point}"  # type: ignore
+
         if self.aoi_nodata is not None:
-            writer_task["nodata"] = self.aoi_nodata
-        pipe.append(writer_task)
-        p = pdal.Pipeline(json.dumps(pipe))
-        p.execute()
+            writer_kwargs["nodata"] = self.aoi_nodata
+
+        pipeline |= pdal.Writer.gdal(**writer_kwargs)
+        pipeline.execute()
 
         self.logger.info(
             f"Registration has been applied to AOI-DSM and saved to: {self.out_name}"
         )
         if self.config["ICP_SAVE_RESIDUALS"]:
             with rasterio.open(self.out_name) as src:
                 dsm = src.read(1)
@@ -248,15 +254,15 @@
             res_z = np.reshape(res_z, dsm.shape)
             res_horiz = np.reshape(res_horiz, dsm.shape)
             res_3d = np.reshape(res_3d, dsm.shape)
 
             # save the interpolated data to a new TIF file. We only save to TIF
             # files since they are known to handle additional bands.
             root, _ = os.path.splitext(self.out_name)
-            out_name_res = root + "_residuals.tif"
+            out_name_res = f"{root}_residuals.tif"
 
             profile.update(count=6, driver="GTiff")
 
             with rasterio.open(out_name_res, "w", **profile) as dst:
                 dst.write(dsm, 1)
                 dst.write(res_x, 2)
                 dst.write(res_y, 3)
@@ -326,31 +332,26 @@
                 f"ICP residuals have been computed for each registered AOI-MESH vertex and saved to: {out_name_res}"
             )
 
     def _apply_pointcloud(self) -> None:
         """
         Applies the registration transformation to a point cloud file.
         """
-        pipe = [
-            self.aoi_file,
-            self.get_registration_transformation(),
-            self.out_name,
-        ]
-        p = pdal.Pipeline(json.dumps(pipe))
-        p.execute()
+        pipeline = pdal.Reader(self.aoi_file)
+        pipeline |= self.get_registration_transformation()
+        pipeline |= pdal.Writer.las(filename=self.out_name)
+
+        pipeline.execute()
         self.logger.info(
             f"Registration has been applied to AOI-PCLOUD and saved to: {self.out_name}"
         )
 
         if self.config["ICP_SAVE_RESIDUALS"]:
             # open up the registered output file, read in xy's
-            pipe = [
-                self.out_name,
-            ]
-            p = pdal.Pipeline(json.dumps(pipe))
+            p = pdal.Reader(self.out_name).pipeline()
             p.execute()
             arrays = p.arrays
             array = arrays[0]
             x = array["X"]
             y = array["Y"]
 
             # interpolate the residual grid for each xy
```

### Comparing `codem-0.25.0/src/codem/registration/dsm.py` & `codem-0.25.1/src/codem/registration/dsm.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,25 @@
 * DsmRegistration: a class for DSM to DSM registration
 * Unscaled3dSimilarityTransform: a class for solving the 6-parameter
   transformation (no scale factor) between two sets of 3D points.
 * Scaled3dSimilarityTransform: a class for solving the 7-parameter
   transformation (includes a scale factor) between two sets of 3D points.
 """
 import logging
+import math
 import os
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Tuple
 
 import cv2
 import numpy as np
 from codem.preprocessing.preprocess import GeoData
+from codem.preprocessing.preprocess import RegistrationParameters
 from rasterio import Affine
 from skimage.measure import ransac
 
 
 class DsmRegistration:
     """
     A class to solve the transformation between two Digital Surface Models.
@@ -105,28 +107,28 @@
         self.fnd_kp, self.fnd_desc = self._get_kp(
             self.fnd_obj.normed, self.fnd_obj.nodata_mask
         )
         self.logger.debug(f"{len(self.fnd_kp)} keypoints detected in foundation")
         if len(self.fnd_kp) < 4:
             raise RuntimeError(
                 (
-                    f"{len(self.fnd_kp)} keypoints were identiifed in the Foundation data"
+                    f"{len(self.fnd_kp)} keypoints were identified in the Foundation data"
                     " (4 required).  Consider modifying the DSM_AKAZE_THRESHOLD parameter,"
                     f" current value is {self.config['DSM_AKAZE_THRESHOLD']}"
                 )
             )
 
         self.aoi_kp, self.aoi_desc = self._get_kp(
             self.aoi_obj.normed, self.aoi_obj.nodata_mask
         )
         self.logger.debug(f"{len(self.aoi_kp)} keypoints detected in area of interest")
         if len(self.aoi_kp) < 4:
             raise RuntimeError(
                 (
-                    f"{len(self.aoi_kp)} keypoints were identiifed in the "
+                    f"{len(self.aoi_kp)} keypoints were identified in the "
                     "AOI data (4 required).  Consider modifying the DSM_AKAZE_THRESHOLD"
                     f"parameter, current value is {self.config['DSM_AKAZE_THRESHOLD']}"
                 )
             )
         self._get_putative()
         self._filter_putative()
         self._save_match_img()
@@ -349,15 +351,15 @@
         Returns
         -------
         xyz: np.array
             Geospatial coordinates
         """
         z = []
         for cr in uv:
-            cr_int = np.int32(np.rint(cr))
+            cr_int = np.rint(cr).astype(np.int32)
             z.append(dsm[cr_int[1], cr_int[0]])
 
         # When using the transform to convert from pixels to object space
         # coordinates, we need to increment the pixel coordinates by 0.5 if the
         # transform origin is defined at  the upper left corner of the upper
         # left pixel
         if area_or_point == "Area":
@@ -399,15 +401,15 @@
         omega = np.rad2deg(np.arctan2(R[2, 1] / c, R[2, 2] / c))
         phi = np.rad2deg(-np.arcsin(R[2, 0] / c))
         kappa = np.rad2deg(np.arctan2(R[1, 0] / c, R[0, 0] / c))
         tx = X[0, 3]
         ty = X[1, 3]
         tz = X[2, 3]
 
-        self.registration_parameters = {
+        self.registration_parameters: RegistrationParameters = {
             "matrix": X,
             "omega": omega,
             "phi": phi,
             "kappa": kappa,
             "trans_x": tx,
             "trans_y": ty,
             "trans_z": tz,
@@ -420,16 +422,15 @@
         }
 
         output_file = os.path.join(self.config["OUTPUT_DIR"], "registration.txt")
 
         self.logger.info(
             f"Saving DSM feature registration parameters to: {output_file}"
         )
-        with open(output_file, "w") as f:
-
+        with open(output_file, "w", encoding="utf_8") as f:
             f.write("DSM FEATURE REGISTRATION")
             f.write("\n------------------------")
             f.write(f"\nTransformation matrix: \n {X}")
             f.write("\nTransformation Parameters:")
             f.write(f"\nOmega = {omega:.3f} degrees")
             f.write(f"\nPhi = {phi:.3f} degrees")
             f.write(f"\nKappa = {kappa:.3f} degrees")
@@ -441,14 +442,21 @@
             f.write("\nRMSEs:")
             f.write(
                 f"\nX = +/-{self.rmse_xyz[0]:.3f},"
                 f"\nY = +/-{self.rmse_xyz[1]:.3f},"
                 f"\nZ = +/-{self.rmse_xyz[2]:.3f},"
                 f"\n3D = +/-{self.rmse_3d:.3f}"
             )
+            f.write("\nPropagated Error:")
+            f.write(
+                "\nAssumed global 3D error = +/-3m"
+                f"\n3D_RMSE = +/-{self.rmse_3d:.3f}"
+                "\nTotal Error is computed as √(global_3d_error²+3D_RMSE²)"
+                f"\nTotal Error = +/-{math.hypot(3, self.rmse_3d):.3f}"
+            )
             f.write("\n\n")
 
 
 class Scaled3dSimilarityTransform:
     """
     A class for solving a 3D similarity transformation between two sets of 3D
     points. For use with scikit-image's RANSAC routing. The _umeyama method is
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `codem-0.25.0/src/codem/registration/icp.py` & `codem-0.25.1/src/codem/registration/icp.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 This module contains the following class:
 
 * IcpRegistration: a class for point cloud to point cloud registration
 """
 from __future__ import annotations
 
 import logging
+import math
 import os
 from typing import Any
 from typing import Dict
 from typing import Tuple
 from typing import TYPE_CHECKING
 
 import numpy as np
@@ -67,16 +68,16 @@
         self.fixed = fnd_obj.point_cloud
         self.normals = fnd_obj.normal_vectors
         self.moving = aoi_obj.point_cloud
         self.resolution = aoi_obj.resolution
         self.initial_transform = dsm_reg.registration_parameters["matrix"]
         self.outlier_thresh = dsm_reg.registration_parameters["rmse_3d"]
         self.config = config
-        self.residual_origins = np.empty((0, 0), np.double)
-        self.residual_vectors = np.empty((0, 0), np.double)
+        self.residual_origins: np.ndarray = np.empty((0, 0), np.double)
+        self.residual_vectors: np.ndarray = np.empty((0, 0), np.double)
 
         assert (
             self.fixed.shape[1] == 3
             and self.moving.shape[1] == 3
             and self.normals.shape[1] == 3
         ), "Point and normal vector data must be 3D."
         assert (
@@ -461,15 +462,15 @@
             "rmse_y": self.rmse_xyz[1],
             "rmse_z": self.rmse_xyz[2],
             "rmse_3d": self.rmse_3d,
         }
         output_file = os.path.join(self.config["OUTPUT_DIR"], "registration.txt")
 
         self.logger.info(f"Saving ICP registration parameters to: {output_file}")
-        with open(output_file, "a") as f:
+        with open(output_file, "a", encoding="utf_8") as f:
             f.write("ICP REGISTRATION")
             f.write("\n----------------")
             f.write(f"\nTransformation matrix: \n {X}")
             f.write("\nTransformation Parameters:")
             f.write(f"\nOmega = {omega:.3f} degrees")
             f.write(f"\nPhi = {phi:.3f} degrees")
             f.write(f"\nKappa = {kappa:.3f} degrees")
@@ -481,8 +482,15 @@
             f.write("\nRMSEs:")
             f.write(
                 f"\nX = +/-{self.rmse_xyz[0]:.3f},"
                 f"\nY = +/-{self.rmse_xyz[1]:.3f},"
                 f"\nZ = +/-{self.rmse_xyz[2]:.3f},"
                 f"\n3D = +/-{self.rmse_3d:.3f}"
             )
+            f.write("\nPropagated Error:")
+            f.write(
+                "\nAssumed global 3D error = +/-3m"
+                f"\n3D_RMSE = +/-{self.rmse_3d:.3f}"
+                "\nTotal Error is computed as √(global_3d_error²+3D_RMSE²)"
+                f"\nTotal Error = +/-{math.hypot(3, self.rmse_3d)}"
+            )
             f.write("\n\n")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `codem-0.25.0/src/codem.egg-info/PKG-INFO` & `codem-0.25.1/src/codem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: codem
-Version: 0.25.0
+Version: 0.25.1
 Summary: A package for co-registering geospatial data
 Author: Jesse Shanahan, Bahirah Adewunmi
 Author-email: Preston Hartzell <pjhartzell@uh.edu>
 Maintainer-email: Ognyan Moore <ogi@hobu.co>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/NCALM-UH/CODEM
 Project-URL: repository, https://github.com/NCALM-UH/CODEM
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CODEM: Multi-Modal Digital Elevation Model Registration
 
 ![Registered Mesh](./docs/img/reg_mesh.png)
```

### Comparing `codem-0.25.0/src/codem.egg-info/SOURCES.txt` & `codem-0.25.1/src/codem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codem-0.25.0/src/vcd/main.py` & `codem-0.25.1/src/vcd/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     GROUNDHEIGHT: float = 1.0
     RESOLUTION: float = 2.0
     VERBOSE: bool = False
     MIN_POINTS: int = 30
     CLUSTER_TOLERANCE: float = 2.0
     CULL_CLUSTER_IDS: Tuple[int, ...] = (-1, 0, 1)
     OUTPUT_DIR: Optional[str] = None
+    COLORMAP: str = "RdBu"
 
     def __post_init__(self) -> None:
         # set output directory
         if self.OUTPUT_DIR is None:
             current_time = time.localtime(time.time())
             timestamp = "%d-%02d-%02d_%02d-%02d-%02d" % (
                 current_time.tm_year,
@@ -167,15 +168,25 @@
         type=str,
         default=",".join(map(str, VcdRunConfig.CULL_CLUSTER_IDS)),
         help="Coma separated list of cluster IDs to cull when producing the meshes",
     )
     ap.add_argument(
         "-v", "--verbose", action="count", default=0, help="turn on verbose logging"
     )
-
+    ap.add_argument(
+        "--colormap",
+        type=str,
+        default=VcdRunConfig.COLORMAP,
+        help=(
+            "Colormap to apply to generated output files where supported.  Name has "
+            "to align with a matplotlib named colormap.  See "
+            "https://matplotlib.org/stable/tutorials/colors/colormaps.html#diverging "
+            "for list of options."
+        ),
+    )
     args = ap.parse_args()
     return args
 
 
 def create_config(args: argparse.Namespace) -> Dict[str, Any]:
     config = VcdRunConfig(
         os.fsdecode(os.path.abspath(args.before)),
```

### Comparing `codem-0.25.0/src/vcd/meshing/mesh.py` & `codem-0.25.1/src/vcd/meshing/mesh.py`

 * *Files identical despite different names*

### Comparing `codem-0.25.0/src/vcd/preprocessing/preprocess.py` & `codem-0.25.1/src/vcd/preprocessing/preprocess.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 Date: February 2021
 
 """
 import contextlib
 import os
 import re
 from typing import List
+from typing import NamedTuple
 from typing import Optional
 from typing import Tuple
 
+import matplotlib.colors as colors
+import matplotlib.pyplot as plt
 import numpy as np
 import numpy.lib.recfunctions as rfn
 import pandas as pd
 import pdal
-import rasterio
+from codem import __version__
 from codem.lib.log import Log
 from pyproj import CRS
 from pyproj.aoi import AreaOfInterest
 from pyproj.database import query_utm_crs_info  # type: ignore
 from pyproj.transformer import TransformerGroup
 from scipy.spatial import cKDTree
 from typing_extensions import TypedDict
@@ -30,29 +33,36 @@
     RESOLUTION: np.float64
     OUTPUT_DIR: str
     BEFORE: str
     AFTER: str
     MIN_POINTS: int
     CLUSTER_TOLERANCE: float
     CULL_CLUSTER_IDS: Tuple[int, ...]
+    COLORMAP: str
     log: Log
 
 
+class Product(NamedTuple):
+    df: pd.DataFrame
+    z_name: str
+    description: str = ""
+
+    @property
+    def slug(self) -> str:
+        """Adapted from https://stackoverflow.com/a/8366771/498396"""
+        return re.sub(r"[^0-9A-Za-z.]", "-", self.description.lower())
+
+
 def get_json(filename: str) -> str:
     with contextlib.suppress(IOError):
         with open(filename, "r") as f:
             content = f.read()
     return content
 
 
-def slugify(text: str) -> str:
-    """Adapted from https://stackoverflow.com/a/8366771/498396"""
-    return re.sub(r"[^0-9A-Za-z.]", "-", text.lower())
-
-
 class PointCloud:
     """
     A class for storing and preparing geospatial data
 
     Parameters
     ----------
     config: VCDParameters
@@ -74,17 +84,19 @@
         self.utm = ""
         self.pipeline = self.open()
 
         if len(self.pipeline.arrays) > 1:
             raise NotImplementedError("VCD between multiple views is not supported")
         self.df = pd.DataFrame(self.pipeline.arrays[0])
 
+        # drop the color information if it is present
+        self.df = self.df.drop(columns=["Red", "Green", "Blue"], errors="ignore")
+
     def open(self) -> pdal.Pipeline:
         def _get_utm(pipeline: pdal.Pipeline) -> pdal.Pipeline:
-
             data = pipeline.quickinfo
             is_reader = [[k.split(".")[0] == "readers", k] for k in data.keys()]
             for k in is_reader:
                 if k[0]:  # we are a reader
                     reader_info = data[k[1]]
                     bounds = reader_info["bounds"]
                     srs = CRS.from_user_input(reader_info["srs"]["compoundwkt"])
@@ -146,49 +158,41 @@
         filters |= pdal.Filter.range(limits="Classification![9:9]")
         filters |= pdal.Filter.returns(groups="only")
         filters |= pdal.Filter.elm(cell=20.0)
         filters |= pdal.Filter.outlier(where="Classification!=7")
         filters |= pdal.Filter.range(limits="Classification![7:7]")
         filters |= pdal.Filter.assign(assignment="Classification[:]=1")
         filters |= pdal.Filter.smrf()
-        self.pipeline = filters
         filters.execute()
+        self.pipeline = filters
         return filters
 
 
 class VCD:
     def __init__(self, before: PointCloud, after: PointCloud) -> None:
         self.before = before
         self.after = after
-        self.products: List[pd.DataFrame] = []
+        self.products: List[Product] = []
         self.gh = before.config["GROUNDHEIGHT"]
         self.resolution = before.config["RESOLUTION"]
 
     def compute_indexes(self) -> None:
-
         after = self.after.df
         before = self.before.df
 
-        tree2d = cKDTree(before[["X", "Y"]])
-        d2d, i2d = tree2d.query(after[["X", "Y"]], k=1)
         tree3d = cKDTree(before[["X", "Y", "Z"]])
         d3d, i3d = tree3d.query(after[["X", "Y", "Z"]], k=1)
 
-        after["dX2d"] = after.X - before.iloc[i2d].X.values
-        after["dY2d"] = after.Y - before.iloc[i2d].Y.values
-        after["dZ2d"] = after.Z - before.iloc[i2d].Z.values
         after["dX3d"] = after.X - before.iloc[i3d].X.values
         after["dY3d"] = after.Y - before.iloc[i3d].Y.values
         after["dZ3d"] = after.Z - before.iloc[i3d].Z.values
 
-        after["d2"] = d2d
         after["d3"] = d3d
 
     def cluster(self) -> None:
-
         after = self.after.df
         gh = self.gh
 
         array = after[(after.Classification != 2) & (after.d3 > gh)].to_records()
         self.ng_clusters = pdal.Filter.cluster(
             min_points=self.after.config["MIN_POINTS"],
             tolerance=self.after.config["CLUSTER_TOLERANCE"],
@@ -196,17 +200,15 @@
         self.ng_clusters.execute()
         ng_cluster_df = pd.DataFrame(self.ng_clusters.arrays[0])
 
         p = self.make_product(
             ng_cluster_df.X,
             ng_cluster_df.Y,
             ng_cluster_df.ClusterID,
-            after["d2"],
             description=f"Non-ground clusters greater than {gh:.2f} height",
-            colorscale="IceFire",
         )
         self.products.append(p)
 
         array = after[(after.Classification == 2) & (after.d3 > gh)].to_records()
         self.ground_clusters = pdal.Filter.cluster(
             min_points=self.after.config["MIN_POINTS"],
             tolerance=self.after.config["CLUSTER_TOLERANCE"],
@@ -214,82 +216,34 @@
         self.ground_clusters.execute()
         ground_cluster_df = pd.DataFrame(self.ground_clusters.arrays[0])
 
         p = self.make_product(
             ground_cluster_df.X,
             ground_cluster_df.Y,
             ground_cluster_df.ClusterID,
-            after["d2"],
             description=f"Ground clusters greater than {gh:.2f} height",
-            colorscale="IceFire",
         )
         self.products.append(p)
 
     def make_products(self) -> None:
         after = self.after.df
-        gh = self.gh
-        resolution = self.resolution
-
         p = self.make_product(
-            after.X, after.Y, after.dZ3d, after["d3"], description="Before minus after"
-        )
-        self.products.append(p)
-
-        p = self.make_product(
-            after[after.d3 < gh].X,
-            after[after.d3 < gh].Y,
-            after[after.d3 < gh].dZ3d,
-            after["d3"],
-            f"Points within {resolution:.2f}m difference",
-        )
-        self.products.append(p)
-
-        p = self.make_product(
-            after[after.d3 > gh].X,
-            after[after.d3 > gh].Y,
-            after[after.d3 > gh].dZ3d,
-            after["d3"],
-            f"Points more than {resolution:.2f}m difference",
-        )
-        self.products.append(p)
-
-        p = self.make_product(
-            after[(after.Classification == 2) & (after.d3 > gh)].X,
-            after[(after.Classification == 2) & (after.d3 > gh)].Y,
-            after[(after.Classification == 2) & (after.d3 > gh)].dZ3d,
-            after["d3"],
-            f"Ground points more than {resolution:.2f}m difference",
-        )
-        self.products.append(p)
-
-        p = self.make_product(
-            after[(after.Classification != 2) & (after.d3 > gh)].X,
-            after[(after.Classification != 2) & (after.d3 > gh)].Y,
-            after[(after.Classification != 2) & (after.d3 > gh)].dZ3d,
-            after["d3"],
-            f"Non-ground points more than {resolution:.2f}m difference",
+            after.X, after.Y, after.dZ3d, description="Before minus after"
         )
         self.products.append(p)
 
     def make_product(
         self,
         x: pd.Series,
         y: pd.Series,
         z: pd.Series,
-        status: pd.Series,
         description: str = "",
-        colorscale: str = "RdBu",
     ) -> pd.DataFrame:
-        product = x.to_frame().join(y.to_frame()).join(z.to_frame())
-        product.z = z.name
-        product.slug = slugify(description)
-        product.description = description
-        product.colorscale = colorscale
-        product.status = status
-        return product
+        df = x.to_frame().join(y.to_frame()).join(z.to_frame())
+        return Product(df=df, z_name=z.name, description=description)
 
     def rasterize(self) -> None:
         resolution = self.before.config["RESOLUTION"]
         rasters_dir = os.path.join(self.before.config["OUTPUT_DIR"], "rasters")
         summary_dir = os.path.join(
             self.before.config["OUTPUT_DIR"], "rasters", "summary"
         )
@@ -297,83 +251,91 @@
             self.before.config["OUTPUT_DIR"], "rasters", "products"
         )
 
         os.makedirs(rasters_dir, exist_ok=True)
         os.makedirs(summary_dir, exist_ok=True)
         os.makedirs(products_dir, exist_ok=True)
 
-        def _rasterize(product: pd.DataFrame, utm: str) -> str:
-
-            array = product.to_records()
-            array = rfn.rename_fields(array, {product.z: "Z"})
+        def _rasterize(product: Product, utm: str) -> str:
+            array = product.df.to_records()
+            array = rfn.rename_fields(array, {product.z_name: "Z"})
 
             outfile = os.path.join(products_dir, product.slug) + ".tif"
 
-            metadata = f"TIFFTAG_XRESOLUTION={resolution},TIFFTAG_YRESOLUTION={resolution},TIFFTAG_IMAGEDESCRIPTION={product.description}"
-            gdalopts = "MAX_Z_ERROR=0.01,COMPRESS=LERC_ZSTD,OVERVIEW_COMPRESS=LERC_ZSTD,BIGTIFF=YES"
+            metadata = (
+                f"TIFFTAG_XRESOLUTION={resolution},"
+                f"TIFFTAG_YRESOLUTION={resolution},"
+                f"TIFFTAG_IMAGEDESCRIPTION={product.description},"
+                f"CODEM_VERSION={__version__}"
+            )
+            gdalopts = (
+                "COMPRESS=LZW," "PREDICTOR=2," "OVERVIEW_COMPRESS=LZW," "BIGTIFF=YES"
+            )
 
             pipeline = pdal.Writer.gdal(
                 filename=outfile,
                 metadata=metadata,
                 gdalopts=gdalopts,
                 override_srs=utm,
                 resolution=resolution,
+                output_type="idw",
             ).pipeline(array)
             pipeline.execute()
             return outfile
 
-        def _merge(rasters: List[str], output_type: str) -> None:
-
-            with rasterio.open(rasters[0]) as src0:
-                meta = src0.meta
-                descriptions = src0.descriptions
-
-            meta.update(count=len(rasters))
-            meta.update(
-                compress="LERC_ZSTD",
-                max_z_error=0.01,
-                bigtiff="YES",
-                overview_compress="LERC_ZSTD",
-            )
-
-            band_id = descriptions.index(output_type) + 1  # bands count from 1
-            outfile = os.path.join(summary_dir, output_type) + ".tif"
+        _ = [_rasterize(p, self.before.utm) for p in self.products]
+        return None
 
-            with rasterio.open(outfile, "w", **meta) as dst:
+    def save(self, format: str = ".las") -> None:
+        with contextlib.suppress(FileExistsError):
+            os.mkdir(os.path.join(self.before.config["OUTPUT_DIR"], "points"))
 
-                for index, layer in enumerate(rasters, start=1):
-                    with rasterio.open(layer) as src:
+        # Determine Colormap
+        flex_max = min(
+            clusters.arrays[0]["dZ3d"].min()
+            for clusters in (self.ng_clusters, self.ground_clusters)
+        )
+
+        new_max = max(
+            clusters.arrays[0]["dZ3d"].max()
+            for clusters in (self.ng_clusters, self.ground_clusters)
+        )
+
+        divnorm = colors.TwoSlopeNorm(vmin=flex_max, vcenter=0, vmax=new_max)
+        # we are only writing the first point-clouds
+        colormap = plt.colormaps[self.before.config["COLORMAP"]]
+
+        # write point cloud output
+        for output in ("ground", "new_ground"):
+            if output == "ground":
+                path = "gnd-clusters"
+                array = self.ground_clusters.arrays[0]
+            elif output == "new_ground":
+                path = "ng-clusters"
+                array = self.ng_clusters.arrays[0]
+            else:
+                raise RuntimeError("How did you even get here?")
 
-                        band_description = src.tags()["TIFFTAG_IMAGEDESCRIPTION"]
-                        band = src.read(band_id)
+            filename = os.path.join(
+                self.before.config["OUTPUT_DIR"], "points", f"{path}{format}"
+            )
 
-                        dst.write_band(index, band)
-                        dst.update_tags(band_id)
-                        dst.set_band_description(index, band_description)
+            # convert colors from [0. 1] floats to [0, 65535] per LAS spec
+            rgb = np.array(
+                [
+                    colors.to_rgba_array(colormap(divnorm(array["dZ3d"])))
+                    * np.iinfo(np.uint16).max
+                ],
+                dtype=np.uint16,
+            )[0, :, :-1]
 
-        rasters = [_rasterize(p, self.before.utm) for p in self.products]
-        for feature in ("idw", "min", "max", "mean", "count"):
-            _merge(rasters, feature)
-        return None
+            array = rfn.append_fields(
+                array, ["Red", "Green", "Blue"], [rgb[:, 0], rgb[:, 1], rgb[:, 2]]
+            )
 
-    def save(self, format: str = ".las") -> None:
-        with contextlib.suppress(FileExistsError):
-            os.mkdir(os.path.join(self.before.config["OUTPUT_DIR"], "points"))
-        new_ground = (
-            os.path.join(self.before.config["OUTPUT_DIR"], "points", "ng-clusters")
-            + format
-        )
-        ground = (
-            os.path.join(self.before.config["OUTPUT_DIR"], "points", "gnd-clusters")
-            + format
-        )
-        pipeline = pdal.Writer.las(
-            minor_version=4, filename=new_ground, extra_dims="all"
-        ).pipeline(self.ng_clusters.arrays[0])
-        pipeline.execute()
-
-        pipeline = pdal.Writer.las(
-            minor_version=4,
-            filename=ground,
-            extra_dims="all",
-        ).pipeline(self.ground_clusters.arrays[0])
-        pipeline.execute()
+            crs = self.after.crs
+            pipeline = pdal.Writer.las(
+                filename=filename,
+                extra_dims="all",
+                a_srs=crs.to_string() if crs is not None else crs,
+            ).pipeline(array)
+            pipeline.execute()
```

