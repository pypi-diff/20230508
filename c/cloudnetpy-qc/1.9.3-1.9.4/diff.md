# Comparing `tmp/cloudnetpy_qc-1.9.3.tar.gz` & `tmp/cloudnetpy_qc-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudnetpy_qc-1.9.3.tar", last modified: Fri May  5 09:51:39 2023, max compression
+gzip compressed data, was "cloudnetpy_qc-1.9.4.tar", last modified: Mon May  8 12:52:23 2023, max compression
```

## Comparing `cloudnetpy_qc-1.9.3.tar` & `cloudnetpy_qc-1.9.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:51:39.739992 cloudnetpy_qc-1.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-05 09:51:39.739992 cloudnetpy_qc-1.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:51:39.731991 cloudnetpy_qc-1.9.3/cloudnetpy_qc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:51:39.739992 cloudnetpy_qc-1.9.3/cloudnetpy_qc/data/
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/data/area-type-table.xml
--rw-r--r--   0 runner    (1001) docker     (123)  4094783 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/data/cf-standard-name-table.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/data/data_quality_config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/data/metadata_config.ini
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/data/standardized-region-list.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    30120 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:51:39.731991 cloudnetpy_qc-1.9.3/cloudnetpy_qc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-05 09:51:39.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 09:51:39.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:51:39.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-05 09:51:39.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 09:51:39.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 09:51:39.739992 cloudnetpy_qc-1.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:52:23.068998 cloudnetpy_qc-1.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-08 12:52:23.064998 cloudnetpy_qc-1.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:52:23.060998 cloudnetpy_qc-1.9.4/cloudnetpy_qc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:52:23.064998 cloudnetpy_qc-1.9.4/cloudnetpy_qc/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/data/area-type-table.xml
+-rw-r--r--   0 runner    (1001) docker     (123)  4094783 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/data/cf-standard-name-table.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/data/data_quality_config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/data/metadata_config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/data/standardized-region-list.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20904 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30120 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:52:23.060998 cloudnetpy_qc-1.9.4/cloudnetpy_qc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-08 12:52:23.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-08 12:52:23.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:52:23.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-08 12:52:23.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 12:52:23.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 12:52:23.068998 cloudnetpy_qc-1.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/setup.py
```

### Comparing `cloudnetpy_qc-1.9.3/LICENSE` & `cloudnetpy_qc-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.3/PKG-INFO` & `cloudnetpy_qc-1.9.4/cloudnetpy_qc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cloudnetpy_qc
-Version: 1.9.3
+Name: cloudnetpy-qc
+Version: 1.9.4
 Summary: Quality control routines for CloudnetPy products
 Home-page: https://github.com/actris-cloudnet/cloudnetpy-qc
 Author: Finnish Meteorological Institute
 Author-email: actris-cloudnet@fmi.fi
 License: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cloudnetpy_qc-1.9.3/README.md` & `cloudnetpy_qc-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.3/cloudnetpy_qc/data/area-type-table.xml` & `cloudnetpy_qc-1.9.4/cloudnetpy_qc/data/area-type-table.xml`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.3/cloudnetpy_qc/data/cf-standard-name-table.xml` & `cloudnetpy_qc-1.9.4/cloudnetpy_qc/data/cf-standard-name-table.xml`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.3/cloudnetpy_qc/data/data_quality_config.ini` & `cloudnetpy_qc-1.9.4/cloudnetpy_qc/data/data_quality_config.ini`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.3/cloudnetpy_qc/data/standardized-region-list.xml` & `cloudnetpy_qc-1.9.4/cloudnetpy_qc/data/standardized-region-list.xml`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.3/cloudnetpy_qc/quality.py` & `cloudnetpy_qc-1.9.4/cloudnetpy_qc/quality.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Cloudnet product quality checks."""
 import dataclasses
 import datetime
+import json
 import logging
 import os
+import re
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
 
 import netCDF4
 import numpy as np
 import scipy.stats
@@ -164,15 +166,15 @@
         for key in self.nc.variables.keys():
             if key not in VARIABLES:
                 continue
             expected = getattr(VARIABLES[key], attribute)
             if expected is not None:
                 value = getattr(self.nc.variables[key], attribute, "")
                 if value != expected:
-                    msg = utils.create_expected_received_msg(key, expected, value)
+                    msg = utils.create_expected_received_msg(expected, value, variable=key)
                     self._add_message(msg)
 
     def _get_date(self):
         date_in_file = [int(getattr(self.nc, x)) for x in ("year", "month", "day")]
         return datetime.date(*date_in_file)
 
 
@@ -301,15 +303,15 @@
             if key not in VARIABLES:
                 continue
             expected = VARIABLES[key].dtype.value
             received = self.nc.variables[key].dtype.name
             if received != expected:
                 if key == "time" and received in ("float32", "float64"):
                     continue
-                msg = utils.create_expected_received_msg(key, expected, received)
+                msg = utils.create_expected_received_msg(expected, received, variable=key)
                 self._add_message(msg)
 
 
 @test("Global attributes", "Check that file contains required global attributes.")
 class TestGlobalAttributes(Test):
     def run(self):
         nc_keys = self.nc.ncattrs()
@@ -374,31 +376,14 @@
         x = range_var[-n_top_ranges:] ** 2
         y = np.std(beta_raw[:, -n_top_ranges:], axis=0)
         res = scipy.stats.pearsonr(x, y)
         if res.statistic < 0.75:
             self._add_message("Data might not be range corrected.")
 
 
-@test(
-    "Instrument PID",
-    "Test that valid instrument PID exists.",
-    ErrorLevel.WARNING,
-    [Product.MWR, Product.LIDAR, Product.RADAR, Product.DISDROMETER],
-)
-class TestInstrumentPid(Test):
-    def run(self):
-        key = "instrument_pid"
-        try:
-            pid = getattr(self.nc, key)
-            if pid == "":
-                self._add_message("Instrument PID is empty.")
-        except AttributeError:
-            self._add_message("Instrument PID is missing.")
-
-
 # ---------------------#
 # ------ Errors ------ #
 # -------------------- #
 
 
 @test(
     "Beta presence",
@@ -479,7 +464,150 @@
                 elif level == "WARN":
                     self.severity = ErrorLevel.WARNING
                 else:
                     continue
                 msg = utils.format_msg(error_msg)
                 msg = f"Variable '{key}': {msg}"
                 self._add_message(msg)
+
+
+@test(
+    "Instrument PID",
+    "Test that valid instrument PID exists.",
+    ErrorLevel.ERROR,
+    [
+        Product.MWR,
+        Product.LIDAR,
+        Product.RADAR,
+        Product.DISDROMETER,
+        Product.DOPPLER_LIDAR,
+        Product.WEATHER_STATION,
+    ],
+)
+class TestInstrumentPid(Test):
+    data: dict = {}
+
+    def run(self):
+        if self._check_exists():
+            self.data = utils.fetch_pid(self.nc.instrument_pid)
+            self._check_serial()
+            self._check_model_name()
+            self._check_model_identifier()
+
+    def _check_exists(self) -> bool:
+        key = "instrument_pid"
+        try:
+            pid = getattr(self.nc, key)
+            if pid == "":
+                self.severity = ErrorLevel.ERROR
+                self._add_message("Instrument PID is empty.")
+                return False
+            if re.fullmatch(utils.PID_FORMAT, pid) is None:
+                self.severity = ErrorLevel.ERROR
+                self._add_message("Instrument PID has invalid format.")
+                return False
+        except AttributeError:
+            self.severity = ErrorLevel.WARNING
+            self._add_message("Instrument PID is missing.")
+            return False
+        return True
+
+    def _get_value(self, kind: str) -> dict | list | None:
+        try:
+            item = next(item for item in self.data["values"] if item["type"] == kind)
+            return json.loads(item["data"]["value"])
+        except StopIteration:
+            return None
+
+    def _check_serial(self):
+        key = "serial_number"
+        try:
+            received = str(getattr(self.nc, key))
+        except AttributeError:
+            return
+        for alt in self._get_value("21.T11148/eb3c713572f681e6c4c3"):
+            if alt["alternateIdentifier"]["alternateIdentifierType"] == "SerialNumber":
+                expected = alt["alternateIdentifier"]["alternateIdentifierValue"]
+                if received != expected:
+                    msg = utils.create_expected_received_msg(expected, received)
+                    self.severity = ErrorLevel.ERROR
+                    self._add_message(msg)
+                return
+        self.severity = ErrorLevel.WARNING
+        self._add_message(
+            f"No serial number was defined in instrument PID but found '{received}' in the file."
+        )
+
+    def _check_model_name(self):
+        key = "source"
+        try:
+            source = getattr(self.nc, key)
+            allowed_values = self.SOURCE_TO_NAME[source]
+        except (AttributeError, KeyError):
+            return
+        model = self._get_value("21.T11148/c1a0ec5ad347427f25d6")
+        if model is None:
+            return
+        received = model["modelName"]
+        if received not in allowed_values:
+            msg = utils.create_expected_received_msg(allowed_values, received)
+            self.severity = ErrorLevel.ERROR
+            self._add_message(msg)
+
+    def _check_model_identifier(self):
+        key = "source"
+        try:
+            source = getattr(self.nc, key)
+            allowed_values = self.SOURCE_TO_IDENTIFIER[source]
+        except (AttributeError, KeyError):
+            return
+        model = self._get_value("21.T11148/c1a0ec5ad347427f25d6")
+        if model is None:
+            return
+        if "modelIdentifier" not in model:
+            return
+        received = model["modelIdentifier"]["modelIdentifierValue"]
+        if received not in allowed_values:
+            msg = utils.create_expected_received_msg(allowed_values, received)
+            self.severity = ErrorLevel.ERROR
+            self._add_message(msg)
+
+    SOURCE_TO_NAME = {
+        "Lufft CHM15k": ["Lufft CHM 15k"],
+        "Lufft CHM15kx": ["Lufft CHM 15k-x"],
+        "TROPOS PollyXT": ["PollyXT"],
+        "Vaisala CL31": ["Vaisala CL31"],
+        "Vaisala CL51": ["Vaisala CL51"],
+        "Vaisala CL61d": ["Vaisala CL61"],
+        "Vaisala CT25k": ["Vaisala CT25K"],
+        "HALO Photonics StreamLine": [
+            "StreamLine",
+            "StreamLine Pro",
+            "StreamLine XR",
+            "StreamLine XR+",
+        ],
+    }
+
+    SOURCE_TO_IDENTIFIER = {
+        "BASTA": ["https://vocabulary.actris.nilu.no/actris_vocab/BASTA"],
+        "METEK MIRA-35": [
+            "https://vocabulary.actris.nilu.no/actris_vocab/METEKMIRA35",
+            "https://vocabulary.actris.nilu.no/actris_vocab/METEKMIRA35S",
+        ],
+        "OTT HydroMet Parsivel2": ["https://vocabulary.actris.nilu.no/actris_vocab/OTTParsivel2"],
+        "RAL Space Copernicus": ["https://vocabulary.actris.nilu.no/actris_vocab/UFAMCopernicus"],
+        "RAL Space Galileo": ["https://vocabulary.actris.nilu.no/actris_vocab/UFAMGalileo"],
+        "RPG-Radiometer Physics HATPRO": [
+            "https://vocabulary.actris.nilu.no/actris_vocab/RPGHATPRO"
+        ],
+        "RPG-Radiometer Physics RPG-FMCW-35": [
+            "https://vocabulary.actris.nilu.no/skosmos/actris_vocab/en/page/RPG-FMCW-35-DP"
+            "https://vocabulary.actris.nilu.no/skosmos/actris_vocab/en/page/RPG-FMCW-35-SP"
+            "https://vocabulary.actris.nilu.no/skosmos/actris_vocab/en/page/RPG-FMCW-35S"
+        ],
+        "RPG-Radiometer Physics RPG-FMCW-94": [
+            "https://vocabulary.actris.nilu.no/actris_vocab/RPG-FMCW-94-DP",
+            "https://vocabulary.actris.nilu.no/actris_vocab/RPG-FMCW-94-SP",
+            "https://vocabulary.actris.nilu.no/actris_vocab/RPG-FMCW-94S",
+        ],
+        "Thies Clima LNM": ["https://vocabulary.actris.nilu.no/actris_vocab/ThiesLNM"],
+    }
```

### Comparing `cloudnetpy_qc-1.9.3/cloudnetpy_qc/variables.py` & `cloudnetpy_qc-1.9.4/cloudnetpy_qc/variables.py`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.3/cloudnetpy_qc.egg-info/PKG-INFO` & `cloudnetpy_qc-1.9.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cloudnetpy-qc
-Version: 1.9.3
+Name: cloudnetpy_qc
+Version: 1.9.4
 Summary: Quality control routines for CloudnetPy products
 Home-page: https://github.com/actris-cloudnet/cloudnetpy-qc
 Author: Finnish Meteorological Institute
 Author-email: actris-cloudnet@fmi.fi
 License: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cloudnetpy_qc-1.9.3/cloudnetpy_qc.egg-info/SOURCES.txt` & `cloudnetpy_qc-1.9.4/cloudnetpy_qc.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 cloudnetpy_qc/__init__.py
 cloudnetpy_qc/py.typed
 cloudnetpy_qc/quality.py
 cloudnetpy_qc/utils.py
 cloudnetpy_qc/variables.py
 cloudnetpy_qc/version.py
```

### Comparing `cloudnetpy_qc-1.9.3/setup.py` & `cloudnetpy_qc-1.9.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,20 +20,22 @@
     author_email="actris-cloudnet@fmi.fi",
     url="https://github.com/actris-cloudnet/cloudnetpy-qc",
     license="MIT License",
     packages=find_packages(),
     include_package_data=True,
     setup_requires=["wheel"],
     python_requires=">=3.10",
-    install_requires=["numpy", "scipy", "netCDF4", "cfchecker"],
+    install_requires=["numpy", "scipy", "netCDF4", "cfchecker", "requests"],
     extras_require={
         "test": [
             "pytest-flakefinder",
             "pylint",
             "mypy",
+            "types-requests",
+            "mypy",
         ],
     },
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

