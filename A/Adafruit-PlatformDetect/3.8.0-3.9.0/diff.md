# Comparing `tmp/Adafruit-PlatformDetect-3.8.0.tar.gz` & `tmp/Adafruit-PlatformDetect-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Adafruit-PlatformDetect-3.8.0.tar", last modified: Mon Apr 26 20:08:23 2021, max compression
+gzip compressed data, was "Adafruit-PlatformDetect-3.9.0.tar", last modified: Wed May  5 18:31:27 2021, max compression
```

## Comparing `Adafruit-PlatformDetect-3.8.0.tar` & `Adafruit-PlatformDetect-3.9.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-26 20:08:23.002776 Adafruit-PlatformDetect-3.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-26 20:08:22.998776 Adafruit-PlatformDetect-3.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-26 20:08:22.998776 Adafruit-PlatformDetect-3.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1464 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      944 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)       86 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    16268 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-26 20:08:22.998776 Adafruit-PlatformDetect-3.8.0/Adafruit_PlatformDetect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4559 2021-04-26 20:08:22.000000 Adafruit-PlatformDetect-3.8.0/Adafruit_PlatformDetect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      671 2021-04-26 20:08:22.000000 Adafruit-PlatformDetect-3.8.0/Adafruit_PlatformDetect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-26 20:08:22.000000 Adafruit-PlatformDetect-3.8.0/Adafruit_PlatformDetect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-04-26 20:08:22.000000 Adafruit-PlatformDetect-3.8.0/Adafruit_PlatformDetect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5987 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4559 2021-04-26 20:08:23.002776 Adafruit-PlatformDetect-3.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3067 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-26 20:08:23.002776 Adafruit-PlatformDetect-3.8.0/adafruit_platformdetect/
--rw-r--r--   0 runner    (1001) docker     (121)     5049 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/adafruit_platformdetect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21336 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/adafruit_platformdetect/board.py
--rw-r--r--   0 runner    (1001) docker     (121)    12121 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/adafruit_platformdetect/chip.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-26 20:08:23.002776 Adafruit-PlatformDetect-3.8.0/adafruit_platformdetect/constants/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/adafruit_platformdetect/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11888 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/adafruit_platformdetect/constants/boards.py
--rw-r--r--   0 runner    (1001) docker     (121)      992 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/adafruit_platformdetect/constants/chips.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-26 20:08:23.002776 Adafruit-PlatformDetect-3.8.0/bin/
--rw-r--r--   0 runner    (1001) docker     (121)     2680 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/bin/detect.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-26 20:08:23.002776 Adafruit-PlatformDetect-3.8.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-26 20:08:23.002776 Adafruit-PlatformDetect-3.8.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      337 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4117 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/docs/beaglebone_eeprom.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5382 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-26 20:08:23.002776 Adafruit-PlatformDetect-3.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2021-04-26 20:08:08.000000 Adafruit-PlatformDetect-3.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 18:31:27.383141 Adafruit-PlatformDetect-3.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 18:31:27.379141 Adafruit-PlatformDetect-3.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 18:31:27.383141 Adafruit-PlatformDetect-3.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1464 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      944 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)    16268 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 18:31:27.383141 Adafruit-PlatformDetect-3.9.0/Adafruit_PlatformDetect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4559 2021-05-05 18:31:27.000000 Adafruit-PlatformDetect-3.9.0/Adafruit_PlatformDetect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      671 2021-05-05 18:31:27.000000 Adafruit-PlatformDetect-3.9.0/Adafruit_PlatformDetect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-05 18:31:27.000000 Adafruit-PlatformDetect-3.9.0/Adafruit_PlatformDetect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-05-05 18:31:27.000000 Adafruit-PlatformDetect-3.9.0/Adafruit_PlatformDetect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5987 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1086 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     4559 2021-05-05 18:31:27.383141 Adafruit-PlatformDetect-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3067 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 18:31:27.383141 Adafruit-PlatformDetect-3.9.0/adafruit_platformdetect/
+-rw-r--r--   0 runner    (1001) docker     (121)     4722 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/adafruit_platformdetect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21336 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/adafruit_platformdetect/board.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12215 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/adafruit_platformdetect/chip.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 18:31:27.383141 Adafruit-PlatformDetect-3.9.0/adafruit_platformdetect/constants/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/adafruit_platformdetect/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11888 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/adafruit_platformdetect/constants/boards.py
+-rw-r--r--   0 runner    (1001) docker     (121)      992 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/adafruit_platformdetect/constants/chips.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 18:31:27.383141 Adafruit-PlatformDetect-3.9.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (121)     2680 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/bin/detect.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 18:31:27.383141 Adafruit-PlatformDetect-3.9.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 18:31:27.383141 Adafruit-PlatformDetect-3.9.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4117 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/docs/beaglebone_eeprom.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5382 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1003 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-05 18:31:27.383141 Adafruit-PlatformDetect-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1553 2021-05-05 18:31:12.000000 Adafruit-PlatformDetect-3.9.0/setup.py
```

### Comparing `Adafruit-PlatformDetect-3.8.0/.github/workflows/build.yml` & `Adafruit-PlatformDetect-3.9.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `Adafruit-PlatformDetect-3.8.0/.github/workflows/release.yml` & `Adafruit-PlatformDetect-3.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `Adafruit-PlatformDetect-3.8.0/.pylintrc` & `Adafruit-PlatformDetect-3.9.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `Adafruit-PlatformDetect-3.8.0/Adafruit_PlatformDetect.egg-info/PKG-INFO` & `Adafruit-PlatformDetect-3.9.0/Adafruit_PlatformDetect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Adafruit-PlatformDetect
-Version: 3.8.0
+Version: 3.9.0
 Summary: Platform detection for use by libraries like Adafruit-Blinka.
 Home-page: https://github.com/adafruit/Adafruit_Python_PlatformDetect
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `Adafruit-PlatformDetect-3.8.0/Adafruit_PlatformDetect.egg-info/SOURCES.txt` & `Adafruit-PlatformDetect-3.9.0/Adafruit_PlatformDetect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Adafruit-PlatformDetect-3.8.0/CODE_OF_CONDUCT.md` & `Adafruit-PlatformDetect-3.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Adafruit-PlatformDetect-3.8.0/LICENSE` & `Adafruit-PlatformDetect-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Adafruit-PlatformDetect-3.8.0/PKG-INFO` & `Adafruit-PlatformDetect-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Adafruit-PlatformDetect
-Version: 3.8.0
+Version: 3.9.0
 Summary: Platform detection for use by libraries like Adafruit-Blinka.
 Home-page: https://github.com/adafruit/Adafruit_Python_PlatformDetect
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `Adafruit-PlatformDetect-3.8.0/README.rst` & `Adafruit-PlatformDetect-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `Adafruit-PlatformDetect-3.8.0/adafruit_platformdetect/__init__.py` & `Adafruit-PlatformDetect-3.9.0/adafruit_platformdetect/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,19 +44,18 @@
         otherwise None.
         """
         # Match a line like 'Hardware   : BCM2709':
         pattern = r"^" + field + r"\s+:\s+(.*)$"
 
         with open("/proc/cpuinfo", "r") as infile:
             cpuinfo = infile.read().split("\n")
-            infile.close()
-            for line in cpuinfo:
-                match = re.search(pattern, line, flags=re.IGNORECASE)
-                if match:
-                    return match.group(1)
+        for line in cpuinfo:
+            match = re.search(pattern, line, flags=re.IGNORECASE)
+            if match:
+                return match.group(1)
         return None
 
     def check_dt_compatible_value(self, value):
         """
         Search /proc/device-tree/compatible for a value and return True, if found,
         otherwise False.
         """
@@ -78,75 +77,58 @@
         try:
             with open("/etc/armbian-release", "r") as release_file:
                 armbian = release_file.read().split("\n")
                 for line in armbian:
                     match = re.search(pattern, line)
                     if match:
                         field_value = match.group(1)
-                release_file.close()
         except FileNotFoundError:
             pass
 
         return field_value
 
     def get_device_model(self):
         """
         Search /proc/device-tree/model for the device model and return its value, if found,
         otherwise None.
         """
-        model = None
-
         try:
             with open("/proc/device-tree/model", "r") as model_file:
-                model = model_file.read()
-                model_file.close()
+                return model_file.read()
         except FileNotFoundError:
             pass
-
-        return model
+        return None
 
     def get_device_compatible(self):
         """
         Search /proc/device-tree/compatible for the compatible chip name.
         """
-        model = None
-
         try:
             with open("/proc/device-tree/compatible", "r") as model_file:
-                model = model_file.read()
-                model_file.close()
+                return model_file.read()
         except FileNotFoundError:
             pass
-
-        return model
+        return None
 
     def check_board_asset_tag_value(self):
         """
         Search /sys/devices/virtual/dmi/id for the device model and return its value, if found,
         otherwise None.
         """
-        tag = None
-
         try:
             with open("/sys/devices/virtual/dmi/id/board_asset_tag", "r") as tag_file:
-                tag = tag_file.read().strip()
-                tag_file.close()
+                return tag_file.read().strip()
         except FileNotFoundError:
             pass
-
-        return tag
+        return None
 
     def check_board_name_value(self):
         """
         Search /sys/devices/virtual/dmi/id for the board name and return its value, if found,
         otherwise None. Debian/ubuntu based
         """
-        board_name = None
-
         try:
             with open("/sys/devices/virtual/dmi/id/board_name", "r") as board_name_file:
-                board_name = board_name_file.read().strip()
-                board_name.close()
+                return board_name_file.read().strip()
         except FileNotFoundError:
             pass
-
-        return board_name
+        return None
```

### Comparing `Adafruit-PlatformDetect-3.8.0/adafruit_platformdetect/board.py` & `Adafruit-PlatformDetect-3.9.0/adafruit_platformdetect/board.py`

 * *Files identical despite different names*

### Comparing `Adafruit-PlatformDetect-3.8.0/adafruit_platformdetect/chip.py` & `Adafruit-PlatformDetect-3.9.0/adafruit_platformdetect/chip.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,14 +185,17 @@
 
         if self.detector.check_dt_compatible_value("sun50i-a64"):
             return chips.A64
 
         if self.detector.check_dt_compatible_value("sun50i-h5"):
             return chips.H5
 
+        if self.detector.check_dt_compatible_value("sun50i-h6"):
+            return chips.H6
+
         if self.detector.check_dt_compatible_value("sun50iw9"):
             return chips.H616
 
         if self.detector.check_dt_compatible_value("mediatek,mt8167"):
             return chips.MT8167
 
         if self.detector.check_dt_compatible_value("imx6ull"):
```

### Comparing `Adafruit-PlatformDetect-3.8.0/adafruit_platformdetect/constants/boards.py` & `Adafruit-PlatformDetect-3.9.0/adafruit_platformdetect/constants/boards.py`

 * *Files identical despite different names*

### Comparing `Adafruit-PlatformDetect-3.8.0/adafruit_platformdetect/constants/chips.py` & `Adafruit-PlatformDetect-3.9.0/adafruit_platformdetect/constants/chips.py`

 * *Files identical despite different names*

### Comparing `Adafruit-PlatformDetect-3.8.0/bin/detect.py` & `Adafruit-PlatformDetect-3.9.0/bin/detect.py`

 * *Files identical despite different names*

### Comparing `Adafruit-PlatformDetect-3.8.0/docs/_static/favicon.ico` & `Adafruit-PlatformDetect-3.9.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `Adafruit-PlatformDetect-3.8.0/docs/beaglebone_eeprom.txt` & `Adafruit-PlatformDetect-3.9.0/docs/beaglebone_eeprom.txt`

 * *Files identical despite different names*

### Comparing `Adafruit-PlatformDetect-3.8.0/docs/conf.py` & `Adafruit-PlatformDetect-3.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Adafruit-PlatformDetect-3.8.0/docs/index.rst` & `Adafruit-PlatformDetect-3.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Adafruit-PlatformDetect-3.8.0/setup.py` & `Adafruit-PlatformDetect-3.9.0/setup.py`

 * *Files identical despite different names*

