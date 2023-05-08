# Comparing `tmp/spotfire-1.9.0.tar.gz` & `tmp/spotfire-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotfire-1.9.0.tar", last modified: Mon Nov 21 18:46:32 2022, max compression
+gzip compressed data, was "spotfire-2.0.0.tar", last modified: Thu Apr 27 16:19:59 2023, max compression
```

## Comparing `spotfire-1.9.0.tar` & `spotfire-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 18:46:32.293846 spotfire-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-11-21 18:46:01.000000 spotfire-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-21 18:46:01.000000 spotfire-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-11-21 18:46:32.293846 spotfire-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-11-21 18:46:01.000000 spotfire-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-21 18:46:01.000000 spotfire-1.9.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-21 18:46:32.293846 spotfire-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-11-21 18:46:01.000000 spotfire-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 18:46:32.293846 spotfire-1.9.0/spotfire/
--rw-r--r--   0 runner    (1001) docker     (121)     3362 2022-11-21 18:46:01.000000 spotfire-1.9.0/spotfire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-11-21 18:46:01.000000 spotfire-1.9.0/spotfire/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2852 2022-11-21 18:46:01.000000 spotfire-1.9.0/spotfire/cabfile.py
--rw-r--r--   0 runner    (1001) docker     (121)    15968 2022-11-21 18:46:01.000000 spotfire-1.9.0/spotfire/codesign.py
--rw-r--r--   0 runner    (1001) docker     (121)    18842 2022-11-21 18:46:01.000000 spotfire-1.9.0/spotfire/data_function.py
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-11-21 18:46:01.000000 spotfire-1.9.0/spotfire/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)    62899 2022-11-21 18:46:01.000000 spotfire-1.9.0/spotfire/sbdf.py
--rw-r--r--   0 runner    (1001) docker     (121)    40036 2022-11-21 18:46:01.000000 spotfire-1.9.0/spotfire/spk.py
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-11-21 18:46:01.000000 spotfire-1.9.0/spotfire/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 18:46:32.293846 spotfire-1.9.0/spotfire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-11-21 18:46:32.000000 spotfire-1.9.0/spotfire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-11-21 18:46:32.000000 spotfire-1.9.0/spotfire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 18:46:32.000000 spotfire-1.9.0/spotfire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-11-21 18:46:32.000000 spotfire-1.9.0/spotfire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-21 18:46:32.000000 spotfire-1.9.0/spotfire.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:19:59.827512 spotfire-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-27 16:19:45.000000 spotfire-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-27 16:19:45.000000 spotfire-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-27 16:19:59.827512 spotfire-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 16:19:45.000000 spotfire-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-27 16:19:45.000000 spotfire-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 16:19:45.000000 spotfire-2.0.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 16:19:59.827512 spotfire-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-27 16:19:45.000000 spotfire-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:19:59.823511 spotfire-2.0.0/spotfire/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-27 16:19:45.000000 spotfire-2.0.0/spotfire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-27 16:19:45.000000 spotfire-2.0.0/spotfire/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-27 16:19:45.000000 spotfire-2.0.0/spotfire/cabfile.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-27 16:19:45.000000 spotfire-2.0.0/spotfire/cabfile_helpers.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-04-27 16:19:45.000000 spotfire-2.0.0/spotfire/codesign.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    18848 2023-04-27 16:19:45.000000 spotfire-2.0.0/spotfire/data_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-27 16:19:45.000000 spotfire-2.0.0/spotfire/public.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-27 16:19:45.000000 spotfire-2.0.0/spotfire/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    84591 2023-04-27 16:19:45.000000 spotfire-2.0.0/spotfire/sbdf.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-04-27 16:19:45.000000 spotfire-2.0.0/spotfire/sbdf_helpers.c
+-rw-r--r--   0 runner    (1001) docker     (123)    44229 2023-04-27 16:19:45.000000 spotfire-2.0.0/spotfire/spk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-27 16:19:45.000000 spotfire-2.0.0/spotfire/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:19:59.823511 spotfire-2.0.0/spotfire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-27 16:19:59.000000 spotfire-2.0.0/spotfire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-27 16:19:59.000000 spotfire-2.0.0/spotfire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:19:59.000000 spotfire-2.0.0/spotfire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-27 16:19:59.000000 spotfire-2.0.0/spotfire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 16:19:59.000000 spotfire-2.0.0/spotfire.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:19:59.823511 spotfire-2.0.0/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/__init__.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:19:59.823511 spotfire-2.0.0/vendor/sbdf-c/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:19:59.827512 spotfire-2.0.0/vendor/sbdf-c/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/all.h
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/all_io.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/bytearray.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/columnmetadata.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/columnslice.h
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/columnslice_io.h
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/config.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/errors.h
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/fileheader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/metadata.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/object.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/object_io.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/sbdfstring.h
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/sectiontypeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/sectiontypeid_io.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/tablemetadata.h
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/tablemetadata_io.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/tableslice.h
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/tableslice_io.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/valuearray.h
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/valuearray_io.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/valuetype.h
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/valuetype_io.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/include/valuetypeid.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:19:59.827512 spotfire-2.0.0/vendor/sbdf-c/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/src/bswap.c
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/src/bswap.h
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/src/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/src/columnmetadata.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/src/columnslice.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/src/errors.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/src/fileheader.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/src/internals.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/src/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/src/metadata.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/src/object.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/src/sbdfstring.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/src/tablemetadata.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/src/tableslice.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/src/valuearray.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/src/valuetype.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:19:59.827512 spotfire-2.0.0/vendor/sbdf-c/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/tests/api_scenario.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/tests/cppsupp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/tests/test.h
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf-c/tests/test_c.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/sbdf_c.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:19:59.827512 spotfire-2.0.0/vendor/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/windows/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/windows/fci.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/windows/mssign32.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/windows/mssign32.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-27 16:19:45.000000 spotfire-2.0.0/vendor/windows/wincrypt.pxd
```

### Comparing `spotfire-1.9.0/LICENSE` & `spotfire-2.0.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-﻿Copyright (c) 2022 TIBCO Software Inc. All Rights Reserved. 
+﻿﻿Copyright (c) 2023 Cloud Software Group, Inc. All Rights Reserved. 
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 
-3. Neither the name of TIBCO Software Inc.  nor the names of any contributors may  be used to endorse or promote products derived from this software without specific prior written permission. 
+3. Neither the name of Cloud Software Group, Inc. nor the names of any contributors may  be used to endorse or promote products derived from this software without specific prior written permission. 
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT OWNER AND CONTRIBUTORS  "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+
```

### Comparing `spotfire-1.9.0/PKG-INFO` & `spotfire-2.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: spotfire
-Version: 1.9.0
+Version: 2.0.0
 Summary: Package for Building Python Extensions to TIBCO Spotfire
 Home-page: https://github.com/TIBCOSoftware/spotfire-python
