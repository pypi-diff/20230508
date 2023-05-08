# Comparing `tmp/ome-zarr-0.7.0.tar.gz` & `tmp/ome-zarr-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ome-zarr-0.7.0.tar", last modified: Thu May  4 09:13:49 2023, max compression
+gzip compressed data, was "ome-zarr-0.7.1.tar", last modified: Mon May  8 08:49:11 2023, max compression
```

## Comparing `ome-zarr-0.7.0.tar` & `ome-zarr-0.7.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:13:49.217231 ome-zarr-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-04 09:13:49.217231 ome-zarr-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:13:49.217231 ome-zarr-0.7.0/ome_zarr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/axes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5601 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/dask_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    24047 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    33247 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:13:49.217231 ome-zarr-0.7.0/ome_zarr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-04 09:13:49.000000 ome-zarr-0.7.0/ome_zarr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-04 09:13:49.000000 ome-zarr-0.7.0/ome_zarr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:13:49.000000 ome-zarr-0.7.0/ome_zarr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 09:13:49.000000 ome-zarr-0.7.0/ome_zarr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-04 09:13:49.000000 ome-zarr-0.7.0/ome_zarr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 09:13:49.000000 ome-zarr-0.7.0/ome_zarr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:13:49.217231 ome-zarr-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:49:11.960908 ome-zarr-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-08 08:49:11.960908 ome-zarr-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:49:11.956908 ome-zarr-0.7.1/ome_zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/axes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5628 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/dask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24047 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33247 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/ome_zarr/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:49:11.960908 ome-zarr-0.7.1/ome_zarr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-08 08:49:11.000000 ome-zarr-0.7.1/ome_zarr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-08 08:49:11.000000 ome-zarr-0.7.1/ome_zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:49:11.000000 ome-zarr-0.7.1/ome_zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-08 08:49:11.000000 ome-zarr-0.7.1/ome_zarr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-08 08:49:11.000000 ome-zarr-0.7.1/ome_zarr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 08:49:11.000000 ome-zarr-0.7.1/ome_zarr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:49:11.960908 ome-zarr-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-08 08:49:10.000000 ome-zarr-0.7.1/setup.py
```

### Comparing `ome-zarr-0.7.0/LICENSE` & `ome-zarr-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.0/PKG-INFO` & `ome-zarr-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ome-zarr
-Version: 0.7.0
+Version: 0.7.1
 Summary: Implementation of images in Zarr files.
 Home-page: https://github.com/ome/ome-zarr-py
 Author: The Open Microscopy Team
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `ome-zarr-0.7.0/README.rst` & `ome-zarr-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.0/ome_zarr/axes.py` & `ome-zarr-0.7.1/ome_zarr/axes.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.0/ome_zarr/cli.py` & `ome-zarr-0.7.1/ome_zarr/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Entrypoint for the `ome_zarr` command-line tool."""
 import argparse
 import logging
 import sys
-from typing import List
+from typing import List, Union
 
 from .csv import csv_to_zarr
 from .data import astronaut, coins, create_zarr
 from .scale import Scaler
 from .utils import download as zarr_download
 from .utils import info as zarr_info
 
@@ -69,15 +69,15 @@
     """Adds csv data to labels properties"""
 
     print("csv_to_labels", args.csv_path, args.zarr_path)
 
     csv_to_zarr(args.csv_path, args.csv_id, args.csv_keys, args.zarr_path, args.zarr_id)
 
 
-def main(args: List[str]) -> None:
+def main(args: Union[List[str], None] = None) -> None:
     """Run appropriate function with argparse arguments, handling errors."""
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-v",
         "--verbose",
         action="count",
         default=0,
```

### Comparing `ome-zarr-0.7.0/ome_zarr/conversions.py` & `ome-zarr-0.7.1/ome_zarr/conversions.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.0/ome_zarr/csv.py` & `ome-zarr-0.7.1/ome_zarr/csv.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.0/ome_zarr/dask_utils.py` & `ome-zarr-0.7.1/ome_zarr/dask_utils.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.0/ome_zarr/data.py` & `ome-zarr-0.7.1/ome_zarr/data.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.0/ome_zarr/format.py` & `ome-zarr-0.7.1/ome_zarr/format.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.0/ome_zarr/io.py` & `ome-zarr-0.7.1/ome_zarr/io.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.0/ome_zarr/reader.py` & `ome-zarr-0.7.1/ome_zarr/reader.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.0/ome_zarr/scale.py` & `ome-zarr-0.7.1/ome_zarr/scale.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.0/ome_zarr/utils.py` & `ome-zarr-0.7.1/ome_zarr/utils.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.0/ome_zarr/writer.py` & `ome-zarr-0.7.1/ome_zarr/writer.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.7.0/ome_zarr.egg-info/PKG-INFO` & `ome-zarr-0.7.1/ome_zarr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ome-zarr
-Version: 0.7.0
+Version: 0.7.1
 Summary: Implementation of images in Zarr files.
 Home-page: https://github.com/ome/ome-zarr-py
 Author: The Open Microscopy Team
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `ome-zarr-0.7.0/setup.py` & `ome-zarr-0.7.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 install_requires += (["requests"],)
 install_requires += (["scikit-image"],)
 install_requires += (["toolz"],)
 
 
 setup(
     name="ome-zarr",
-    version="0.7.0",
+    version="0.7.1",
     author="The Open Microscopy Team",
     url="https://github.com/ome/ome-zarr-py",
     description="Implementation of images in Zarr files.",
     long_description=read("README.rst"),
     packages=["ome_zarr"],
     py_modules=["ome_zarr"],
     python_requires=">=3.6",
```