-Author: TIBCO Software Inc.
+Author: Cloud Software Group, Inc.
 Maintainer: Spotfire Python Package Support
 Maintainer-email: spotfirepython@tibco.com
 License: BSD 3-Clause License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Cython
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Package for Building Python Extensions to TIBCO Spotfire® 
 
 This package provides functions used for integrating Python with Spotfire, including:
```

### Comparing `spotfire-1.9.0/README.md` & `spotfire-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `spotfire-1.9.0/spotfire/__init__.py` & `spotfire-2.0.0/spotfire/public.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2021. TIBCO Software Inc.
+# Copyright © 2021. Cloud Software Group, Inc.
 # This file is subject to the license terms contained
 # in the license file that is distributed with this file.
 
 """User visible utility functions."""
 
 import typing
 import warnings
@@ -27,25 +27,31 @@
     if isinstance(source, pd.Series) and not isinstance(destination, pd.Series):
         raise TypeError("both source and destination must be Series")
 
     # Handle DataFrames
     if isinstance(source, pd.DataFrame):
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
-            destination.spotfire_table_metadata = source.spotfire_table_metadata
+            try:
+                destination.spotfire_table_metadata = source.spotfire_table_metadata
+            except AttributeError:
+                pass
         for col in source.columns:
             try:
                 source1 = source[col]
                 destination1 = destination[col]
                 destination1.spotfire_column_metadata = source1.spotfire_column_metadata
             except AttributeError:
                 pass
     # Handle Series
     elif isinstance(source, pd.Series):
-        destination.spotfire_column_metadata = source.spotfire_column_metadata
+        try:
+            destination.spotfire_column_metadata = source.spotfire_column_metadata
+        except AttributeError:
+            pass
 
 
 # Spotfire type functions
 
 def get_spotfire_types(dataframe: pd.DataFrame) -> pd.Series:
     """Get Spotfire column type names from an imported DataFrame.
 
@@ -72,12 +78,11 @@
     """
     if not isinstance(dataframe, pd.DataFrame):
         raise TypeError("dataframe is not a DataFrame")
     for col, spotfire_type in column_types.items():
         if col not in dataframe:
             warnings.warn(f"Column '{col}' not found in data")
             continue
-        # pylint: disable=protected-access
-        if not sbdf._ValueTypeId.from_typename_string(spotfire_type):
-            warnings.warn(f"Spotfire type '{spotfire_type}' for column '{col}' not recognized")
+        if not sbdf.spotfire_typename_to_valuetype_id(spotfire_type):
+            warnings.warn(f"Spotfire type '{spotfire_type}' for column '{col}' not recognized", sbdf.SBDFWarning)
             continue
         dataframe[col].attrs['spotfire_type'] = spotfire_type
```

### Comparing `spotfire-1.9.0/spotfire/_utils.py` & `spotfire-2.0.0/spotfire/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2021. TIBCO Software Inc.
+# Copyright © 2021. Cloud Software Group, Inc.
 # This file is subject to the license terms contained
 # in the license file that is distributed with this file.
 
 """Utilities used by multiple submodules."""
 import os
 import tempfile
```

### Comparing `spotfire-1.9.0/spotfire/data_function.py` & `spotfire-2.0.0/spotfire/data_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2021. TIBCO Software Inc.
+# Copyright © 2021. Cloud Software Group, Inc.
 # This file is subject to the license terms contained
 # in the license file that is distributed with this file.
 
 """Automatically manage the protocol between Spotfire and a data function written in Python."""
 
 import io
 import os.path
@@ -209,15 +209,15 @@
         :param script: the Python script code this data function will run
         """
         self.analytic_type = analytic_type
         self.inputs = inputs if isinstance(inputs, list) else []
         self.outputs = outputs if isinstance(outputs, list) else []
         self.script = script
         self.debug_enabled = False
-        self.globals = dict(__builtins__=__builtins__)
+        self.globals = {'__builtins__': __builtins__}
         self.log = io.StringIO()
         self.compiled_script = None
 
     def __repr__(self) -> str:
         return f"{_utils.type_name(type(self))}({self.analytic_type!r}, \
             {self.inputs!r}, {self.outputs!r}, {self.script!r})"
```

### Comparing `spotfire-1.9.0/spotfire/spk.py` & `spotfire-2.0.0/spotfire/spk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2021. TIBCO Software Inc.
+# Copyright © 2021. Cloud Software Group, Inc.
 # This file is subject to the license terms contained
 # in the license file that is distributed with this file.
 
 """Pure Python implementation of a Spotfire package (.spk extension) builder tool."""
 
 import abc
 import argparse
@@ -68,44 +68,49 @@
     sys.stdout.write(os.linesep)
 
 
 # Packaging helper functions
 
 class _SpkVersion:
     """Represents a version number as presented in Spotfire SPK package files.  Version numbers have four components
-    (organized from largest scope to smallest): major, minor, service pack, and identifier."""
+    (organized from the largest scope to smallest): major, minor, service pack, and identifier."""
 
     def __init__(self, major: int = 1, minor: int = 0, service_pack: int = 0, identifier: int = 0) -> None:
         self._versions = [major, minor, service_pack, identifier]
 
     @staticmethod
     def from_str(str_: str) -> '_SpkVersion':
         """Parse a string into a version.
 
         :param str_: the string to parse into a version number
+        :return: new SPK package version object
         """
         components = str_.split(".")
         if len(components) > 4:
             raise ValueError("Must have four components in version number.")
         return _SpkVersion(*map(int, components))
 
     @staticmethod
     def from_version_info(identifier: int) -> '_SpkVersion':
-        """Extract the SPK version of the running Python installation."""
+        """Extract the SPK version of the running Python installation.
+
+        :param identifier: fourth component for the generated version object
+        :return: new SPK package version object of the form `X.YYZZ.ABBCC.identifier` (where `X.Y.Z` is the Python
+                   version, and `A.B.C` is the version of the `spotfire` package)
+        """
         spk_minor = (sys.version_info.minor * 100) + sys.version_info.micro
         spotfire_version_components = spotfire.version.__version__.split(".")
         spk_service_pack = (int(spotfire_version_components[0]) * 10000) + \
                            (int(spotfire_version_components[1]) * 100) + \
                            (int(spotfire_version_components[2]))
         version = _SpkVersion(sys.version_info.major, spk_minor, spk_service_pack, identifier)
         return version
 
     def __str__(self):
-        # pylint: disable=consider-using-f-string
-        return "%d.%d.%d.%d" % tuple(self._versions)
+        return '.'.join([str(x) for x in self._versions])
 
     def __repr__(self):
         return f"{self.__class__.__module__}.{self.__class__.__qualname__}{tuple(self._versions)!r}"
 
     def increment_major(self) -> None:
         """Increment the major component of the version number.  Resets all smaller components to zero."""
         self._versions[0] += 1
@@ -205,39 +210,55 @@
 
     # Reassemble data and parse the JSON object from the brand.
     data_json = "".join(map(lambda x: x[len(comment):].rstrip(), lines))
     return json.loads(data_json) if data_json else {}
 
 
 class _PackageBuilder(metaclass=abc.ABCMeta):
-    # pylint: disable=too-many-instance-attributes,consider-using-f-string
+    # pylint: disable=too-many-instance-attributes
     def __init__(self) -> None:
         self.name = None
         self.version = None
         self.id = None
         self.output = None
         self.excludes = []
         self.last_scan_dir = None
         self._contents = []
+        self._cleanup_dirs = []
+        self._cleanup_files = []
         if platform.system() == "Windows":
             self._site_packages_dirname = "Lib\\site-packages"
         else:
-            self._site_packages_dirname = "lib/python%d.%d/site-packages" % sys.version_info[:2]
+            self._site_packages_dirname = f"lib/python{'.'.join([str(x) for x in sys.version_info[:2]])}/site-packages"
+
+    def cleanup(self):
+        """Clean up temporary files used to create the package."""
+        for dirname in self._cleanup_dirs:
+            shutil.rmtree(dirname)
+        for filename in self._cleanup_files:
+            os.unlink(filename)
 
     def add(self, filename: str, archive_name: str) -> None:
-        """Add a file to the package."""
+        """Add a file to the package.
+
+        :param filename: the file name on disk to add to the package
+        :param archive_name: the name within the package to add the file as
+        """
         archive_backslash = archive_name.replace("/", "\\")
         if self.excludes is not None:
             for exclude in self.excludes:
                 if archive_backslash.startswith(exclude):
                     return
         self._contents.append((filename, archive_backslash))
 
     def scan_python_installation(self, prefix: str) -> None:
-        """Scan all the files in the Python installation."""
+        """Scan all the files in the Python installation.
+
+        :param prefix: the directory within the package to locate the Python installation at
+        """
         try:
             py_prefix = sys.base_prefix
         except AttributeError:
             py_prefix = getattr(sys, "real_prefix", sys.prefix)
         _message(f"Scanning Python installation at {py_prefix} for files to include.")
 
         # Scan all files in the running Python's prefix
@@ -247,82 +268,82 @@
                 filename_relative = os.path.relpath(filename_ondisk, py_prefix)
                 filename_payload = f"{prefix}/{filename_relative}"
                 if not filename_relative.startswith(self._site_packages_dirname):
                     # Omit any packages installed in site-packages
                     self.add(filename_ondisk, filename_payload)
 
     def scan_spotfire_package(self, prefix: str) -> None:
-        """Scan the 'spotfire' package (and it's .dist-info directory) into site-packages."""
+        """Scan the 'spotfire' package (and it's .dist-info directory) into spotfire-packages.
+
+        :param prefix: the directory within the package the Python installation is located at
+        """
         _message("Scanning 'spotfire' package files.")
 
         # Grab the files of the 'spotfire' package.
         for root, _, filenames in os.walk(spotfire.__path__[0]):
             for filename in filenames:
                 filename_ondisk = os.path.join(root, filename)
                 filename_relative = os.path.relpath(filename_ondisk, spotfire.__path__[0])
-                filename_payload = f"{prefix}/{self._site_packages_dirname}/spotfire/{filename_relative}"
+                filename_payload = f"{prefix}/spotfire-packages/spotfire/{filename_relative}"
                 self.add(filename_ondisk, filename_payload)
 
         # Grab the .dist-info directory.
         site_packages_dir = os.path.dirname(spotfire.__path__[0])
         spotfire_dist_info_re = re.compile(r"^spotfire(-.*)?\.(dist|egg)-info$")
         for subdir in next(os.walk(site_packages_dir))[1]:
             if spotfire_dist_info_re.match(subdir):
                 spotfire_dist_info_dir = os.path.join(site_packages_dir, subdir)
                 for root, _, filenames in os.walk(spotfire_dist_info_dir):
                     for filename in filenames:
                         filename_ondisk = os.path.join(root, filename)
                         filename_relative = os.path.relpath(filename_ondisk, spotfire_dist_info_dir)
-                        filename_payload = f"{prefix}/{self._site_packages_dirname}/{subdir}/{filename_relative}"
+                        filename_payload = f"{prefix}/spotfire-packages/{subdir}/{filename_relative}"
                         self.add(filename_ondisk, filename_payload)
 
     def scan_requirements_txt(self, requirements: str, constraint: str, prefix: str, prefix_direct: bool = False,
-                              use_deny_list: bool = False) -> \
-            typing.Tuple[typing.Callable[[], None], typing.Dict[str, str]]:
+                              use_deny_list: bool = False) -> typing.Dict[str, str]:
         """Scan the contents of a pip 'requirements.txt' file into site-packages.
 
         :param requirements: the filename of the requirements file that declares the pip packages to put in the
-        SPK package
+                               SPK package
         :param constraint: the filename of the constraints file that declares the constraints pip should apply
-        when resolving requirements
+                             when resolving requirements
         :param prefix: the directory prefix under which the pip packages should be scanned into
-        :param prefix_direct: whether to scan the pip packages into the ``site-packages`` directory
+        :param prefix_direct: whether to scan the pip packages into the ``site-packages`` directory or directly
+                                into the prefix directory
         :param use_deny_list: whether to delete the packages included with the Interpreter from the
                                 temporary package area before bundling.
-        :return: a function that cleans up the temporarily installed packages, and a dict that maps the names of
-        pip packages that were scanned into the SPK package to their installed versions
+        :return: a dict that maps the names of pip packages that were scanned into the SPK package to their
+                   installed versions
         """
-        # pylint: disable=too-many-locals,subprocess-run-check
+        # pylint: disable=too-many-locals
 
         tempdir = tempfile.mkdtemp(prefix="spk")
         self.last_scan_dir = tempdir
-
-        def cleanup():
-            """Cleanup the created tempdir."""
-            shutil.rmtree(tempdir)
+        self._cleanup_dirs.append(tempdir)
 
         # Install the packages from the requirement file into tempdir.
         _message(f"Installing pip packages from {requirements} to temporary location.")
-        command = [sys.executable, "-m", "pip", "install", "--upgrade", "--disable-pip-version-check",
+        command = [sys.executable, "-m", "pip", "install", "--disable-pip-version-check",
                    "--target", tempdir, "--requirement", requirements]
         if constraint:
             command.extend(["--constraint", constraint])
-        pip_install = subprocess.run(command)
+        pip_install = subprocess.run(command, check=False)
         if pip_install.returncode != 0:
             _error("Error installing required packages.  Aborting.")
-            cleanup()
+            self.cleanup()
             sys.exit(1)
 
         # List packages that were installed.
         command = [sys.executable, "-m", "pip", "list", "--disable-pip-version-check", "--path", tempdir,
                    "--format", "json"]
-        pip_list = subprocess.run(command, capture_output=True)
+        pip_list = subprocess.run(command, capture_output=True, check=False)
         if pip_list.returncode != 0:
             _error("Error installing required packages.  Aborting.")
-            cleanup()
+            self.cleanup()
             sys.exit(1)
         package_versions_json = json.loads(pip_list.stdout.decode(locale.getpreferredencoding()))
         package_versions = {x['name']: x['version'] for x in package_versions_json}
 
         # Delete duplicate packages if needed
         if use_deny_list:
             package_versions = self.scan_duplicate_packages(tempdir, package_versions)
@@ -336,22 +357,26 @@
                 if prefix_direct:
                     filename_payload = f"{prefix}/{filename_relative}"
                 else:
                     filename_payload = f"{prefix}/{self._site_packages_dirname}/{filename_relative}"
                 if not filename_relative.startswith(f"bin{os.path.sep}"):
                     self.add(filename_ondisk, filename_payload)
 
-        return cleanup, package_versions
+        return package_versions
 
     @staticmethod
-    def scan_duplicate_packages(tempdir: str, package_versions):
-        """ When building a custom Python Packages SPK, find and delete duplicate packages.
-        :return:
+    def scan_duplicate_packages(tempdir: str, package_versions: typing.Dict[str, str]) -> typing.Dict[str, str]:
+        """Find and delete duplicate packages from a directory of packages .
+
+        :param tempdir: the temporary on-disk directory to which the packages to scan for duplicates have been
+                          downloaded
+        :param package_versions: the dictionary returned by :method:`scan_requirements_txt` that maps package names
+                                   to versions
+        :return: `package_versions`, but with duplicate packages removed from the mapping
         """
-        # Disable Pylint `Too many nested blocks`
         # pylint: disable=too-many-nested-blocks,too-many-locals
         # Use the spotfire requirements file as a deny list.
         if "spotfire.zip" in spotfire.__path__[0]:
             # Handle getting the requirements.txt from a zip file.
             with zipfile.ZipFile(os.path.split(spotfire.__path__[0])[0]) as zfile:
                 with zfile.open("spotfire/requirements.txt") as deny_file:
                     deny_requirements = deny_file.readlines()
@@ -409,14 +434,30 @@
                 try:
                     shutil.rmtree(package_directory_file)
                 except OSError:
                     _message(f"Unable to remove directory {package_directory_file}")
         _message("Completed removing files and directories for packages on the deny list.")
         return package_versions
 
+    def scan_path_configuration_file(self, prefix: str) -> None:
+        """Add a path configuration file for the 'spotfire-packages' directory to the Python interpreter.
+
+        :param prefix: the directory within the package the Python installation is located at
+        """
+        _message("Adding path configuration file for spotfire-packages directory.")
+        fd, temp = tempfile.mkstemp()
+        with os.fdopen(fd, "w") as file:
+            file.write('import sys, os; '
+                       'sys.path.insert(min([i for i, x in enumerate(["site-packages" in x for x in sys.path]) if x]), '
+                       'f"{sys.prefix}{os.sep}spotfire-packages")\n')
+        if platform.system() != 'Windows':
+            os.chmod(temp, 0o644)
+        self._cleanup_files.append(temp)
+        self.add(temp, f"{prefix}/{self._site_packages_dirname}/spotfire.pth")
+
     @abc.abstractmethod
     def _payload_name(self) -> str:
         """Get the payload archive name for this package."""
 
     def _create_module(self) -> ElementTree.Element:
         """Create the module document."""
         module = ElementTree.Element("module")
@@ -484,23 +525,22 @@
     # Serialize the element to a string
     temp_io = io.BytesIO()
     ElementTree.ElementTree(element).write(temp_io, encoding="utf-8", xml_declaration=True)
     return temp_io.getvalue()
 
 
 def _et_indent(element: ElementTree.Element, indent="  ", level=0) -> None:
-    # pylint: disable=redefined-argument-from-local
     indent_text = "\n" + (level * indent)
     if element:
         if not element.text or not element.text.strip():
             element.text = indent_text + indent
         if not element.tail or not element.tail.strip():
             element.tail = indent_text
-        for element in element:
-            _et_indent(element, indent, level + 1)
+        for elem in element:
+            _et_indent(elem, indent, level + 1)
         if not element.tail or not element.tail.strip():
             element.tail = indent_text
     else:
         if level and (not element.tail or not element.tail.strip()):
             element.tail = indent_text
 
 
@@ -585,15 +625,19 @@
         self._resources = []
 
     def _payload_name(self) -> str:
         """Get the payload archive name for this package."""
         return f"{self.name}.cab"
 
     def add_resource(self, name: str, location: str) -> None:
-        """Add a public resource provided by this package."""
+        """Add a public resource provided by this package.
+
+        :param name: name of the resource to add to this package
+        :param location: the location within the package the resource refers to
+        """
         self._resources.append((name, location))
 
     def _create_module(self) -> ElementTree.Element:
         """Create the module document."""
         module = super()._create_module()
         module_intended_client = ElementTree.SubElement(module, "intendedClient")
         module_intended_client.text = "Forms"
@@ -605,18 +649,19 @@
                 "name": resource_name,
                 "relativePath": resource_location
             })
         return module
 
     def _build_payload(self, metadata: ElementTree.Element, module: ElementTree.Element, payload_dest: str) -> None:
         """Build the main payload archive for the SPK package."""
-        # pylint: disable=import-outside-toplevel
+        # pylint: disable=import-outside-toplevel,no-name-in-module
         from spotfire import cabfile, codesign
         metadata_files = metadata.find("Files")
 
+        # pylint: disable=not-context-manager
         with cabfile.CabFile(payload_dest) as payload:
             # Add all files that are supposed to go into the package
             for filename_ondisk, filename_payload in self._contents:
                 payload.write(filename_ondisk, filename_payload)
                 stat = os.lstat(filename_ondisk)
                 ElementTree.SubElement(metadata_files, "File", {
                     "TargetRelativePath": filename_payload,
@@ -690,35 +735,33 @@
     # Get the version of the Python installation
     if sys.version_info.major == 3 and sys.version_info.minor < 5:
         print(f"Error: Unsupported version of Python ('{sys.version}').")
         sys.exit(1)
     package_builder.version = _SpkVersion.from_version_info(version_identifier)
 
     # Scan the files required to create the Python interpreter SPK
-    def cleanup():
-        """Dummy cleanup function."""
-
     if analyst:
         prefix = "python"
         package_builder.add_resource("default.python.interpreter.directory", prefix)
     else:
         prefix = "root/python"
     package_builder.scan_python_installation(prefix)
+    package_builder.scan_path_configuration_file(prefix)
     package_builder.scan_spotfire_package(prefix)
     spotfire_requirements = os.path.join(spotfire.__path__[0], "requirements.txt")
     try:
         constraints = getattr(args, "constraint")
-        cleanup, _ = package_builder.scan_requirements_txt(spotfire_requirements, constraints, prefix)
+        package_builder.scan_requirements_txt(spotfire_requirements, constraints, prefix)
         if hook is not None:
             hook.scan_finished(package_builder)
 
         # Build the package
         package_builder.build()
     finally:
-        cleanup()
+        package_builder.cleanup()
 
 
 @subcommand([argument("spk-file", help="path to the SPK file to build"),
              argument("requirements", help="package the Python packages listed in the file"),
              argument("-v", "--version", help="set the version number of the built SPK file"),
              argument("-f", "--force", action="store_true", help="ignore errors about downgrading version numbers"),
              argument("--versioned-filename", action="store_true", help="modify the filename of the SPK file to "
@@ -735,17 +778,14 @@
                                                          "(Analyst only)"),
              argument("--sha256", action="store_true", help="use SHA-256 for file and timestamp digests (Analyst only)")
              ])
 def packages(args) -> None:
     """Package a list of Python packages as an SPK package"""
     # pylint: disable=too-many-statements
 
-    def cleanup():
-        """Dummy cleanup function."""
-
     try:
         # Set up the package builder
         analyst = getattr(args, "analyst")
         if analyst:
             package_builder = _CabPackageBuilder()
             package_builder.cert_file = getattr(args, "cert")
             package_builder.cert_password = getattr(args, "password")
@@ -781,16 +821,16 @@
             prefix = "site-packages"
             prefix_direct = True
             package_builder.add_resource(f"python.package.{package_builder.id}.whl", prefix)
         else:
             prefix = "root/python"
             prefix_direct = False
         constraints = getattr(args, "constraint")
-        cleanup, installed_packages = package_builder.scan_requirements_txt(requirements_file, constraints, prefix,
-                                                                            prefix_direct, True)
+        installed_packages = package_builder.scan_requirements_txt(requirements_file, constraints, prefix,
+                                                                   prefix_direct, True)
 
         # Based on the packages we installed, determine how to increment the version number
         _handle_versioning(package_builder, installed_packages, brand, brand_subkey, version, force, versioned_filename)
 
         # Build the package
         package_builder.build()
 
@@ -800,31 +840,51 @@
         brand[brand_subkey]["BuiltFile"] = package_builder.output
         brand[brand_subkey]["BuiltName"] = package_builder.name
         brand[brand_subkey]["BuiltId"] = package_builder.id
         brand[brand_subkey]["BuiltVersion"] = str(package_builder.version)
         brand[brand_subkey]["BuiltPackages"] = installed_packages
         _brand_file(requirements_file, brand, "## spotfire.spk: ")
     finally:
-        cleanup()
+        package_builder.cleanup()
+
 
+def _promote_brand(brand: typing.Dict, analyst: bool) -> typing.Dict:
+    """Promote the version of a brand to the current representation.
 
-def _promote_brand(brand, analyst):
+    :param brand: the brand to promote
+    :param analyst: whether the brand represents an Analyst package
+    :return: `brand`, promoted to the current version
+    """
     brand_version = brand.get("BrandVersion") or 1
 
     # Promote 1 to 2
     if brand_version < 2:
         if analyst:
             brand = {"BrandVersion": 2, "Analyst": brand, "Server": {}}
         else:
             brand = {"BrandVersion": 2, "Analyst": {}, "Server": brand}
 
     return brand
 
 
-def _handle_versioning(package_builder, installed_packages, brand, brand_subkey, version, force, versioned_filename):
+def _handle_versioning(package_builder: _PackageBuilder, installed_packages: typing.Dict[str, str], brand: typing.Dict,
+                       brand_subkey: str, version: typing.Optional[str], force: bool, versioned_filename: bool) -> None:
+    """Properly handle the SPK package version given the packages installed by prior versions of the SPK package
+    (from the brand) and the set of packages that were downloaded.
+
+    :param package_builder: the package builder that is building the SPK package
+    :param installed_packages: the dictionary from :method:`_PackageBuilder.scan_requirements_txt` indicating the
+                                 packages and versions that were downloaded
+    :param brand: the brand containing information about the prior version of the SPK package
+    :param brand_subkey: the name of the subkey of the brand to look for information under
+    :param version: user-specified version for the SPK package, or `None` if unspecified
+    :param force: whether the user has asked to ignore error conditions in versioning
+    :param versioned_filename: whether the user has asked to have the generated version added to the SPK package's
+                                 filename
+    """
     # pylint: disable=too-many-arguments
     package_builder.version = _SpkVersion()
     if "BuiltVersion" in brand[brand_subkey]:
         package_builder.version = _SpkVersion.from_str(brand[brand_subkey]["BuiltVersion"])
         package_builder.version.increment_minor()
         if "BuiltPackages" in brand[brand_subkey]:
             # Tick the major version if required
@@ -840,15 +900,23 @@
         package_builder.version = given_version
     # Handle versioned filenames
     if versioned_filename:
         package_builder.output = re.sub(r"(\.spk)?$", fr"-{str(package_builder.version)}\1",
                                         package_builder.output, 1)
 
 
-def _should_increment_major(old_packages, new_packages, force):
+def _should_increment_major(old_packages: typing.Dict[str, str], new_packages: typing.Dict[str, str],
+                            force: bool) -> bool:
+    """Determine if the major version of the SPK package should be incremented, instead of the minor version.
+
+    :param old_packages: dictionary mapping packages to versions present in the old version of the SPK package
+    :param new_packages: dictionary mapping packages to versions present in the new version of the SPK package
+    :param force: whether the user has asked to ignore error conditions in versioning
+    :return: whether the major component of the version should be incremented
+    """
     tick_major = False
     # Check for removed packages
     if old_packages.keys() - new_packages.keys():
         tick_major = True
     # Check for package downgrades
     for pkg in old_packages.keys() & new_packages.keys():
         previous_version = pip_version.parse(old_packages[pkg])
```

### Comparing `spotfire-1.9.0/spotfire.egg-info/PKG-INFO` & `spotfire-2.0.0/spotfire.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: spotfire
-Version: 1.9.0
+Version: 2.0.0
 Summary: Package for Building Python Extensions to TIBCO Spotfire
 Home-page: https://github.com/TIBCOSoftware/spotfire-python
-Author: TIBCO Software Inc.
+Author: Cloud Software Group, Inc.
 Maintainer: Spotfire Python Package Support
 Maintainer-email: spotfirepython@tibco.com
 License: BSD 3-Clause License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Cython
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Package for Building Python Extensions to TIBCO Spotfire® 
 
 This package provides functions used for integrating Python with Spotfire, including:
```

